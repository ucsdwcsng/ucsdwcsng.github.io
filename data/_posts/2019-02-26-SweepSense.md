---
layout: publication
title: "SweepSense: Sensing 5 GHz in 5 Milliseconds with Low-cost Radios"
short_title: "SweepSense"
tags: Spectrum-Sensing
cover: /data/images/pubpic/sweepsense.png
authors: "Yeswanth Guddeti, Raghav Subbaraman, Moein Khazraee, Aaron Schulman, Dinesh Bharadia"
conference: "NSDI 2019"
paper: https://www.usenix.org/conference/nsdi19/presentation/guddeti
github: https://github.com/ucsdsysnet/SweepSense/tree/master
extra: This work won the Qualcomm Innovation Fellowship 2019!
osd: "We propose a new receiver architecture for spectrum sensing radios where sampling is done along with quick sweeping of the center frequency. This is motivated by the intuition that a sweeping radio may miss lesser transmissions than one that sequentially tunes to different bands. We implement this using an open loop VCO fed with a sawtooth voltage waveform. The output of the VCO is used to drive a mixer and implement the sweeping radio. The architecture has been prototyped on a USRP N210 with a CBX daughterboard. Downconverting while sweeping introduces distortions in the signal, which we remove using an 'unsweeping' process and is discussed in the paper."
---

Wireless transmissions occur intermittently across the entire spectrum. For example, WiFi and Bluetooth devices transmit frames across the 100 MHz-wide 2.4 GHz band, and LTE devices transmit frames between 700 MHz and 3.7 GHz. Today, only high-cost radios can sense across the spectrum with sufficient temporal resolution to observe these individual transmissions. We present “SweepSense”, a low-cost radio architecture that senses the entire spectrum with high-temporal resolution by rapidly sweeping across it. Sweeping introduces new challenges for spectrum sensing: SweepSense radios only capture a small number of distorted samples of transmissions. To overcome this challenge, we correct the distortion with self-generated calibration data, and classify the protocol that originated each transmission with only a fraction of the transmission’s samples. We demonstrate that SweepSense can accurately identify four protocols transmitting simultaneously in the 2.4 GHz unlicensed band. We also demonstrate that it can simultaneously monitor the load of several LTE base stations operating in disjoint bands.