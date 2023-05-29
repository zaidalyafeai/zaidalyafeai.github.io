---
layout: archive
title: "Selected Publications"
permalink: /publications/
author_profile: true
---

See full list of articles at <a href="https://scholar.google.com/citations?user=vb6w6j4AAAAJ&hl=en">my Google Scholar profile</a>.

{% include base_path %}

<!-- {% assign publications = site.publications | sort: Citations.size %} -->

<!-- {% for i in site.publications %}
  {% assign wrapped = i.Citations | floor | compact %}
  {% assign b = b | concat: wrapped %}
{% endfor %}

{% assign c = b | sort %} -->

{% for post in site.publications %}
  {% assign citations = post.Citations | plus: 0 %}
  {% if citations >= 400 %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

{% for post in site.publications %}
  {% assign citations = post.Citations | plus: 0 %}
  {% if citations >= 200 and citations <= 400 %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

{% for post in site.publications %}
  {% assign citations = post.Citations | plus: 0 %}
  {% if citations >= 50 and citations <= 100 %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

{% for post in site.publications %}
  {% assign citations = post.Citations | plus: 0 %}
  {% if citations >= 30 and citations <= 50 %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

{% for post in site.publications %}
  {% assign citations = post.Citations | plus: 0 %}
  {% if citations >= 20 and citations <= 30 %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

{% for post in site.publications %}
  {% assign citations = post.Citations | plus: 0 %}
  {% if citations >= 10 and citations <= 20 %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
