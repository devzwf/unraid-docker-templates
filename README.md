<h1 align="center" id="heading"> devzwf's unraid docker templates </h1>

<a href="https://github.com/devzwf/unraid-docker-templates/blob/main/CHANGELOG.MD"><img src="https://img.shields.io/badge/🔶-Changelog-blue" /></a> <a
href="https://ko-fi.com/O5O0FG195"><img src="https://img.shields.io/badge/%E2%98%95-Buy%20me%20a%20coffee-red" /></a>

Template for Docker Containers to use UnRaid

Templates for adding containers to unRAID via more GUI-friendly way and allowing easier updates in the future.
The docker containers referenced in this repo point to Docker Containers maintained by other individuals.

# Unraid Templates

- [Bambuddy](#bambuddy)
- [Bichon](#bichon) 
- [Binner](#binner)
- [BirdNET-Go](#birdnet-go)
- [Blocky](#blocky)
- [Cups-Airprint](#cups-airprint)
- [Databasement](#databasement)
- [Docmost](#docmost)
- [DumbAssets](#dumbassets)
- [DumbBudget](#dumbbudget)
- [DumbDo](#dumbdo)
- [DumbDrop](#dumbdrop)
- [DumbKan](#dumbkan)
- [DumbPad](#dumbpad)
- [DumbTerm](#dumbterm)
- [DumbWhoIs](#dumbwhois)
- [Glance](#glance)
- [Hawser](#hawser)
- [homebox](#homebox)
- [hydroqc2mqtt](#hydroqc2mqtt)
- [iventoy](#iventoy)
- [juicepass2mqtt](#juicepass2mqtt)
- [lightNVR](#lightnvr)
- [LubeLogger](#lubelogger)
- [M.I.M.O.S.A](#mimosa)
- [Myspeed.dev](#myspeeddev)
- [nebula-sync](#nebula-sync)
- [Onedev](#onedev)
- [pihole DoT/DoH](#pihole-dot-doh)
- [Postfix-Relay](#postfixrelay)
- [proxmox-backup-server](#proxmox-backup-server-dockerfiles)
- [proxmox-datacenter-manager](#proxmox-datacenter-manager)
- [pulse](#pulse)
- [silverbullet](#silverbullet)
- [speedtest-tracker](#speedtest-tracker)
- [tasks.md](#tasksmd)
- [termix](#termix)
- [Vouchervault](#vouchervault)
- [walos](#wallos)
- [Zerobyte](#zerobyte)


---
# Bambuddy

![bambuddy](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/bambuddy-logo.png)

A powerful, self-hosted print archive and management system for Bambu Lab 3D printers. No cloud dependency, complete privacy, full control. 

**Application Name:** bambuddy

**Images repository** https://github.com/maziggy/bambuddy

**Application Site:** https://bambuddy.cool/index.html

**[`^back to top^`](#unraid-templates)**

# Bichon

![bichon](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/bichon-logo.png)

Bichon is an open-source email archiving system that synchronizes emails from IMAP servers, indexes them for full-text search, and provides a REST API for programmatic access. Unlike email clients, Bichon is designed for archiving and searching rather than sending/receiving emails. It runs as a standalone server application that continuously synchronizes configured email accounts and maintains a searchable local archive. Built in Rust, it requires no external dependencies and provides fast, efficient email archiving, management, and search through a built-in WebUI. 

**Application Name:** Bichon

**Images repository** https://github.com/rustmailer/bichon

**[`^back to top^`](#unraid-templates)**

# Binner

![binner](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/binner-logo.png)

Binner is a free open-source parts inventory tracking system you can run locally in Windows or Unix environments. It was created for makers (like myself), hobbyists or professionals to keep track of your parts inventory

**Application Name:** Binner

**Images repository** https://github.com/replaysMike/Binner

**Application Site:** https://binner.io/

**[`^back to top^`](#unraid-templates)**

# BirdNET-Go

![birdnetgo](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/birdnet-go-logo.png)

BirdNET-Go is an AI solution for continuous avian monitoring and identification

* 24/7 realtime bird song analysis of soundcard capture, analysis output to log file, SQLite or MySQL
* Utilizes BirdNET AI model trained with more than 6500 bird species
* Local processing, Internet connectivity not required
* Easy to use Web user interface for data visualisation
* Supports over 40 languages for species names
* Advanced features like Deep Detection for improved accuracy and Live Audio Streaming.
* BirdWeather.com API integration
*  Realtime log file output can be used as overlay in OBS for bird feeder streams etc.
* Minimal runtime dependencies, BirdNET Tensorflow Lite model is embedded in compiled binary
* Provides endpoint for Prometheus data scraping
* Runs on Windows, Linux and macOS
* Low resource usage, works on Raspberry Pi 3 and equivalent 64-bit single board computers

**Application Name:** BirdNET-Go

**Application repository** https://github.com/tphakala/birdnet-go

**Application Site:** https://github.com/tphakala/birdnet-go

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

# Databasement

![databasement](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/databasement-logo.png)

Databasement is a web application for managing database server backups. It allows you to register database servers (MySQL, PostgreSQL, MariaDB), test connections, schedule automated backups, and restore snapshots to any registered server.

**Application Name:** Databasement

**Images repository** https://github.com/David-Crty/databasement

**Application Site:** https://david-crty.github.io/databasement/

**Application Documentation:** https://david-crty.github.io/databasement/

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

# DumbAssets

![dumbassets](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/dumbassets-logo.png)

A stupid simple asset tracker for keeping track of your physical assets, their components, and applicable warranties and routine maintenance.

**Application Name:** DumbAssets

**Images repository** https://github.com/DumbWareio/DumbAssets

**Application Site:** https://www.dumbware.io/

**Application Documentation:** https://github.com/DumbWareio/DumbAssets

**[`^back to top^`](#unraid-templates)**

# DumbBudget

![dumbbudget](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/dumbbudget-logo.png)

A simple, secure personal budgeting app with PIN protection. Track your income and expenses with a clean, modern interface.

**Application Name:** DumbBudget

**Images repository** https://github.com/DumbWareio/DumbBudget

**Application Site:** https://www.dumbware.io/

**Application Documentation:** https://github.com/DumbWareio/DumbBudget

**[`^back to top^`](#unraid-templates)**

# DumbDo

![dumbdo](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/dumbdo-logo.png)

A stupidly simple todo list application that just works. No complex database, no unnecessary features - just todos.

**Application Name:** DumbDo

**Images repository** https://github.com/DumbWareio/DumbDo

**Application Site:** https://www.dumbware.io/

**Application Documentation:** https://github.com/DumbWareio/DumbDo

**[`^back to top^`](#unraid-templates)**

# DumbDrop

![dumbdrop](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/dumbdrop-logo.png)

A stupid simple file upload application that provides a clean, modern interface for dragging and dropping files. Built with Node.js and vanilla JavaScript.

**Application Name:** DumbDrop

**Images repository** https://github.com/DumbWareio/DumbDrop

**Application Site:** https://www.dumbware.io/

**Application Documentation:** https://github.com/DumbWareio/DumbDrop

**[`^back to top^`](#unraid-templates)**

# DumbKan

![dumbkan](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/dumbkan-logo.png)

A lightweight, mobile-friendly Kanban board application for managing tasks and projects. Built with vanilla JavaScript and Node.js.

**Application Name:** DumbKan

**Images repository** https://github.com/DumbWareio/DumbKan

**Application Site:** https://www.dumbware.io/

**Application Documentation:** https://github.com/DumbWareio/DumbKan

**[`^back to top^`](#unraid-templates)**

# DumbPad

![dumbpad](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/dumbpad-logo.png)

A stupid simple, no auth (unless you want it!), modern notepad application with auto-save functionality and dark mode support.

**Application Name:** DumbPad

**Images repository** https://github.com/DumbWareio/DumbPad

**Application Site:** https://www.dumbware.io/

**Application Documentation:** https://github.com/DumbWareio/DumbPad

**[`^back to top^`](#unraid-templates)**

# DumbTerm

![dumbterm](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/dumbterm-logo.png)

A stupidly simple web-based terminal emulator, with common tools and Starship enabled! &#x1F680;

**Application Name:** DumbTerm

**Images repository** https://github.com/DumbWareio/DumbTerm

**Application Site:** https://www.dumbware.io/

**Application Documentation:** https://www.dumbware.io/DumbTerm

**[`^back to top^`](#unraid-templates)**

# DumbWhoIs

![dumbwhois](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/dumbdo-logo.png)

A simple web application for looking up WHOIS, IP, and ASN information using free APIs. The application automatically detects the type of query and provides formatted results with a clean, modern UI that supports both light and dark modes.

**Application Name:** DumbWhoIS

**Images repository** https://github.com/DumbWareio/DumbWhoIs

**Application Site:** https://www.dumbware.io/

**Application Documentation:** https://github.com/DumbWareio/DumbWhoIs

**[`^back to top^`](#unraid-templates)**

# Glance

![glance](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/glance_logo.png)

<p align="center"><em>What if you could see everything at a...</em></p>
<h1 align="center">Glance</h1>

**Application Name:** Glance

**Application Site:** https://github.com/glanceapp/glance

**[`^back to top^`](#unraid-templates)**

# Hawser

![hawser](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/hawser-logo.png)

    Remote Docker agent for [Dockhand](https://dockhand.pro) - manage Docker hosts anywhere.
    Hawser is a lightweight Go agent that enables Dockhand to manage Docker hosts in various network configurations. It supports two operational modes:

    - **Standard Mode**: Agent listens for incoming connections (ideal for LAN/homelab with static IPs)
**Application Name:** Hawser

**Application Site:** https://github.com/Finsys/hawser

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


# LightNVR

![lightnvr](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/lightnvr-logo.png)

LightNVR is a tiny, memory-optimized Network Video Recorder software written in C. While originally designed for resource-constrained devices like the Ingenic A1 SoC with only 256MB of RAM, it can run on any Linux system.&#13;

LightNVR provides a lightweight yet powerful solution for recording and managing IP camera streams. It's designed to run efficiently on low-power, memory-constrained devices while still providing essential NVR functionality with a modern, responsive web interface.
**Application Name:** LightNVR

**Application Site:** https://github.com/opensensor/lightNVR

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
This image also support unbound
nscrypt-proxy for DoH - 127.1.1.1#5153. Uses Cloudflare Security (1.1.1.2 )
stubby for DoT - 127.2.2.2#5253 Uses google (8.8.8.8 / 8.8.4.4) by default
unbound for recursive - 127.0.0.1#5335
**Application Name:** pihole DoT/DoH

**Application Site:** https://github.com/devzwf/pihole-dot-doh

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

# pulse

![pulse](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/pulse-logo.png)

    Real-time monitoring for Proxmox VE, Proxmox Mail Gateway, PBS, and Docker infrastructure with alerts and webhooks.
    Monitor your hybrid Proxmox and Docker estate from a single dashboard. Get instant alerts when nodes go down, containers misbehave, backups fail, or storage fills up. Supports email, Discord, Slack, Telegram, and more.

    [Try the live demo](https://demo.pulserelay.pro/)  (read-only with mock data)

**Application Name:** Pulse
**Application Site:** https://github.com/rcourtman/Pulse


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

# termix

![termix](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/termix_logo.png)

Termix is an open-source forever free self-hosted SSH (other protocols planned, see [Planned Features](#planned-features)) server management panel inspired by [Nexterm](https://github.com/gnmyt/Nexterm). Its purpose is to provide an all-in-one docker-hosted web solution to manage your servers in one easy place. I'm using this project to help me learn [React](https://github.com/facebook/react), [Vite](https://github.com/vitejs/vite-plugin-react), and [Docker](https://www.docker.com) but also because I could never settle on a server management software that I enjoyed to use.

> [!WARNING]  
> This app is in the VERY early stages of development. Expect bugs, data loss, and unexplainable issues! For that reason, I recommend you securely tunnel your connection to Termix through a VPN.

**Application Name:** termix

**Application Site:** https://github.com/LukeGus/Termix

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

# zerobyte

![zerobyte](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/zerobyte-logo.png)

Zerobyte is a backup automation tool that helps you save your data across multiple storage backends. Built on top of Restic, it provides an modern web interface to schedule, manage, and monitor encrypted backups of your remote storage.

Features

- Automated backups with encryption, compression and retention policies powered by Restic
- Flexible scheduling For automated backup jobs with fine-grained retention policies
- End-to-end encryption ensuring your data is always protected
- Multi-protocol support: Backup from NFS, SMB, WebDAV, or local directories

**Application Name:** Zerobyte

**Application Site:** https://github.com/nicotsx/zerobyte

**[`^back to top^`](#unraid-templates)**