---
layout: infolab-toplevel
title: Publications
permalink: /publications/
header:
  overlay_image: /assets/images/banner_small.jpg
  overlay_filter: "0.4"
toc: true
---

Here we only list publications related to the activities of the lab. For other publications of the lab members you can consult their personal pages.

{% for publist in site.data.publications %}
## {{ publist.year }}

{% for pub in publist.publications %}
**{{ pub.title }}**<br/>
*{{ pub.author }}*<br/>
{% if pub.type == "article" %}{{ pub.journal }}, {% if pub.volume != nil %}Vol. {{ pub.volume }}{% if pub.number != nil %}({{ pub.number }}){% endif %},{% endif %} {{ pub.year }} {{% pub.note }}
{% elsif pub.type == "inproceedings" %}In: {{ pub.booktitle }}, {% if pub.volume != nil %}Vol. {{ pub.volume }}{% if pub.number != nil %}({{ pub.number }}){% endif %},{% endif %} {{ pub.year }} {{% pub.note }}
{% elsif pub.type == "chapter" %}Chapter in: {{ pub.book }}, {{ pub.year }} {{% pub.note }}
{% elsif pub.type == "thesis" %}{{ pub.description }}, {{ pub.year }} {{% pub.note }}
{% endif %}{% if pub.doi != nil %} doi: <a href="https://doi.org/{{ pub.doi }}">{{ pub.doi }}</a>{% endif %}{% if pub.pdf != nil %} (<a href="{{ pub.pdf }}">pdf</a>){% endif %}
{% if pub.arxiv != nil %} <b><font color=DarkGray>arXiv</font></b> preprint: <a href="https://doi.org/10.48550/arXiv.{{ pub.arxiv }}">arXiv.{{ pub.arxiv }}</a>{% endif %}
{% if pub.code != nil %} <b><font color=DarkOrange>Code</font></b> available at <a href="{{ pub.code }}">{{ pub.code }}</a>{% endif %}
{% endfor %}

{% endfor %}
