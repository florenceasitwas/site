---
layout: page
title: Contributors
---

{% assign current = site.contributors | where:"status","current" %}
{% assign past = site.contributors | where:"status","past" %}
{% assign collab = site.contributors | where:"status","collaborator" %}

<!-- is this as sleek as possible, or can it be further optimized? AV -->

# Current
<div class="posts">
  {% for person in current %}
    <article>
      <span><img src="assets/images/headshots/{{person.image}}" /></span>
      {{ person.content }}
    </article>
  {% endfor %}
</div>

# Past
<div class="posts">
  {% for person in past %}
    <article>
      <span><img src="assets/images/headshots/{{person.image}}" /></span>
      {{ person.content }}
    </article>
  {% endfor %}
</div>

# Collaborators
<div class="posts">
  {% for person in collab %}
    <article>
      <span><img src="assets/images/headshots/{{person.image}}" /></span>
      {{ person.content }}
    </article>
  {% endfor %}
</div>
