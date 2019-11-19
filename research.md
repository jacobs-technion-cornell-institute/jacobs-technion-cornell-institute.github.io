---
layout: single
title: Research
---

{% assign cornell_list  = site.data.partners | where: "tag", "cornell"  | sort: "name" %}
{% assign technion_list = site.data.partners | where: "tag", "technion" | sort: "name" %}


Some research collaborations in the urban tech space:

## At Cornell
<ul>
{%- for item in cornell_list -%}
    <li><a href="{{item.url}}">{{item.name}}</a></li>
{%- endfor -%}
</ul>

## At the Technion
<ul>
{%- for item in technion_list -%}
    <li><a href="{{item.url}}">{{item.name}}</a></li>
{%- endfor -%}
</ul>