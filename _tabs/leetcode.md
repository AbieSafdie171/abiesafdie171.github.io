---
layout: page
icon: fas fa-code-compare
order: 1
---

<div class="leetcode-overview">
  <h1>Check out my work on the Daily Leetcode!</h1>
  <ul>
    {% assign sorted_posts = site.leetcode | sort: "date" | reverse %}
    {% for post in sorted_posts %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.date | date: "%B %d, %Y" }} - {{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>
</div>
