---
layout: archive
title: "Other"
permalink: /other/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## Conferences attended

## Organisation
{% if site.organisation_category %}
  {% for category in site.organisation_category  %}
    {% assign title_shown = false %}
    {% for post in site.organisation reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        <h2>{{ category[1].title }}</h2><hr />
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.organisation reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %} 
  
## Teaching
 I worked as a learning support assistant for mathematics in Bristol Brunel Academy between 2023 and 2025.
