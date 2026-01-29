---
title: "Talks and Presentations"
permalink: /talks/
layout: single
author_profile: true
---

## Invited seminars

{% assign invited_talks = site.talks | where: "talk_type", "invited" | sort: "date" | reverse %}
{% for talk in invited_talks %}
  {% include archive-single.html item=talk %}
{% endfor %}

---

## Conference and workshop presentations

{% assign conf_talks = site.talks | where: "talk_type", "conference" | sort: "date" | reverse %}
{% for talk in _talks %}
  {% include archive-single.html item=talk %}
{% endfor %}
