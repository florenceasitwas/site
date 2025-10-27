---
layout: page
title: Encyclopedia Fiorentina
image:
excerpt: Here you will find the compendium of all our Florentine research and scholarship.
status: live
---

  <p><em>Here you will find the compendium of all our Florentine research and scholarship.</em></p>

***

<div class="row">
<div class="col">
  <h2><span class="icon fa-university"></span> Architecture</h2>
  <ul>
   
  {% assign var1 = site.architecture | where:"status","live" | sort: "title", "first" %}
  {% for item in var1 %}
    <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
  {% endfor %}
  </ul>

   <h2><span class="icon fa-paint-brush"></span> Art</h2>

  {%- comment -%} Live art items, sorted by title {%- endcomment -%}
  {% assign art_all = site.art | where:"status","live" | sort_natural:"title" %}

  {%- comment -%}
  Group by artist:
  - Prefer front-matter 'artist'
  - Fallback: first chunk of title before the comma
  {%- endcomment -%}
  {% assign groups = art_all
     | group_by_exp: "i", "i.artist | default: i.title | split: ',' | first | strip" %}
  {% assign groups = groups | sort: "name" %}

  <div class="accordion" id="accordionArt">
    {% for g in groups %}
      {% assign artist = g.name %}
      {% assign panel_id = artist | slugify %}
      <div class="accordion-item">
        <h2 class="accordion-header" id="heading-{{ panel_id }}">
          <button class="accordion-button {% unless forloop.first %}collapsed{% endunless %}"
                  type="button"
                  data-bs-toggle="collapse"
                  data-bs-target="#collapse-{{ panel_id }}"
                  aria-expanded="{{ forloop.first }}"
                  aria-controls="collapse-{{ panel_id }}">
            {{ artist }} ({{ g.items | size }})
          </button>
        </h2>
        <div id="collapse-{{ panel_id }}"
             class="accordion-collapse collapse {% if forloop.first %}{% endif %}"
             data-bs-parent="#accordionArt">
          <div class="accordion-body">
            <ul class="mb-0">
              {% assign items_sorted = g.items | sort_natural:"title" %}
              {% for item in items_sorted %}
                <li><a href="{{ item.url | absolute_url }}">{{ item.title }}</a></li>
              {% endfor %}
            </ul>
          </div>
        </div>
      </div>
    {% endfor %}
  </div>


  <h2><span class="icon fa-balance-scale"></span> Culture</h2>
  <ul>
  {% assign var3 = site.culture | where:"status","live" | sort: 'title' %}
  {% for item in var3 %}
    <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
  {% endfor %}
  </ul>
</div>
<div class="col">

  <h2><span class="icon fa-file-text"></span> Sources</h2>
  <h3>Primary Source Documents</h3>

  <ul>
  {% assign var4 = site.sources | where:"status","live" | where:"type","primary-source" | sort: 'title' %}
    {% for item in var4 %}
        <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>      
    {% endfor %}
  </ul>

<h3>Modern Descriptions</h3>

{% assign desc = site.sources | where:"status","live" | where:"type","description" | sort:"title" %}

{%- comment -%} Build Paatz set by tag OR title {%- endcomment -%}
{% assign paatz_tagged = desc | where_exp:"i","i.tags and i.tags contains 'Paatz'" %}
{% assign paatz_titled = desc | where_exp:"i","i.title and i.title contains 'Paatz,'"%}
{% assign paatz_all = paatz_tagged | concat: paatz_titled %}



<div class="accordion" id="accordionDescriptors">
  <!-- Paatz -->
  <div class="accordion-item">
    <h2 class="accordion-header" id="heading-paatz">
      <button class="accordion-button" type="button"
              data-bs-toggle="collapse" data-bs-target="#collapse-paatz"
              aria-expanded="true" aria-controls="collapse-paatz">
        Paatz
      </button>
    </h2>
    <div id="collapse-paatz" class="accordion-collapse collapse" data-bs-parent="#accordionDescriptors">
      <div class="accordion-body">
        <ul class="mb-0">
          {% assign seen = "" %}
          {% for item in paatz_all %}
            {% unless seen contains item.url %}
              <li><a href="{{ item.url | absolute_url }}">{{ item.title }}</a></li>
              {% assign seen = seen | append: item.url | append: "|" %}
            {% endunless %}
          {% endfor %}
        </ul>
      </div>
    </div>
  </div>

  <!-- Others -->
  <div class="accordion-item">
    <h2 class="accordion-header" id="heading-others">
      <button class="accordion-button collapsed" type="button"
              data-bs-toggle="collapse" data-bs-target="#collapse-others"
              aria-expanded="false" aria-controls="collapse-others">
        Others (temp)
      </button>
    </h2>
    <div id="collapse-others" class="accordion-collapse collapse" data-bs-parent="#accordionDescriptors">
      <div class="accordion-body">
        <ul class="mb-0">
          {% for item in desc %}
            {% unless item.tags and item.tags contains 'Paatz' or item.title and item.title contains 'Paatz,' %}
              <li><a href="{{ item.url | absolute_url }}">{{ item.title }}</a></li>
            {% endunless %}
          {% endfor %}
        </ul>
      </div>
    </div>
  </div>
</div>

  <h2><span class="icon fa-users"></span> People</h2>
  <ul>
  {% assign var5 = site.people | where:"status","live" | sort: 'title' %}
  {% for item in var5 %}
    <li><a href="{{ item.url | absolute_url }}">{{item.title}}</a></li>
  {% endfor %}
  </ul>

  <h2>19th Century Views of Florence</h2>
  <p><a href="{{site.url}}/19th-century-views-of-florence.html">View paintings by Fabio Borbottoni</a></p>
</div>


</div>

