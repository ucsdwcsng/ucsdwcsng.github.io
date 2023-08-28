---
layout: publication
title: "SyncScatter: Enabling WiFi like synchronization and range for WiFi backscatter Communication"
tags: Communications Backscatter
cover: /assets/images/pubpic/syncscatter.png
authors: "Manideep Dunna, Miao Meng, Po-Han Wang, Chi Zhang, Patrick Mercier, Dinesh Bharadia"
conference: "NSDI 2021"
paper: files/syncscatter.pdf
video: https://drive.google.com/file/d/1HLOmupRVde8Akssg3BT88-4PR7vTBsR5/view
slides: files/nsdi21_slides_dunna.pdf
---

WiFi backscattering can enable direct connectivity of IoT de-vices with commodity WiFi hardware at low power. However,most existing work in this area has overlooked the importanceof synchronization and, as a result, accepted either limited range between the transmitter and the IoT device, reducedthroughput via bit repetition, or both. We present SyncScatter, which achieves accurate synchronization with incident signals at the IoT device level while realizing maximum possible sensitivity afforded by a backscatter link budget. SyncScatter creates a novel modeling framework and derives the maximal optimal range and synchronization error that the receiver can tolerate without significant performance compromises. Next, SyncScatter builds a novel hierarchical wakeup protocol, which, together with a custom ASIC, achieves arange of 30+ meters and the peak throughput of 500Kbps, with an average power consumption of 30μW.