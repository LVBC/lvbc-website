---
title: Sermon Archive
layout: layouts/base.njk
subtitle: Click on a link from the list below to listen to a previous sermon.
---

<ul class="listing">
{%- for page in collections.sermons -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLLL d, y") }}</time>
  </li>
{%- endfor -%}
</ul>