---
layout: project
type: project
image: img/parrotFish.png 
title: "Modeling The Hybridization of Pacific Parrot Fish Through Comprassion of Several Phylogetic Softwares"
date: 2025-01-25
published: true
labels:
  - Population Genomics
  - Computational Statistical Genomics
  - Genomics Software Testing
summary: "I performed an Indepenedent Research study with the Carlon Lab at Bowdoin college to better understand population structure of parrot fish populations. This was accomplished through testing previosly established computational programs in comparasion to open sourced programs to not onlty derive the phylogeny of parrot fish but also to test efficiency and accurancy of softwares used."
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

I performed an Independent Research study with the Carlon Lab at Bowdoin College to better understand the population structure of parrotfish across the Pacific. To do this, I worked with a dataset of 81 parrotfish samples in the form of VCF (variant call format) files, which record genetic variation across individuals. From these data, I applied multiple computational methods designed for phylogenetic inference and species tree construction, including PAUP+ with the SVDquartets algorithm, CASTER, and ASTRAL. Each program brings different assumptions and computational strategies for analyzing genomic data, making them well-suited for comparative evaluation. My project aimed not only to reconstruct the phylogeny of these parrotfish populations but also to test how software choice may affect both accuracy and efficiency in drawing biological conclusions.

The core of the study involved comparing previously established, widely cited programs such as PAUP+ with SVDquartets—which partitions sequence data into quartets and infers relationships based on singular value decomposition—with newer or more open-source pipelines like CASTER and ASTRAL. ASTRAL, for example, is commonly used in phylogenomics to infer species trees from sets of gene trees, while CASTER provides an alternative framework that emphasizes computational speed and accessibility. By applying these methods directly to my dataset, I was able to assess how well each program handled large-scale genomic data, the ease of use for researchers without deep computational backgrounds, and the congruence of their inferred trees. These comparisons helped highlight trade-offs between accuracy, runtime, and usability that are central to population genomics research.

Through this study, I gained hands-on experience with both the biological and computational aspects of phylogenetic analysis. On the biological side, I explored questions of population structure and divergence in Pacific parrotfishes, a group with important ecological roles in coral reef systems. On the computational side, I developed a framework for testing and validating software performance across large genomic datasets. By systematically comparing tools like PAUP+, CASTER, and ASTRAL, I demonstrated that open-source and emerging methods can provide competitive alternatives to traditional approaches, while also identifying scenarios where one program may outperform another. Ultimately, this research not only advanced our understanding of parrotfish phylogeny but also provided insight into the best practices for integrating computational tools in evolutionary biology.

