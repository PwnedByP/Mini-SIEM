---
title: Windows 10 Configuration
description: Basic configuration of the W10 machine
date: 2025-04-19 17:00:00 +0700
categories: [Project Set Up]
layout: post
---

Once we have our Windows 10 installed we will have to join it to the domain.

To do that we need to go to This PC and click to Properties:

![Proerties](/assets/images/properties.JPG)

Once we are here we can go to Rename this PC (advanced)

![Advanced](/assets/images/advanced.JPG)

Then we will change the name of the computer and the Domain:

![Change](/assets/images/change.JPG)

We then rename it to PC01 and put the name of our domain:

![Rename](/assets/images/rename.JPG)

Once we have it it will ask us for a login, we will login with john's account

![John Login](/assets/images/john-login.JPG)

It will welcome us to the domain and it will ask us to restart to apply the changes, what we then do.

We will then login with other user and will introduce john's user:

![Other User](/assets/images/other-user.JPG)

We can now see that we are logged in as jsmith and we are part of the domain:

![John](/assets/images/john.JPG)

That's all the initial configuration needed for our Windows client.