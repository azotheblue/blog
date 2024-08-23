---
layout: post
title: What Makes A Good Detection
date: 2024-08-2 22:00:00
categories: cyber
excerpt_separator: <!--more-->
---

"An ounce of prevention is worth a pound of cure." - Benjamin Franklin

<!--more-->

# INTRODUCTION

A detection is the lifeblood of any cyber security operations.  It is how an organizations knows that evil has occurred within an environment.  **But have you ever wondered, what makes a good detection?**  Working in the queues as a Security Operations Center (SOC) Analyst, I had a idea what made a bad one.  Since transitioning to the role of a Detection Engineer, I my mindset  has changed to what makes a good one!

First before going into my dissertation, it might be a good idea in to bring in the definition of a detection, specifically a threat detection.  There are many out there so this is a combination of a few. 

> A cyber threat detection is the  identification of potential security risks to  prevent or mitigate cyberattacks.

With this, let's move on!

# WHAT'S IN A DETECTION?

Given my journey in switching from a negative frame of mind to a positive one, I wanted to include both ends of the spectrum.   There are 3 pieces of the detection Puzzle.  


🗃️ **Context** - This piece represent the "why" of an alert.  This also represent the surrounding documentation of the alert and following actions to research. 

💥 **Potency** - Is the ability for a detection to find it was intended to find without noise.

🎖️ **Confidence** - A detection is trustworthy if we know that it been put through rigorous validation

It not might be feasible to accomplish all the pieces but these are nice goal post 🥅

With this pieces below is a scale to put it all together!

| Topic      | Bad                                    | Good                                         |
| ---------- | -------------------------------------- | -------------------------------------------- |
| Context    | No Context for Alerting                 | Lot of surrounding data to understand the alert |
| Potency    | Issues with alerting volume      | Detects only when evil happen                |
| Confidence    |    Detect evil 🤷    | Alert has been rigorously tested and validated |

# WHAT DOES IT MEAN?

Ideally, when I build a detection, these are the principles that I try in cooperate into it.  However its might be hard to know what to look for without something to go off of.  So what better way to do this then a checklist ✅! 

**🗃️ Context**
- [ ] Does the alert have a detailed "Why?"
- [ ] Is the following documented?
	- [ ] What does a True Positive look like? 
	- [ ] What does a False Positive look like?
	- [ ] Triage Steps?
	- [ ] References

**💥 Potency**
- [ ] Could the alert produce unwanted noise?
	- [ ] Yes -> Can there be any initial tuning? 
- [ ] Does this detection fit a specific detection need? 
- [ ] Is this a need to have this alert run quickly?
- [ ] Is this alert setup to be reviewed in the  future?

**🎖️Confidence**
- [ ] Has the alert's logic been tested?
- [ ] Has the alert been validated in a Lab Environment or against valid logs?

# CLOSING

An effective detection is vital to any cyber operations team.  My goals was the share my insight and experiences that I have gathered over the few years I can been developing detections.  Hope this helps in your fight to find evil!  