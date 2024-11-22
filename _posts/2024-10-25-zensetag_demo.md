---
layout: publication
title : "Demo - ZenseTag: Real-Time Passive RFID Sensing"
short_title: "ZenseTag-Demo"
tags: Backscatter
cover: /assets/images/zensetag/zeta-demo-overview.jpg
conference: "ACM MobiCom'24 Demo"
conference_site: https://www.sigmobile.org/mobicom/2024/
authors: "Ishan Bansal, Nagarjun Bhat, Agrim Gupta, Harine Govindarajan, Dinesh Bharadia"
author_list:
    - name: Ishan Bansal
      url: https://b-ishan.github.io/
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
paper: /files/demo_zensetag_mobicom24.pdf
video: https://www.youtube.com/embed/7mvNrl5CLU8
video_str: Demonstration of ZenseTag
miscs:  # whatever you need to add Extra
    - content_type: Project Webpage
      content_url: https://wcsng.ucsd.edu/zensetag
#     - content_type: Poster
#       content_url: /files/edgeric_poster.pdf # hat tip: do not use tabs for idnentation, yaml doesnt support it
#     - content_type: Github Repo
#       content_url: https://github.com/ushasigh/EdgeRIC-A-real-time-RIC.git
    
description: # all combinations are possible: (title+text+image, title+image, text+image etc), things will be populated in orders
    - title: Winner of Best Demo - Runner Up at MobiCom 2024 
    - title: Applications for ZenseTag
      text: "Sensing enables interaction with and quantification of the natural world, yet the adoption of sensing systems is limited due to battery dependence, complex interfaces, energy-harvesting needs, and readout latency. To address these issues, we introduce ZenseTag—a miniaturized, sticker-like platform that interfaces commercial sensors directly with COTS RFID tags. ZenseTag leverages the impedance response of these sensors to stimuli at Radio Frequencies, specifically tuned to the UHF RFID band. It integrates reliable differential analog sensing hardware with robust software for accurate, low-latency readouts, even amidst multipath effects. \nFor demonstration, a PC will connect to an Impinj RF reader, which is linked to a high-gain antenna positioned near the trialing ZenseTag. The tag consists of a ZenseTag PCB interfaced with a sticker-like antenna and two RF ICs, with one IC connected to a sensor for specific applications. For example, testing the soil moisture tag will require a pot of dry soil, while the light sensor will need an external light source. \nTo showcase ZenseTag's capabilities in detecting soil moisture, force, and luminosity, we will vary the soil moisture by adding water to the pot, press and release the force-sensitive resistor (FSR), and cover/uncover the photodiode. The response for each application will be displayed on a GUI developed for this purpose. Additionally, the demonstration will highlight ZenseTag’s robustness against obstacles and the movement of people around the sensors. We have thoroughly evaluated all three sensors: soil moisture, force, and light."    
      image: /assets/images/zensetag/zeta-apps.jpg
      image_width: 800 # px  
---