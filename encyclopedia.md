---
layout: page
title: Encyclopedia Fiorentina
image:
---

Here you will find the compendium of all our Florentine research and scholarship.

*Work in Progress*

---

<!-- dear future website worker: I'm sure there's a better way to do this, which is why I have entrusted it to your capable mind. AV -->


### Culture

 <ul>
{% assign var1 = site.culture | where:"status","live" %}
  {% for item in var1 %}
     <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
  {% endfor %}

</ul>

---

### People

<ul>
{% assign var2 = site.people | where:"status","live" %}
  {% for item in var2 %}
     <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
  {% endfor %}
</ul>

---


### Sites
<ul>
  {% assign var3 = site.sites | where:"status","live" %}
    {% for item in var3 %}
      <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
    {% endfor %}
</ul>

---

### Texts
<ul>
{% assign var4 = site.texts | where:"status","live" %}
  {% for item in var4 %}
      <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>      
  {% endfor %}
</ul>