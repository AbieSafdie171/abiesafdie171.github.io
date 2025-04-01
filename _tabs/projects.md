---
layout: page
icon: fas fa-diagram-project
order: 2
---

<div class="projects-overview">
  <h1>Check out some of my projects!</h1>
  <ul>
    {% assign sorted_posts = site.projects | sort: "date" | reverse %}
    {% for post in sorted_posts %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.date | date: "%B %d, %Y" }} - {{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>
</div>