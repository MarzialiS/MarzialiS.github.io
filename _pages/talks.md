---
title: "Talks and Presentations"
permalink: /talks/
layout: single
author_profile: true
---

{% assign all_talks = site.talks | sort: "date" | reverse %}

{% if all_talks.size > 0 %}
  {% for talk in all_talks %}
    {% include archive-single.html item=talk %}
  {% endfor %}
{% else %}
  <p>No talks to display.</p>
{% endif %}
