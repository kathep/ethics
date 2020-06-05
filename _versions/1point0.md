---
object-id: 1point0
layout: version
version: 1.0
title: Ethical Visualization Workflow
date: 2018-12-01
image:
pdf:
---

Some summary of this version here.

{% capture label %}{{ page.object-id  }}{% endcapture %}


  {% for person in site.data.acknowledgements.[label].people %}

    <li>

    {% if person.link %}
      <a href="{{ person.link }}">
      {{ person.name }}
      </a>
    {% else %}
      {{ person.name }}
    {% endif %}

    {% if person.company %}
       at {{ person.company }}
    {% else %}

    {% endif %}

    </li>

  {% endfor %}
