---
title: Performance Calendar
permalink: /calendar/
layout: page
---

{% assign events = site.events | sort: 'start-date' %}

{% for event in events %}
  <h2><a href="{{ event.url }}">{{ event.title }}</a></h2>
  <p>{{ event.summary }}</p>
{% endfor %}
