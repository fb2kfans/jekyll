---
layout: page
title: Hello World!
tagline: Supporting tagline
---
{% include JB/setup %}

记录遇到的问题，以作参考。

记录总结经验。

学习和分享。

# Posts list

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>

<p class="rss-subscribe">subscribe <a href="{{ "/rss.xml" | prepend: site.baseurl }}">via RSS</a></p>
