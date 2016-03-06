---
layout: page
title: Archives
---

{% for post in site.posts %}
  {% assign currentdate = post.date | date: "%Y" %}
  {% if currentdate != date %}
    {% unless forloop.first %}</ul>{% endunless %}
   <strong id="y{{post.date | date: "%Y"}}">{{ currentdate }}</strong>
   <ul>
    {% assign date = currentdate %}
  {% endif %}
   <li>{{ post.date | date: "%b %Y" }} – <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
  {% if forloop.last %}</ul>{% endif %}
{% endfor %}