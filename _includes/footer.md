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
		<p>Website by <a href="https://haroen.me">Haroen</a></p>
	</div>
</footer>
{% if site.google-analytics %}
<script>
(function (i, s, o, g, r, a, m) {
  i['GoogleAnalyticsObject'] = r;
  i[r] = i[r] || function() {
    (i[r].q = i[r].q || []).push(arguments)
  }, i[r].l = 1 * new Date();
  a = s.createElement(o),
  m = s.getElementsByTagName(o)[0];
  a.async = 1;
  a.src = g;
  m.parentNode.insertBefore(a, m)
})(window, document, 'script', '//www.google-analytics.com/analytics.js', 'ga');

ga('create', '{{ site.google-analytics }}', 'auto');
ga('send', 'pageview');
</script>
{% endif %}
</body>
</html>
