---
layout: page
---
{% for image in site.static_files %}
    {% if image.path contains 'assets/kuvat' %}
<img src="{{ site.baseurl }}{{ image.path }}" alt="kuva" />
    {% endif %}
{% endfor %}