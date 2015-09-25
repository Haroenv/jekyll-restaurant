{% include header.md %}
	<section class="content">
		{{ content }}
		{% if site.details.maps.token and site.details.maps.query %}
		<div class='embed-container map'>
				<iframe src='https://www.google.com/maps/embed/v1/place?key={{site.details.maps.token}}&amp;q={{site.details.maps.query}}'></iframe>
			</div>
		{% endif %}
	</section>
{% include footer.md %}
