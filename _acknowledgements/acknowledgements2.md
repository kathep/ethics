---
title: Acknowledgements
---
# Acknowledgements

{% for acknowledgement in site.data.acknowledgements %}
## Version {{ acknowledgement.version }}
#### Date: {{ acknowledgement.date-start | date_to_long_string }} - {{ acknowledgement.date-start | date_to_long_string }}

<!--  <div class="people">
    <ul>
      {% for people in site.data.acknowledgements.people %}
        <li>
          <strong>Ms {{ people.name }}</strong><br>
          {{ people.company }}, {{ people.company }}
        </li>
      {% endfor %}
  </ul>
  </div>
{% endfor %} -->
