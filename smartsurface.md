---
layout: page
title: "Adaptive Smart Surfaces for Wireless Channel Morphing to enable full multiplexing and multi-user gains"
## excerpt: "Bringing Interference Alignment to Reality"
permalink: smartsurfaces
##tags: miscellanious
---


---

<!-- ### NSDI 2021
```
Authors: Manideep Dunna, Miao Meng, Po-Han Wang, Chi Zhang, Patrick Mercier, and Dinesh Bharadia
```
 -->

<!-- #### <a href="{{ site.url }}{{ site.baseurl }}/files/syncscatter.pdf" style="background-color: white; color: orange;">[Paper]</a> <a href="{{ site.url }}{{ site.baseurl }}/files/nsdi21_slides_dunna.pdf" style="background-color: white; color: purple;">[Slides]</a> <a href="https://drive.google.com/file/d/1HLOmupRVde8Akssg3BT88-4PR7vTBsR5/view?usp=sharing">[Video]</a>
 -->


### Synopsis
<p style="font-size:20px"> Modern wireless standards promise to enable high throughput wireless links by using multiple antennas on the UEs and Basestations. However, the increase in the number of antennas do not lead to proportional increase in the achieved link througput. The primary reason for this is that the wireless channel do not have good enough multipath and is not well conditioned to support projected MIMO throughput. As shown in Fig. 1a, closely spaced antennas on the device have correlated wireless channels and do not allow for efficient spatial multiplexing of data streams. </p>

<!-- In today's wireless networks, the typical operating paradigm is to have different users occupying different frequency band such that they don't interfere. Multiple user MIMO (mu-MIMO) has been previously attempted to solve this problem and have multiple users communicating over a single frequency band. However, mu-MIMO implementations have never been robust since it requires favorable channel conditions not always guaranteed in real wireless channels. Typical reasons for this is that user locations being close to each other (Fig. 1) makes the channels correlated, and does not allow for efficient interference separations, as interference is almost indistinguishable from the intended users' signals. -->

<div class="col-sm-12 clearfix">

<div class="col-sm-9" style="float: left;">
 <img src="{{ site.url }}{{ site.baseurl }}/assets/images/pubpic/smartsurface_fig.png" width="100%" height="250px" style="float: center" > 
 <!--</a> a href="{{ site.url }}{{ site.baseurl }}/assets/images/pubpic/smartsurface_fig1.jpg"-->
 <p style="font-size:20px">Fig 1: Smartsurface can lead to multiplexing gain</p>
</div>


<!-- <div class="col-sm-6" style="float: left;">
 <a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/ia_fig2.png"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/ia_fig2.png" width="100%" height="250px" style="float: center" > </a>
 <p style="font-size:20px">Fig. 2</p>
</div> -->

</div>


<p style="margin-top:1cm; font-size:20px"> In this project, we increase the multiplexing capability of the wireless channel by creating new multipath in the channel. We achieve this by designing smartsurfaces that can be deployed on walls as shown in Fig. 1c to create diverse paths from a UE to Basestation. The smartsurfaces create a strong reflection and makes the wireless channel well-conditioned to support multiple spatial streams. </p>



### Personnel


<div class="row">


<!--div class="col-sm-3" style="float: left;">
 <p style="font-size:20px">Dinesh Bharadia: PI, UC San Diego</p>
<a href="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/dinesh.jpg"><img src="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/dinesh.jpg" width="50%" height="250px" style="float: center" > </a>
</div>

<div class="col-sm-3" style="float: left;">
 <p style="font-size:20px">Daniel Sievenpiper: PI, UC San Diego</p>
<a href="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/DanSievenpiper.jpeg"><img src="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/DanSievenpiper.jpeg" width="50%"  height="250px" style="float: center" > </a>
</div>

<div class="col-sm-3" style="float: left;">
 <p style="font-size:20px">Alireza Vahid: PI, CU Denver</p>
<a href="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/alireza.png"><img src="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/alireza.png" width="100%"  height="250px" style="float: center" > </a>
</div>


<div class="col-sm-3" style="float: left;">
 <p style="font-size:20px">Manideep Dunna: Ph.D. Student, UC San Diego</p>
<a href="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/manideep.jpg"><img src="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/manideep.jpg" width="50%"  height="250px" style="float: center" > </a>
</div>
-->

<div class="col-sm-3" style="float: left; margin-right: 20px;">
    <p style="font-size:20px">Dinesh Bharadia: PI, UC San Diego</p>
    <a href="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/dinesh.jpg">
        <img src="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/dinesh.jpg" width="200px" height="200px" style="display: block; margin: auto;">
    </a>
</div>

<div class="col-sm-3" style="float: left; margin-right: 20px;">
    <p style="font-size:20px">Daniel Sievenpiper: PI, UC San Diego</p>
    <a href="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/DanSievenpiper.jpeg">
        <img src="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/DanSievenpiper.jpeg" width="200px" height="200px" style="display: block; margin: auto;">
    </a>
</div>

<div class="col-sm-3" style="float: left; margin-right: 20px;">
    <p style="font-size:20px">Alireza Vahid: PI, CU Denver</p>
    <a href="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/alireza.png">
        <img src="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/alireza.png" width="200px" height="200px" style="display: block; margin: auto;">
    </a>
</div>

<div class="col-sm-3" style="float: left;">
    <p style="font-size:20px">Manideep Dunna: Ph.D. Student, UC San Diego</p>
    <a href="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/manideep.jpg">
        <img src="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/manideep.jpg" width="200px" height="200px" style="display: block; margin: auto;">
    </a>
</div>


<div class="col-sm-3" style="float: left;">
 <p style="font-size:20px">Xiaozhen Yang: Ph.D. Student, UC San Diego</p>
<a href="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/XiaozhenYang.jpg"><img src="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/XiaozhenYang.jpg" width="200px"  height="200px" style="display: block; margin: auto;"> </a>
</div>

</div>




### Publications


<div class = "row">
<div class="container">
<a style="background-color: white; color: orange;" href="{{ site.url }}{{ site.baseurl }}/files/scattermimo.pdf"> ScatterMIMO: Enabling Virtual MIMO using smartsurfaces</a> <br>
Manideep Dunna, Chi Zhang, Daniel Sievenpiper, Dinesh Bharadia
</div>
</div>

<div class = "row">
<div class="container">
<a style="background-color: white; color: orange;" href="{{ site.url }}{{ site.baseurl }}/files/Xiaozhen_ACES.pdf"> Simultaneous Beam-Steering and Polarization COnversion Using a Varactor-Integrated Metasurface</a> <br>
Xiaozhen Yang, Dinesh Bharadia, Daniel Sievenpiper
</div>
</div>

<div class = "row">
<div class="container">
<a style="background-color: white; color: orange;" href="{{ site.url }}{{ site.baseurl }}/files/Arxiv_alireza.pdf"> Control and Placement of Intelligent Surfaces for IoT systems</a> <br>
Sajjad Nassirpour, Alireza Vahid, Dinh-Thuan Do, Dinesh Bharadia
</div>
</div>

<!-- <div class = "row">
<div class="container">
<a style="background-color: white; color: orange;" href="https://doi.org/10.1016/j.acha.2021.03.004"> Ranking recovery from limited pairwise comparisons using low-rank matrix completion</a> <br>
    Levy, Tal and Vahid, Alireza and Giryes, Raja<br>
    Harmonic Analysis Journal, 2021
</div>
</div>


<div class = "row">
<div class="container">
<a style="background-color: white; color: orange;" href="https://ieeexplore.ieee.org/abstract/document/9518272"> Capacity of the Torn Paper Channel with Lost Pieces</a> <br>
    Ravi, Aditya Narayan and Vahid, Alireza and Shomorony, Ilan <br>
    ISIT 2021
</div>
</div>


<div class = "row">
<div class="container">
<a style="background-color: white; color: orange;" href="https://ieeexplore.ieee.org/abstract/document/9348147"> Communicating over the Torn-Paper Channel</a> <br>
    Shomorony, Ilan and Vahid, Alireza<br>
    Globecom 2020
</div>
</div> -->


