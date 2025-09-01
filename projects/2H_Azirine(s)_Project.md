---
layout: project
type: project
image: img/2H_Azirine.png 
title: "Modeling the Synthesis of Azirine-based Biological Probes Using Density Functional Theory"
date: 01-22-2025
published: true
labels:
  - Quntum Chemistry
  - Computational Chemistry
  - Computation & Modeling of New Chemical Syntheses
summary: "I calculated the relative chemical energies (Gibbs-Free Energy, Enthalpy, Electronic) of multiple new synthetic pathways that create biological probes from 2H-Azirine Reactant to better support experimental resuls obtained by the Seebald Lab."
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

Azirines are highly reactive three-membered nitrogen rings that readily break ring strain to form more stable, lower-energy structures. These properties make Azirines useful in biology, where they can covalently attach to specific amino acids in proteins by making covalent probes out of them. This enables scientists to track protein activity, study molecular interactions, and investigate protein function in cells in order to develop new drugs. In this project, we studied a specific azirine called Az-Me, which serves as a model compound for understanding how azirines enable the synthesis of covalent probes.

To study how and why Az-Me can synthesize covalent probes, we used a quantum computational method called Density Functional Theory (DFT) to gather reactivity data. This allowed us to compare the relative energies of different synthesis pathways and relate them to experimental results from our experimental in lab collaborators the Seebald Group at Haverford College. DFT models electron behavior by using  electron density rather than the many body wave functions. The goal of this project is to analyze how Az-Me reacts with various nucleophiles—such as ethanol, ethanethiol, and acetic acid—to form covalent probes. Based on these results, we aim to identify the most viable reaction mechanism for each nucleophile. This summer, we focused on two ethanol-based reactions and compared their pathways for covalent probe formation.

To understand reactivity and confirm predicted mechanisms, we calculate the vibrational frequency of a modeled molecule. This helps determine whether a structure is a reactant, intermediate, transition state, or product. Molecules without a negative frequency are stable species, while transition states sit at saddle points on the potential energy surface (PES) and are identified by a single negative frequency corresponding to motion between bonding atoms due to them having high potential energy. Finding transition states is challenging and time-consuming due to their sensitivity to initial geometry of Az-Me and the precise bonding distance between Az-Me and the nucleophile all in the same input. To locate them, I used the Nudged Elastic Band (NEB) method, which maps the minimum energy path between reactants and products by optimizing a series of intermediate “images.” This reveals the highest-energy point along the path that represents the transition state. I also used scans, which involve varying the distance between reactive atoms to explore energy changes along the reaction coordinate. These combined techniques allowed me to successfully identify transition states in the system.
Using DFT and calculating the energy differences from the reactants to the products, an entire system can be represented as a reaction coordinate diagram. 

This allows us to identify the rate-determining step and quantitatively compare competing reaction mechanisms.
Our results demonstrate that the proposed reaction mechanisms are not only plausible but energetically accessible. Importantly, the energy barrier for TS1 is not insurmountable, supporting the experimental hypothesis that the desired product can indeed form. For the first transition state, two bonds are broken and formed simultaneously, while in the second, bond changes occur asynchronously. These differences arise from variations in energy barriers and structural geometry changes as the reaction progresses. Additionally, the identification of transition states for certain byproducts helped assess competing pathways, further reinforcing the likelihood of the preferred product being formed. 

Future work will focus on determining the exact distances between Az-Me and other nucleophiles (Ethanethiol and Acetic Acid) to identify additional transition states for these compounds. This will expand the ability to compare the different synthesis pathways and will point to a reaction that is the most efficient in creating the most covalent probes with the lowest amount of energy.

