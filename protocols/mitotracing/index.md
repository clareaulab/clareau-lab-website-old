---
title: Mitochondrial genomics and lineage tracing
---

# {% include icon.html icon="fa-solid fa-dna" %}Methods for mtDNA tracing

Our lab has been active in the development of new technologies to enable
lineage tracing in humans via mitochondrial DNA mutations. All of these works have been 
collaborative efforts with the [Leif Ludwig](https://www.mdc-berlin.de/ludwig) Lab
while we were trainees with Aviv Regev and Vijay Sankaran. See a summary of these major technologies, software, and informal guidelines below.


## Interested in mtDNA tracing?

Feel free to [reach out to Caleb](mailto:lareauc@mskcc.org), who can either answer your questions
or refer you to the right person who can help! 

# Genotyping via mtDNA

## Mitochondrial single-cell ATAC-seq

The mitochondrial single-cell ATAC-seq (mtscATAC-seq) protocol is an adaptation of 
commercial single-cell ATAC-seq workflows. At a basic level, by fixing and permeabilizing
cells (versus just nuclei), Tn5 also tagments the more accessible mitochondrial genome.
Accessible chromatin profiling can thereby be combined with single-cell whole mitochondrial genome sequencing.

{% include figure.html name="mtscatac" image="images/researchpngs/mtscatac-overview-wide.png" %}


## ASAP-seq and DOGMA-seq


Multiple mtscATAC-seq variant assays have been developed, for example,
[ATAC with select antigen profiling by sequencing (ASAP-seq)](https://www.nature.com/articles/s41587-021-00927-2) (with Eleni Mimitou and Peter Smibert); 
as well as 

{% include figure.html name="ASAP" image="images/researchpngs/asap-seq-wide.png" %}


The 10x Genomics Multiome kit has further facilitated the integration of transcriptional profiles,
yielding [DOGMA-seq](https://www.nature.com/articles/s41587-021-00927-2) (with Eleni Mimitou and Peter Smibert); 
this enables the single-cell capture of up to four data modalities, including transcriptome,
accessible chromatin, surface markers and mtDNA mutations.

{% include figure.html name="DOGMA" image="images/researchpngs/dogma-seq-wide.png" %}


## PHAGE-ATAC
[PHAGE-ATAC](https://www.nature.com/articles/s41587-021-01065-5) (with Evgenij Fiskin),
which in addition facilitate surface-marker profiling. In our experience, these approaches both work well 
and right-out-of-the-box if you have experience working with antibodies and/or phages. 

{% include figure.html name="MAESTER" image="images/researchpngs/phage-atac-wide.png" %}


Unless you have a specific reason to want the transcriptome (then use DOGMA-seq) or 
the surface proteome (then use ASAP-seq due to ease of commercially available reagents),
we recommend mtscATAC-seq due to the ease 
and cost-efficiency of the workflow. 


Another extension of the approach (though unrelated to our group) for the genotyping of 
targeted loci with single-cell chromatin accessibility [(GoT-ChA)](https://www.nature.com/articles/s41586-024-07388-y)
utilizes targeted primers to genotype nuclear variants in addition to optional mtDNA sequencing for high-resolution clonal analyses.


{% include section.html background="images/scistories-clear-cut.png" dark=false %}
{% include section.html %}

# Genotyping via mtRNA

## MAESTER
As >90% of mtDNA is transcribed, full-length RNA-seq techniques (e.g., Smart-seq) that capture
the entire sequence of a transcript are particularly attractive to capture genetic variants.
As relatively few groups use Smart-seq nowadays, approaches that are compatible with 
the more high-throughput and more popular 3′- or 5′-based scRNA-seq approaches were necessary. 
However, it's important to note that these approaches sequence 
only part of the transcript and thus tend to suffer from limited coverage of the mitochondrial
transcriptome for confident variant detection.

Enter [(MAESTER, below)](https://pubmed.ncbi.nlm.nih.gov/35210612/).
MAESTER can enrich mitochondrial mutations from existing cDNA libraries,
massively improving the suitability of these data for detecting and analyzing mtDNA
variants from high-throughput scRNA-seq data. 
MAESTER was the brain child of 
[Tyler Miller](https://tymillerlab.org/) and [Peter van Galen](https://vangalenlab.bwh.harvard.edu/), 
and we were happy to help out in finalizing its development. 

{% include figure.html name="MAESTER" image="images/researchpngs/maester-overview-wide.png" %}


In general, if you are regular user of 10x scRNA-seq, MAESTER may be a great entry-level 
assay for looking at mitochondrial genomes in your cells
However, there are a few noteworthy limitations of genotyping mitochondrial mutations from RNA alone.
First, note a high degree of inherent transcriptional error of the mitochondrial RNA polymerase,
which we have observed will lead to false-positive heteroplasmy detection. 
Additionally, not all mtDNA molecules may be equally transcribed or captured, including 
the 22 mitochondrial tRNAs are not reverse transcribed by poly(A)-based priming. 
We advise to download public data related to the assay that you plan to use
and compute the per-singe-cell coverage to get an estimate of what your data may look like. 

One of the best applications of MAESTER resolved the 
[malignant evolution in Barrett’s esophagus](https://pmc.ncbi.nlm.nih.gov/articles/PMC9900873/)
(from [Syd Shaffer's Lab](https://www.sydshafferlab.com/)) providing a unified view of the cell
states and dynamics along a disease trajectory.


{% include section.html background="images/scistories-clear-cut.png" dark=false %}

{% include section.html %}

# Pathogenic mitochondrial mutations

## Purifying selection in congenital mitochondrial disease

{% include figure.html name="MAESTER" image="images/researchpngs/pearson-wide.png" %}



{% include section.html background="images/scistories-clear-cut.png" dark=false %}

{% include section.html %}

# Software for analyses

As part of these tools, our lab has been the primary developers of genotyping software for processing sequencing reads 
from the protocols and identifying high-confidence single-cell heteroplasmy. 

- For analyzing mtDNA (from any ATAC data), we currently recommend the [mgatk package](https://github.com/caleblareau/mgatk).
- To call mtDNA deletions, we recommend the [mgatk-del utility](https://github.com/caleblareau/mgatk) part of mgatk.
- For analyzing MAESTER/mRNA data, we recommend the [maegatk workflow](https://github.com/caleblareau/maegatk).

The major differences between the software tools [are described here](https://github.com/caleblareau/maegatk/wiki/FAQ).


