{% include header.md %}
	<section class="content">
		{{ content }}
	</section>
	{% for dish in site.data.menu %}
		<li>{{dish}}</li>
	{% endfor %}
{% include footer.md %}
