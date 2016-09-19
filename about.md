---
layout: page
title: About
permalink: /about.html/
---

<ul>
{% for member in site.data.members %}
  <li>
    <a href="https://github.com/{{ member.github }}">
      {{ member.name }}
    </a>
  </li>
{% endfor %}
</ul>


Some information about you!

### More Information

A place to include any other types of information that you'd like to include about yourself.

### Contact me

[tungns.stackoverflow@gmail.com](mailto:tungns.stackoverflow@gmail.com)
