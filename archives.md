---
title: Time-based Archives
layout: page
---

{% for post in site.posts %}
{% assign currentdate = post.date | date: "%B %Y" %}
{% if currentdate != date %}
{% unless forloop.first %}</ul>{% endunless %}

<h3 id="y{{post.date | date: "%B %Y"}}">{{ currentdate }}</h3>
<ul>
{% assign date = currentdate %}
{% endif %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% if forloop.last %}</ul>{% endif %}
{% endfor %}
