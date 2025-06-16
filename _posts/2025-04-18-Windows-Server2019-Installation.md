---
title: Installing Windows Server 2019 in VMWare
description: Installation manual of the WS2019 VM
date: 2025-04-18 12:00:00 +0700
categories: [Project Set Up]
layout: post
---

I will make a dedicated post for this since I've found some problems while trying to install Windows Server 2019 in VMWare.

First we will download the ISo image from the official website: https://www.microsoft.com/en-us/evalcenter/download-windows-server-2019

We can get 180 days to try it for free so we don't need to pay for the license.

If we try to add it and install it like usually in VMWare I'm finding the next error: "Windows cannot find the microsoft software license terms."

So I've made some research and instead of installing it the "easy way" we will use another approach.

We just need to select that we will install the OS later:

![Manual installation](/assets/images/Manually.JPG)

After that we can just go to manage our machine before powering up and select the file where the ISO with the Windows Server 2019 is:

![Select the ISO](/assets/images/Select.JPG)

After that we can start the machine and it should work without any further problems.