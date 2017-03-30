---
layout: group
title: activitysim
category: activitysim
tags: [activitysim, abm-platform ]
short-description: activitysim
github: https://github.com/UDST/activitysim
---

The following is a list of the projects 

<section class="tiles">

															
{% for project in site.projects %}
  	{% if project.tags contains page.category %}
  		<article class="style1 bigtile">
  			{% if project.img %}
  			<img src='{{ site.url }}/img/{{ project.img }}' alt="" />
  			{% else %}
  			<img src='{{ site.url }}/img/{{ site.default-tile-img }}' alt="" />
  			{% endif %}
    		<a href='{{ project.url }}'>
				<h2>{{ project.title }}</h2>
				<div class="content">
					<p>{{ project.short-description }}</p>
				</div>
			</a>
  		</article>
  
  	{% endif %}
{% endfor %}

</section>






