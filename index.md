---
layout: home
title: Home
---

<img src="/public/img/logo-700.jpg" alt="Marina orgánica." title="Marina orgánica.">

# Biopoder en manos del agricultor.

En _Marina orgánica_ producimos abonos y biofertilizantes orgánicos siguiendo recetas de la agricultura regenerativa. Nuestros productos son buenos para la tierra, las personas, la cosecha y el bolsido del agricultor.

## Productos

Actualmente tenemos disponibles los siguientes productos:

<div class="productos">
  {% assign items = site.productos | sort: 'weight' %}
  {% for producto in items %}
  <div class="producto">
    <h3 class="producto-title">
      <a href="{{ site.baseurl }}{{ producto.url }}">
        {{ producto.title }}
      </a> - {{ producto.price }}
    </h3>
  </div>
  {% endfor %}
  
  {% include pedidos.html %}
  
</div>
