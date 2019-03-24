---
layout: layout
title: Jekyll Base
---

<div class="content">
  <div class="related">
    <ul>
      {% for post in site.posts %}
      <li>
	<span>{{ post.date | date: "%B %e, %Y" }}</span> <a href="blog/{{ post.url }}">{{ post.title }}</a>
      </li>
      {% endfor %}
    </ul>
  </div>
</div>
