---
title: Acknowledgements2
---
# Acknowledgements2

{% for acknowledgement in site.data.acknowledgements %}
## Version {{ acknowledgement.version }}
#### Date: {{ acknowledgement.date-start | date_to_long_string }} - {{ acknowledgement.date-end | date_to_long_string }}

  {% for person in version.people %}
Mr {{person.name}}</p>
  {% endfor %}

  {% for person2 in site.data.acknowledgements.version %}
- <strong>Ms {{ person2.name }}</strong>  
  {{ person2.company }}, {{ person2.company }}
  {% endfor %}

{% endfor %}
