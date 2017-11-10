---
layout: page
title: Encyclopedia Fiorentina
image:
---

Here you will find the compendium of all our Florentine research and scholarship.

*Work in Progress*

---
{% assign var1 = site.culture where:“status”,"live" %}
{% for item in var1 %}
  [{{ item.title }}]({{ item.url }})
{% endfor %}
---
{% assign var2 = site.people where:“status”,“live” %}
{% for person in var2 %}
  [{{ person.title }}]({{ person.url }})
{% endfor %}
---
{% assign var3 = site.sites where:“status”,“live” %}
{% for var3 in site.sites %}
  [{{ place.title }}]({{ place.url }})
{% endfor %}
---
{% assign var4 = site.texts where:“status”,“live” %}
{% for var4 in site.texts %}
  [{{ text.title }}]({{ text.url }})
{% endfor %}
