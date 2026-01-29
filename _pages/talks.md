---
title: "Talks and Presentations"
permalink: /talks/
layout: single
author_profile: true
---

## Invited seminars

{% assign invited_talks = site.talks 
   | where: "talk_type", "invited" 
   | sort: "date" 
   | reverse %}

{% if invited_talks.size > 0 %}
  {% for talk in invited_talks %}
    {% include archive-single.html item=talk %}
  {% endfor %}
{% else %}
  <p>No invited seminars to display.</p>
{% endif %}

---

## Conference and workshop presentations

{% assign conf_talks = site.talks 
   | where: "talk_type", "conference" 
   | sort: "date" 
   | reverse %}

{% if conf_talks.size > 0 %}
  {% for talk in conf_talks %}
    {% include archive-single.html item=talk %}
  {% endfor %}
{% else %}
  <p>No conference or workshop presentations to display.</p>
{% endif %}
