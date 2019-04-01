---
layout: layout
---

<div class="content">
<div class="timeline">
  {% assign postsByYear = site.posts | group_by_exp:"post", "post.date | date: '%Y'" %}
      {% for year in postsByYear %}

        <div class="yearblock">
          <div class="year">{{ year.name }}</div>



        {% assign postsByMonth = year.items | group_by_exp:"post", "post.date | date: '%B'" %}

        {% for month in postsByMonth %}

<div class="divider"></div>
        <div class="monthblock">
          <div class="monthdot"></div>
          <div class="monthlabel">{{ month.name }}</div>
        </div>

  {% for post in month.items %}

        <div class="divider"></div>
        <div class="postblock">
          <div class="daylabel">22</div>
          <div class="posttitle"><a class="postlink" href="{{ post.url | prepend:'/blog' }}">{{ post.title }}</a></div>
        </div>
          {% endfor %}


        {% endfor %}
      {% endfor %}

      </div>
      </div>

      </div>
