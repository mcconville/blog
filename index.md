---
layout: layout
---

  <div class="content">
    <div class="related">
      <ul>
        {% for post in site.posts %}
        <li class="blogline">
    	    <span class="blogdate">{{ post.date | date: "%B %e, %Y" }}</span>
          <a class="bloglink" href="{{ post.url | prepend:'/blog' }}">{{ post.title }}</a>
        </li>
        {% endfor %}
      </ul>
    </div>
  </div>
