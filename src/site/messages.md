---
title: Messages Archive
layout: layouts/base.njk
subtitle: Click on a link from the list below to listen to a previous message.
---

<ul class="listing">
{%- for page in collections.message -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
  </li>
{%- endfor -%}
</ul>