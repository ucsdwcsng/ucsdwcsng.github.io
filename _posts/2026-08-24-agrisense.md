---
layout: publication
title: "AgriSense: Battery-Free Soil Sensing for Next-Gen Connected Agriculture"
short_title: "AgriSense"
tags: Backscatter
cover: /assets/images/agrisense/agrisense-overview.png
authors: "Ishan Bansal, Nagarjun Bhat, Agrim Gupta, Harine Govindarajan, Dinesh Bharadia" # needed for publications/
author_list:
    - name: Ishan Bansal
      url: https://b-ishan.github.io/
      email: isbansal@ucsd.edu
    - name: Nagarjun Bhat
      email:  nbhat@ucsd.edu
    - name: Agrim Gupta
      url: https://agrim9.github.io/
      email: agg003@ucsd.edu
    - name: Harine Govindarajan
      email: hgovindarajan@ucsd.edu
    - name: Dinesh Bharadia
      url: https://dineshb-ucsd.github.io/
      email: dineshb@ucsd.edu
eqcon: false #Put true if you want equal contrribution on pub page
conference: "AgWireless 2026"
conference_site: Ames, Iowa
video: https://www.youtube.com/embed/7eiO4BO_wTQ
video_str: Demonstration of AgriSense
miscs:  # whatever you need to add Extra
#    - content_type: Poster
#      content_url:  /files/poster-agrisense.pdf # TODO: add poster PDF, then uncomment
description: # all combinations are possible: (title+text+image, title+image, text+image etc), things will be populated in orders
    - title: The Illusion of Sparse Data
      text: "Sparse sensor deployments create a false sense of security: with only a handful of nodes spread across a field, the system interpolates that the gaps between sensors are in an optimal state, so the field appears 100% healthy according to the sensor reports. In reality, hidden dry zones degrade crop yields and threats fall between the sensors — interpolation creates false confidence. The sensors said the field was fine."
      # image: /assets/images/agrisense/agrisense-sparse-data.jpg # TODO: add image
      # image_width: 800 # px
    - title: Why Data Stays Sparse
      text: "Deployment and maintenance costs are what prevent dense sensing from scaling. At $100+ per node, prohibitive unit cost means dense deployment bankrupts the operation. On top of that, the battery trap makes long-term, large-scale maintenance impossible — replacing thousands of buried batteries even every few years is untenable across a large field."
      # image: /assets/images/agrisense/agrisense-cost-problem.jpg # TODO: add image
      # image_width: 800 # px
    - title: "Deploy & Forget: Permanent Soil Intelligence"
      text: "AgriSense builds on our ZenseTag battery-free sensing platform to make dense soil sensing viable: each node costs about $1 to deploy, needs no batteries to replace, and offers a perpetual operating life. This removes the two biggest barriers to scale — unit cost and maintenance — enabling truly dense, permanent soil intelligence."
      # image: /assets/images/agrisense/agrisense-zensetag-platform.jpg # TODO: add image
      # image_width: 800 # px
    - title: Automated Data Harvesting at Scale
      text: "To read thousands of battery-free nodes without fixed reader infrastructure, we mount an RFID reader on a drone that flies a fixed path over the field and harvests data from every node en-route over a wireless backhaul. For a representative 5-hectare field (250m x 200m) with a 2000-node sensor grid, a 10km drone path at 3m/s covers the whole deployment in about 60 minutes. Compared to active sensor networks (~$350,000 total) and vanilla battery-free networks with fixed readers (~$225,000 total), our drone-based approach brings the total cost down to roughly $5,000 — a 50-70x cost reduction over conventional systems."
      image: /assets/images/agrisense/agrisense-drone-harvesting.png
      image_width: 800 # px
    - text: "
        <table style=\"border-collapse: collapse; width: 100%; max-width: 900px; margin: 0 auto; text-align: center; font-size: 15px;\">
          <thead>
            <tr style=\"background-color: #f2f2f2;\">
              <th style=\"border: 1px solid #ccc; padding: 8px;\">Cost Category</th>
              <th style=\"border: 1px solid #ccc; padding: 8px;\">Active Sensor Networks</th>
              <th style=\"border: 1px solid #ccc; padding: 8px;\">Vanilla Battery-free Networks</th>
              <th style=\"border: 1px solid #ccc; padding: 8px;\">Our Approach</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td style=\"border: 1px solid #ccc; padding: 8px;\">Nodes</td>
              <td style=\"border: 1px solid #ccc; padding: 8px;\">$200,000<br>($100/node)</td>
              <td style=\"border: 1px solid #ccc; padding: 8px;\">$2,000<br>($1/node)</td>
              <td style=\"border: 1px solid #ccc; padding: 8px;\">$2,000<br>($1/node)</td>
            </tr>
            <tr>
              <td style=\"border: 1px solid #ccc; padding: 8px;\">Gateways / Equipment</td>
              <td style=\"border: 1px solid #ccc; padding: 8px;\">$10,000<br>(4-5 LoRa-WANs)</td>
              <td style=\"border: 1px solid #ccc; padding: 8px;\">$200,000<br>(200 fixed readers)</td>
              <td style=\"border: 1px solid #ccc; padding: 8px;\">$2,000<br>(drone + reader)</td>
            </tr>
            <tr>
              <td style=\"border: 1px solid #ccc; padding: 8px;\">Long Term (10yr) Maintenance</td>
              <td style=\"border: 1px solid #ccc; padding: 8px;\">$150,000<br>(batteries + labor)</td>
              <td style=\"border: 1px solid #ccc; padding: 8px;\">~$20,000<br>(readers + labor)</td>
              <td style=\"border: 1px solid #ccc; padding: 8px;\">~$1,000<br>(basic servicing)</td>
            </tr>
            <tr style=\"font-weight: bold;\">
              <td style=\"border: 1px solid #ccc; padding: 8px;\">Total Gross</td>
              <td style=\"border: 1px solid #ccc; padding: 8px;\">~$350,000</td>
              <td style=\"border: 1px solid #ccc; padding: 8px;\">~$225,000</td>
              <td style=\"border: 1px solid #ccc; padding: 8px;\">~$5,000</td>
            </tr>
          </tbody>
        </table>
        "
    - title: From Labs to Landscapes
      text: "We validated the full pipeline end-to-end: from linear soil moisture transduction (IDC capacitance vs. volumetric water content, characterized against the Topp model at 915 MHz) to autonomous aerial harvesting with a drone-mounted RFID reader flying over dense ZenseTag deployments, to spatial insights delivered through an AR application. Dense sensor deployment is what makes precise spatial mapping possible in the first place, and each stage of this pipeline was validated in real field conditions rather than lab-only settings."
      # image: /assets/images/agrisense/agrisense-field-validation.jpg # TODO: add image
      # image_width: 800 # px
    - title: "Closing the Loop: Physical Sensor Foundation Models & Automated Farm Orchestration"
      text: "Our long-term vision is a fully closed loop for precision agriculture. Stage 1 harvests data from dense sensor deployments to produce on-demand soil maps. Stage 2 feeds this data into sensor LLMs and spatial foundation models that predict root-zone dynamics and act as an agronomy agent. Stage 3 uses these predictions to drive automated closed-loop precision actuation, delivering water and nutrition based on exact spatial needs — with the grower kept in the loop through smart AR applications that require zero manual intervention. The result is autonomous, field-scale precision fertigation driven by a dense network of battery-free sensors."
      # image: /assets/images/agrisense/agrisense-closing-the-loop.jpg # TODO: add image
      # image_width: 800 # px
    - title: Related Publications
      text: "AgriSense builds directly on our line of work on battery-free RFID sensing: [ZenseTag](/zensetag/), our RFID-assisted twin-tag single antenna COTS sensor interface (ACM SenSys 2024); its [MobiCom 2024 demo](/zensetag_demo/) (Best Runner-up Demo Award); [SenSync](/sensync/), our real-time and accurate passive sensing technique (IEEE RFID 2025, Best Paper Award); the [SIGAR demo](/sigar_demo/), a sensor integration gateway using augmented reality (ACM/IEEE SenSys 2025, Best Runner-up Demo Award); and TuneTag, our long-range reliable battery-free sensing work (IEEE Journal of RFID 2025)."
---
