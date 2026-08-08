---
permalink: /research/
title: "Research"
description: "Quantum geometry and nonlinear response, topological superconductivity and excitons, non-equilibrium spatiotemporal order, and interpretable machine learning for materials discovery."
author_profile: true
redirect_from:
  - /Research/
  - /portfolio/
toc: true
toc_label: "Research areas"
toc_sticky: true
---

<!--
  NOTE: this page no longer uses {% raw %}{% for post in site.research %}{% endraw %}.
  The _research/ collection was deleted in commit 281f9f8, so that loop
  iterated over nothing. These are static sections instead. If you later
  want per-project subpages, recreate the collection and add the loop back
  under whichever section it belongs to.

  Each section below has a placeholder for a figure. Do add them — a
  distinctive figure per section is what makes these pages linkable, and
  image filenames and alt text are themselves indexed.
-->

## Quantum geometry and nonlinear response

The Bloch wavefunctions of a crystal carry geometric structure that the band energies alone do not capture. Berry curvature and the quantum metric — the imaginary and real parts of the same underlying quantum geometric tensor — determine how electrons respond to fields in ways that have no counterpart in a free-electron picture.

Our interest is in the **nonlinear** regime, where this geometry becomes most visible. At second order and beyond, response functions acquire contributions that are pure geometry: shift currents, injection currents, and rectification terms that survive in clean systems and vanish only when symmetry forbids them outright. We have developed the general formalism for nonlinear optical response in materials that break time-reversal symmetry, separating the roles of Berry curvature, quantum metric, and diabatic interband motion — a decomposition that matters because these terms scale differently with frequency, disorder, and temperature, and can therefore be separated experimentally.

Specific directions:

- **Nonlinear Hall response in magnets.** We predicted an anomalous nonlinear Hall effect in a topological antiferromagnet, where the effect is allowed by the magnetic point group even though the linear anomalous Hall response vanishes. Magnetic symmetry analysis is doing real work here — it tells you which of a material's many response tensors can be nonzero before any computation begins.
- **Rectification and optical magnetoelectricity.** Working in the length gauge, we derived the polarization operator to second order in the electric field for magnetoelectric antiferromagnets. In Cr₂O₃, the combination of broken time-reversal and broken inversion with preserved PT symmetry forces the rectified response to be *helicity-odd* — an inverse optical magnetoelectric effect, with a sign that flips with the circular polarization of the drive.
- **Response beyond the clean-limit intuition.** It is commonly assumed that in-gap transitions into extended states are smoothly suppressed as disorder goes to zero. We have shown by counterexample that this intuition fails past linear response.
- **Altermagnetism and magnetic symmetry.** Classifying candidate altermagnets by magnetic space group and identifying which permit spin-split bands without net magnetization, then asking what nonlinear signatures follow.

<!-- ![Quantum geometry](/images/research-geometry.png){: .align-center} -->

## Topology and exotic phenomena

Topology in band structure is by now familiar. What interests us is what happens when topology meets strong interactions — where the single-particle classification stops being the whole story and new ordered states appear that inherit geometric character from the bands they are built from.

**Superconductivity from repulsion.** We predicted superconductivity in twisted transition-metal dichalcogenides arising from repulsive interactions, not phonons. The mechanism runs through finite-momentum instabilities: the charge-charge susceptibility of a moiré band structure can diverge at incommensurate wavevectors, and quantum geometry of the Bloch states controls where. We have applied the same framework to rhombohedral multilayer graphene, where band renormalization, spin-valley-polarized quarter metals, and chiral superconductivity appear in close proximity, and calculated the anomalous Hall conductivity of these states in the presence of both weak-and-dense and sparse-and-strong impurities.

**Topological crystalline phases.** Berry curvature can drive the formation of crystalline electronic states with no classical analogue. We have been working on topological Wigner crystals and skyrmion crystals stabilized by chiral ring exchange, including a 24-sublattice tetra-skyrmion phase reached through a devil's-staircase sequence of commensurate lock-ins. The transport signature is sharp and unusual — an integer Hall conductivity at fractional filling — which makes the prediction falsifiable in a single measurement.

**Excitons in topological matter.** Bound electron-hole pairs inherit the geometry of the bands they are formed from. This changes their dispersion, their optical selection rules, and their response to fields, and it opens the possibility of exciton states that are themselves topologically nontrivial.

**Correlated and heavy-fermion systems.** Multiplet-projected impurity models and DMFT for materials where the interplay of local moments, lattice coupling, and itinerant carriers governs the spectrum — with ARPES lineshapes as the target observable.

<!-- ![Topological phases](/images/research-topology.png){: .align-center} -->

## Out-of-equilibrium order

A material driven by light is not simply a hot material. Under the right conditions, driving can create order that does not exist in equilibrium, and can create *kinds* of order that equilibrium thermodynamics does not permit at all.

**Optical Faraday waves.** Faraday waves — patterns arising from the interplay of nonlinearity and parametric amplification — are familiar in driven fluids. We developed a theory showing that optical pulses can generate the analogous phenomenon in ordered quantum solids, producing spatiotemporal order that persists far longer than the pump that created it. The state is genuinely spatiotemporal: periodic in both space and time, and not reducible to a transiently modified equilibrium phase.

**Light-driven phases stable against temperature.** A recurring objection to photoinduced order is that it should melt as soon as the deposited energy thermalizes. We have identified regimes where the driven state is stable against thermal disordering, which changes what a realistic experiment needs to look for.

**Melting mechanisms in charge density waves.** In ultrafast electron diffraction, the amplitude and the phase of a CDW order parameter can melt independently. We have used this distinction to interpret experiments in which CDW superlattice peaks collapse while the associated lattice distortion survives — a phase-melting signature rather than amplitude melting — and developed the Landau theory relating a primary CDW order parameter to secondary improper strain through cubic lock-in invariants.

**Collective modes.** Phasons, amplitudons, and phase phonons in incommensurate systems, and what optical reflectivity can and cannot distinguish among them.

<!-- ![Non-equilibrium order](/images/research-nonequilibrium.png){: .align-center} -->

## AI-inspired materials science

Machine learning has become good at predicting material properties and bad at explaining them. We are interested in the second half of that problem, because a model that cannot tell you *why* a compound should superconduct cannot tell you where else to look.

Our approach uses kernel methods with tractable structure — in particular the empirical neural tangent kernel — to make the learned representation itself the object of study. Applied to a database of several thousand known superconductors, this yields a similarity geometry over compositions that can be clustered and embedded, revealing chemical families the model has organized itself around. Because the kernel is explicit, we can ask questions that a black-box network cannot answer: how confident is the model at this composition, which training compounds are actually supporting a given prediction, and where is the model extrapolating rather than interpolating.

This has produced concrete predictions of *de novo* superconductors — candidates that are not minor variations on known families. It also produces something more useful in the long run: a map of where the training data is thin, which is exactly where new experiments are worth doing.

We are also interested in transfer learning between related materials properties, and in the more general question of what makes a materials representation good — a question on which physical insight and statistical performance do not always agree.

<!-- ![Machine learning](/images/research-ml.png){: .align-center} -->

---

Full publication list on [Google Scholar](https://scholar.google.com/citations?user=n2RYBTwAAAAJ&hl=en) and [arXiv](https://arxiv.org/a/kaplan_d_3). Code from our projects is on [GitHub](https://github.com/danielkaplan137).
