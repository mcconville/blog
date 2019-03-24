---
layout: layout
title: bringing this back to life ...
---

<div class="content">
<div>version 0.1.0</div>
  <div class="related">
    <ul>
      {% for post in site.posts %}
      <li>
	<span>{{ post.date | date: "%B %e, %Y" }}</span> <span>{{ post.url | prepend:'/blog' }}</span><a href="{{ post.url | prepend:'/blog' }}">{{ post.title }}</a>
      </li>
      {% endfor %}
    </ul>
  </div>
</div>
