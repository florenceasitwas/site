---
layout: default
---
<!-- Section -->
<section>
	<header class="major">
		<h2>Project Blog</h2>
	</header>
	<div class="posts">
		{% for post in site.posts limit:6 %}
		<article>
				<h3>{{ post.title }}</h3>
				{% if post.tags.size > 0 %}
  				<ul class="tags">Tag{% if post.tags.size > 1 %}s{% endif %}:
  				<a href="{{ 'blog.html' | absolute_url }}">{{ post.tags | join: " " }}</a></ul>
				{% endif %}
				{{ post.excerpt }}
				<ul class="actions">
	        <li><a href="{{ 'blog.html' | absolute_url }}" class="button small">Continue</a></li>
	      </ul>
				<!-- <ul class="actions">
					<li><a href="{{ 'blog.html' | absolute_url }}" class="button">More</a></li>
				</ul> -->
		</article>
		{% endfor %}
	</div>
</section>

<!-- Section -->
<section>
	<header class="major">
		<h2>Resources</h2>
	</header>
	<div class="features">
		<article>
			<span class="icon fa-newspaper-o"></span>
			<div class="content">
				<h3>The Bigallo</h3>
				<p>Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.</p>
			</div>
		</article>
		<article>
			<span class="icon fa-newspaper-o"></span>
			<div class="content">
				<h3>Orsanmichele</h3>
				<p>One of the city's grandest examples of the Medieval and Renaissance connection between religion, politics, and art, the granary and later of Orsanmichele has an extremely complex history. To help make sense of it, we've collected some sources here for edification.</p>
			</div>
		</article>
	</div>
</section>

<!-- Section -->
<section>
	<header class="major">
		<h2>Buildings</h2>
	</header>
	<div class="posts">
		<article>
			<a href="{{ 'bigallo.html' | absolute_url }}" class="image"><img src="assets/images/bigallo_1.jpg" alt="" /></a>
			<h3>Bigallo</h3>
			<p>Explore the headquarters of one of the city's most prominent charities, the Confraternity of the Misericordia, later merged with that of the Bigallo, </p>
			<ul class="actions">
				<li><a href="{{ 'bigallo.html' | absolute_url }}" class="button">More</a></li>
			</ul>
		</article>
		<article>
			<a href="{{ 'orsanmichele.html' | absolute_url }}" class="image"><img src="assets/images/orsanmichele_1.jpg" alt="" /></a>
			<h3>Orsanmichele</h3>
			<p>View the monumental statues produced by Florence's leading sculptors for the city's guilds, which </p>
			<ul class="actions">
				<li><a href="{{ 'orsanmichele.html' | absolute_url }}" class="button">More</a></li>
			</ul>
		</article>
	</div>
</section>

<section>
	<div class="affiliation">
	<h2>Affiliations</h2>
	<a href="https://mellon.org/">
		<img src="assets/images/logo_mellon.png" alt="" height="100"></a>
	</div>
</section>
