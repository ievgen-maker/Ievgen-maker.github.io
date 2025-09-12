---
layout: project
type: project
image: img/2H_Azirine.png 
title: "Modeling The Synthesis of Azirine-based Biological Probes Using Density Functional Theory"
date: 2025-01-25
published: true
labels:
  - Quantum Chemistry
  - Computational Chemistry
  - Computation & Modeling of New Chemical Syntheses
summary: "I calculated the relative chemical energies (Gibbs-Free Energy, Enthalpy, Electronic) of multiple new synthetic pathways that create biological probes from 2H-Azirine Reactant to better support experimental resuls obtained by the Seebald Lab."
---

<img src="../img/Orca.png" width="200" height="200" style="object-fit:cover;float:left;margin-right:1rem;">




This project explored the reactivity of azirines, a class of three-membered nitrogen rings that are highly strained and therefore highly reactive. Their ability to relieve ring strain by forming more stable structures makes them attractive candidates for covalent probes—molecules that can bind to proteins and help track their activity, study interactions, and guide drug development. In particular, we studied a model compound called Az-Me to understand how it reacts with common nucleophiles such as ethanol, ethanethiol, and acetic acid. By applying Density Functional Theory (DFT), we sought to compare the relative energies of different reaction pathways and identify which mechanisms were most plausible, in support of experimental work being carried out by our collaborators in the Seebald Group at Haverford College.

My role was to lead the computational modeling and analysis. I was responsible for setting up DFT calculations, analyzing the potential energy surface, and identifying transition states for the key bond-forming and bond-breaking steps. This involved applying specialized techniques such as vibrational frequency analysis to confirm whether structures were stable intermediates or true transition states, and using the Nudged Elastic Band (NEB) method to trace the minimum energy path between reactants and products. I also ran energy scans by systematically varying distances between reactive atoms to visualize energy changes along the reaction coordinate. I independently located and verified multiple transition states, compared asynchronous and concerted bond-forming pathways, and related these computational results to the experimental data.

From this experience, I gained a much deeper understanding of both computational chemistry methods and their connection to real-world chemical biology. I learned how to interpret negative vibrational frequencies to validate transition states, how to troubleshoot the sensitivity of NEB pathways to starting geometries, and how to construct reaction coordinate diagrams that quantify competing mechanisms. More broadly, I developed the ability to connect computational predictions with experimental observations—using energy barriers and structural changes to explain why certain products are favored. This project taught me how to integrate quantum chemistry, mechanistic reasoning, and biological relevance, and it showed me the value of computational chemistry as a tool for guiding experimental design and validating hypotheses in chemical biology.

<!-- Bottom GIF (click to open full size) -->
<div class="text-center my-5">
  <a href="/img/Orca_Frequency.gif" target="_blank" rel="noopener">
    <img src="/img/Orca_Frequency.gif"
         alt="ORCA vibrational frequency animation (Az-Me) of a transiotion state"
         style="max-width: 100%; width: 720px; height: auto; border-radius: 12px;">
  </a>
  <p class="mt-2"><em>ORCA vibrational frequency animation (Az-Me) of a transition state.</em></p>
  <p class="small">Direct link: <a href="/img/Orca_Frequency.gif">/img/Orca_Frequency.gif</a></p>
</div>


