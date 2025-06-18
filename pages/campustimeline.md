---
title: Campus Building Timeline
layout: default
permalink: /campustimeline.html
---

<div class="py-3" markdown="1">
{%- assign buildings = '/assets/data/timeline-buildings.json' -%}
{% include feature/timelinejs.html json=buildings %}
</div>