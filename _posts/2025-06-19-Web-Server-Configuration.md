---
title: Web Server Configuration
description: Manual on how to install the vulnerable web site in our Web Server
date: 2025-04-20 09:00:00 +0700
categories: [Project Set Up]
layout: post
---

Now it's time to set up our web server.

For this we will download an Ubuntu Server and set it up in a different subnet, an we will install the famous Juice Shop from OWASP in it which is a website with many known vulnerabilities in it so we can further practice our attacks and defenses.

I'll not cover here how to install the Ubuntu Server, once we have it in a VM we will the proceed to install what we need for the website.

First we will head to the documentation:

[Juice Shop]https://github.com/juice-shop/juice-shop

Here we can find that we need to install node.js first, to install it we will use apt:

![Node.js](/assets/images/nodejs.PNG)

If we want to make sure it's installed we can use:

```
node-v
```

This will give us back the version of node installed.

After we have installed node.js we can then clone the repository with all the files needed to run the website, for that we will use git clone:

```
git clone https://github.com/juice-shop/juice-shop.git --depth 1
```

![Download Juice Shop](/assets/images/download_juiceshop.PNG)

Then we just need to go into the directory and install it with:

````
cd juice-shop

npm install

```

![Install Juice Shop](/assets/images/npminstall.PNG)

After the installation is complete it will show us the amount of vulnerabilities in the website:

![Vulnerabilities](/assets/images/vulnerabilities.PNG)

After that we can just start our website with ``` npm start ``` :

![NPM Start](/assets/images/npmstart.PNG)

We then will see that our website is running on port 3000.

We can go and check it out from our Windows 11 machine for example.

We will see that it already displays the website:

![JuiceShop Website](/assets/images/juiceshoppage.PNG)