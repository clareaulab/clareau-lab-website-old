---
title: Mitochondrial lineage tracing
---

# {% include icon.html icon="fa-solid fa-dna" %}Methods for mtDNA tracing

Our lab has been active in the development of new technologies to enable
lineage tracing in humans via mitochondrial DNA mutations. All of these works have been 
collaborative efforts with the [Leif Ludwig](https://www.mdc-berlin.de/ludwig) Lab.
See a summary of these major technologies and software below: 


## Mitochondrial single-cell ATAC-seq

The mitochondrial single-cell ATAC-seq (mtscATAC-seq) protocol is an adaptation of 
commercial single-cell ATAC-seq workflows. At a basic level, by fixing and permeabilizing
cells (versus just nuclei), Tn5 also tagments the more accessible mitochondrial genome.
Accessible chromatin profiling can thereby be combined with single-cell whole mitochondrial genome sequencing.

{% include figure.html name="mtscatac" image="images/researchpngs/mtscatac-overview-wide.png" %}


## MAESTER
As >90% of mtDNA is transcribed, full-length RNA-seq techniques (e.g., Smart-seq) that capture
the entire sequence of a transcript are particularly attractive to capture genetic variants.
As relatively few groups use Smart-seq nowadays, 

The more high-throughput and more popular 3′- or 5′-based scRNA-seq approaches sequence 
only part of the transcript and thus tend to suffer from limited coverage of the mitochondrial
transcriptome for confident variant detection.

However, the primer-based tiling of mitochondrial transcripts and a modified computational toolkit
(‘MAESTER’, below) has successfully demonstrated variant determination from cDNA libraries.
One recent application of MAESTER resolved the malignant evolution in Barrett’s esophagus,
providing a unified view of the cell states and dynamics along a disease trajectory.

{% include figure.html name="MAESTER" image="images/researchpngs/maester-overview-wide.png" %}


There are a few noteworthy limitations of genotyping mitochondrial mutations from RNA alone.
First, there is a high degree of inherent transcriptional error of the mitochondrial RNA polymerase,
which may confound variant determination.  Yet, RNA-based methods do have limitations. For example, not all mtDNA molecules may be equally transcribed or captured; for example, the 22 mitochondrial tRNAs are not reverse transcribed by poly(A)-based priming, which is most commonly utilized in scRNA-seq.

{% include section.html background="images/scistories-clear-cut.png" dark=false %}

{% include section.html %}

## Software for analyses

As part of these tools, our lab has been the primary developers of genotyping software for processing sequencing reads 
from the protocols and identifying high-confidence single-cell heteroplasmy. 

- For analyzing mtDNA (from any ATAc data), we currently recommend the [mgatk package](https://github.com/caleblareau/mgatk).
- For analyzing MAESTER data, we recommend the [maegatk workflow](https://github.com/caleblareau/maegatk).

The major differences between the software tools [are described here](https://github.com/caleblareau/maegatk/wiki/FAQ).

