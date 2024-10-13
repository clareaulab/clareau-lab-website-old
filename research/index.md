---
title: Research
nav:
  order: 2
  tooltip: Research focuses
---

# {% include icon.html icon="fa-solid fa-flask" %} Research Philosophy

We are a team of interdisciplinary scientists that specializes in <b>computational and translational immunology</b>.
Specifically, our group develops and utilizes single-cell multi-omics technologies and
computational biology to study human hematopoietic system as how immune cells change as we age and 
are exposed to pathogens, including endemic viruses. 
We seek to leverage principles from genomics technologies to improve the safety and efficacy of 
new therapies for cancer and other diseases.


{% include section.html %}

## Focus areas

Check out our publications on each of the lab's major areas of focus:

{% include list.html component="card" data="projects" filters="group: " style="small" %}


{% include section.html %}

## Funding

Our research is currently supported by the generous contributions from these sources:

{% capture mskcc %}
{%
  include figure.html
  image="images/funding/mskcc.png"
%}
{% endcapture %}

{% capture kravis %}
{%
  include figure.html
  image="images/funding/kravis-ecosystems.png"
%}
{% endcapture %}

{% capture nhgri %}
{%
  include figure.html
  image="images/funding/nhgri.png"
%}
{% endcapture %}

{% capture c4s %}
{%
  include figure.html
  image="images/funding/c4s.png"
%}
{% endcapture %}

{% capture hvp %}
{%
  include figure.html
  image="images/funding/hvp.png"
%}
{% endcapture %}

{% capture commonfund %}
{%
  include figure.html
  image="images/funding/commonfund.png"
%}
{% endcapture %}

{% capture ncicc %}
{%
  include figure.html
  image="images/funding/nci-cc.png"
%}
{% endcapture %}


{% include cols.html col1=c4s col2=kravis col3=hvp %}
{% include cols.html col1=commonfund col2=nhgri col3=ncicc %}

