---
title: Research
nav:
  order: 2
  tooltip: Research focuses
---

# {% include icon.html icon="fa-solid fa-flask" %} Research Philosophy

The focus of the Lareau Lab is to understand how cells in our bodies adapt, expand, and
evolve during the course of our lives, particularly in the immune system.
The theme of our lab's research is **Computational and Translational Immunology**,
which is purposefully broad but grounds our research program in these tenets:
1. Each of our studies develops or utilizes advanced <b>computational</b> methods to discern patterns from large datasets, typically generated from genomics sequencing.
2. Inspired by the promise and demonstrated efficacy of immunotherapies, we focus our research to understand and manipulate properties of <b>immune</b> and hematopoietic cells.
3. We ask questions with <b>translational</b> relevance in mind. These may be derived from a specific clinical observation or framed to study a biological principle that may underlie disease or response to therapy.

We are particularly interested in how somatic evolution—the collection of mutations,
infections, and exposures to therapies that humans experience over a lifetime—reshapes fundamental cellular processes in the immune system. 

To conduct our work, our group develops and applies computational methods
and genomics-based technologies. 
We specialize in utilizing single-cell multi-omics approaches that profile multiple
orthogonal properties of the same cells, including cell state (i.e. accessible chromatin, RNA, and protein) as well as cell lineage (i.e. somatic mtDNA and nuclear mutations).
In addition to resolving the functional heterogeneity of immune cells throughout the body,
we hope to help translate our basic observations into safer and more efficacious cancer immunotherapies. 


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


{% include cols.html col1=c4s col2=kravis col3=nhgri %}

