---
title: 'Weisi Yang presents work on detecting intimate partner infiltrations on smartphones at Discovery Partners Institute'
author: imec
group: recent
image: images/news/04-11-2025/IMG_3456.jpeg
---

{%
  include figure.html
  image="images/news/04-11-2025/IMG_3456.jpeg"
%}

{%
  include figure.html
  image="images/news/04-11-2025/IMG_3455.jpeg"
%}



Weisi Yang presents our work on a [smartphone-based platform for detecting and monitoring intimate partner infiltration](https://arxiv.org/pdf/2502.03682) at the SIGCHI sponsored [Mobile Social Networking Workshop](https://dpi.illinois.edu/wp-content/uploads/2025/03/Call-for-posters-MSN-workshop-at-DPIv2.pdf) at Discovery Partners Institute.

Our work introduces AID (Automated IPI Detection), the first system designed specifically to detect Intimate Partner Infiltration, a class of abuse that slips past traditional cybersecurity defenses because the perpetrator often already has the phone, the passcode, or the victim’s trust.

Rather than treating these incidents as conventional cyberattacks, we formalize a new threat model that captures the reality of intimate partner abuse: attackers are insiders, not hackers, and harm comes from what they do on the phone as much as who is holding it.

Building on this foundation, AID introduces a dual-branch AI architecture that continuously and silently monitors smartphones. One branch determines whether the current user is the device owner or not, while the other infers whether their actions reflect harmful IPI intent. Only when both conditions are met does the system flag risk—dramatically reducing false alarms that could otherwise retraumatize victims or escalate abuse. Crucially, AID runs entirely on-device, relies only on background-accessible signals, and is designed to remain invisible to abusers.

{%
  include figure.html
  image="images/news/04-11-2025/ipv_aid_system_flow-1.png"
  caption="AID system architecture."
%}
