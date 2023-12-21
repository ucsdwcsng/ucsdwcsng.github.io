---
layout: publication
title: "Two beams are better than one: Towards Reliable and High Throughput mmWave Links"
short_title: "mmReliable"
tags: Communications
cover: /assets/images/pubpic/mmreliable.png
authors: "Ish Kumar Jain, Raghav Subbaraman, Dinesh Bharadia"
author_list:
    - name: Ish Kumar Jain
      url: https://ishjain.github.io/
      email: ikjain@ucsd.edu
    - name: Raghav Subbaraman
      url: https://rsubbaraman.github.io/
      email: rsubbaraman@ucsd.edu
    - name: Dinesh Bharadia
      url: https://dineshb-ucsd.github.io/
      email: dineshb@ucsd.edu
conference: "Sigcomm 2021"
conference_site: https://conferences.sigcomm.org/sigcomm/2021/program.html
paper: /files/mmreliable.pdf
slides: /files/mmreliable_slides.pdf
dataset: https://github.com/ucsdwcsng/mMobile
github: https://github.com/ucsdwcsng/mmReliable
video: https://www.youtube.com/embed/w2ZUX00-p_A
video_str: Video
description:
    - text: "Millimeter-wave communication with high throughput and high reliability is poised to be a gamechanger for V2X and VR applications. However, mmWave links are notorious for low reliability since they suffer from frequent outages due to blockage and user mobility. We build mmReliable, a reliable mmWave system that implements multi-beamforming and user tracking to handle environmental vulnerabilities. It creates constructive multi-beam patterns and optimizes their angle, phase, and amplitude to maximize the signal strength at the receiver. Multi-beam links are reliable since they are resilient to occasional blockages of few constituent beams compared to a single-beam system. We implement mmReliable on a 28 GHz testbed with 400 MHz bandwidth, and a 64 element phased array supporting 5G NR waveforms. Rigorous indoor and outdoor experiments demonstrate that mmReliable achieves close to 100% reliability providing 2.3x improvement in the throughput-reliability product than single-beam systems."
      image: /assets/images/respic/5G/mmreliable.png
      image_width: 800 # px
medias: 
    - type: UCSD News
      url: https://jacobsschool.ucsd.edu/news/release/3322
    - type: Interesting Engineering
      url: https://interestingengineering.com/innovation/a-new-laser-like-system-could-put-5g-in-your-home
    - type: DailyTimes
      url: https://dailytimes.com.pk/808141/new-tech-provides-fast-reliable-5g-connections/
    - type: TechXplore
      url: https://techxplore.com/news/2021-08-technology-fastest-version-5g-home.html
    - type: NewsWise
      url: https://www.newswise.com/articles/this-technology-could-bring-the-fastest-version-of-5g-to-your-home-and-workplace
extra: "This work won the Qualcomm Innovation Fellowship 2022!"
osd: "This repository contains the artifact for submission #441, ACM SIGCOMM 2021. The artifact is composed of simulations and algorithms implemented on real-life mmWave channel estimates."
---
