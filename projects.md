---
layout: page
title: Projects
---

<ul class="post-list">
{%- for apage in site.pages -%}
    {%- if apage.project == true -%}
    <li>
    <h3>
        <a class="post-link" href="{{ apage.url | relative_url }}">
        {{ apage.title | escape }}
        </a>
    </h3>
        {{ apage.excerpt }}
    </li>
    {%- endif -%}    
{%- endfor -%}
</ul>