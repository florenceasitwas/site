---
layout: page
title: Project Blog
---

<div class="posts">
	{% for post in site.posts %}
	<article>
		<h3>{{ post.title }}</h3>
		{% if post.tags.size > 0 %}
			<ul class="tags">Tag{% if post.tags.size > 1 %}s{% endif %}:
			<a href="{{ 'blog.html' | absolute_url }}">{{ post.tags | join: " " }}</a></ul>
		{% endif %}
		{{ post.excerpt }}
		<ul class="actions">
      <li><a href="{{ post.url | absolute_url }}" class="button small">Continue</a></li>
    </ul>
	</article>
	{% endfor %}
</div>
