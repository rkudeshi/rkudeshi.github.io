---
layout: page
title: Archives
permalink: /archives
---

{% for post in site.posts %}
  {% assign currentdate = post.date | date: "%Y" %}
  {% if currentdate != date %}
    {% unless forloop.first %}</ul>{% endunless %}
   <h4 id="y{{post.date | date: "%Y"}}">{{ currentdate }}</h4>
   <ul>
    {% assign date = currentdate %}
  {% endif %}
   <li>{{ post.date | date: "%b %Y" }} – <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
  {% if forloop.last %}</ul>{% endif %}
{% endfor %}

---

{% for post in site.posts %}
  {% assign currentdate = post.date | date: "%Y" %}
  {% if currentdate != date %}
    {% unless forloop.first %}{% endunless %}
   <h4 id="y{{post.date | date: "%Y"}}">{{ currentdate }}</h4>
    {% assign date = currentdate %}
  {% endif %}
   <div class="archives-list">
   <span class="archives-dates">{{ post.date | date: "%b %Y" }}</span>
   <span class="archives-titles"><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></span>
   </div>
  {% if forloop.last %}{% endif %}
{% endfor %}