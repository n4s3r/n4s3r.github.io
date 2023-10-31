---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<!DOCTYPE html>
<html>
<head>
    <!-- Tu código de encabezado aquí -->
</head>
<body>
    <!-- Contenido de la página de inicio -->
{% for lang in site.languages %}
  {% if forloop.index0 == 0 %}
    <a href="{{ page.url }}" class="footer__link">{{ lang }}</a>
  {% else %}
    |<a href="/{{ lang }}{{ page.url }}" class="footer__link">{{ lang }}</a>
  {% endif %}
{% endfor %}

     {{ content }}
</body>
</html>
