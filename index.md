---
layout: default
---
<!-- Section -->
<section>
	<header class="major">
		<h2>Project Blog</h2>
	</header>
	<div class="posts">
		{% for post in site.posts limit:4 %}
		<article>
				<a href="florence-site/{{ post.url }}" class="image"><img src="assets/images/{{ post.image }}"></a>
				{{ post.excerpt }}
				<ul class="actions">
					<li><a href="{{ 'blog.html' | absolute_url }}" class="button">More</a></li>
				</ul>
		</article>
		{% endfor %}
	</div>
</section>

<!-- Section -->
<section>
	<header class="major">
		<h2>Articles</h2>
	</header>
	<div class="features">
		<article>
			<span class="icon fa-newspaper-o"></span>
			<div class="content">
				<h3>The Bigallo</h3>
				<p>Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.</p>
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
			<a href="#" class="image"><img src="assets/images/pic01.jpg" alt="" /></a>
			<h3>Bigallo</h3>
			<p>Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.</p>
			<ul class="actions">
				<li><a href="#" class="button">More</a></li>
			</ul>
		</article>
		<article>
			<a href="#" class="image"><img src="assets/images/pic02.jpg" alt="" /></a>
			<h3>Baptistery</h3>
			<p>Aenean ornare velit lacus, ac varius enim lorem ullamcorper dolore. Proin aliquam facilisis ante interdum. Sed nulla amet lorem feugiat tempus aliquam.</p>
			<ul class="actions">
				<li><a href="#" class="button">More</a></li>
			</ul>
		</article>
	</div>
</section>

<section>
	<div class="affiliation">
	<a href="https://mellon.org/">
		<img src="assets/images/logo_mellon.png" alt="" height="100"></a>
	</div>
</section>
