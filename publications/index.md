---
title: Publications
nav:
  order: 4
  tooltip: Lab papers
---

# {% include icon.html icon="fa-solid fa-book" %}Publications

{% include search-box.html %}
{% include search-info.html %}

{% include section.html %}

{%
  include button.html
  type="featured"
  text="Featured works"
  tooltip="Our greatest hits"
  link="https://clareaulab.com/publications/?search=featured"
%}

{%
  include button.html
  type="fire"
  text="Fresh preprints"
  tooltip="Pre-publication works"
  link="https://clareaulab.com/publications/?search=preprint"
%}

{%
  include button.html
  type="journal"
  text="Papers by topic"
  tooltip="Papers by lab focus"
  link="https://clareaulab.com/research/#focus-areas"
%}

{% include list.html data="citations" component="citation" style="rich" %}


