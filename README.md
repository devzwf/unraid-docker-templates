# devzwf's unraid docker templates

Template for Docker Containers to use UnRaid

Templates for adding containers to unRAID via more GUI-friendly way and allowing easier updates in the future.
The docker containers referenced in this repo point to Docker Containers maintained by other individuals.

# Unraid Templates

- [hydroqc2mqtt](#hydroqc2mqtt)

---

# hydroqc2mqtt

![hydroqc2mqtt](https://raw.githubusercontent.com/devzwf/unraid-docker-templates/main/images/hydroqc-logo.png)

This project was created to provide a way to access Hydro-Québec account and winter credit data in Home-Assistant.
This module use the hydroqc library to fetch all pertinent account information and winter credit signals to be sent to MQTT. It also provide Home-Assistant discovery topics to create all the relevant sensors in Home-Assistant.
It also includes a separate logic that sends the hourly consumption statistics to Home-Assitant via websocket

**Application Name:** hydroqc2mqtt

**Application Site:** https://hydroqc.ca/

**[`^back to top^`](#unraid-templates)**
