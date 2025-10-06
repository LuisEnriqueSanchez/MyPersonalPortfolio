<!--
---
layout: list
title: Portfolio
permalink: /portfolio/
---
TESTING TEXT Here you will find my personal projects
-->

<!-- texto que me puso al IA-->
---
layout: page
title: Portfolio
---

This is a try to include the other post

<h1>My Projects</h1>
<ul>
{% for project in site.projects %}
  <li>
    <a href="{{ project.url }}">{{ project.title }}</a> - {{ project.description }}
  </li>
{% endfor %}
</ul>




