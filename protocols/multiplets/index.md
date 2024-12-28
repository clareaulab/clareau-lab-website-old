---
title: Identifying multiple beads per droplet in ATAC-seq data
---

# {% include icon.html icon="fa-solid fa-droplet" %}What are barcode multiplets?

A common / foundational assumption in single-cell genomics analyses is that a single oligonucleotide barcode
represents the nucleic acid of an individual cell. However, there are scenarios where an individual single cell 
can have its contents barcoded by multiple distinct oligonucleotides, termed barcode multiplets. 
These scenarios include i) a single droplet containing multiple beads or ii) multiple oligonucleotides
present on the same individual bead. Every single-cell assay has barcode multiplets to varying degrees. 


{% include figure.html name="Overview of multiplets" image="images/researchpngs/barcode-multiplets-wide.png" %}


## Barcode multiplets used to develop dscATAC-seq

{% include figure.html name="biorad" image="images/researchpngs/biorad-wide.png" %}

## Accuracy of bap



## Application to 10x Genomics scATAC data

In 

[fully supports processing 10x Genomics data](https://github.com/caleblareau/bap/wiki/10X-scATAC).

{% include figure.html name="biorad" image="images/researchpngs/10x-bm-wide.png" %}

When applying bap to scATAC-seq datasets released from 10x Genomics, instances of 9+ bead barcodes
were annotated by bap of belonging to the same droplet (all barcodes annotated as ‘cells’
having a sequence in the whitelist and read abundances above the knee threshold).
These barcodes were enriched in the same biological cluster, supportive of the idea that
they may be ‘replicates’ of the same cell. Examining the underlying barcode sequence,
a common 7 nucleotide variable region followed by a 9 base constant in these barcodes, 
consistent with the idea that multiple ‘whitelisted’ barcode sequences were installed on an individual bead during synthesis. 

As far as we know, this issue was prevalent in the early ATAC beads that were synthesized 
by 10x but have been since resolved in the ATAC and other kits. Further, 
a software implementation (that gives nearly identical results to bap)
realeased from 10x Genomics was incorporated into CellRanger-ATAC v1.2. 
This functionality similarly analyzes shared transposition events between pairs of barcode
sequences to identify multiplets. Whereas bap merges different bead barcode sequences
into a single cell barcode, the implementation in CellRanger-ATAC simply discards
multiplet barcodes after retaining the one bead barcode with the highest number of fragments. 

In short, as long as you are using v1.2+ of CellRanger-ATAC, you shouldn't have to worry about barcode multiplets 