---
layout: infolab-toplevel
title: Research
permalink: /research/
header:
  overlay_image: /assets/images/banner_small.jpg
  overlay_filter: "0.4"
toc: true
---

Through interdisciplinary collaborations, we strive to advance data-driven life science and to bridge the gap between algorithmic innovation and real-world impact in healthcare and beyond.

Our research is currently focused on developing AI-based methods for 

- early detection of oral cancer from cytology data, and 
- immuno-therapy response prediction for lung cancer from histology data. 

# Research projects
{: .page-title}

<h2> Test header (does it go to ToC?) </h2>

{% for area in site.data.research_areas %}
---
<div class="research-area-entry">
<a href="{{ area.url }}" class="research-area-box">
     <div class="research-area-figure">
          <figure class="no-margins">
               <img src="{{ area.img }}" class="research-area-img" alt="{{ area.img_alt }}"/>
          </figure>
     </div>
     <div class="pull-up">
          <h2 class="research-area-text-size text-in-img research-area-header">{{ area.name }}</h2>
     </div>
</a>
<div class="research-area-text">
{{ area.description }} <a href="{{ area.url }}">Read more</a>
</div>
</div>
{% endfor %}
---
               




