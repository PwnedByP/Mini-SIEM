---
title: "Windows 10 Pro VM"
date: 2025-04-19 09:00:00 +0700
categories: [Project Set Up]
layout: post
---

We are going to install a Windows 10 VM (simulating a worker in the company)

I've had problems in the past installing it because it required to add the Trusted Platform Module (TPM).

I'll explain you here how to add it, first you need to encrypt the disk:

![Encrypt Disk](/assets/images/Windows10-en.JPG)

Once you have done that it will let you add the Module:

![TPM](/assets/images/TPM.JPG)

Once this is done you can go ahead and install Windows 10. I'm installing the Pro N version on this lab.