{% include header.md %}
	<section class="content">
		{{ content }}
	</section>
	<section class="menu">
		<ul>
		{% for dish in site.data.menu %}
			<li>
				<ul>
					<li class="name">{{dish.name}}</li>
					<li class="contains">{{dish.contains}}</li>
					<li class="price">{{dish.price}}</li>
				</ul>
			</li>
		{% endfor %}
		</ul>
	</section>
{% include footer.md %}
