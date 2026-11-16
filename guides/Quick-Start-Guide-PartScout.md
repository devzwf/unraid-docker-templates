<p align="center"><img src="../images/partscout-logo.png" width="96" alt="PartScout logo"></p>

# Quick Start Guide: PartScout on Unraid

[PartScout](https://github.com/devzwf/partscout) searches several electronic component suppliers at once (DigiKey, Mouser, element14, TME…) and compares stock, prices, price breaks, MOQ, lifecycle and datasheets, from a web interface in English or French.

Support thread: *(link to the Unraid forum thread)* · Bugs: [GitHub issues](https://github.com/devzwf/partscout/issues)

---

### 1. Generate two secrets
Open the Unraid **Terminal** and run this twice:
```bash
openssl rand -base64 32
```
- The first value is the **Master Key**. It encrypts your supplier API keys. **Save it somewhere safe, outside appdata**: if you lose it, you will have to enter your API keys again.
- The second value is the **Setup Token**. You need it only once, to create the admin password.

### 2. Install from Community Applications
**Apps** tab → search **PartScout** → **Install**, then fill in:

| Field | Value |
|---|---|
| **Web UI Port** | `5070` by default. Do not use `5060` or `5061`: browsers block them. |
| **Data** | `/mnt/user/appdata/partscout/data` (database, settings, daily backups) |
| **Master Key** | first value from step 1 |
| **Setup Token** | second value from step 1 |

Click **Apply**.

> If you point **Data** to a folder that already exists, it must belong to `nobody:users`:
> `chown -R 99:100 /mnt/user/appdata/partscout/data`

### 3. First sign-in
1. Open the **WebUI** (`http://<unraid-ip>:5070`).
2. Enter the **Setup Token**, then choose your admin password.
3. Go to **Settings** and add your supplier API keys. Each supplier has its own free developer portal. A supplier without a key still shows up as a link to its website.
4. Also in **Settings**: default currency, suppliers and DigiKey site (Canada by default), and other user accounts if needed. There is no public sign-up.

### 4. Behind a reverse proxy (optional)
Click **Show more settings** in the template:
- **Trusted Proxy IP**: the IP address of your proxy (SWAG, NPM, Caddy…).
- **Secure Cookie**: `always` once you reach PartScout over HTTPS. Keep `auto` for plain HTTP on your LAN.

Use HTTPS as soon as several people sign in. PartScout is meant for a home network or a VPN, **not for direct exposure to the Internet**.

### 5. Backups and restore
- Every hour, PartScout writes a consistent copy of its database to `/mnt/user/appdata/partscout/data/backups/`: one file per day, kept 14 days.
- Back up the `data` folder **and** your Master Key.
- **Restore:** stop the container, delete `partscout.db`, `partscout.db-wal` and `partscout.db-shm`, copy `backups/partscout-YYYY-MM-DD.db` to `partscout.db`, run `chown 99:100 partscout.db`, then start the container again.

### 6. Updates
The template uses the `latest` tag: update it from the **Docker** tab like any other container. To pin a version, edit the container and set the repository to `devzwf/partscout:0.1.6` (for example). Changes are listed in the [CHANGELOG](https://github.com/devzwf/partscout/blob/main/CHANGELOG.md).

### Troubleshooting
- **The Console button does nothing:** expected. The image has no shell (read-only, hardened container).
- **The log says `/data` is not writable:** the Data folder does not belong to `99:100`. See the `chown` command in step 2.
- **The page will not load on port 5060/5061:** browsers block these ports. Change the Web UI Port.

---

PartScout is a web version derived from [Win-PartsFinder](https://github.com/Ian-Johnston/WinPartsFinder) by Ian Johnston, for personal and non-commercial use only ([LICENSE](https://github.com/devzwf/partscout/blob/main/LICENSE), [NOTICE](https://github.com/devzwf/partscout/blob/main/NOTICE.md)).

☕ If PartScout saves you some time, you can support its development on [Ko-fi](https://ko-fi.com/devzwf) or [Buy Me a Coffee](https://www.buymeacoffee.com/devzwf). Thank you!
