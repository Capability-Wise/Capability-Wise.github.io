---
layout: blog-master
title: Capability Wise Pty Ltd - Insights
permalink: /insights/
---

<div class="row">
	<div class="col-md-6 col-md-offset-4 text-center">
		<ul class="nav nav-pills nav-pills-primary">
			<li class="active"><a href="#all" data-toggle="tab">All</a></li>
			<li><a href="#business" data-toggle="tab">Business</a></li>
			<!-- <li><a href="#supplychain" data-toggle="tab">Supply Chain</a></li> -->
			<li><a href="#technology" data-toggle="tab">Technology</a></li>
		</ul>
	</div>
</div>
<div class="row">
		<div class="tab-content tab-space">

		<div class="tab-pane active" id="all">
		{% for blog-page in site.categories.blog  limit:10 %}

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
			<h6 class="category text-info">{{blog-page.categories[1]}}</h6>
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
	</div>
		{%else%}
		<div class="col-md-6">
			<div class="card card-raised card-background" style="background-image: url({{ blog-page.excerpt-image}})">
			<div class="card-content">
				<h6 class="category text-info">{{blog-page.categories[1]}}</h6>
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
		</div>
		{%endif%}

 {% endfor %}
 </div>



			<div class="tab-pane" id="business">
				{% for blog-page in site.categories.business  limit:10 %}
				{% if forloop.index <=3 %}
					<div class="col-md-6">
						<div class="card card-raised card-background" style="background-image: url({{ blog-page.excerpt-image}})">
							<div class="card-content">
								<h6 class="category text-info">Business</h6>
								<a href="{{ blog-page.url | absolute_url }}">
									<h3 class="card-title">{{ blog-page.title }}</h3>
								</a>
								<p class="card-description">
									{{blog-page.excerpt | truncate: 250}}
								</p>
								<a href="{{ blog-page.url | absolute_url }}" class="btn btn-danger btn-round">
									<i class="material-icons">format_align_left</i> Read Article
								</a>
							</div>
						</div>
					</div>
				{%endif%}
				{%endfor%}
			</div>
							<div class="tab-pane" id="supplychain">
							{% for blog-page in site.categories.supplychain  limit:10 %}
				{% if forloop.index <=3 %}
					<div class="col-md-6">
						<div class="card card-raised card-background" style="background-image: url({{ blog-page.excerpt-image}})">
							<div class="card-content">
								<h6 class="category text-info">Supply Chain </h6>
								<a href="{{ blog-page.url | absolute_url }}">
									<h3 class="card-title">{{ blog-page.title }}</h3>
								</a>
								<p class="card-description">
									{{blog-page.excerpt | truncate: 250}}
								</p>
								<a href="{{ blog-page.url | absolute_url }}" class="btn btn-danger btn-round">
									<i class="material-icons">format_align_left</i> Read Article
								</a>
							</div>
						</div>
					</div>
				{%endif%}
				{%endfor%}
							</div>
							<div class="tab-pane" id="technology">
							{% for blog-page in site.categories.technology  limit:10 %}
				{% if forloop.index <=3 %}
					<div class="col-md-6">
						<div class="card card-raised card-background" style="background-image: url({{ blog-page.excerpt-image}})">
							<div class="card-content">
								<h6 class="category text-info">Technology</h6>
								<a href="{{ blog-page.url | absolute_url }}">
									<h3 class="card-title">{{ blog-page.title }}</h3>
								</a>
								<p class="card-description">
									{{blog-page.excerpt | truncate: 250}}
								</p>
								<a href="{{ blog-page.url | absolute_url }}" class="btn btn-danger btn-round">
									<i class="material-icons">format_align_left</i> Read Article
								</a>
							</div>
						</div>
					</div>
				{%endif%}
				{%endfor%}

						</div>

					</div>
				</div>

