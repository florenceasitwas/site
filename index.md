---
layout: default
---

<!-- Section -->
<section>
	<header class="major">
		<h2>Buildings</h2>
	</header>
	<div class="posts">
		<article>
			<a href="{{ '/buildings/bigallo.html' | absolute_url }}" class="image"><img src="assets/images/bigallo_1.jpg" alt="" /></a>
			<h3>Bigallo</h3>
			<p>Built in c. 1360, the Oratory of the Misericordia, as it was then known, has endured expansions, fires, renovations, a merger, and more to become the elegant structure that stands on the Piazza del Duomo today. Read more about the structure's tumultous history here. Explore the headquarters of one of the city's most prominent charities, the Confraternity of the Misericordia, later merged with that of the Bigallo, and see the art that it commissioned to assert its place in Florentine society.</p>
			<ul class="actions">
				<li><a href="{{ '/buildings/bigallo.html' | absolute_url }}" class="button small">More</a></li>
			</ul>
		</article>
		<article>
			<a href="{{ '/buildings/orsanmichele.html' | absolute_url }}" class="image"><img src="assets/images/orsanmichele_1.jpg" alt="" /></a>
			<h3>Orsanmichele</h3>
			<p>View the monumental statues produced by Florence's leading sculptors for the city's guilds, which were commissioned to decorate this grain market-turned-church. One of the city's grandest examples of the Medieval and Renaissance connection between religion, politics, and art, the granary and later church of Orsanmichele has an extremely complex history. To help make sense of it, we've collected some sources here for edification.</p>
			<ul class="actions">
				<li><a href="{{ '/buildings/orsanmichele.html' | absolute_url }}" class="button small">More</a></li>
			</ul>
		</article>
	</div>
</section>

<section>
	<header class="major">
		<h2>Models</h2>
	</header>
	<div class="posts">
		<article>
			<div class="sketchfab-embed-wrapper">
			<iframe width="100%" height="480" src="https://sketchfab.com/models/611e480a37db4ddca53216bfe7c98dc0/embed" frameborder="0" allowvr allowfullscreen mozallowfullscreen="true" webkitallowfullscreen="true" onmousewheel=""></iframe>
				<p style="font-size: 12px; font-weight: normal; margin: 5px; color: #4A4A4A;">
				    <a href="https://sketchfab.com/models/611e480a37db4ddca53216bfe7c98dc0?utm_medium=embed&utm_source=website&utm_campain=share-popup" target="_blank_" style="font-weight: bold; color: #1CAAD9;">Bigallo</a>
				    by <b>Sam Joseph</b> for <a href="https://sketchfab.com/FLAW?utm_medium=embed&utm_source=website&utm_campain=share-popup" target="_blank_" style="font-weight: bold; color: #1CAAD9;">Florence As It Was</a>
				    on <a href="https://sketchfab.com?utm_medium=embed&utm_source=website&utm_campain=share-popup" target="_blank_" style="font-weight: bold; color: #1CAAD9;">Sketchfab</a>
				</p>
			</div>
		</article>
		<article>
			<h3>The Loggia of the Bigallo</h3>
			<p>Florence As It Was's first 3D model is that of the Loggia of the Bigallo—one of Florence's most visible structures on the Piazza and a physical reminder of the city's rich Medieval past.</p>
			<p>Sam Joseph created the model using thousands images (which he took with a point-and-shoot camera and a tripod over the summer of 2017) and pieced it together using a process called photogrammetry. For future models, we hope to gain access to a high-resolution drone for detailed exteriors and a laser scanner for interiors.</p>
		</article>
	</div>
</section>

<!-- Section -->
<section id="resources">
	<header class="major">
		<h2>Resources</h2>
	</header>
	<div class="features">
		<article>
			<span class="icon fa-newspaper-o"></span>
			<div class="content">
				<h3>Del Migliore</h3>
				<p>Ferdinando del Migliore was born in 1628 and spent his adult life researching and writing about the history of Florence. A gifted archivist, del Migliore scoured the registers and contracts of individuals and institutions in an effort to present to his readers accurate accounts of the city’s past.</p>
				<span class="opener">Buildings</span>
				<ul>
				</ul>
			</div>
		</article>
		<article>
			<span class="icon fa-newspaper-o"></span>
			<div class="content">
				<h3>Richa</h3>
				<p>Richa - Italian, 1752-1760</p>
				<span class="opener">Buildings</span>
				<ul>
					<li><a href="http://florenceasitwas.wlu.edu/texts/bigallo-richa.html">Bigallo</a></li>
				</ul>
			</div>
		</article>
		<article>
			<span class="icon fa-newspaper-o"></span>
			<div class="content">
				<h3>Paatz</h3>
				<p>Paatz - German, 1952-1955 - A German husband-and-wife team of art historians with an incredible attention to detail.</p>
				<span class="opener">Buildings</span>
				<ul>
					<li><a href="http://florenceasitwas.wlu.edu/texts/bigallo-paatz.html">Bigallo</a></li>
				</ul>
			</div>
		</article>
		<article>
			<span class="icon fa-newspaper-o"></span>
			<div class="content">
				<h3>Miscellaneous</h3>
				<p>Miscellaneous - Context-dependent</p>
				<span class="opener">Buildings</span>
				<ul>
					{% assign texts = (site.texts | where:"category", "misc") %}
					{% for text in texts %}
					<li><a href="{{ text.url | absolute_url }}">{{ text.title }}</a></li>
					{% endfor %}
				</ul>
			</div>
		</article>
	</div>
</section>

<!-- Something here about Copyright and how we are not in violation of any copyright laws because the bulk of these materials have passed out of protection -->

<section>
	<div class="affiliation">
	<h2>Affiliations</h2>
	<a href="https://digitalhumanities.wlu.edu/">
		<img src="/assets/images/logo_dhwlu.png" alt="" height ="100"></a>&emsp;
	<a href="https://mellon.org/">
		<img src="assets/images/logo_mellon.png" alt="" height="100"></a>
	</div>
</section>
