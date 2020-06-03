---
title: Acknowledgements2
---
# Acknowledgements2

{% for acknowledgement in site.data.acknowledgements.versions %}
## Version {{ acknowledgement.version }}  {{ acknowledgement.title }}
**Date:** {{ acknowledgement.date-start | date_to_long_string }} - {{ acknowledgement.date-end | date_to_long_string }}

### Credits
The {{ number.people | size }} people who influenced this version are detailed below, along with details of their contribution.

  {% for person in acknowledgement.people %}
- #### [{{person.name}}](person.link), {{person.company}}  
  *Contribution:* {{person.contribution}}
  {% endfor %}

{% endfor %}
