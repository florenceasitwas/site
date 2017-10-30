---
layout: page
title: Contributors
---

## Current
{% assign current = site.contributors where:“status”,“current” %}
<div class="posts">
  {% for person in current %}
  <article>
    <div class="content">
      <h3>{{person.title}}</h3>
      {{ person.excerpt }}
      <h4>Contributions</h4>
      {{ person.content }}
    </div>
  </article>
  {% endfor %}
</div>
___

## Past
{% assign past = site.contributors where:“status”,"past" %}
<div class="posts">
  {% for person in past %}
  <article>
    <div class="content">
      <h3>{{person.title}}</h3>
      {{ person.excerpt }}
      <h4>Contributions</h4>
      {{ person.content }}
    </div>
  </article>
  {% endfor %}
</div>
___

## Collaborators
{% assign collaborators = site.contributors where:“status”,"collaborator" %}
<div class="posts">
  {% for person in collaborators %}
  <article>
    <div class="content">
      <h3>{{person.title}}</h3>
      {{ person.excerpt }}
      <h4>Contributions</h4>
      {{ person.content }}
    </div>
  </article>
  {% endfor %}
</div>
