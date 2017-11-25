---
layout: page
title: Encyclopedia Fiorentina
image:
---

Here you will find the compendium of all our Florentine research and scholarship.

*Work in Progress*

## Culture
<div class="posts">
  {% assign var1 = site.culture | where:"status","live" %}
  {% for item in var1 %}
    <article>
      <a href="{{ item.url }}">{{ item.title }}</a>
    </article>
  {% endfor %}
</div>

---

## People
<div class="posts">
  {% assign var2 = site.people | where:"status","live" %}
  {% for person in var2 %}
    <article>
      <a href="{{ person.url }}">{{ person.title }}</a>
    </article>
  {% endfor %}
</div>

---

## Sites
<div class="posts">
  {% assign var3 = site.sites | where:"status","live" %}
  {% for place in var3 %}
    <article>
      <a href="{{ place.url }}">{{ place.title }}</a>
    </article>
  {% endfor %}
</div>

---

## Texts
<div class="posts">
  {% assign var4 = site.texts | where:"status","live" %}
  {% for text in var4 %}
    <article>
      <a href="{{ text.url }}">{{ text.title }}</a>
    </article>
  {% endfor %}
</div>
