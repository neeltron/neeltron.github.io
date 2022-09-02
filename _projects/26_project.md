---
layout: page
title: EyeLand
description: Real-Time Heuristic Framework for Safe Landing of UAVs in Dynamic Scenarios
img: assets/img/r1.jpeg
importance: 2
category: Research
---

EyeLand is a safe landing framework for multi-rotor unmanned aerial vehicles, that can be installed in any companion computer, as long as it contains a GPU. The whole project was divided into two phases: 
<ol type = "a">
    <li>
        Potential Landing Zone Detection - In this phase, the canny edge algorithm detects the empty spaces to land, depending upon the edges that are found by the algorithm. For distant spaces, an area estimation algorithm is written for checking whether the drone will fit in that region or not. The regions for landing are marked in circles and after testing the Area Estimation Algorithm against the ground truth taken individually from the ToF sensor, the error in estimation turned out to be less than 2%.
    </li>
    <li>
        Real-time Potential Landing Zone State Estimation and Navigation in Dynamic Scenarios - In this phase, the moving objects are detected using the frame differenciation and summing technique and using the shift in pixels, the change in pixels and time is calculated. A velocity estimation algorithm is written, which uses the same formula as in the area estimation algorithm and translates the value from pixels to meters. After testing the velocity estimation algorithm against the ground truth recorded from the ground vehicle's odometer, the error turned out to be 2.2%.
    </li>
</ol>

The hardware used for experimentation and testing is as follows:
<ul>
    <li>
        TeraBee Evo 60m ToF (Time of Flight) Sensor
    </li>
    <li>
        ZED Depth Camera
    </li>
    <li>
        Nvidia Jetson Nano
    </li>
    <li>
        S500 Quadcopter Frame
    </li>
    <li>
        40 A ESC x 4
    </li>
    <li>
        Emax 935 kV BLDC Motor x 4 (2 CW, 2 CCW)
    </li>
    <li>
        5200 mAh LiPo 3S Battery
    </li>
    <li>
        RadioLink Pixhawk Flight Controller
    </li>
</ul>    
<br>


The above hardware is recommended to run the setup in the best possible way, although the framework will work if there are minor deviations from the list.


<!--<iframe width="560" height="315" src="https://www.youtube.com/embed/bfZO2NFVPgA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>-->
<br>
<!--
<a href = "https://presentquick.neeltron.repl.co/">Live demo</a><br>
Product Hunt: <a href = "https://www.producthunt.com/posts/presentquick">https://www.producthunt.com/posts/presentquick</a>
-->
