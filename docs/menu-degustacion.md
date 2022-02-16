---
layout: default
title: Menu Degustación
permalink: /menu-degustacion/
---
<div class="menu_degustacion_title">MENÚ DEGUSTACIÓN</div>
<div class="menu_degustacion_subtitle"><span class="menu_number">BAJO RESERVA</span></div>
{% for menu_item in site.data.menu %}
{% if menu_item.id == 0 %}
<p>{{menu_item.name}}</p>
{% else%}
{% if menu_item.id < 7 %}
<p><span class="menu_number">{{ menu_item.id }}</span>{{ menu_item.name }}</p>
{% endif%}
{% if menu_item.id == 7 %}
<p class="last_menu_item"><span class="menu_number">{{menu_item.id}}</span>{{menu_item.name}}</p>
{% endif %}
{% endif %}
{% endfor %}

<p>Menú corto 5 pases: 37 €</p>
<p>Menú largo 7 pases: 45 €</p>
<p>El menú degustación incluye agua, pan y cafe</p>
<p>El menú degustación se sirve mesa completa</p>