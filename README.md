<h1 align="center" id="heading"> devzwf's unraid docker templates </h1>

<a href="https://github.com/devzwf/unraid-docker-templates/blob/main/CHANGELOG.MD"><img src="https://img.shields.io/badge/🔶-Changelog-blue" /></a> <a
href="https://ko-fi.com/O5O0FG195"><img src="https://img.shields.io/badge/%E2%98%95-Buy%20me%20a%20coffee-red" /></a>

Template for Docker Containers to use UnRaid

Templates for adding containers to unRAID via more GUI-friendly way and allowing easier updates in the future.
The docker containers referenced in this repo point to Docker Containers maintained by other individuals.

# Unraid Templates

- [hydroqc2mqtt](#hydroqc2mqtt)
- [pihole-sync-sender](#pihole-sync-sender)

---

# hydroqc2mqtt

![hydroqc2mqtt](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/hydroqc-logo.png)

This project was created to provide a way to access Hydro-Québec account and winter credit data in Home-Assistant.
This module use the hydroqc library to fetch all pertinent account information and winter credit signals to be sent to MQTT. It also provide Home-Assistant discovery topics to create all the relevant sensors in Home-Assistant.
It also includes a separate logic that sends the hourly consumption statistics to Home-Assitant via websocket

**Application Name:** hydroqc2mqtt

**Application Site:** https://hydroqc.ca/

**[`^back to top^`](#unraid-templates)**

# pihole-sync-sender

![pihole-sync-sender](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/pihole-logo-bw.png)

A Pihole runs your entire network. If it goes down, your whole network goes down. If you have a family at home, they're going to be pretty annoyed that the wifi goes out everytime you want to do some maintainence. The only solution to this problem is to have a redundant pihole on your network, but you don't want to change your settings in two different places.

This repo allows you to synchronize between two piholes where one is the master and one is the slave. I'll be adding support for more piholes in future. Just update one pihole and the rest automatically update. It supports the /etc/pihole/ and /etc/dnsmasq.d/ directories, excluding some directories which should be client-independent.

**Application Name:** pihole-sync

**Application Site:** https://github.com/ShiromMakkad/docker-pihole-sync

**[`^back to top^`](#unraid-templates)**
