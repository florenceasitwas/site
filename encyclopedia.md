---
layout: page
title: Encyclopedia Fiorentina
image:
---

Here you will find the compendium of all our Florentine research and scholarship.

*Work in Progress*

---
{% for item in site.culture | where: "status", "live" %}
  [{{ item.title }}]({{ item.url }})
{% endfor %}
---
{% for person in site.people | where: "status", "live" %}
  [{{ person.title }}]({{ person.url }})
{% endfor %}
---
{% for place in site.sites | where: "status", "live" %}
  [{{ place.title }}]({{ place.url }})
{% endfor %}
---
{% for text in site.texts | where: "status", "live" %}
  [{{ text.title }}]({{ text.url }})
{% endfor %}
