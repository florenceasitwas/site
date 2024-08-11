---
layout: page
title: Contributors
---
{% assign principle = site.contributors | where:"status","principle" %}
{% assign current = site.contributors | where:"status","current" %}
{% assign past = site.contributors | where:"status","past" %}
{% assign collab = site.contributors | where:"status","collaborator" %}

<!-- is this as sleek as possible, or can it be further optimized? AV -->

# Principal Investigators

<div class="row">
    {% for person in principle %}
    <div class="col-lg-4">
        <img src="assets/images/headshots/{{ person.image }}" alt="{{ person.name }}" class="bd-placeholder-img rounded-circle" width="250" height="250" style="margin-bottom: 1rem;" preserveAspectRatio="xMidYMid slice" focusable="false">
        {{ person.content }}
    </div><!-- /.col-lg-4 -->
    {% endfor %}
</div><!-- /.row -->

# Current

<div class="row">
    {% for person in current %}
    <div class="col-lg-4">
        <img src="assets/images/headshots/{{ person.image }}" alt="{{ person.name }}" class="bd-placeholder-img rounded-circle" width="250" height="250" style="margin-bottom: 1rem;" preserveAspectRatio="xMidYMid slice" focusable="false">
        {{ person.content }}
    </div><!-- /.col-lg-4 -->
    {% endfor %}
</div><!-- /.row -->

{% comment %}
<div class="posts">
  {% for person in current %}
    <article>
      <span><img src="assets/images/headshots/{{person.image}}" /></span>
      {{ person.content }}
    </article>
  {% endfor %}
</div> 
{% endcomment %}

# Past

<div class="row">
    {% for person in past %}
    <div class="col-lg-4">
        <img src="assets/images/headshots/{{ person.image }}" alt="{{ person.name }}" class="bd-placeholder-img rounded-circle" width="250" height="250" >
        {{ person.content }}
    </div><!-- /.col-lg-4 -->
    {% endfor %}
</div><!-- /.row -->

{% comment %}
<div class="posts">
  {% for person in past %}
    <article>
      <span><img src="assets/images/headshots/{{person.image}}" /></span>
      {{ person.content }}
    </article>
  {% endfor %}
</div>
{% endcomment %}

# Collaborators

<div class="row">
    {% for person in collab %}
    <div class="col-lg-4">
        <img src="assets/images/headshots/{{ person.image }}" alt="{{ person.name }}" class="bd-placeholder-img rounded-circle" width="250" height="250" s>
        {{ person.content }}
    </div><!-- /.col-lg-4 -->
    {% endfor %}
</div><!-- /.row -->


{% comment %}
<div class="posts">
  {% for person in collab %}
    <article>
      <span><img src="assets/images/headshots/{{person.image}}" /></span>
      {{ person.content }}
    </article>
  {% endfor %}
</div>
{% endcomment %}












