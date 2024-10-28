---
title: Mitochondrial lineage tracing
---

# {% include icon.html icon="fa-solid fa-dna" %}Methods for mtDNA tracing

Our lab has been active in the development of new technologies to enable
lineage tracing in humans via mitochondrial DNA mutations. All of these works have been 
collaborative efforts with the [Leif Ludwig](https://www.mdc-berlin.de/ludwig) Lab
while we were trainees with Aviv Regev and Vijay Sankaran. 
See a summary of these major technologies, software, and informal guidelines below:


## Interested in mtDNA tracing?

Feel free to [reach out to Caleb](mailto:lareauc@mskcc.org), who can either answer your questions
or refer you to the right person who can help! 


## Mitochondrial single-cell ATAC-seq

The mitochondrial single-cell ATAC-seq (mtscATAC-seq) protocol is an adaptation of 
commercial single-cell ATAC-seq workflows. At a basic level, by fixing and permeabilizing
cells (versus just nuclei), Tn5 also tagments the more accessible mitochondrial genome.
Accessible chromatin profiling can thereby be combined with single-cell whole mitochondrial genome sequencing.

{% include figure.html name="mtscatac" image="images/researchpngs/mtscatac-overview-wide.png" %}

Multiple mtscATAC-seq variant assays have been developed, for example,
[ATAC with select antigen profiling by sequencing (ASAP-seq)](https://www.nature.com/articles/s41587-021-00927-2) (with Eleni Mimitou and Peter Smibert); 
as well as 
[PHAGE-ATAC](https://www.nature.com/articles/s41587-021-01065-5) (with Evgenij Fiskin),
which in addition facilitate surface-marker profiling. In our experience, the 

The 10x Genomics Multiome kit has further facilitated the integration of transcriptional profiles,
yielding [DOGMA-seq](https://www.nature.com/articles/s41587-021-00927-2) (with Eleni Mimitou and Peter Smibert); 
this enables the single-cell capture of up to four data modalities, including transcriptome,
accessible chromatin, surface markers and mtDNA mutations.

Another extension of the approach (though unrelated to our group) for the genotyping of 
targeted loci with single-cell chromatin accessibility [(GoT-ChA)](https://www.nature.com/articles/s41586-024-07388-y)
utilizes targeted primers 
to genotype nuclear variants in addition to optional mtDNA sequencing for high-resolution clonal analyses.



Unless you have a specific reason to want the transcriptome (then use DOGMA-seq) or 
the surface proteome (then use ASAP-seq), we recommend mtscATAC-seq due to the ease 
and cost-efficiency of the workflow. 

{% include section.html background="images/scistories-clear-cut.png" dark=false %}
{% include section.html %}


## MAESTER
As >90% of mtDNA is transcribed, full-length RNA-seq techniques (e.g., Smart-seq) that capture
the entire sequence of a transcript are particularly attractive to capture genetic variants.
As relatively few groups use Smart-seq nowadays, 

The more high-throughput and more popular 3′- or 5′-based scRNA-seq approaches sequence 
only part of the transcript and thus tend to suffer from limited coverage of the mitochondrial
transcriptome for confident variant detection.

However, the primer-based tiling of mitochondrial transcripts and a modified computational toolkit
[(‘MAESTER’, below)](https://pubmed.ncbi.nlm.nih.gov/35210612/) 
can enrich mitochondrial mutations from existing cDNA libraries. MAESTER was developed with
[Tyler Miller](https://tymillerlab.org/) and [Peter van Galen](https://vangalenlab.bwh.harvard.edu/).


One of the best applications of MAESTER resolved the 
[malignant evolution in Barrett’s esophagus](https://pmc.ncbi.nlm.nih.gov/articles/PMC9900873/)
(from [Syd Shaffer's Lab](https://www.sydshafferlab.com/)) providing a unified view of the cell
states and dynamics along a disease trajectory.

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

{% include section.html background="images/scistories-clear-cut.png" dark=false %}

{% include section.html %}

## Software for analyses

As part of these tools, our lab has been the primary developers of genotyping software for processing sequencing reads 
from the protocols and identifying high-confidence single-cell heteroplasmy. 

- For analyzing mtDNA (from any ATAc data), we currently recommend the [mgatk package](https://github.com/caleblareau/mgatk).
- For analyzing MAESTER data, we recommend the [maegatk workflow](https://github.com/caleblareau/maegatk).

The major differences between the software tools [are described here](https://github.com/caleblareau/maegatk/wiki/FAQ).


