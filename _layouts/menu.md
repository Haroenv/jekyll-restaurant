{% include header.md %}
	<section class="content">
		{{ content }}
	</section>
	<section class="menu">
		<ul>
		{% for dish in site.data.menu %}
			<li>
				<ul class="dish">
					<li class="name">{{dish.name}}</li>
					<li class="price">{{dish.price}}</li>
					<li class="contains">{{dish.contains}}</li>
				</ul>
			</li>
		{% endfor %}
		</ul>
	</section>
<!-- 	<pre>
{% for dish in site.data.menu %}
{{ dish }}
{% endfor %}
	</pre> -->
{% include footer.md %}
