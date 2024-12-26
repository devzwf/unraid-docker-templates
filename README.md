<h1 align="center" id="heading"> devzwf's unraid docker templates </h1>

<a href="https://github.com/devzwf/unraid-docker-templates/blob/main/CHANGELOG.MD"><img src="https://img.shields.io/badge/🔶-Changelog-blue" /></a> <a
href="https://ko-fi.com/O5O0FG195"><img src="https://img.shields.io/badge/%E2%98%95-Buy%20me%20a%20coffee-red" /></a>

Template for Docker Containers to use UnRaid

Templates for adding containers to unRAID via more GUI-friendly way and allowing easier updates in the future.
The docker containers referenced in this repo point to Docker Containers maintained by other individuals.

# Unraid Templates

- [Binner](#binner)
- [Blocky](#blocky)
- [Cups-Airprint](#cups-airprint)
- [Docmost](#docmost)
- [Glance](#glance)
- [homebox](#homebox)
- [hydroqc2mqtt](#hydroqc2mqtt)
- [iventoy](#iventoy)
- [juicepass2mqtt](#juicepass2mqtt)
- [LubeLogger](#lubelogger)
- [M.I.M.O.S.A](#mimosa)
- [Myspeed.dev](#myspeeddev)
- [nebula-sync](#nebula-sync)
- [Onedev](#onedev)
- [pihole DoT/DoH](#pihole-dot-doh)
- [pihole-sync-receiver](#pihole-sync-receiver)
- [pihole-sync-sender](#pihole-sync-sender)
- [Postfix-Relay](#postfixrelay)
- [proxmox-backup-server](#proxmox-backup-server-dockerfiles)
- [proxmox-datacenter-manager](#proxmox-datacenter-manager)
- [silverbullet](#silverbullet)
- [speedtest-tracker](#speedtest-tracker)
- [tasks.md](#tasksmd)
- [Vouchervault](#vouchervault)
- [walos](#wallos)

---

# Binner

![binner](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/binner-logo.png)

Binner is a free open-source parts inventory tracking system you can run locally in Windows or Unix environments. It was created for makers (like myself), hobbyists or professionals to keep track of your parts inventory

**Application Name:** Binner

**Images repository** https://github.com/replaysMike/Binner

**Application Site:** https://binner.io/

**[`^back to top^`](#unraid-templates)**

# Blocky

![blocky](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/blocky-logo.png)

Blocky is a DNS proxy and ad-blocker for the local network written in Go.
Create new config.yaml with your configuration ( see https://0xerr0r.github.io/blocky/configuration/ for more details and all configuration options)

**Application Name:** Blocky

**Images repository** https://github.com/0xERR0R/blocky

**Application Site:**https://0xerr0r.github.io/blocky

**[`^back to top^`](#unraid-templates)**

# CUPS-Airprint

![CUPS-Airprint](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/cups-logo.png)

CUPS instance that is meant as an AirPrint relay for printers that are already on the network but not AirPrint capable.
This Image is based on openprinting

**Application Name:** CUPS-Airprint

**Images repository** https://github.com/chuckcharlie/cups-avahi-airprint

**Application Site:** https://openprinting.github.io/cups/index.html

**[`^back to top^`](#unraid-templates)**

# Docmost

![docmost](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/docmost-logo.png)

Open-source collaborative wiki and documentation software
Create, collaborate, and share knowledge seamlessly with Docmost.
Ideal for managing your wiki, knowledge-base, documentation and a lot more.

**Application Name:** Docmost

**Images repository** https://github.com/docmost/docmost

**Application Site:** https://docmost.com/

**Application Documentation:** https://docmost.com/docs/

**[`^back to top^`](#unraid-templates)**

# Glance

![glance](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/glance_logo.png)

<p align="center"><em>What if you could see everything at a...</em></p>
<h1 align="center">Glance</h1>

**Application Name:** Glance

**Application Site:** https://github.com/glanceapp/glance

**[`^back to top^`](#unraid-templates)**

# Homebox

![homebox](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/homebox_logo.png)

Homebox is the inventory and organization system built for the Home User! With a focus on simplicity and ease of use, Homebox is the perfect solution for your home inventory, organization, and management needs.

**Application Name:** Homebox

**Application Site:** https://hay-kot.github.io/homebox/

**[`^back to top^`](#unraid-templates)**

# hydroqc2mqtt

![hydroqc2mqtt](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/hydroqc-logo.png)

This project was created to provide a way to access Hydro-Québec account and winter credit data in Home-Assistant.
This module use the hydroqc library to fetch all pertinent account information and winter credit signals to be sent to MQTT. It also provide Home-Assistant discovery topics to create all the relevant sensors in Home-Assistant.
It also includes a separate logic that sends the hourly consumption statistics to Home-Assitant via websocket

**Application Name:** hydroqc2mqtt

**Application Site:** https://hydroqc.ca/

**[`^back to top^`](#unraid-templates)**

# iventoy

![iventoy](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/iventoy.png)

iVentoy is an enhanced version of the PXE server.
With iVentoy you can boot and install OS on multiple machines at the same time through the network.
iVentoy is extremely easy to use, without complicated configuration, just put the ISO file in the specified location and select PXE boot in the client machine.
iVentoy supports x86 Legacy BIOS, IA32 UEFI, x86_64 UEFI and ARM64 UEFI mode at the same time.
iVentoy support 110+ common types of OS (Windows/WinPE/Linux/VMware)

**Application Name:** iventoy

**Application Site:** https://www.iventoy.com/en/index.html

**[`^back to top^`](#unraid-templates)**

# juicepass2mqtt

![juicepass2mqtt](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/juicenet.png)

This tool will publish Juicebox data from a UDP proxy to MQTT discoverable by HomeAssistant.
Hopefully we won't need this if EnelX fixes their API!
It is required that both your JuiceBox and the machine you are running juicepassproxy on have internal static IPs on your intranet.

**Application Name:** juicepass2mqtt

**Application Site:** https://github.com/snicker/juicepassproxy

**[`^back to top^`](#unraid-templates)**

# LubeLogger

![lubelogger](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/lubelogger_logo.png)

A self-hosted, open-source vehicle service records and maintainence tracker.

**Application Name:** LubeLogger

**Images repository** https://github.com/hargata/lubelog

**Application Site:** https://github.com/hargata/lubelog

**[`^back to top^`](#unraid-templates)**

# M.I.M.O.S.A

![mimosa](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/mimosa-logo.png)

MIMOSA - short for "Mellow_Labs Inventory Management and Organization System Apparatus". Just like a refreshing mimosa, this system will make your life brighter and more organized!

**Application Name:** M.I.M.O.S.A

**Images repository** https://github.com/FireMarshmellow/M.I.M.O.S.A

**Application Site:** https://github.com/FireMarshmellow/M.I.M.O.S.A

**[`^back to top^`](#unraid-templates)**

# Myspeed.dev

![myspeed](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/myspeed_logo.png)

MySpeed is a Software that helps you keeping track of your network speed.

It automatically creates speedtests based on your schedule and displays them in a list.

**Application Name:** Myspeed.dev

**Images repository** https://github.com/gnmyt/myspeed

**Application Site:** https://myspeed.dev/

**[`^back to top^`](#unraid-templates)**

# nebula-sync

![nebula-sync](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/pihole-logo-bw.png)

Synchronize Pi-hole v6.x configuration to replicas.

This project is not a part of the official Pi-hole project, but uses the api provided by Pi-hole instances to perform the synchronization actions.

Features
* Full sync: Use Pi-hole Teleporter for full synchronization.
* Manual sync: Selective feature synchronization.
* Cron schedule: Run on chron schedule.

*** REQUIRE PI-HOLE V6 ***
Reminder Pihole V6 is still under heavy development 

**Application Name:** nebula-sync

**Application Site:** https://github.com/lovelaze/nebula-sync

**[`^back to top^`](#unraid-templates)**

# Onedev

![onedev](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/onedev-logo.png)

OneDev is an all-in-one DevOps platform that features Git repository management with language-aware code search, issue management with custom states and fields, and a docker-first Kubernetes native build/CI engine. An alternative to GitLab, it is easier to use and maintain, with lots of unique features

**Application Name:** Onedev

**Images repository** https://github.com/theonedev/onedev

**Application Site:** https://code.onedev.io/projects/160

**[`^back to top^`](#unraid-templates)**

# pihole-dot-doh

![pihole-dot-doh](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/pihole-logo-bw.png)

Official pihole docker with both DoT (DNS over TLS) and DoH (DNS over HTTPS) clients. Don't browse the web securely and yet still send your DNS queries in plain text!

**Application Name:** pihole DoT/DoH

**Application Site:** https://github.com/devzwf/pihole-dot-doh

**[`^back to top^`](#unraid-templates)**

# pihole-sync-receiver

![pihole-sync-receiver](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/pihole-logo-bw.png)

A Pihole runs your entire network. If it goes down, your whole network goes down. If you have a family at home, they're going to be pretty annoyed that the wifi goes out everytime you want to do some maintainence. The only solution to this problem is to have a redundant pihole on your network, but you don't want to change your settings in two different places.

This repo allows you to synchronize between two piholes where one is the master and one is the slave. I'll be adding support for more piholes in future. Just update one pihole and the rest automatically update. It supports the /etc/pihole/ and /etc/dnsmasq.d/ directories, excluding some directories which should be client-independent.

**Application Name:** pihole-sync

**Application Site:** https://github.com/ShiromMakkad/docker-pihole-sync

**[`^back to top^`](#unraid-templates)**

# pihole-sync-sender

![pihole-sync-sender](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/pihole-logo-bw.png)

A Pihole runs your entire network. If it goes down, your whole network goes down. If you have a family at home, they're going to be pretty annoyed that the wifi goes out everytime you want to do some maintainence. The only solution to this problem is to have a redundant pihole on your network, but you don't want to change your settings in two different places.

This repo allows you to synchronize between two piholes where one is the master and one is the slave. I'll be adding support for more piholes in future. Just update one pihole and the rest automatically update. It supports the /etc/pihole/ and /etc/dnsmasq.d/ directories, excluding some directories which should be client-independent.

**Application Name:** pihole-sync

**Application Site:** https://github.com/ShiromMakkad/docker-pihole-sync

**[`^back to top^`](#unraid-templates)**

# postfixrelay

![postfixrelay](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/postfix-logo.gif)

    This runs Postfix (as a relay) in Docker.
    - Most home ISPs block port 25, so outbound emails must be relayed through an external SMTP server (e.g., Gmail).
    - This container acts as a single collections point for devices needing to send email.
    - ⚠️ Postfix acts as an open relay. As such, this is not meant to be run on the internet, only on a trusted internal network! ⚠️
    - You must already have a account on an external SMTP server (e.g., Gmail, AWS SES, etc...).
    - Your external SMTP server must be using encryption (i.e., plaintext is not allowed)

**Application Name:** Postfix-Relay

**Application Site:** https://github.com/loganmarchione/docker-postfixrelay

**[`^back to top^`](#unraid-templates)**

# proxmox-backup-server dockerfiles

![proxmox-backup-server](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/pbs-logo.jpg)

    This is an unofficial compilation of Proxmox Backup Server to run it in a container for AMD64 and ARM64.

    Running in a container might result in some functions not working properly. Feel free to create an issue to debug those.

**Application Name:** proxmox-backup-server

**Application Site:** https://github.com/ayufan/pve-backup-server-dockerfiles

**Documentation** https://pbs.proxmox.com/docs/

**[`^back to top^`](#unraid-templates)**

# proxmox-datacenter-manager

![proxmox-datacenter-manager](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/pdm-logo.jpg)

     This a unofficial dockerized version of the [Proxmox Datacenter Manager](https://forum.proxmox.com/threads/proxmox-datacenter-manager-first-alpha-release.159323) (PDM)
     
     This is an Alpha preview

**Application Name:** proxmox-datacenter-manager

**Application Site:** https://forum.proxmox.com/threads/proxmox-datacenter-manager-first-alpha-release.159323


**[`^back to top^`](#unraid-templates)**


# silverbullet

![silverbullet](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/silverbullet-logo.png)

SilverBullet is a note-taking application optimized for people with a [hacker mindset](https://en.wikipedia.org/wiki/Hacker). We all take notes. There’s a million note taking applications out there. [Literally](https://www.noteapps.ca/). Wouldn’t it be nice to have one where your notes are _more_ than plain text files? Where your notes essentially become a _database_ that you can query; that you can build custom knowledge applications on top of?

**Application Name:** silverbullet

**Application Site:** https://github.com/silverbulletmd/silverbullet

**Documentation** https://silverbullet.md/

**[`^back to top^`](#unraid-templates)**

# speedtest-tracker

![speedtest-tracker](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/speedtest-tracker-icon.png)

A Docker image to check your internet speed using Ookla's Speedtest service. Build using Laravel and the Speedtest CLI.

Speedtest Tracker is a self-hosted internet performance tracking application that runs speedtest checks against Ookla's Speedtest service.

**Application Name:** speedtest-tracker

**Application Site:** https://github.com/alexjustesen/speedtest-tracker

**Documentation** https://docs.speedtest-tracker.dev/

**[`^back to top^`](#unraid-templates)**

# tasks.md

![tasks.md](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/tasks_md_logo.png)

A self-hosted, Markdown file based task management board.

**Application Name:** tasks.md

**Application Site:** https://github.com/BaldissaraMatheus/Tasks.md

**[`^back to top^`](#unraid-templates)**

# Vouchervault

![vouchervault](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/vouchervault-logo.png)

Django web application to store and manage vouchers, coupons, loyalty and gift cards digitally

**Application Name:** Vouchervault

**Images repository** https://github.com/l4rm4nd/VoucherVault

**Application Site:** https://github.com/l4rm4nd/VoucherVault

**[`^back to top^`](#unraid-templates)**

# wallos

![wallos](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/wallos.png)

Wallos is a powerful, open-source, and self-hostable web application designed to empower you in managing your finances with ease. Say goodbye to complicated spreadsheets and expensive financial software – Wallos simplifies the process of tracking expenses and helps you gain better control over your financial life.

**Application Name:** wallos

**Application Site:** https://github.com/ellite/Wallos

**[`^back to top^`](#unraid-templates)**
