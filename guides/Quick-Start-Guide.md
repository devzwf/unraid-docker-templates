# Quick Start Guide

### Environment

-   Primary pihole on the unraid docker host A (**unraidA**) has it's files typically in `/mnt/user/appdata/pihole`. There are two important directories there that this app is going to sync:
    -   `/mnt/user/appdata/pihole/pihole`
    -   `/mnt/user/appdata/pihole/dnsmasq.d`
-   The pihole-sync sender is going to reside on the same docker host as the master pihole server as it has direct access to the same filesystem. A sensible path for this would be
    -   `/mnt/user/appdata/pihole-sync-sender` (on **unraidA**)
-   Secondary pihole on unraid docker host B (**unraidB**) should probably have a similar filesystem setup for consistency. Of course the path for the receiver should be similarly
    -   `/mnt/user/appdata/pihole-sync-receiver` (on **unraidB**)
-   NETWORKING:
    -   If you use **Bridge** mode for your containers, the sync will be employing TCP ports `22222`. Defaults will work for you.
    -   If you use **br0** mode for a dedicated IP per container, you can just use the standard ssh port `22` (change `22222` to `22`).
    -   *Remember that your sync hosts are going to be on different IPs than your piholes if you use br0 method, so don't confuse that in your setup.*
-   Operations: *you should be able to ssh from **unraidA** to **unraidB**. Otherwise you can use the clipboard and web terminal.*

### Install the Receiver

1.  On **unraidB**, use Community Apps to install Pihole-Sync-Receiver. In the Add Container dialog you are going to have the following fields to fill:
    -   **Name**: I recommend renaming the docker image to `pihole-sync-receiver` (lowercase) for consistency (this will make it less tedious in the CLI later)
    -   **Network**: as discussed above in **Networking**
    -   **Remote Host IP**: as discussed above in **Networking**
    -   **Root directory**: `/mnt/user/appdata/pihole-sync-receiver/root`
    -   **Etc-ssh**: `/mnt/user/appdata/pihole-sync-receiver/ssh`
    -   **Pi-Hole Path**: `/mnt/user/appdata/pihole-sync-receiver/pihole`  (we're going to change this later to a symlink)
    -   **Pi-Hole DNSmasq path**: `/mnt/user/appdata/pihole-sync-receiver/dnsmasq.d`   (we're going to change this later to a symlink)
    -   *click* `Show more settings`
    		-   Node Type: receiver
       	-   Remote SSH port: as discussed above in **Networking**
    -   *click* `Apply`
2.  Stop the Receiver container for now.
3.  Open a Terminal on **unraidB**
    -   `cd /mnt/user/appdata/pihole-sync-receiver`
    -   `mkdir root/.ssh`
    -   *later you will be symlinking the pihole and dnsmasq.d directories here to your secondary pihole server's paths one level up. But let's get this working first.*

*Note: We installed the Receiver first because the sender is going to thrash against the receiver trying to connect until we complete the ssh key installation.*

### Install the Sender and copy the ssh key to the Receiver

1.  On **unraidA**, use *Community Apps* to install *Pihole-Sync-Sender*. In the *Add Container* dialog you are going to have the following fields to fill:
    -   **Name**: I recommend renaming the docker image to pihole-sync-sender for consistency (this will make it less tedious in the CLI later)
    -   **Network**: as discussed above in Networking
    -   **Remote Host IP**: as discussed above in Networking
    -   **Root directory**: `/mnt/user/appdata/pihole-sync-sender/root`
    -   **Etc-ssh**: `/mnt/user/appdata/pihole-sync-sender/ssh`
    -   **Pi-Hole Path**: `/mnt/user/appdata/pihole-sync-sender/pihole`  *(we're going to change this later to a symlink)*
    -   **Pi-Hole DNSmasq path**: `/mnt/user/appdata/pihole-sync-sender/dnsmasq.d`   *(we're going to change this later to a symlink)*
		-   *click* `Show more settings`
    		-   Node Type: sender
       	-   Remote SSH port: as discussed above in Networking
    -   *click* `Apply`
2.  On first startup, the container is going to generate a ssh host key. If you used the paths defined above, it will be located in
    -   `/mnt/user/appdata/pihole-sync-sender/root/.ssh/`
3.  Open Terminal on unraidA
    -   `docker logs pihole-sync-sender`
    -   *there is a message early on in the logs that mentions the steps to copy the ssh key to the receiver. I'll re-iterate these instructions below.*
    -   `cd /mnt/user/appdata/pihole-sync-sender/root/.ssh/`
    -   `scp id_ed25519.pub root@unraidB:/mnt/user/appdata/pihole-sync-receiver/root/.ssh/authorized_keys`
			-   *enter the root password for unraidB when prompted to authenticate this secure copy*
4.  Now start the Receiver on **unraidB**
5.  Open Terminal on **unraidB**
    -   `docker exec -it pihole-sync-receiver /bin/bash`
    -   `cd /`
    -   `chown root root`
    -   `chgrp root root`
    -   `exit`
6.  On **unraidA**
    -   `cd /mnt/user/appdata/pihole-sync-sender`
    -   `touch pihole/psynctestfile`
    -   `touch dnsmasq.d/dsynctestfile`
7.  Now start the Sender on **unraidA**
    -   `docker logs pihole-sync-sender`
8.  On **unraidB**
    -   `docker logs pihole-sync-receiver`
    -   `cd /mnt/user/appdata/pihole-sync-receiver`
    -   `ls -a pihole`  *(do you see your `psynctestfile` ?)*
    -   ls -a dynsmasq.d   *(do you see your `dsynctestfile` ?)*
9.  Once you know its syncing properly, the setup is ready to be connected to your primary and secondary piholes.
    -   stop both the sender and receiver containers
    -   delete the sync test files at both ends
    -   Use symlinks:
			-   on **unraidA** (sender) it would be something like this:
            -   `ln -s /mnt/user/appdata/pihole/pihole /mnt/user/appdata/pihole-sync-sender/pihole`
            -   `ln -s /mnt/user/appdata/pihole/dnsmasq.d /mnt/user/appdata/pihole-sync-sender/dnsmasq.d`
      -   on unraidB (receiver) it would be something like:
      			-   `ln -s /mnt/user/appdata/pihole/pihole /mnt/user/appdata/pihole-sync-receiver/pihole`
        		-   `ln -s /mnt/user/appdata/pihole/dnsmasq.d /mnt/user/appdata/pihole-sync-receiver/dnsmasq.d`
    -   Start the Receiver, then the Sender... check the logs!
10. *This is where the more specific pihole configuration begins (beyond scope of this quick start guide)*

### Frequently Asked Questions & Notes

**Q**: Why am I doing this again?
**A**: To have a fault tolerant pihole across two separate servers. This is necessary if you want to be able to do maintenance on one or the other host machines.

**Q**: How do I configure my clients?
**A**: In your DHCP server settings, issue pihole1 as your first NS and pihole2 as your second NS. Voila, redundant DNS.

**Q**: Can I pause both pi-hole filters at the same time?
**A**: Yes, the PiHole Browser Extension supports multiple PiHoles, just add the respective URLs and API keys

**Q**: I use pihole for DHCP. Does it failover DHCP?
**A**: No, you have to intervene manually to enable DHCP service on the secondary pihole. Existing client leases will remain active for the pre-defined period, so you may not need to do this for short maintenance intervals.
