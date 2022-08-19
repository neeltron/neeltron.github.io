---
layout: page
title: AIAA DBF'22
description: Held in Wichita, Kansas
img: assets/img/12.jpg
importance: 1
category: 2022
---

Design/Build/Fly, or DBF, is a radio-controlled aircraft competition sponsored by the American institute of Aeronautics and Astronautics (AIAA), Cessna Aircraft Company, and Raytheon Missile Systems. The competition is intended to challenge the AIAA student branches of each university to design, build, and fly a remote controlled airplane that can complete specific ground and flight missions. Additionally, the teams are required to submit a comprehensive design report detailing the most important aspects of their designs.

The problem statement for DBF'22 was to design, build and test an aircraft to deliver vaccination components. Missions included deployment of the aircraft, staging of vaccination syringes, and delivery of environmentally sensitive vaccine vial packages.

As a part of <a href = "https://instagram.com/teamagastya">Team Agastya</a>, my role was to work on the Design aspect of the aircraft and prepare the CAD Models, along with the drawings for the design report, which can be seen below. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Three-view drawing of the aircraft, along with dimensions.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Structural arrangement of the aircraft, along with its subsystems.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/7.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Layout of the aircraft and its subsystems.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/8.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Arrangement and accommodation of the payload inside the fuselage.
</div>

During the fly-off, I was the ground crew member, representing the University of Petroleum and Energy Studies, India at Wichita, Kansas. To get acquainted with our Fly-off Journey, <a href = "https://www.instagram.com/p/CfnmnlwvvS4/">click here</a>.

TL;DR We achieved 7th place in the Proposal phase, while in the designed report phase, we got the order 10th and in the fly-off, we stood 43rd!




<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}
```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
```
{% endraw %}
