---
layout: default
---
|Product  |Price  |Description  |
|---|---|
{% if product.name -%}
{% for product in site.products -%}
|{{ product.name }}  |{{ product.price }}  |{{ product.content | remove: '<p>' | remove: '</p>' }}  |
{% endif %}
{%- endfor -%}