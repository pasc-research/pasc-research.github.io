---
title: "Donate"
permalink: "/donate.html"
---


<header>
	<div class="container">
		<div class="column">
			<div>
				<h1 class="editable">Some Text</h1>
				<p class="editable">Some Text</p>
				<div class="button">
					<a href="#donate">Donate Now</a>
				</div>
			</div>
		</div>
		<div class="column">
			<img src="{{ site.baseurl }}/assets/images/1.png" alt="Sheep">
		</div>
	</div>
</header>

<!-- <div class="container">
	<h2 class="editable" style="text-align: center;">Some Text</h2>

	<ul class="thirds">
		<li>
			<div class="image">{% include icons/site.html icon="population" %}</div>
			<h3 class="editable">Some Text</h3>
			<p class="editable">Some Text </p>
		</li>

		<li>
			<div class="image">{% include icons/site.html icon="economy" %}</div>
			<h3 class="editable">Some Text</h3>
			<p class="editable">Some Text</p>
		</li>

		<li>
			<div class="image">{% include icons/site.html icon="conditions" %}</div>
			<h3 class="editable">Some Text</h3>
			<p class="editable">Some Text</p>
		</li>
	</ul>
</div> -->

<!-- <div class="container">
	<div class="columns">
		<div>
			<img src="{{ site.baseurl }}/images/sheep2.jpg" alt="Sheep">
		</div>
		<div>
			<h2 class="editable">Our Mission</h2>

			<p class="editable">Some Text</p>
		</div>
	</div>
</div>

<div class="container">
	<hr>
	<blockquote>
		<p class="quote editable">The ultimate measure of a sheep is not where he stands in moments of comfort and convenience, but where he stands at times of challenge and controversy.</p>
		<div class="attribute">
			<p class="meta">
				<span class="image"><img class="editable" src="{{ site.baseurl }}/images/wooly.jpg" alt="Wooly"></span>
				<span class="author editable"><strong>Wooly McBaa</strong></span>
			</p>
		</div>
	</blockquote>
</div> -->

<div class="darker">
	<div class="container">
		<h2 class="editable">Join us</h2>
		<p class="editable" style="text-align: center;">Sign up to hear the latest news and progress </p>
		<form action="{{ site.newsletter_action }}" method="post">
			<input type="text" name="EMAIL" placeholder="Email">
			<input type="submit" value="Sign up"/>
		</form>
	</div>
</div>

<div class="container" id="donate">
	<h2 class="editable">Make a donation</h2>
	<div class="donate">
		{{ site.donation_embed }}
	</div>
</div>

<div class="darker">
	<div class="container">
		<h2 class="editable">Updates</h2>
		<p class="editor-link"><a href="cloudcannon:collections/_posts" class="btn"><strong>&#9998;</strong> Add Update</a></p>
		<div class="posts">
			{% for post in site.posts %}
				<div class="post">
					<!-- <div class="image" style="background-image: url({{ post.featured_image}})"></div> -->
					<div class="post-content">
						<p class="date">{{ post.date | date: '%B %d, %Y' }}</p>
						<h3>{{ post.title }}</h3>

						{{ post.content }}
						<p class="editor-link"><a href="cloudcannon:collections/{{ post.path }}" class="btn"><strong>&#9998;</strong> Edit Update</a></p>
					</div>
				</div>
			{% endfor %}
		</div>
	</div>
</div>