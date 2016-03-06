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
   <li>{{ post.date | date: "%b %Y" }} – <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
  {% if forloop.last %}</ul>{% endif %}
{% endfor %}

---

{% for post in site.posts %}
  {% assign currentdate = post.date | date: "%Y" %}
  {% if currentdate != date %}
### {{ currentdate }}
    {% assign date = currentdate %}
  {% endif %}
   * {{ post.date | date: "%b %Y" }} – [{{ post.title }}]({{ site.baseurl }}{{ post.url }})
{% endfor %}