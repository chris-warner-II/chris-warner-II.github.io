---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
header:
  image: "https://chris-warner-ii.github.io/images/flower_path.JPG"
---

{% include base_path %}

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

<ol>{% for post in site.publications reversed %}
  <li>{% include archive-single.html %}</li>
{% endfor %}</ol>
