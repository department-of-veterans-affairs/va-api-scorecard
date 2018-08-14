---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: documentation
---
## VA API Scorecard

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec a viverra augue. Duis ipsum ex, scelerisque quis semper nec, sollicitudin et tortor. Donec ac lobortis mauris, a malesuada metus. In hac habitasse platea dictumst. Mauris ac sodales nibh. Sed a gravida leo, et placerat metus. Quisque sed scelerisque turpis. Vivamus id imperdiet ipsum.

### API's
{% for api in site.data.store %}
  {% include api.html api=api %}
{% endfor %}
