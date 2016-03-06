---
layout: page
title: Archive
---

{% for post in site.posts %}
  {% assign currentdate = post.date | date: "%Y" %}
  {% if currentdate != date %}
    {% unless forloop.first %}</ul>{% endunless %}
   <h3 id="y{{post.date | date: "%Y"}}">{{ currentdate }}</h3>
   <ul>
    {% assign date = currentdate %}
  {% endif %}
   * {{ post.date | date: "%b %Y" }} — [ {{ post.title }} ]({{ site.baseurl }}{{ post.url }})
  {% if forloop.last %}</ul>{% endif %}
{% endfor %}