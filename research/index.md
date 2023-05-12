---
title: Research
nav:
  order: 2
  tooltip: 
---

# {% include icon.html icon="fa-solid fa-wrench" %}Research

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.



{% capture content %}
  {% include images/gifs/mitochondria.gif ... %}
{% endcapture %}

{%
  include float.html
  content=content
  flip=true
%}

Several paragraphs of text here on mitos


{% capture content %}
  {% include mages/gifs/DNK.gif ... %}
{% endcapture %}

{%
  include float.html
  content=content
  flip=true
%}

Several paragraphs of text here on mitos

{% include float.html clear=true %}


{% include tags.html tags="publication, resource, website" %}

{% include search-info.html %}

{% include section.html %}

## Featured

{% include list.html component="card" data="projects" filters="group: featured" %}

{% include section.html %}

## More

{% include list.html component="card" data="projects" filters="group: " style="small" %}
