---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
>
All the models shown on this website are created by the extremely talented [Dennis Haupt](https://3dhaupt.com/). I chose to use his models because they are all made to the highest quality possible and there is minimal hassle in texturing the models because he has provided all the texture files that he used throughout his project (unlike many other models I've found). Please note that this site is just a proof of concept, and that I am not actually selling the models that he has made available to the world for the low, low price of $0. 

<hr>

{% for product in site.products %}
  {% include product.html %}
{% endfor %}