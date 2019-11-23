---
layout: default
---
|Product  |Price  |Description  |
|---|---|---|
{% for product in site.products -%}
{%- if product.name -%}
|{{ product.name }}  |{{ product.price }}  |{{ product.content | remove: '<p>' | remove: '</p>' }}  |
{%- endif -%}
{%- endfor -%}