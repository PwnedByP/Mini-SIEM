---
title: "List of VMs used in the lab"
date: 2025-04-19 10:00:00 +0700
categories: [Project Set Up]
layout: post
---

The list of the VMs that we are going to use in the lab is the next one:

- Windows Server 2019 (AD)
- Windows 10 (Simulating a worker)
- Ubuntu Server(Wazuh Server, SIEM)
- Ubuntu Server(Web Server)
- Kali Linux (Attacker Machine)

We want to simulate a company with a server (WS2019) and a user (W10), our SIEM (Ubuntu Server), a web server with a vulnerable website (Ubuntu Server) and an attacker (Kali Linux).

It might be useful to add an extra machine with pfSense for a firewall but I will keep it simple first and do it without it.