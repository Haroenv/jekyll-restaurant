{% include header.md %}
	<section class="content">
		<span class="date">{{ page.date | date: "%-d %B %Y %-H:%M" }}</span>
		{{ content }}
		{% if page.next %}<a href="{{site.baseurl}}{{ page.next.url }}" rel="next">next</a> {% endif %}
		{% if page.previous %}<a href="{{site.baseurl}}{{ page.previous.url }}" rel="prev">prev</a> {% endif %}
	</section>
	{% if site.disqus %}
	<div id="disqus_thread"></div>
	<script src="//{{site.disqus}}.disqus.com/embed.js" async></script>
	{% endif %}
{% include footer.md %}
