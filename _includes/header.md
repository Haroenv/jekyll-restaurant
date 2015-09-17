<!DOCTYPE html>
<html lang="en">
<head>
	<title> {{ site.details.name }}{% if page.title %} | {{ page.title }}{% endif %} </title>
	<meta charset="utf-8" />
	<meta name="viewport" content="width=device-width, initial-scale=1.0" />
	<meta name="apple-mobile-web-app-capable" content="yes" />
	<meta name="mobile-web-app-capable" content="yes" />
	<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent" />
	<meta name="theme-color" content="#{{ site.design.colours.accent }}" />
	<link rel="stylesheet" href="/css/style.css" />
	<!-- <link rel="icon" type="image/png" href="/assets/favicon.png" /> -->
	<!-- <link rel="apple-touch-icon" href="/assets/apple-touch-icon.png" /> -->
	<!-- <link rel="icon" href="/assets/apple-touch-icon.png"> -->
	<meta name="description" content="{{site.details.slogan}}" />
</head>

<body>
	<header>
		<h1><a href="/">{{site.details.name}}</a></h1>
		<nav>
			<ul>
				<li><a href="/">Home</a></li>
				<li><a href="/menu">Menu</a></li>
				<li><a href="/blog">Blog</a></li>
				<li><a href="/contact">Contact</a></li>
			</ul>
		</nav>
	</header>
