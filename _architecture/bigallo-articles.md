---
layout: page
title: Articles on the Bigallo 
status: 
---

<div class="encyclopedia">
<article>
<h2><span class="icon fa-paint-brush"></span> Art</h2>
<ul>
{% assign var1 = site.art | where:"building","bigallo" %}
{% for item in var1 %}
  <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
{% endfor %}
</ul>
</article>

<article>
<h2><span class="icon fa-users"></span> People</h2>
<ul>
{% assign var2 = site.people | where:"building","bigallo" %}
{% for item in var2 %}
  <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
{% endfor %}
</ul>
</article>
</div>