---
layout: page
title: Historic Figures
---

## Artists
{% assign artists = (site.people | where:"category", "artist") %}
<div class="posts">
  {% for person in artists %}
  <article>
    <span><img src="{{ person.image | absolute-url }}" />
    <div class="content">
      <h3>{{person.title}}</h3>
      {{ person.excerpt }}
      <ul class="actions">
        <li><a href="{{ person.url | absolute-url }}" class="button small">Continue</a></li>
      </ul>
    </div></span>
  </article>
  {% endfor %}
</div>

## Patrons
{% assign patrons = (site.people | where:"category", "patron") %}
<div class="posts">
  {% for person in patrons %}
  <article>
    <span><img src="{{ person.image }}" /></span>
    <div class="content">
      <h3>{{person.title}}</h3>
      {{ person.excerpt }}
      <ul class="actions">
        <li><a href="{{ person.url | absolute_url }}" class="button small">Continue</a></li>
      </ul>
    </div>
  </article>
  {% endfor %}
</div>

## Politicians
{% assign politicians = (site.people | where:"category", "politician") %}
<div class="posts">
  {% for person in politicians %}
  <article>
    <span><img src="{{ person.image }}" /></span>
    <div class="content">
      <h3>{{person.title}}</h3>
      {{ person.excerpt }}
      <ul class="actions">
        <li><a href="{{ person.url | absolute_url }}" class="button small">Continue</a></li>
      </ul>
    </div>
  </article>
  {% endfor %}
</div>

<hr>

## Historians
{% assign historians = (site.people | where:"category", "historian") %}
<div class="posts">
  {% for person in historians %}
  <article>
    <span><img src="{{ person.image }}" /></span>
    <div class="content">
      <h3>{{person.title}}</h3>
      {{ person.excerpt }}
      <ul class="actions">
        <li><a href="{{ person.url | absolute_url }}" class="button small">Continue</a></li>
      </ul>
    </div>
  </article>
  {% endfor %}
</div>
