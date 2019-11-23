---
layout: default
---
|Product  |Price  |Description  |
|---|---|
{% if product.name -%}
{% for product in site.products -%}
|{{ product.name }}  |{{ product.content | remove: '<p>' | remove: '</p>' }}  |{{ product.price }}  |
{% endif %}
{%- endfor -%}