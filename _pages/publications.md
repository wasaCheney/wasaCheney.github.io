---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<!-- {% if author.googlescholar %} -->
For full list of publications, please refer to <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
<!-- {% endif %} -->

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
