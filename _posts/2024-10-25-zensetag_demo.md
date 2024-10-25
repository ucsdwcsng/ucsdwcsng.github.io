---
layout: publication
title : "ZenseTag: Real-Time Passive RFID Sensing"
short_title: "ZenseTag-Demo"
tags: Communications
cover: /assets/images/pubpic/windex.png
conference: "ACM Conference on Mobile Computing and Networking Demo 2024"
conference_site: https://www.sigmobile.org/mobicom/2024/
authors: "Ishan Bansal, Nagarjun Bhat, Agrim Gupta, Harine Govindarajan, Dinesh Bharadia"
author_list:
    - name: Ishan Bansal
      email: isbansal@ucsd.edu
    - name: Nagarjun Bhat
      email: nbhat@ucsd.edu
    - name: Agrim Gupta
      url: https://agrim9.github.io
      email: agg003@ucsd.edu
    - name: Harine Govindarajan
      email: hgovindarajan@ucsd.edu
    - name: Dinesh Bharadia
      url: https://dineshb-ucsd.github.io/
      email: dineshb@ucsd.edu
paper: https://arxiv.org/html/2406.01888v1
#slides: https://www.usenix.org/system/files/nsdi24_slides-ko.pdf
# miscs:  # whatever you need to add Extra
#     - content_type: Project Website
#       content_url: https://edgeric.github.io
#     - content_type: Poster
#       content_url: /files/edgeric_poster.pdf # hat tip: do not use tabs for idnentation, yaml doesnt support it
#     - content_type: Github Repo
#       content_url: https://github.com/ushasigh/EdgeRIC-A-real-time-RIC.git
    
description: # all combinations are possible: (title+text+image, title+image, text+image etc), things will be populated in orders
    - text: "Sensing enables interaction with and quantification of the natural world, yet the adoption of sensing systems is limited due to battery dependence, complex interfaces, energy-harvesting needs, and readout latency. To address these issues, we introduce ZenseTag—a miniaturized, sticker-like platform that interfaces commercial sensors directly with COTS RFID tags. ZenseTag leverages the impedance response of these sensors to stimuli at Radio Frequencies, specifically tuned to the UHF RFID band. It integrates reliable differential analog sensing hardware with robust software for accurate, low-latency readouts, even amidst multipath effects. \nFor demonstration, a PC will connect to an Impinj RF reader, which is linked to a high-gain antenna positioned near the trialing ZenseTag. The tag consists of a ZenseTag PCB interfaced with a sticker-like antenna and two RF ICs, with one IC connected to a sensor for specific applications. For example, testing the soil moisture tag will require a pot of dry soil, while the light sensor will need an external light source. \nTo showcase ZenseTag's capabilities in detecting soil moisture, force, and luminosity, we will vary the soil moisture by adding water to the pot, press and release the force-sensitive resistor (FSR), and cover/uncover the photodiode. The response for each application will be displayed on a GUI developed for this purpose. Additionally, the demonstration will highlight ZenseTag’s robustness against obstacles and the movement of people around the sensors. We have thoroughly evaluated all three sensors: soil moisture, force, and light."      
---
We address the resource allocation challenge in NextG cellular radio access networks (RAN), where resources must be shared among diverse user applications, each requiring guarantees on throughput and service regularity. Due to factors such as fluctuating channel quality, user mobility, and scalability, this problem quickly becomes combinatorial and complex. We begin by analytically modeling it as a constrained Markov decision process, drawing from control theory. By leveraging the structural properties of this model, we decompose the problem into a more manageable form, allowing for the independent computation of relative priorities for each user. By allocating resources in descending order of these priorities, we reduce the combinatorial complexity of resource allocation to a linear one. We introduce Windex, a lightweight method for training neural networks to compute these priorities, taking into account service guarantees, channel quality, and system load. Implemented on a real-time RAN Intelligent Controller (RIC), Windex enables resource allocation decisions in under 20μs per user, efficiently managing resources within each 1 ms scheduling time slot. Our approach, evaluated across standardized 3GPP service classes, demonstrates the least service violations compared to state-of-the-art systems. These results have been validated through simulations and real-world emulations using over-the-air channel traces on a 5G testbed.
