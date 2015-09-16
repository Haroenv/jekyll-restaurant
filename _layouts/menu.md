{% include header.md %}
	<section class="content">
		{{ content }}
	</section>
	{% for dish in site.data.menu %}
		<li>
			<ul>
				<li>{{dish.name}}</li>
				<li>{{dish.contains}}</li>
				<li>{{dish.price}}</li>
			</ul>
		</li>
	{% endfor %}
{% include footer.md %}
