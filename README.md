# ZappyZap Unraid Community Apps

A curated collection of Unraid Docker template XML definitions maintained by `devzwf`.


## Current templates

This repository currently includes templates for the following apps:

- [Bambuddy](templates/bambuddy.xml) — A powerful, self-hosted print archive and management system for Bambu Lab 3D printers. No cloud dependency, complete privacy, full control. NOTE: This container MUST run in HOST...  
    - [Project](https://bambuddy.cool/index.html) · `ghcr.io/maziggy/bambuddy:latest`
- [Bichon](templates/bichon.xml) — Bichon is an open-source email archiving system that synchronizes emails from IMAP servers, indexes them for full-text search, and provides a REST API for programmatic access.  
    - [Project](https://github.com/rustmailer/bichon) · `rustmailer/bichon:latest`
- [Binner](templates/binner.xml) — Binner is a free open-source parts inventory tracking system you can run locally in Windows or Unix environments. It was created for makers (like myself), hobbyists or professionals to keep track of your parts inventory.  
    - [Project](https://github.com/replaysMike/Binner) · `devzwf/binner:latest`
- [birdnet-go](templates/birdnet-go.xml) — BirdNET-Go is an AI solution for continuous avian monitoring and identification 24/7 realtime bird song analysis of soundcard capture, analysis output to log file, SQLite or MySQL...  
    - [Project](https://github.com/tphakala/birdnet-go) · `ghcr.io/tphakala/birdnet-go:nightly`
- [blocky](templates/blocky.xml) — Blocky is a DNS proxy and ad-blocker for the local network written in Go Create new config.yaml with your configuration ( see https://0xerr0r.github.io/blocky/configuration/ for...  
    - [Project](https://github.com/0xERR0R/blocky) · `spx01/blocky`
- [Bootimus](templates/boutimus.xml) — A production-ready, self-contained PXE and HTTP boot server written in Go with embedded iPXE bootloaders, SQLite/PostgreSQL support, and a full-featured web admin interface. Dep...  
    - [Project](https://bootimus.com/) · `garybowers/bootimus:latest`
- [Cups-Airprint](templates/cups-airprint.xml) — CUPS instance that is meant as an AirPrint relay for printers that are already on the network but not AirPrint capable. CUPS supports printing to: AirPrint™ and IPP Everywhere™...  
    - [Project](https://github.com/chuckcharlie/cups-avahi-airprint) · `chuckcharlie/cups-avahi-airprint:latest`
- [databasement](templates/databasement.xml) — Databasement is a web application for managing database server backups. It allows you to register database servers (MySQL, PostgreSQL, MariaDB), test connections, schedule autom...  
    - [Project](https://github.com/David-Crty/databasement) · `davidcrty/databasement:latest`
- [Dbackup](templates/dbackup.xml) — DBackup is a comprehensive, self-hosted backup solution designed to automate and secure your database backups. It provides AES-256-GCM encryption, flexible storage options, and...  
    - [Project](https://dbackup.app/) · `skyfay/dbackup:latest`
- [Docmost](templates/docmost.xml) — Open-source collaborative wiki and documentation software Create, collaborate, and share knowledge seamlessly with Docmost. Ideal for managing your wiki, knowledge-base, documen...  
    - [Project](https://github.com/docmost/docmost) · `docmost/docmost:latest`
- [DumbDrop](templates/dumbDrop.xml) — A stupid simple file upload application that provides a clean, modern interface for dragging and dropping files. Built with Node.js and vanilla JavaScript.  
    - [Project](https://github.com/DumbWareio/DumbDrop) · `dumbwareio/dumbdrop:latest`
- [DumbKan](templates/dumbKan.xml) — A lightweight, mobile-friendly Kanban board application for managing tasks and projects. Built with vanilla JavaScript and Node.js.  
    - [Project](https://github.com/DumbWareio/DumbKan) · `dumbwareio/dumbkan:latest`
- [DumbPad](templates/dumbPad.xml) — A stupid simple, no auth (unless you want it!), modern notepad application with auto-save functionality and dark mode suppo rt..  
    - [Project](https://github.com/DumbWareio/DumbPad) · `dumbwareio/dumbpad:latest`
- [DumbAssets](templates/dumbassets.xml) — A stupid simple asset tracker for keeping track of your physical assets, their components, and applicable warranties and routine maintenance.  
    - [Project](https://github.com/DumbWareio/DumbAssets) · `dumbwareio/dumbassets:latest`
- [DumbBudget](templates/dumbbudget.xml) — A simple, secure personal budgeting app with PIN protection. Track your income and expenses with a clean, modern inte rface.  
    - [Project](https://github.com/DumbWareio/DumbBudget) · `dumbwareio/dumbbudget:latest`
- [DumbDo](templates/dumbdo.xml) — A stupidly simple todo list application that just works. No complex database, no unnecessary features - just todos.  
    - [Project](https://github.com/DumbWareio/DumbDo) · `dumbwareio/dumbdo:latest`
- [DumbTerm](templates/dumbterm.xml) — A stupidly simple web-based terminal emulator, with common tools and Starship enabled! 🚀  
    - [Project](https://github.com/DumbWareio/DumbTerm) · `dumbwareio/dumbterm:latest`
- [DumbWhoIs](templates/dumbwhois.xml) — A simple web application for looking up WHOIS, IP, and ASN information using free APIs. The application automatically detects the type of query and provides formatted results wi...  
    - [Project](https://github://github.com/DumbWareio/DumbWhoIs) · `dumbwareio/dumbwhois:latest`
- [Glance](templates/glance.xml) — What if you could see everything at a... Glance  
    - [Project](https://github.com/glanceapp/glance) · `glanceapp/glance`
- [Hawser](templates/hawser.xml) — Remote Docker agent for (https://dockhand.pro) - manage Docker hosts anywhere. Hawser is a lightweight Go agent that enables Dockhand to manage Docker hosts in various network c...  
    - [Project](https://dockhand.pro/) · `ghcr.io/finsys/hawser:latest`
- [Homebox](templates/homebox.xml) — Homebox is the inventory and organization system built for the Home User! With a focus on simplicity and ease of use, Homebox is the perfect solution for your home inventory, or...  
    - [Project](https://github.com/sysadminsmedia/homebox) · `ghcr.io/sysadminsmedia/homebox:latest`
- [hydroqc2mqtt](templates/hydroqc2mqtt.xml) — This project was created to provide a way to access Hydro-Québec account and winter credit data in Home-Assistant. This module use the hydroqc library to fetch all pertinent acc...  
    - [Project](https://hydroqc.ca/) · `registry.gitlab.com/hydroqc/hydroqc2mqtt:latest`
- [iventoy](templates/iventoy.xml) — iVentoy is an enhanced version of the PXE server. With iVentoy you can boot and install OS on multiple machines at the same time through the network. iVentoy is extremely easy t...  
    - [Project](https://www.iventoy.com/en/index.html) · `devzwf/iventoy:latest`
- [Juicepass2mqtt](templates/juicepass2mqtt.xml) — This tool will publish Juicebox data from a UDP proxy to MQTT discoverable by HomeAssistant. Hopefully we won't need this if EnelX fixes their API! It is required that both your...  
    - [Project](https://github.com/snicker/juicepassproxy) · `ghcr.io/snicker/juicepassproxy:latest`
- [lightnvr](templates/lightnvr.xml) — LightNVR is a tiny, memory-optimized Network Video Recorder software written in C. While originally designed for resource-constrained devices like the Ingenic A1 SoC with only 2...  
    - [Project](https://github.com/opensensor/lightNVR) · `ghcr.io/opensensor/lightnvr`
- [LubeLogger](templates/lubelogger.xml) — A self-hosted, open-source vehicle service records and maintainence tracker.  
    - [Project](https://github.com/hargata/lubelog) · `ghcr.io/hargata/lubelogger:latest`
- [M.I.M.O.S.A](templates/mimosa.xml) — MIMOSA - short for "Mellow_Labs Inventory Management and Organization System Apparatus". Just like a refreshing mimosa, this system will make your life brighter and more organiz...  
    - [Project](https://github.com/FireMarshmellow/M.I.M.O.S.A) · `devzwf/mimosa:latest`
- [MySpeed](templates/myspeed.xml) — MySpeed is a Software that helps you keeping track of your network speed. It automatically creates speedtests based on your schedule and displays them in a list.  
    - [Project](https://myspeed.dev/) · `germannewsmaker/myspeed`
- [nebula-sync](templates/nebula-sync.xml) — Synchronize Pi-hole v6.x configuration to replicas. This project is not a part of the official Pi-hole project, but uses the api provided by Pi-hole instances to perform the syn...  
    - [Project](https://github.com/lovelaze/nebula-sync) · `ghcr.io/lovelaze/nebula-sync:latest`
- [Nutify](templates/nutify.xml) — Nutify is a comprehensive monitoring system designed to track the health and performance of your Uninterruptible Power Supply (UPS) devices. It provides real-time insights into...  
    - [Project](https://github.com/DartSteven/Nutify) · `dartsteven/nutify:amd64-latest`
- [Onedev](templates/onedev.xml) — OneDev is an all-in-one DevOps platform that features Git repository management with language-aware code search, issue management with custom states and fields, and a docker-fir...  
    - [Project](https://code.onedev.io/projects/160) · `1dev/server`
- [pihole-dot-doh](templates/pihole-dot-doh.xml) — Pi-Hole - let's block those pesky ads! Now with DNS-over-HTTPS and DNS-over-TLS! pihole.doh! Don't send your DNS queries in plain text. YOU MUST ASSIGN A STATIC IP TO THE DOCKER...  
    - [Project](https://docs.pi-hole.net/guides/dns-over-https/) · `devzwf/pihole-dot-doh:latest`
- [Pihole-Sync-receiver](templates/pihole-sync-receiver.xml) — A Docker Container To Sync Two Piholes. This is the Receiver/Secondary, you will need a Sender/Master on the host who is running the Sender/Master Pi-Hole. NOTE: The sending and...  
    - [Project](https://github.com/ShiromMakkad/docker-pihole-sync) · `shirom/pihole-sync:latest`
- [Pihole-Sync-Sender](templates/pihole-sync-sender.xml) — A Docker Container To Sync Two Piholes. This is the Sender/Master, you will need a receiver/secondary on the host who is running the receiver/secondary Pi-Hole. Note: after star...  
    - [Project](https://github.com/ShiromMakkad/docker-pihole-sync) · `shirom/pihole-sync:latest`
- [Postfix-Relay](templates/postfixrelay.xml) — This runs Postfix (as a relay) in Docker. Most home ISPs block port 25, so outbound emails must be relayed through an external SMTP server (e.g., Gmail). This container acts as...  
    - [Project](https://github.com/loganmarchione/docker-postfixrelay) · `loganmarchione/docker-postfixrelay:latest`
- [proxmox-backup-server](templates/proxmox-backup-server.xml) — Proxmox Backup Server in a Container This is an unofficial compilation of Proxmox Backup Server to run it in a container for AMD64 and ARM64. Running in a container might resu lt...  
    - [Project](https://github.com/ayufan/pve-backup-server-dockerfiles) · `ayufan/proxmox-backup-server:latest`
- [proxmox-datacenter-manager](templates/proxmox-datacenter-manager.xml) — Proxmox Datacenter Manager A stand-alone API + GUI product with the following main features for multiple instances of Proxmox VE, Proxmox Backup Server and potentially also Prox...  
    - [Project](https://github.com/proxmox/proxmox-datacenter-manager) · `devzwf/proxmox-datacenter-manager:latest`
- [Pulse](templates/pulse.xml) — Real-time monitoring for Proxmox VE, Proxmox Mail Gateway, PBS, and Docker infrastructure with alerts and webhooks. Monitor your hybrid Proxmox and Docker estate from a single d...  
    - [Project](https://github.com/rcourtman/Pulse) · `rcourtman/pulse:latest`
- [silverbullet](templates/silverbullet.xml) — SilverBullet is a note-taking application optimized for people with a [hacker mindset](https://en.wikipedia.org/wiki/Hacker). We all take notes. There’s a million note taking ap...  
    - [Project](https://silverbullet.md/) · `zefhemel/silverbullet`
- [sketchforge](templates/sketchforge.xml) — A local-first 3D design editor that runs in your browser. Build shapes, cut holes, group parts, import STL files, and export models without accounts, cloud lock-in, or heavyweig...  
    - [Project](https://github.com/Formsmith746/SketchForge-3D) · `ghcr.io/formsmith746/sketchforge-3d:latest`
- [tasks.md](templates/tasks-md.xml) — A self-hosted, Markdown file based task management board.  
    - [Project](https://github.com/BaldissaraMatheus/Tasks.md) · `baldissaramatheus/tasks.md`
- [Termix](templates/termix.xml) — Termix is an open-source forever free self-hosted SSH (other protocols planned, see Planned Features) server management panel inspired by Nexterm. Its purpose is to provide an a...  
    - [Project](https://github.com/LukeGus/Termix) · `ghcr.io/lukegus/termix:latest`
- [unifi-toolkit](templates/unifi-toolkit.xml) — A comprehensive suite of tools for UniFi network management and monitoring.  
    - [Project](https://github.com/Crosstalk-Solutions/unifi-toolkit) · `ghcr.io/crosstalk-solutions/unifi-toolkit:latest`
- [VoucherVault](templates/vouchervault.xml) — Django web application to store and manage vouchers, coupons, loyalty and gift cards digitally Once the container is up and running, you can access the web portal at http://127....  
    - [Project](https://github.com/l4rm4nd/VoucherVault) · `l4rm4nd/vouchervault:1.5.x`
- [Wallos](templates/wallos.xml) — Wallos is a powerful, open-source, and self-hostable web application designed to empower you in managing your finances with ease. Say goodbye to complicated spreadsheets and exp...  
    - [Project](https://hub.docker.com/r/bellamy/wallos) · `bellamy/wallos:latest`
- [zerobyte](templates/zerobyte.xml) — Zerobyte is a backup automation tool that helps you save your data across multiple storage backends. Built on top of Restic, it provides an modern web interface to schedule, man...  
    - [Project](https://github.com/nicotsx/zerobyte) · `ghcr.io/nicotsx/zerobyte:latest`

## Guides

This repository contains quick-start and configuration guides in the `guides/` folder. Each guide includes step-by-step instructions and example commands.

- [Quick Start: Docmost](guides/Quick-Start-Guide-Docmost.md) — Steps to install Redis, PostgreSQL and Docmost, configure secrets, and start the web UI.  
    - See `guides/Quick-Start-Guide-Docmost.md`
- [Quick Start: UniFi Toolkit](guides/Quick-Start-Guide-Unifi-toolkit.md) — Install UniFi Toolkit, set permissions, generate an encryption key, and finalize setup with optional video walkthrough.  
    - See `guides/Quick-Start-Guide-Unifi-toolkit.md`
- [Quick Start: Pi-hole Sync](guides/Quick-Start-Guide-pihole-sync.md) — Guide to install and configure Pi-hole sync sender/receiver containers, SSH key setup, and using symlinks for production sync.  
    - See `guides/Quick-Start-Guide-pihole-sync.md`

For full list and additional notes, see [guides/README.md](guides/README.md).

## License

This repository is licensed under the [MIT License](LICENSE).

## Support

If you have questions or want to request a new app template, open an issue in this repository.

For best results, donate to the upstream app creators first, and support template maintenance through the repo issue tracker.
