---
layout: infolab-toplevel
title: Software
permalink: /software/
header:
  overlay_image: /assets/images/MIDA_logo.png
  overlay_filter: "0.4"
  overlay_position: "center 60%"
toc: true
---

# [GitHub pages](https://github.com/MIDA-group/) 
We strive to release all pieces of software that we create as open sorce on [GitHub](https://github.com/MIDA-group/).

---

# Maintained software
{: .page-title}

{% for software in site.data.softwares %}
---
<div class="research-area-entry">
<a href="{{ software.url }}" class="research-area-box">
     <div class="research-area-figure">
          <figure class="no-margins">
               <img src="{{ software.img }}" class="research-area-img" alt="{{ software.img_alt }}"/>
          </figure>
     </div>
     <div class="pull-up">
          <h2 id="header_{{ software.name }}" class="research-area-text-size text-in-img research-area-header">{{ software.name }}</h2>
     </div>
</a>
<div class="research-area-text">
{{ software.description }} <a href="{{ software.url }}">Read more</a>
</div>
</div>
{% endfor %}
---
