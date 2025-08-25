---
layout: post
title: SKT incident final assessment explained
subtitle: for all to understand
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/thumb.png
share-img: /assets/img/path.jpg
tags: [cellular network]
author: Joonyoung Jeong
---

# Final Report Summary

The Ministry of Science and ICT has released the **final report** on the SKT incident, in which a massive amount of user information was leaked.  
The investigation committee examined **42,605 servers** and identified **33 malware samples**, including **27 BPFDoor variants** found across 33 servers.

The committee also confirmed that **25 different types of USIM-related data** had been leaked, totaling **approximately 9.82 GB** in size.

For further details, please refer to the official report [here](https://www.msit.go.kr/bbs/view.do?sCode=user&mId=307&mPid=208&pageIndex=1&bbsSeqNo=94&nttSeqNo=3185964&searchOpt=ALL&searchTxt).

---

# Attack Chain

### 1. Initial Access
According to the final report, the attacker first compromised the **system management subnet** used for maintenance and operation.  

The committee suggested several possible attack scenarios, including:

- **Exploitation of VPN vulnerabilities:**  
  Taiwan-based cybersecurity company **TeamT5** suggested that vulnerabilities in **Ivanti VPN products** might have been exploited to gain access to the system management subnet.  

  > There is no definitive evidence that SKT was using Ivanti VPN products to operate their servers. Also, SKT has not identified that they are using Ivanti products. However, TeamT5 noted:  
  > *“Since April 2025, multiple devices have been compromised, where Ivanti VPN devices were leveraged in the attack.”*

SKT itself has not confirmed the use of Ivanti VPN products in its 4G/5G architecture. What is confirmed, however, is that the **first anomalous activity** was detected by SKT’s incident response team on **April 18**, originating from a **Linux-based charging analysis server** located within the VPN route that connected to the internet.
