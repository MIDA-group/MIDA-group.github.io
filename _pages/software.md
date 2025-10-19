---
layout: infolab-toplevel
title: Software
permalink: /software/
header:
  overlay_image: /assets/images/banner_small.jpg
  overlay_filter: "0.4"
toc: true
---

We strive to release all pieces of software that we create as open sorce on our [GitHub pages](https://github.com/MIDA-group/).


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
          <h2 class="research-area-text-size text-in-img research-area-header">{{ software.name }}</h2>
     </div>
</a>
<div class="research-area-text">
{{ software.description }} <a href="{{ software.url }}">Read more</a>
</div>
</div>
{% endfor %}
---
