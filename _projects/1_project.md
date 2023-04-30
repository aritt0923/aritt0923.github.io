---
layout: page
title: Multi-Radar Odometry
description: Senior Capstone Project, Sponsored by Trimble Autonomy
img: assets/img/dynapack.png
importance: 1
category: work
---

Trimble produces industry leading autonomous machinery solutions for agriculture and heavy industry. These products use a range of technologies, including GNSS and radar, to navigate complex physical environments without the need for human intervention. Currently, Trimble offers a suite of technologies that enable the autonomous operation of Dynapack soil compactor. This compactor is equipped with GNSS, used to locate the machine, as well as radar, which is used for collision detection. Occasionally, GNSS signal is interrupted for brief periods of time and the coordinate position of the compactor is lost. As a result, the compactor must cease operation until GNSS signal is recovered.

However, the compactor is also equipped with six radar sensors, as shown in the image below, which are used by the machine to detect and avoid obstacles. Our team was tasked with investigating whether a redundant odometry solution using the machine's radars was possible, to provide recommendations to Trimble for improving odometry performance, and to develop a prototype odometry algorithm. 


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/radar_pos.png" title="example image" class="img-fluid rounded z-depth-0" %}
    </div>
</div>
<div class="caption">
    Positions of the radars on the soil compactor
</div>



