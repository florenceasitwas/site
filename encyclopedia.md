---
layout: page
title: Encyclopedia Fiorentina
image:
---

Here you will find the compendium of all our Florentine research and scholarship.

*Work in Progress*

---

<!-- dear future website worker: I'm sure there's a better way to do this, which is why I have entrusted it to your capable mind. AV -->

# Culture
<div class="posts">
  {% assign var1 = site.culture | where:"status","live" %}
  {% for item in var1 %}
    <article>
      {% if item.image %}
        <span class="image"><img src="assets/images/{{item.image}}" /></span>
      {% endif %}
      {{ item.excerpt }}
      <ul class="actions">
        <li><a href="{{ item.url | absolute_url }}" class="button small">More</a></li>
      </ul>
    </article>
  {% endfor %}
</div>

---

# People
<div class="posts">
  {% assign var2 = site.people | where:"status","live" %}
  {% for person in var2 %}
    <article>
      {% if person.image %}
        <span class="image"><img src="assets/images/{{person.image}}" /></span>
      {% endif %}
      <h2>{{ person.title }}: {{ person.dates }}</h2>
      {{ person.excerpt }}
      <ul class="actions">
        <li><a href="{{ person.url | absolute_url }}" class="button small">More</a></li>
      </ul>
    </article>
  {% endfor %}
</div>

---

# Sites
<div class="posts">
  {% assign var3 = site.sites | where:"status","live" %}
  {% for place in var3 %}
    <article>
      {% if place.image %}
        <span class="image"><img src="assets/images/{{place.image}}" /></span>
      {% endif %}
      <h2>{{ place.title }}: {{ place.dates }}</h2>
      {{ place.excerpt }}
      <ul class="actions">
        <li><a href="{{ place.url | absolute_url }}" class="button small">More</a></li>
      </ul>
    </article>
  {% endfor %}
</div>

---

# Texts
<div class="posts">
  {% assign var4 = site.texts | where:"status","live" %}
  {% for text in var4 %}
    <article>
      {% if text.image %}
        <span class="image"><img src="assets/images/{{text.image}}" /></span>
      {% endif %}
      <a href="{{ text.url }}">{{ text.title }}</a>
    </article>
  {% endfor %}
</div>
