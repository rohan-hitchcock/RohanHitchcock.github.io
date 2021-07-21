---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

My name is Rohan Hitchcock and I am currently a Masters student studying at 
the University of Melbourne. My supervisor is Dr Daniel Murfet. 


## Projects
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
