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
		<h3>Social</h3>
		<ul>
			{% if site.details.twitter %}<li><a href="https://twitter.com/{{site.details.twitter}}">twitter</a>{% endif %}
			{% if site.details.facebook %}<li><a href="https://facebook.com/{{site.details.facebook}}">facebook</a>{% endif %}
			{% if site.details.email %}<li><a href="mailto:{{site.details.email}}">email</a>{% endif %}
		</ul>
		<p>Website by <a href="http://haroen.me">Haroen</a></p>
	</div>
</footer>
</body>
</html>
