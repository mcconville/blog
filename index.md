---
layout: layout
---

  <div class="content">
    <div class="related">
      <ul>
        {% for post in site.posts %}
        <li>
    	    <span>{{ post.date | date: "%B %e, %Y" }}</span>
          <a href="{{ post.url | prepend:'/blog' }}">{{ post.title }}</a>
        </li>
        {% endfor %}
      </ul>
    </div>
  </div>
