---
layout: page
title: Encyclopedia Fiorentina
image:
---

Here you will find the compendium of all our Florentine research and scholarship.


<div class="row encyclopedia">
<article>
<h2><span class="icon fa-university"></span> Architecture</h2>
<ul>
{% assign var1 = site.architecture | where:"front_page","live"  %}
{% for item in var1 %}
  <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
{% endfor %}
</ul>
</article>



<article>
<h2><span class="icon fa-paint-brush"></span> Art</h2>
<ul>
{% assign var2 = site.art | where:"status","live" | sort: 'title' %}
{% for item in var2 %}
  <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
{% endfor %}
</ul>
</article>
</div>


<div class="row encyclopedia">
<article>
<h2><span class="icon fa-balance-scale"></span> Culture</h2>
<ul>
{% assign var3 = site.culture | where:"status","live" | sort: 'title' %}
{% for item in var3 %}
  <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
{% endfor %}
</ul>
</article>


<article>
  <h2><span class="icon fa-file-text"></span> Original Sources</h2>
  <ul>
  {% assign var4 = site.sources | where:"status","live" | sort: 'title' %}
    {% for item in var4 %}
        <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>      
    {% endfor %}
  </ul>
</article>

</div>


<div class="row encyclopedia">


<article>
<h2><span class="icon fa-users"></span> People</h2>
<ul>
{% assign var5 = site.people | where:"status","live" | sort: 'title' %}
{% for item in var5 %}
  <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
{% endfor %}
</ul>
</article>



</div>