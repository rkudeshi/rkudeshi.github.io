---
layout: page
title: Topics
---

{% comment %}
=======================
The following part extracts all the tags from your posts and sort tags, so that you do not need to manually collect your tags to a place.
=======================
{% endcomment %}

{% assign rawtags = "" %}
{% for post in site.posts %}
	{% assign ttags = post.tags | join:'|' | append:'|' %}
	{% assign rawtags = rawtags | append:ttags %}
{% endfor %}
{% assign rawtags = rawtags | split:'|' | sort %}



{% comment %}
=======================
The following part removes duplicated tags and invalid tags like blank tag.
=======================
{% endcomment %}

{% assign tags = "" %}
{% for tag in rawtags %}
	{% if tag != "" %}
		{% if tags == "" %}
			{% assign tags = tag | split:'|' %}
		{% endif %}
		{% unless tags contains tag %}
			{% assign tags = tags | join:'|' | append:'|' | append:tag | split:'|' %}
		{% endunless %}
	{% endif %}
{% endfor %}

{% comment %}
=======================
The purpose of this snippet is to list all the tags you have in your site.
=======================
{% endcomment %}

{% for tag in tags %}
<a href="#{{ tag | slugify }}"> {{ tag }} </a>
{% endfor %}


{% comment %}
=======================
The purpose of this snippet is to list all your posts posted with a certain tag.
=======================
{% endcomment %}

{% for tag in tags %}
<h4 id="{{ tag | slugify }}">{{ tag }}</h4>
<ul>
	{% for post in site.posts %}
	{% if post.tags contains tag %}
	<li>
		<a href="{{ post.url }}">{{ post.title }}</a>
		{% for tag in post.tags %}
		<small><small><a class="tag" href="#{{ tag | slugify }}">[{{ tag }}]</a></small></small>
		{% endfor %}
	</li>
	{% endif %}
	{% endfor %}
</ul>
{% endfor %}
