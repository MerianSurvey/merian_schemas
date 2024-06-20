---
layout: schema_index
title: Science Data Model Schemas for Merian
---
This schema browser provides a view on a curated subset of the Merian Survey data products. 

Schemas available here for browsing include:

<ul>
    {%- assign schemas = site.pages | where: 'dir','/browser/' | sort: 'sort-index' %}
    {%- for schema in schemas %}
    {%- if schema.name != 'index.md' %}
    <li><a href="{{ schema.url | relative_url }}">{{ schema.title }}</a> {{ schema.content }}</li>
    {%- endif %}
    {%- endfor %}
</ul>
