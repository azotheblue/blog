---
layout: post
title: Security Onion - Playbook Creation
date: 2024-03-01 21:00:00
categories: securityonion
excerpt_separator: <!--more-->
---

Let's peel back another layer for Security Onion by using Playbook!

## SECURITY ONION

Before diving into how to set up playbook on on Security Onion, it would probably be a good idea to explain what in the world a Security Onion is.  Security Onion is a fantastic open source Cyber Defense Tool.  It provides many of the needed tools and functionality need for a Security Operations Team to operate, all in a single package.   I personally have been using it since 2016 and have seen the great improvements the Security Onion Team has made over the years.  

I won't be going in detail over what Security Onion is, how to setup it up, and detailed functionality. I will however be zooming into one area of the tool, **Playbooks**.  If you would like more information, please visit the below resources

- [Youtube - Playlist for 2.4 Essentials](https://www.youtube.com/watch?v=ITuVYSxAna4&list=PLljFlTO9rB17azL-HwV4BUWUv7Egmcx3T&ab_channel=SecurityOnion)
- [Docs - Security Onion Docs](https://docs.securityonion.net/en/2.4/)

## PLAYBOOK

Let's Dive in.  

First let me describe what a playbook from Security Onion

> Playbook allows you to create a Detection Playbook, which itself consists of individual plays. These plays are fully self-contained and describe the different aspects around the particular detection strategy.

Initially, Security Onion comes defaulted with lots of Suricata rules for network based detection.  However, if you wanted to detect on endpoint activities, this is where Playbook comes in to ... play.  Playbook allows you to alert on basically any log that you Security Onion Instances receives.  

In the most recent update, 2.4, Security Onion has switched from Wazuh to the Elastic Agent.  This allows for a very robust logging from an endpoint.  Which in returns provides more areas for detection.

One other note, playbook is utilizes Sigma.  In essences, Sigma is nothing more than a `.yml` file.  However, Sigma is a great provides a standardized way to share detection content and provides interoperability with other SIEM tools.  

- [Website - More Info on Sigma](https://socprime.com/blog/sigma-rules-the-beginners-guide/)

## PLAYBOOK - HOW TO SETUP 

*(Note this blog is not going to go through how to setup an Security Onion Infrastructure, just the setups for a Playbook.  Future blog material 🤷)*

Lets say for some reason we wanted to detect when someone used the `base64` command on a host.  Obviously this is not an high priority threat and is likely common based. Just picked this one based on its simplicity to reproduce in my lab environment. This might deviate from official documentation, but these are the steps I took to create a Playbook.  Furthermore, if you would like to view the rule I used view it below

[Github - Sigma Rule for Base64](https://github.com/SigmaHQ/sigma/blob/6b8cd1f0f1d222dcffa95394b4cbcec2a05137a0/rules/linux/process_creation/proc_creation_lnx_base64_decode.yml)


1 **Click Playbook**

![Security Onion Playbook - Step 1](/blog/assets/ONION-PLAYBOOK-STEP1.GIF)

2 **Create New Play**

![Security Onion Playbook - Step 1](/blog/assets/ONION-PLAYBOOK-STEP2.JPG)

 3 **Submit the Play**

![Security Onion Playbook - Step 1](/blog/assets/ONION-PLAYBOOK-STEP3.JPG)

4 **Active the Play**

![Security Onion Playbook - Step 1](/blog/assets/ONION-PLAYBOOK-STEP4.JPG)


5 **Wait for Evil**

![Security Onion Playbook - Step 1](/blog/assets/ONION-PLAYBOOK-STEP5.JPG)


## CONCLUSION

In closing, playbooks help extension the detection frontier for Security Onion.  

This was more or less a way for me to explore how to setup and turn on a Playbook.  This was something I wanted to research for a while, and I figured writing a blog about it was the best way to do it.  

Hope you enjoyed!