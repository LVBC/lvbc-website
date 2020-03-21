---
title: Messages
layout: layouts/base.njk
subtitle: Listen to our archive of previous messages.
---

<ul class="listing">
{%- for page in collections.message -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
  </li>
{%- endfor -%}
</ul>