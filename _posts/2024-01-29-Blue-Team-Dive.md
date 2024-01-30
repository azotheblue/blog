---
layout: post
title: A Way To Organize Board Games
date: 2024-01-29 17:00:00
categories: cyber
excerpt_separator: <!--more-->
---

Go Blue Team! But who is in it? 

## WHATS IN A BLUE TEAM?

If you are in the cybersecurity  space, you have likely heard of the Blue Team / Red Team monikers.   These are pretty well known in the space for describing defensive vs offensive activities in a organization. For the most part, I believe they do a good job representing two sides of Cyber Security.    

However, I think there is a lot to unpack when one says Blue Team.  I want to dive into what makes up a Blue Team, based on my opinion and experience.  This is by no means a well-tested and validated team format.  Think of this of more a thought exercise.  

## THE BREAKDOWN

This is not a exhaustive list of every entity within a Blue Team.  There are a few more that could probably add but for now let's keep it simple shall we. (Future blog idea 🤔) 

Teams included: 

🎯 Hunt
⚙️ Detection Engineering
🔍 SOC
🔒 DFIR
🌍 Threat Intel

Let's break down each team and their function within a Blue Team

🎯 Hunt

- Hunt Teams lives in the discovery land.  They mostly live in the past. Hunt teams  tries to find evidence of malicious behavior that goes undetected  through deep analysis and research.  Usually their findings will produce more alerts or recommendation for the organization.

⚙️ Detection Engineering

- This is the Team that build the detections for the SOC.  They are responsible for creating, tuning, and enhancing the logic, alerts that the SOC consumes.  Their work is often depending on the Threat Intel Teams feeding them new content and the SOC tuning existing content

🔍 SOC

- This team consumes the products that the Detection Engineering team creates.  The SOC is the last line of defense for any Organization.  Once the SOC determines an alert that fires is a true positive variety, they would escalate this to the DFIR Team

🔒 DFIR

-  The DFIR team's job is to stop and prevent adversaries in their tracks and clean up their mess. A DFIR team should move fast and calm during an incident.  This team might also investigations into internal users as well. 

🌍 Threat Intel

- One team that doesn't get talked about enough is the Cyber Threat Intel team. In my opinion, this team should be involved in all parts cyber.  They should be able to provide meaningful input to any team. Their connection to the happenings in the cyber space can be relevant during all phases of an incident. 

When we put these all together we get *(Que the fancy graphic)*

![Blue Team Graphic](/blog/assets/BLUETEAM-DIAGRAM.PNG)


## CONCLUSION 

Although this isn't going to change the defensive cyber landscape, I thought it was a good exercise to describe a blue team more in depth.    Hopefully now when someone says "Blue Team", this will help fill in the gaps a bit more.   