---
layout: default
---
|Product  |Description  |Price  |
|---|---|
{% for product in site.products -%}
{% if product.name -%}
|{{ product.name }}  |{{ product.content | remove: '<p>' | remove: '</p>' }}  |
{% endif %}
{%- endfor -%}