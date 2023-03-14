---
layout: page
title: Sources for the Bargello 
status: 
---

<div class="encyclopedia">
<article>
<h2><span class="icon fa-file-text"></span> Documents</h2>
<ul>
{% assign var1 = site.sources | where:"building","baptistery" | where:"category","document" %}
{% for item in var1 %}
  <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
{% endfor %}
</ul>
</article>
