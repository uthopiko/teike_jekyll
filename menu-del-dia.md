---
layout: default
title: Menu del día
permalink: /menu-del-dia/
---
{% for section in site.data.menu-del-dia.sections %}
<div class="menu_degustacion_subtitle">{{ section.name }}</div>
{% for dish in section.dishes %}
<div>{{ dish }}</div>
{% endfor %}
{% endfor %}