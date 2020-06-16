---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---


{% include base_path %}

{% if author.googlescholar %}
  <p>
    For full list of publications, please refer to
    <u>
      <a href="{{author.googlescholar}}">my Google Scholar profile</a>.
    </u>
  </p>
{% endif %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
