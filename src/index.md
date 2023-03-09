---
title: Home
layout: base.njk
tags: navItem
---
# {{title}}

My Home Page!

This is the home page. Replace this with your text.

1. First item
2. Second item
3. Third item

## heading 2

### Design Work

<ul>
    {%- for project in collections.design -%}
    <li><a href="{{project.url}}">{{project.data.title}}</a></li>
    {%- endfor -%}
</ul>

<div class="projects">
{%- for project in collections.design -%}
<figure class="project"><a href="{{project.url}}"><img src="/images/{{project.data.img.src}}" alt="{{project.data.img.alt}}"></a>
    <figcaption><a href="{{project.url}}">{{project.data.title}}</a></figcaption>
    </figure>
{%- endfor -%}
</div>

