{% include header.md %}
	<section class="content">
		{{ content }}
	</section>
	<section class="menu">
		<ul>
		{% for dish in site.data.menu %}
			<li>
				<ul>
					<li>{{dish.name}}</li>
					<li>{{dish.contains}}</li>
					<li>{{dish.price}}</li>
				</ul>
			</li>
		{% endfor %}
		</ul>
	</section>
{% include footer.md %}
