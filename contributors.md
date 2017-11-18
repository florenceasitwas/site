---
layout: page
title: Contributors
---

{% assign current = site.contributors | where:"status","current" %}
{% assign past = site.contributors | where:"status","past" %}
{% assign collab = site.contributors | where:"status","collaborator" %}

## Current
<div class="posts">
  {% for person in current %}
    <article>
      {{ person.image }}
      {{ person.content }}
    </article>
  {% endfor %}
</div>

## Past
<div class="posts">
  {% for person in past %}
    <article>
      {{ person.content }}
    </article>
  {% endfor %}
</div>

## Collaborators
<div class="posts">
  {% for person in collab %}
    <article>
      {{ person.content }}
    </article>
  {% endfor %}
</div>
<!--

## Past

<div class="posts">
  {% for person2 in past %}
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
---

## Collaborators

<div class="posts">
  {% for person3 in collaborators %}
  <article>
    <div class="content">
      <h3>{{person3.title}}</h3>
      {{ person3.excerpt }}
      <h4>Contributions</h4>
      {{ person3.content }}
    </div>
  </article>
  {% endfor %}
</div>

-->
