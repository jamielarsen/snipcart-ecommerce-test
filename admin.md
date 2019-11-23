---
layout: default
---
|Product  |Description  |Price  |
|---|---|
{% for product in site.products -%}
|{{ product.name }}  |{{ product.content | remove: '<p>' | remove: '</p>' }}  |{{ product.price }}  |
{%- endfor -%}