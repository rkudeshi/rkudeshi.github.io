---
layout: page
title: Archives
permalink: /archives
redirect_from: /archive
---

{% for post in site.posts %}
  {% assign currentdate = post.date | date: "%Y" %}
  {% if currentdate != date %}
    {% unless forloop.first %}{% endunless %}
   <h4 id="archives-year">{{ currentdate }}</h4>
    {% assign date = currentdate %}
  {% endif %}
   <div class="archives-list">
   <span class="archives-dates">{{ post.date | date: "%b %Y" }}</span>
   <span class="archives-titles"><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></span>
   </div>
  {% if forloop.last %}{% endif %}
{% endfor %}