---
title: Performance Calendar
permalink: /calendar/
layout: page
---

{% assign events = site.events | sort: 'start-date' %}

{% for event in events %}
  <h2><a href="{{ event.url }}">{{ event.title }}</a></h2>
  <p>{{ event.summary }}
  <a href="{{ event.url }}">Click here</a> for more information.</p>
{% endfor %}
