---
layout: page
title: Encyclopedia Fiorentina
image:
excerpt: Here you will find the compendium of all our Florentine research and scholarship.
status: live
---

  <p><em>Here you will find the compendium of all our Florentine research and scholarship.</em></p>

***

<div class="row">
<div class="col">
  <h2><span class="icon fa-university"></span> Architecture</h2>
  <ul>
   
  {% assign var1 = site.architecture | where:"status","live" | sort: "title", "first" %}
  {% for item in var1 %}
    <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
  {% endfor %}
  </ul>

  <h2><span class="icon fa-paint-brush"></span> Art</h2>
  <ul>
  {% assign var2 = site.art | where:"status","live" | sort: 'title' %}
  {% for item in var2 %}
    <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
  {% endfor %}
  </ul>


  <h2><span class="icon fa-balance-scale"></span> Culture</h2>
  <ul>
  {% assign var3 = site.culture | where:"status","live" | sort: 'title' %}
  {% for item in var3 %}
    <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
  {% endfor %}
  </ul>
</div>
<div class="col">

  <h2><span class="icon fa-file-text"></span> Original Sources</h2>
  <ul>
  {% assign var4 = site.sources | where:"status","live" | sort: 'title' %}
    {% for item in var4 %}
        <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>      
    {% endfor %}
  </ul>



  <h2><span class="icon fa-users"></span> People</h2>
  <ul>
  {% assign var5 = site.people | where:"status","live" | sort: 'title' %}
  {% for item in var5 %}
    <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
  {% endfor %}
  </ul>

  <h2>19th Century Views of Florence</h2>
  <p><a href="{{site.url}}/19th-century-views-of-florence.html">View paintings by Fabio Borbottoni</a></p>
</div>


</div>

