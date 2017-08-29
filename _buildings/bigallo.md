---
layout: page
title: The Bigallo
---

<div class="sketchfab-embed-wrapper">
<iframe width="100%" height="480" src="https://sketchfab.com/models/611e480a37db4ddca53216bfe7c98dc0/embed" frameborder="0" allowvr allowfullscreen mozallowfullscreen="true" webkitallowfullscreen="true" onmousewheel=""></iframe>
  <p style="font-size: 14px; font-weight: normal; margin: 5px; color: #4A4A4A;">
      <a href="https://sketchfab.com/models/611e480a37db4ddca53216bfe7c98dc0?utm_medium=embed&utm_source=website&utm_campain=share-popup" target="_blank_" style="font-weight: bold; color: #1CAAD9;">Bigallo</a>
      by <a href="https://sketchfab.com/FLAW?utm_medium=embed&utm_source=website&utm_campain=share-popup" target="_blank_" style="font-weight: bold; color: #1CAAD9;">Florence As It Was</a>
      on <a href="https://sketchfab.com?utm_medium=embed&utm_source=website&utm_campain=share-popup" target="_blank_" style="font-weight: bold; color: #1CAAD9;">Sketchfab</a>
  </p>
</div>

<!--<img src="assets/images/borbottoni_bigallo.jpg" width="100%">-->
<div>
<span><img src="/assets/images/borbottoni_bigallo.jpg" width="100%">
<img src="/assets/images/tobia_e_tobiolo.jpg" width="100%"></span>
</div>
<!--<ul>
  <a href="{{ 'bigallo_paatz.html' | absolute-url }}">Notes on the Bigallo by Paatz</a>
  <br/>
  <a href="{{ '' | absolute-url }}">Del Migliore</a>
  <br/>
  <a href="{{ '' | absolute-url }}">Richa</a>
  <br/>
  <a href="{{ 'bigallo_passerini.html' | absolute-url }}">Passerini</a>
  <br/>
  <a href="{{ 'bigallo_hotspots.html' | absolute-url }}">Model Hotspots</a>
</ul>-->


{% assign texts = (site.texts | where:"building", "bigallo") %}
{% for text in texts %}
<ul><a href="{{ text.url | absolute_url }}">{{ text.title }}</a></ul>
{% endfor %}
