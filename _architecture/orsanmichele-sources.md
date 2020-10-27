---
layout: page
title: Original Sources on Orsanmichele 
status: 
---

<div class="encyclopedia">
<article>
<h2><span class="icon fa-file-text"></span> Documents</h2>
<ul>
{% assign var1 = site.sources | where:"building","orsanmichele" | where:"category","document" %}
{% for item in var1 %}
  <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
{% endfor %}
</ul>
</article>

<article>
<h2><span class="icon fa-globe"></span> Translations</h2>
<ul>
{% assign var2 = site.sources | where:"category","translation" | where:"building","orsanmichele" %}
{% for item in var2 %}
  <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
{% endfor %}
</ul>
</article>
</div>
