---
layout: single
title: Our Team
---

{% assign sorted_team = site.data.team | sort:"last","first" %}


|:-:|--:|--:|--:|{% for member in sorted_team %}
| ![]({{member.photo}}){: style="border-radius:50%;"} |  {{ member.name }} | {{ member.title }} | <a href="{{member.linkedin}}"><i class="fab fa-linkedin"></i></a> <a href="{{member.web}}"><i class="fas fa-external-link-alt"></i></a> |{% endfor %}
