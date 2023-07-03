---
title: Publications
nav:
  order: 3
  tooltip: Lab papers
---

# {% include icon.html icon="fa-solid fa-book" %}Publications


{%
  include button.html
  type="featured"
  text="Featured works"
  tooltip="Our greatest hits"
  link="https://clareaulab.com/publications/?search=featured"
%}

{%
  include button.html
  type="preprint"
  text="Fresh preprints"
  tooltip="Pre-publication works"
  link="https://clareaulab.com/publications/?search=preprint"
%}

{%
  include button.html
  type="address"
  text="Papers by topic"
  tooltip="Papers by lab focus"
  link="https://clareaulab.com/research/#focus-areas"
%}

{% include section.html %}

{% include search-box.html %}
{% include search-info.html %}

{% include list.html data="citations" component="citation" style="rich" %}


