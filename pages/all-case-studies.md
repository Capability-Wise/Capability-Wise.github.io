---
layout: case-study-master
title: Capability Wise Pty Ltd - Case Studies
permalink: /case-studies/
---

<div class="row">
		{% for blog-page in site.categories.case-study %}

		{% assign loopItr = forloop.index | modulo: 3 %}

		{% assign loopClr = forloop.index | modulo: 3 %}
		{% if loopClr == 0 %}
			{% assign btn-colour = "warning" %}
		{% elsif loopClr ==1 %}
			{% assign btn-colour = "primary" %}
		{% else %}
			{% assign btn-colour = "danger" %}
		{% endif %}

	{% if loopItr == 0 %}
		<div class="col-md-12">
			<div class="card card-raised card-background" style="background-image: url({{ blog-page.excerpt-image}})">
			<div class="card-content">
				<h6 class="category text-info">Case Study</h6>
				<a href="{{ blog-page.url | absolute_url }}">
					<h3 class="card-title">{{ blog-page.title }}</h3>
				</a>
				<p class="card-description">
					{{blog-page.excerpt | truncate: 250}}
				</p>
				<a href="{{ blog-page.url | absolute_url }}" class="btn btn-{{btn-colour}} btn-round">
					<i class="material-icons">format_align_left</i> Read Article
				</a>
			</div>
		</div>
	{% else %}
<div class="col-md-6">
	<div class="card card-raised card-background" style="background-image: url({{ blog-page.excerpt-image}})">
		<div class="card-content">
			<h6 class="category text-info">Case Study</h6>
			<a href="{{ blog-page.url | absolute_url }}">
				<h3 class="card-title">{{ blog-page.title }}</h3>
			</a>
			<p class="card-description">
				{{blog-page.excerpt | truncate: 250}}
			</p>
			<a href="{{ blog-page.url | absolute_url }}" class="btn btn-{{btn-colour}} btn-round">
				<i class="material-icons">format_align_left</i> Read Article
			</a>
		</div>
	</div>
	{% endif %}  
</div>
	
 {% endfor %}
 </div>
