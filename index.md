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
			<a href="{{ '/sites/bigallo.html' | absolute_url }}" class="image"><img src="assets/images/bigallo_1.jpg" alt="" /></a>
			<h3>Bigallo</h3>
			<p>Built in c. 1360, the Oratory of the Misericordia, as it was then known, has endured expansions, fires, renovations, a merger, and more to become the elegant structure that stands on the Piazza del Duomo today. Read more about the structure's tumultous history here. Explore the headquarters of one of the city's most prominent charities, the Confraternity of the Misericordia, later merged with that of the Bigallo, and see the art that it commissioned to assert its place in Florentine society.</p>
			<ul class="actions">
				<li><a href="{{ '/sites/bigallo.html' | absolute_url }}" class="button small">More</a></li>
			</ul>
		</article>
		<article>
			<a href="{{ '/sites/orsanmichele.html' | absolute_url }}" class="image"><img src="assets/images/orsanmichele_1.jpg" alt="" /></a>
			<h3>Orsanmichele</h3>
			<p>View the monumental statues produced by Florence's leading sculptors for the city's guilds, which were commissioned to decorate this grain market-turned-church. One of the city's grandest examples of the Medieval and Renaissance connection between religion, politics, and art, the granary and later church of Orsanmichele has an extremely complex history. To help make sense of it, we've collected some sources here for edification.</p>
			<ul class="actions">
				<li><a href="{{ '/sites/orsanmichele.html' | absolute_url }}" class="button small">More</a></li>
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
			<p>Florence As It Was' first 3D model is that of the Loggia of the Bigallo, one of Florence's most visible structures on the Piazza San Giovanni and a physical reminder of the city's rich Medieval past. The structure housed charitable organizations that ministered to orphaned children, poor unwed girls, the homeless, and pilgrims on the way to and from Rome. These confraternities sponsored the creation of some of the city's most unique art in order to decorate their residence and proclaim their importance in the fabric of Florentine society. And like much of Florence's past, the Bigallo has undergone significant changes—changes that we hope to unravel, peeling back the layers of time to find the Medieval city that gave birth to the Italian Renaissance. The Bigallo, then, is a perfect starting point for our work, and a snapshot that captures the essence of Florence As It Was.</p>
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
				<p>Italian, 1628-1696</p>
				<p>Ferdinando del Migliore was born in 1628 and spent his adult life researching and writing about the history of Florence. A gifted archivist, del Migliore scoured the registers and contracts of individuals and institutions in an effort to present to his readers accurate accounts of the city’s past.</p>
					<li><a href="http://florenceasitwas.wlu.edu/texts/bigallo-migliore.html" class="essaylink">Migliore on the Bigallo</a></li>
			</div>
		</article>
		<article>
			<span class="icon fa-newspaper-o"></span>
			<div class="content">
				<h3>Richa</h3>
				<p>Italian, 1752-1760</p>
				<p></p>
					<li><a href="http://florenceasitwas.wlu.edu/texts/bigallo-richa.html" class="essaylink">Richa on the Bigallo</a></li>
			</div>
		</article>
		<article>
			<span class="icon fa-newspaper-o"></span>
			<div class="content">
				<h3>Paatz</h3>
				<p>Paatz - German, 1952-1955 - A German husband-and-wife team of art historians with an incredible attention to detail.</p>
				<li>
					<a href="http://florenceasitwas.wlu.edu/texts/bigallo-paatz.html" class="essaylink">Paatz on the Bigallo</a>
				</li>
			</div>
		</article>
		<article>
			<span class="icon fa-newspaper-o"></span>
			<div class="content">
				<h3>Miscellaneous</h3>
				<p>Context-Dependent Sources</p>
				{% assign texts = site.texts | where:"category", "misc" %}
				{% for text in texts %}
				<li><a href="{{ text.url | absolute_url }}">{{ text.title }}</a></li>
				{% endfor %}
			</div>
		</article>
	</div>
</section>

<!-- Something here about Copyright and how we are not in violation of any copyright laws because the bulk of these materials have passed out of protection -->

<section>
	<div class="affiliation">
	<h2>Affiliations</h2>
	<div>
		<a href="https://wlu.edu/">
			<img src="/assets/images/logo_wlu.png" alt="" height ="80"></a>&emsp;
		<a href="https://digitalhumanities.wlu.edu/">
			<img src="/assets/images/logo_dhwlu.png" alt="" height ="80"></a>&emsp;
		<a href="https://mellon.org/">
			<img src="assets/images/logo_mellon.png" alt="" height="80"></a>&emsp;
		<a href="https://www.uchicago.edu/">
			<img src="assets/images/logo_uchicago.png" alt="" height="60"></a>
	</div>
	</div>
</section>
