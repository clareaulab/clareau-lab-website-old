---
title: Research
nav:
  order: 2
  tooltip: What we do
---

# {% include icon.html icon="fa-solid fa-wrench" %}Computational and Translational Immunology

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

{% include section.html %}

{% capture immuno %}

{%
  include figure.html
  image="images/immune.jpg"
  caption="Our group focuses on questions involving the immune system and immunotherapies."
%}

{% endcapture %}

{% capture nycr %}

{%
  include figure.html
  image="images/nyc.jpg"
  caption="The lab is located in Zuckerman Research Center at Sloan Kettering in New York City."
%}

{% endcapture %}

{% capture csb %}

{%
  include figure.html
  image="images/cs.jpg"
  caption="We specialize in computational methods for massive-scale genomics data."
%}

{% endcapture %}

{% include cols.html col1=immuno col2=csb col3=nycr %}


## Research focuses

{% include list.html component="card" data="projects" filters="group: " style="small" %}
