---
layout: page
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts %}
    <li>
      <span>{{ post.date | date_to_string }}</span> &raquo;
      <h3>{{ post.title }}</h3>
      <p>{{ post.content | strip_html | truncate:300 }}<strong> ... <a href="{{ BASE_PATH }}{{ post.url }}">Read More</a></strong></p>
      <hr>
    </li>
  {% endfor %}
</ul>
