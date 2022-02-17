---
layout: default
title: Carta
permalink: /carta/
---
<div class="menu_degustacion_title">CARTA</div>
{% for section in site.data.carta.sections %}
<div class="menu_degustacion_subtitle">{{ section.name }} {{section.note}}</div>
{% for dish in section.dishes %}
{% if section.name == "BURGER" %}<p class="burger_title"><strong>{{ dish.name }}</strong></p><p class="dish_info"><div class="dish_name">{{dish.description}}</div> <div class="dish_price">{{ dish.price }}</div></p>
{% else %}
<p class="dish_info"><div class="dish_name">{{dish.name}}</div> <div class="dish_price">{{ dish.price }}</div></p>
{% endif %}


{% endfor %}
{% endfor %}