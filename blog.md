---
layout: page
title: Project Blog
image: team-croce-feb22.jpg
---

This blog represents an ongoing record of our contributors' efforts, thoughts, work processes, and more.

<div class="posts">
	{% for post in site.posts %}
	<ul >
      <li><a href="{{ post.url | absolute_url }}" class="button small">{{post.title}}</a> - {{ post.date | date_to_long_string  }}</li>
    </ul>
	{% endfor %}
</div>




<div class="posts">
	{% for post in site.posts %}
		<h3>{{ post.title }}</h3>
		{% if post.tags.size > 0 %}
			<ul class="tags">Tag{% if post.tags.size > 1 %}s{% endif %}:
			<a href="{{ 'blog.html' | absolute_url }}">{{ post.tags | join: " " }}</a></ul>
		{% endif %}
		{{ post.excerpt }}
		<ul class="actions">
      <li><a href="{{ post.url | absolute_url }}" class="button small">Continue</a></li>
    </ul>
	{% endfor %}
</div>
