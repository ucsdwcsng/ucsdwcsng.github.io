---
title: "Cross-Layer Interference Management: Bringing Interference Alignment to Reality"
layout: page
excerpt: "Bringing Interference Alignment to Reality"
sitemap: false
permalink: interf_align
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
<p style="font-size:20px"> In today's wireless networks, the typical operating paradigm is to have different users occupying different frequency band such that they don't interfere. Multiple user MIMO (mu-MIMO) has been previously attempted to solve this problem and have multiple users communicating over a single frequency band. However, mu-MIMO implementations have never been robust since it requires favorable channel conditions not always guaranteed in real wireless channels. Typical reasons for this is that user locations being close to each other (Fig. 1) makes the channels correlated, and does not allow for efficient interference separations, as interference is almost indistinguishable from the intended users' signals. </p>

<div class="col-sm-12 clearfix">

<div class="col-sm-6" style="float: left;">
 <a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/ia_fig1.png"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/ia_fig1.png" width="100%" height="250px" style="float: center" > </a>
 <p style="font-size:20px">Fig. 1</p>
</div>


<div class="col-sm-6" style="float: left;">
 <a href="{{ site.url }}{{ site.baseurl }}/images/pubpic/ia_fig2.png"><img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/ia_fig2.png" width="100%" height="250px" style="float: center" > </a>
 <p style="font-size:20px">Fig. 2</p>
</div>

</div>


<p style="margin-top:9cm; font-size:20px"> In this project, we aim to make the mu-MIMO gains robust by creating favorable channel conditions to enable multi-user communications. This is done by implementing interference alignment (IA), by having a larger number of antennas at the base station, which can be turned on-off. The goal of the project is to create variations in the received wireless channel by turning these antennas on-off strategically, in a way that the interfered channel always aligns in a single direction (Fig. 2), wheres the targeted user channel remains variable. This guarantees a good operating point for interference management, since the interference is aligned across the switching antenna states and thus can be suppressed easily. </p>

### Personnel


<div class="row">


<div class="col-sm-3" style="float: left;">
 <p style="font-size:20px">Dinesh Bharadia: PI, UCSD</p>
<a href="{{ site.url }}{{ site.baseurl }}/images/teampic/dinesh.jpg"><img src="{{ site.url }}{{ site.baseurl }}/images/teampic/dinesh.jpg" width="100%" height="250px" style="float: center" > </a>
</div>


<div class="col-sm-3" style="float: left;">
 <p style="font-size:20px">Alireza Vahid: PI, CU Denver</p>
<a href="{{ site.url }}{{ site.baseurl }}/images/teampic/alireza.png"><img src="{{ site.url }}{{ site.baseurl }}/images/teampic/alireza.png" width="100%"  height="250px" style="float: center" > </a>
</div>

<div class="col-sm-3" style="float: left;">
 <p style="font-size:20px">Agrim Gupta: Ph.D. Student, UCSD</p>
<a href="{{ site.url }}{{ site.baseurl }}/images/teampic/agrim.png"><img src="{{ site.url }}{{ site.baseurl }}/images/teampic/agrim.png" width="100%"  height="250px" style="float: center" > </a>
</div>


<div class="col-sm-3" style="float: left;">
 <p style="font-size:20px">Sajjad Nassirpour: Ph.D. Student, CU Denver</p>
<a href="{{ site.url }}{{ site.baseurl }}/images/teampic/sajjad.jpeg"><img src="{{ site.url }}{{ site.baseurl }}/images/teampic/sajjad.jpeg" width="100%"  height="250px" style="float: center" > </a>
</div>

</div>




### Publications


<div class = "row">
<div class="container">
<a style="background-color: white; color: orange;" href="{{ site.url }}{{ site.baseurl }}/files/TIMO.pdf"> TIMO: Time Interleaved Multiple Outputs for enabling multiplexing gainswith a single RF Chain</a> <br>
    Under submission
</div>
</div>


<div class = "row">
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
</div>


