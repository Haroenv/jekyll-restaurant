<footer>
	<div>
		<h3>Contact</h3>
		<ul>
		{% for nr in site.details.phone %}
			<li><a href="tel:{{ nr }}">{{ nr }}</a></li>
		{% endfor %}
		{% for u in site.details.address %}
			<li>{{ u }}</li>
		{% endfor %}
		</ul>
	</div>
	<div>
		<h3>About</h3>
		<p>{{ site.details.slogan }}</p>
	</div>
	<div>
		<p>Made by <a href="http://haroen.me">Haroen</a></p>
	</div>
</footer>
</body>
</html>
