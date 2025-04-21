---
title: "Wazuh Server Installation and Configuration"
date: 2025-04-20 09:00:00 +0700
categories: [Project Set Up]
layout: post
---

In this post I will explain how to install Wazuh Server, which we will use as our SIEM.

We will use an Ubuntu Server for it. Once we have installed the server we can follow the installation of Wazuh from the official page:

https://documentation.wazuh.com/current/installation-guide/wazuh-server/installation-assistant.html

It's pretty straightforward, just download the installation script:

curl -sO https://packages.wazuh.com/4.11/wazuh-install.sh

And then install it:

sudo bash wazuh-install.sh -a

The -a flag is used to install all of its components (manager, indexer and dashboard)

Once we finish the installation it will give us the credentials:

![Wazuh Creds](/assets/images/finish-install.JPG)

Once we have done that we can install the agent on Windows 10, just need to download the installer and install it, once we have it we can open it to configure it, we will need the Manager IP and the Authentication Key, for the Manager IP we will put the Wazuh Server IP (192.168.56.20) and for the Authentication Key we will need to register the agent first, so we have to head back to our Wazuh Server.

Once in the Wazuh Server we need to add the agent, to do that, we will use the manage_agents tool. Once inside the tool we add it and after that we extract it's key as you can see in the follow image:

![Add Agent](/assets/images/add-agent.JPG)

We now put the IP and the key in the Windows 10 agent:

![Agent Credentials](/assets/images/agent-creds.JPG)

I will use the same Windows 10 to see if I can access the web interface.

We will need to login, once we do we will see the home dashboard:

![Wazuh Dashboard](/assets/images/wazuh-dashboard.JPG)

That's all for the basic configuration, I've had some compatibility problems while installing the manager and the agent, have to make sure we are using the same version for both (4.11 in my case).
