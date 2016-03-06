---
layout: page
title: Archive
---

{% for post in site.posts %}
  * {{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ site.baseurl }}{{ post.url }})
{% endfor %}

---

{% for post in site.posts %}
  {% assign currentdate = post.date | date: "%Y" %}
  {% if currentdate != date %}
   <li id="y{{currentdate}}">{{ currentdate }}</li>
    {% assign date = currentdate %} 
  {% endif %}
   <li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}