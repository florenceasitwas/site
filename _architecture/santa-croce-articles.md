---
layout: page
title: Articles on Santa Croce 
status: 
---

<div class="encyclopedia">




<article>
<h2><span class="icon fa-paint-brush"></span> Art</h2>
<ul>
{% assign var1 = site.art | where:"building","santa-croce" %}
{% for item in var1 %}
  <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
{% endfor %}
</ul>
</article>

<article>
<h2><span class="icon fa-balance-scale"></span> Culture</h2>
<ul>
{% assign var3 = site.culture | where:"building","santa-croce" | sort: 'title' %}
{% for item in var3 %}
  <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
{% endfor %}
</ul>
</article>
</div>
<div class="encyclopedia">
<article>
<h2><span class="icon fa-users"></span> People</h2>
<ul>
{% assign var2 = site.people | where:"building","santa-croce" %}
{% for item in var2 %}
  <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
{% endfor %}
</ul>
</article>
</div>