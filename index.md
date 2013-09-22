---
layout: page
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts %}
    <li>
      <span>{{ post.date | date_to_string }}</span> &raquo;
      <h3>{{ post.title }}</h3>
      <p>{{ post.content[ 0 .. 100 ] }}<i> ... <a href="{{ BASE_PATH }}{{ post.url }}">Read More</a></i></p>
      <hr>
    </li>
  {% endfor %}
</ul>
