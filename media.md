---
layout: page
---
<h2>Videot</h2>
<div class="video">
	<iframe width="560" height="315" src="https://www.youtube.com/embed/LUHV2qxK0K8" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

<h2>Kuvat</h2>
{% for image in site.static_files %}
    {% if image.path contains 'assets/kuvat' %}
<img src="{{ site.baseurl }}{{ image.path }}" alt="kuva" />
    {% endif %}
{% endfor %}