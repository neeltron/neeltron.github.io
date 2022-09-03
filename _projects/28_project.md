---
layout: page
title: Visual Servoing
description: Visual Servoing on an Aerial Manipulator
img: assets/img/r3.jpg
importance: 3
category: Research
---

The proposed work consists of an Unmanned Aerial Vehicle, with an Aerial Manipulator mounted at the bottom. The goal of this project was to grab an object and carry it around while balancing the weight of the vehicle and the payload.
<br>
The assumptions considered during the project are:
<ul>
    <li>
        The object will have at least two april tags, located on top and frontal face.
    </li>
    <li>
        The aerial manipulator will have a camera near the gripper.
    </li>
    <li>
        The UAV will have a camera mounted on any of the sides in which the aerial manipulator has its degrees of freedom.
    </li>
    <li>
        Instead of giving the aerial manipulator 4 degrees of freedom, it will have 2 degrees of freedom and the UAV will yaw in case the object lies out of the range.
    </li>
</ul>

This project was carried out as per the following steps:

<ol type = "a">
    <li>Object Identification - For the identification of the objects (i.e., which object to pick), the objects are labelled with 36h11 family AprilTags.</li>
    <li>Object Tracking - The camera mounted on the top first identifies the April Tag on top of the object. Once the identification is done from the bottom facing camera, the Aerial Manipulator faces onto that side and the camera mounted on it stops as soon as it locates the same AprilTag.</li>
    <li>Movement around the Vertical Axis - If the object is not in range of the aerial manipulator, the control system of the vehicle will yaw towards the direction to locate the object.</li>
    <li>Object Dimensions - Taking the size of april tags as reference, the size of the object is known, so before moving to the object's location, the gripper opens up with enough clearance to grab the object.</li>
    <li>Post-Navigation - After the manipulator navigates towards the object, the gripper closes and the manipulator is then set up in an erect state to make sure that the center of gravity of the vehicle is maintained.</li>
</ol>

Project Advisor: <a href = "https://www.iiit.ac.in/people/faculty/Harikumar/">Dr. Harikumar Kandath</a>
<br>
Affiliation: <a href = "https://iiit.ac.in">International Institute of Information Technology, Hyderabad</a>
<br>
<!--<iframe width="560" height="315" src="https://www.youtube.com/embed/bfZO2NFVPgA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>-->
<br>
<!--
<a href = "https://presentquick.neeltron.repl.co/">Live demo</a><br>
Product Hunt: <a href = "https://www.producthunt.com/posts/presentquick">https://www.producthunt.com/posts/presentquick</a>
-->
