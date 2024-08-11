---
layout: page
title: Pointcloud Models
status:
---

<div class="row">
        <div class="col-6">
            <h2>Models by Building</h2>
  <ul>
  {% assign var1 = site.architecture | where:"status","live" | sort:"title","first"  %}
  {% for item in var1 %}
    <li><a href="{{ item.model_link | absolute_url }}">{{item.title}}</a></li>
  {% endfor %}
  </ul>

  <h2>Potree Pointcloud Tutorial</h2>
            <p>To learn more about using our Pointcloud Models, click below for a YouTube tutorial on navigating the interface.</p>
            <iframe width="100%" height="400px" src="https://www.youtube.com/embed/xWqQ1-G3MvQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen=""></iframe>
        </div>
        <div class="col-6">

<h2>Potree Pointcloud Models</h2>
More than twenty-five Florentine institutions or independent buildings built before 1500 have been scanned by the Florence As It Was team since 2018. Most of these scanned structures have been edited, modeled, and posted in the list below. 

Data has been collected using two LiDAR scanners produced by Leica Geosystems: the BLK360 and the RTC360. Point clouds have been edited and modeled with Cyclone Register 360 and, in some cases, enhanced through a program called Reality Capture. These models are exported to an open source program called Potree, where they are made available to the public gratis.

<h2>Navigating Models</h2>

<p>To navigate through a model like this one (<a href="https://3d.wlu.edu/v21/pages/SCroce/SCroce.html">S. Croce</a>) or this one (S. Maria Novella)...</p>

<p>Go to the options bar on the left:</p>
<ul>
<li>Slide the "point budget" button all the way to the right (10,000,000) to increase the resolution of the model.</li>
<li>Check “Enable” to outline contours of objects. Uncheck to remove this feature.</li>
<li>Scroll down to “Navigation”</li>
<li>Left click on the icon of the BIRD (second from left)</li>
<li>Slide the “Speed” button to the left until it reads ca. 4.0</li>
<li>Move mouse to the desired destination on the model.</li>
<li>Press the “Up” arrow on the keyboard to advance, the “Down” arrow to retreat, and the “Left” and “Right” arrows to move sideways.</li>
<li>Left click to begin the navigation.</li>
<li>Control speed with the scrollbar on the mouse.</li>
<li>To inspect in 360, left click and drag on the model to rotate it.</li>
<li>Right click and drag on the model to pan across it.</li>
<li>Double left click to move immediately to a specific place in the model.</li>
</ul>
</div></div>

