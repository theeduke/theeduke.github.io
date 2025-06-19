---
title: "Projects"
permalink: /projects/
layout: archive
author_profile: true
collection: projects
---

Explore my portfolio of projects, showcasing my expertise in backend development, RESTful APIs, and Python-based frameworks. Each project highlights the problem solved, technologies used, and my contributions.
<ul>
  {% for project in site.projects %}
    <li><a href="{{ project.url }}">{{ project.title }}</a></li>
  {% endfor %}
</ul>


