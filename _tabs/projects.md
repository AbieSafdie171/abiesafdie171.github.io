---
layout: page
icon: fas fa-diagram-project
order: 2
---

<div class="projects-overview">
  <h1>Check out my projects!</h1>
	<ul>
	  {% assign sorted_projects = site.projects | sort: "title" %}
	  {% for project in sorted_projects %}
	    <li>
	      <a href="{{ project.url | relative_url }}">{{ project.title }}</a>
	    </li>
	  {% endfor %}
	</ul>
</div>