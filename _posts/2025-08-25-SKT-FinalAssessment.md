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

The ministry of Science, Technology and Info-Communication has announced the final report regarding the SKT incident, where massive user private information had leaked. The incident committee had examined 42,605 servers
and concluded that it has identified 33 malwares including 27 BPFDoor from 33 servers. 

Also, the committee identified 25 different types of information regarding USIM have been leaked by malwares, where the total size of the leaked data is estimated to be 9.82GB.

For further detailed contents of the report, please refer [here](https://www.msit.go.kr/bbs/view.do?sCode=user&mId=307&mPid=208&pageIndex=1&bbsSeqNo=94&nttSeqNo=3185964&searchOpt=ALL&searchTxt)

# Attack chain
1. Initial access
   According to the final report, the attacker firstly compromised the system management subnet that was for maintenance and operation. The committee suggested possible attack scenarios that include:
   - **Exploiting vulnerability in VPN devices:** Taiwan cybersecurity company, TeamT5, said CVE regarding Ivanti VPN product might have been exploited to access the system management subnet.
     > There is no clear evidence that SKT was using Ivanti VPN products to operate their servers. However TeamT5 revealed that "Since April 2025, multiple devices have been compromised, where Ivanti VPN devices are used for the attack"
     SKT has not clearly identified that it was using Ivanti VPN products for their 4G/5G architecture. Yet, the first anomaly behavior was detected by SKT incident response team in April 18 and it was from a linux server for fee analysis that was located in the middle of the VPN route connecting to internet. 
