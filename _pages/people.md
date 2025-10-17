---
layout: infolab-toplevel
title: People
permalink: /people/
header:
  overlay_image: /assets/images/banner_small.jpg
  overlay_filter: "0.4"
---

# Members

<div class="profiles"> 
{% for person in site.data.people.members %}
{% if person.url != nil %}<a href="{{ person.url }}">{% endif %}
<figure class="profile">
  <img class="profilepic" src="{{ person.pic }}" alt="{{ person.name }}">
  <figcaption class="profile">
  <p>{{ person.name }} <br/> {{ person.title }}</p>
  </figcaption>
</figure>
{% if person.url != nil %}</a>{% endif %}
{% endfor %}
<div class="stop"/>
</div>



# Alumni

{% for person in site.data.people.alumni %}
**{{ person.name }}**, {{ person.role }} ({{ person.year }})<br/>
{% if person.url != "" %}<a href="{{ person.url }}">*{{ person.thesis }}*</a>.
{% else %}*{{ person.thesis }}*.{% endif %}
{% endfor %}
