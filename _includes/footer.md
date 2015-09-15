<footer>
	<section>
		<h3>Contact</h3>
		<ul>
		{% for nr in site.details.phone %}
			<li><a href="tel:{{ nr }}">{{ nr }}</a></li>
		{% endfor %}
		{% for u in site.details.address %}
			<li>{{ u }}</li>
		{% endfor %}
		</ul>
	</section>
	<section>
		<h3>About</h3>
		<p>{{ site.details.slogan }}</p>
	</section>
	<section>
	</section>
</footer>
</body>
</html>
