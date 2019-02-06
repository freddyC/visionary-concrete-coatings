---
title: Learn
layout: layouts/base.njk
---

## Topics

<ul class="listing">
{%- for page in collections.post -%}
  <div>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLL d, y") }}</time>
  </div>
{%- endfor -%}
</ul>

## Past Jobs
<ul class="listing">
{%- for page in collections.jobs -%}
  <div>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLL d, y") }}</time>
  </div>
{%- endfor -%}
</ul>