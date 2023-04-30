---
layout: page
title: Multi-Radar Odometry
description: Senior Capstone Project, Sponsored by Trimble Autonomy
img: assets/img/dynapack.png
importance: 1
category: work
---

Trimble produces industry leading autonomous machinery solutions for agriculture and heavy industry. These products use a range of technologies, including GNSS and radar, to navigate complex physical environments without the need for human intervention. Currently, Trimble offers a suite of technologies that enable the autonomous operation of Dynapack soil compactor. This compactor is equipped with GNSS, used to locate the machine, as well as radar, which is used for collision detection. Occasionally, GNSS signal is interrupted for brief periods of time and the coordinate position of the compactor is lost. As a result, the compactor must cease operation until GNSS signal is recovered.

However, the compactor is also equipped with six radar sensors, as shown in the image below, which are used by the machine to detect and avoid obstacles. Our team was tasked with developing a redundant odometry solution using the data from these radars so that the machine might continue operation during brief periods of GNSS signal loss. 



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/radar_pos.png" title="example image" class="img-fluid rounded z-depth-0" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal its glory in the next row of images.


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
