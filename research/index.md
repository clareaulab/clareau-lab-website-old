---
title: Research
nav:
  order: 3
  tooltip: Scientific focuses
---

# {% include icon.html icon="fa-solid fa-flask" %} Research Philosophy

We are a team of interdisciplinary scientists that specializes in <b>data-driven translational genomics</b>.
Our lab is a hybrid "wet" (experimental) and "dry" (bioinformatics) team. Our work tends to be interdisciplinary, 
but each individual project or researcher may focus more on experimental or computational innovation. Our lab does not rely on a model system or a specific experimental setting and instead focuses on data-driven
exploration, including the development of new technologies. Though not required, projects tend to fit within a part or all of a general framework with these three tenets:

<b>1. Translational motivation</b>. As our approach can be applied to any organism profiled
via DNA sequencing, we focus on questions that may directly impact human health,
including stem cell reconstitution, treatment side-effects, or limited therapeutic efficacy 
of cancer immunotherapies.

<b>2. Massive-scale data analyses</b>. The most appealing part of DNA- and RNA-sequencing
technologies, in our view, is that they sample a breadth and depth of nucleic acids
from cells or tissues. Rather than quantifying only some genes or proteins,
modern genomics technologies enable hypothesis generation and testing simultaneously
if handled with appropriate statistical rigor and data science convention.
In retrospective analyses, multiple datasets can be combined to structure questions that help mitigate observational biases.

<b>3. Genomics technology development</b>. Data-driven hypotheses can crystalize
from reanalyses but often lack definitive evidence. Our prior work has taught us that new
technologies are often required to test retrospective findings rigorously or 
scale up the number of measurements for proper inference. Thus, a major focus of the
experimental component of our group is to establish new technologies that, once developed, 
explain phenomenon in high-dimensional data or enable foundational new directions. 



{% include section.html background="images/scistories-clear-cut.png" dark=false %}

{% include section.html %}

## Focus areas

Check out our publications on each of the lab's major areas of focus:

{% include list.html component="card" data="projects" filters="group: " style="small" %}

{% include section.html background="images/scistories-clear-cut.png" dark=false %}

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
{% include cols.html col1=commonfund col2=ncicc col3=nhgri %}

