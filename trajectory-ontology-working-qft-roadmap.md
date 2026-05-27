# QFT interface — gap diagnosis and reading roadmap

## Status

A working roadmap for engaging seriously with quantum field theory and its interpretations. 
The ontology currently invokes QFT loosely; several of its central claims require grounding 
in QFT-specific structure rather than generic quantum mechanics.

This file diagnoses the gap, maps the relevant territory, and proposes a staged approach.
This file is largely the result of LLM synthesis and at this writing (May 2026)
not verified by the human author at all, due to knowledge gaps.
Consequently, care shall be taken (also by the LLMs) when working in this territory.

Current status as of May 2, 2026:  The human author reading Haag (1996).

## Diagnosis of the current gap

The project's initial QFT-facing bibliography — Everett, Griffiths, Gell-Mann & Hartle, Zurek, D'Ariano — 
operates primarily at the level of quantum *mechanics*: wave functions, Hilbert space, measurement, decoherence. 
These are QM interpretations. They are not QFT-specific.

QFT differs from QM in ways that do appear to matter for this ontology:

- The fundamental entities are *fields*, not particles or wave functions of particles.
- There is no fixed particle number; particles are excitations of fields.
- The vacuum is not empty: it has structure, fluctuations, and entanglement across all spatial regions.
- There is no globally preferred decomposition into particles; *particle content is observer- and state-dependent.*
- Locality has a precise algebraic formulation (Haag-Kastler) that differs from the informal notion used in QM.
- In systems with infinitely many degrees of freedom, 
  unitarily inequivalent representations of the canonical commutation relations exist 
  (relevant to Haag's theorem and the Unruh effect).

At this writing (early May 2026), the human author does not understand the last point, yet.

The result is that four of the ontology's strongest claims are currently asserted without adequate physical grounding:

1. **The experiential bubble as a region of effective coupling** 
   — requires QFT's precise notion of locality, not a geometric intuition.
2. **Persisting entanglement beyond the bubble** 
   — sounds speculative; in fact seems to be a structural consequence of the Reeh-Schlieder theorem. To be verified.
3. **The block-universe multiverse claim** 
   — needs to specify which version: Everettian branching, decoherent-histories, or other. 
     These have structurally different shapes at the QFT level.
     It is unclear which of these are compatible with the joint assumptions, if any.
4. **"Compatible with large parts of current physical theory"** 
   — needs to become a claim with visible support rather than a disclaimer.

## The relevant QFT interpretive landscape

There are three broad camps in QFT interpretation, each with different consequences for the ontology.

At this writing (May 2026), the human writer does not understand the differences, yet.

### A. Algebraic QFT (AQFT) / Haag-Kastler

Defines a QFT as a *net of local algebras*: 
to each bounded open spacetime region O one assigns a C\*-algebra A(O) of observables, subject to:

- **Isotony**: O₁ ⊂ O₂ ⟹ A(O₁) ⊂ A(O₂)
- **Einstein causality**: spacelike-separated O₁, O₂ ⟹ [A(O₁), A(O₂)] = 0
- **Covariance**: the Poincaré group acts consistently on the net
- **Spectrum condition**: energy-momentum is in the forward light cone
- **Vacuum**: a unique Poincaré-invariant state

This framework makes locality a structural, algebraic fact rather than an intuition. 
For the ontology, the significance is that the experiential bubble can be mapped directly onto a local subalgebra A(O):
the algebra of observables accessible within a bounded region. 
"Effective coupling" becomes algebraic inclusion; 
"boundary of the bubble" becomes the algebraic boundary of the local net.

The mathematical background required for AQFT — C\*-algebras, von Neumann algebras, states as positive linear functionals, the GNS construction — maps well onto abstract algebra and basic category theory. 
The net of algebras is itself a functor from the poset category of spacetime regions (ordered by inclusion) to the category of C\*-algebras (with inclusion morphisms). This categorical structure is explicit in the literature.

### B. Lagrangian / path-integral QFT

The version actually used by working physicists. 
Defined by a Lagrangian density, renormalisation group methods, perturbation theory. 
This is the QFT of the Standard Model.

The ontological content is harder to extract rigorously.
Haag's theorem shows the interaction picture does not strictly exist.
Hoever, this is the version that best describes the actual physical world. 
Wallace argues, contra Fraser, that this should be the primary target of interpretation.

### C. Everettian QFT (Wallace)

Applies the Everett interpretation to QFT rather than to non-relativistic QM. 
Branching emerges from decoherence in a QFT context; 
quasi-classicality is a feature of the physical field theory, not an approximation added by hand. 
The block-universe multiverse claim of this ontology is closest to this camp.

## Five structural results with direct relevance

At this writing (May 2026), the human writer does not understand these results, yet.

### 1. The Reeh-Schlieder theorem

**What it says**: In any QFT satisfying the Haag-Kastler axioms, the vacuum state (and any state of bounded energy) is cyclic and separating for the local algebra A(O) of any bounded open region O. Cyclicity means local operators in O can approximate any global state arbitrarily well. Separating means no local operator in O annihilates the vacuum.

**Why it matters here**: The vacuum is entangled across every spatial boundary. Entanglement does not respect the bubble boundary; it pervades the entire field. The ontology's claim that "outside the experiential bubble, wider entanglement persists" is not a speculative addition — it is a structural feature of QFT that this theorem makes precise. The bubble does not mark a boundary of entanglement; it marks a boundary of *effective coupling* and quasi-classical stability, which is a different thing.

This converts a speculative hypothesis into a supportable claim.

### 2. AQFT locality and the bubble boundary

The Haag-Kastler isotony and causality axioms give the bubble a rigorous structural meaning. Local quasi-classicality within A(O) — the fact that the experiential system decoheres and stabilises within its coupled region — is compatible with non-factorising entanglement in the wider net. The bubble is better understood as the domain within which the relevant decoherence functional is active, not as a domain of clean separation from the rest.

### 3. The Unruh effect as observer-dependent ontology

A uniformly accelerating observer (Rindler observer) and an inertial observer both look at the same underlying quantum field state — the Minkowski vacuum — but assign it different particle content. For the inertial observer it is the vacuum; for the Rindler observer it appears as a thermal bath at the Unruh temperature T = ℏa / 2πck.

This is not a physical disagreement: both descriptions are consistent accounts of the same field state, expressed in different mode decompositions adapted to different trajectories. It shows concretely that particle content — and by extension quasi-classical object content — is observer- and trajectory-dependent at the QFT level, not absolute.

This is the sharpest available physical illustration of the trajectory ontology's observer-coupled picture. Different trajectories through the same underlying field state yield different quasi-classical contents.

### 4. Haag's theorem and inequivalent representations

In a QFT with infinitely many degrees of freedom, there exist unitarily inequivalent representations of the canonical commutation relations. The free and interacting field theories live in different, mutually inaccessible Hilbert spaces. This is Haag's theorem.

The relevance is primarily epistemological: it shows that the naive picture of a unique quantum state evolving in a fixed Hilbert space — the picture imported from QM — does not hold in QFT. Different physical situations may require genuinely different representational structures. This is background for why AQFT takes the algebraic (representation-independent) approach as primary.

### 5. Quasi-classicality as emergent, not given

In Wallace's Everettian QFT, quasi-classical branches are not put in by hand; they emerge from decoherence applied to the actual quantum field. This is relevant to the ontology's treatment of histories-as-compatibility-classes: quasi-classical histories are not globally fixed branches but emergent structures stabilised by local decoherence. This supports the claim that histories are better treated as large-scale compatibility structures than as fundamentally fixed entities.

## The Fraser–Wallace debate

This debate sets the epistemological landscape and should be understood before committing the ontology to either version of QFT.

**Fraser's position**: Only the rigorous algebraic formulation (AQFT) is a proper candidate for interpretation. The Lagrangian formulation is mathematically inconsistent (Haag's theorem, non-existence of the interaction picture) and should not be interpreted directly.

**Wallace's position**: The Lagrangian formulation, understood via renormalisation group methods and effective field theory, is the actual physical theory. Its apparent inconsistencies are artefacts of taking it beyond its domain of validity. AQFT, while mathematically rigorous, describes an idealisation (no interaction, infinite volume) that may not represent the physical world.

**Consequence for this ontology**: The Reeh-Schlieder theorem and the AQFT locality structure belong to Fraser's camp. The quasi-classicality and branching arguments belong to Wallace's. The ontology uses both. It should be explicit that it is drawing selectively from each, and that the two do not form a single unified framework.

## Stage 1 — minimal integration (immediate)

Targeted revisions to the structural continuity blueprint:

1. Ground the experiential bubble explicitly in the AQFT local subalgebra concept. 
   Replace the informal "region of effective coupling" with a reference to A(O) and the Haag-Kastler locality structure.

2. Ground the persisting-entanglement claim in the Reeh-Schlieder theorem. 
  This converts a speculative hypothesis into a claim with physical backing.

3. Note the Unruh effect as a concrete physical case of observer-dependent quasi-classical content.

Bibliography additions required for Stage 1: Haag (1996), Halvorson & Müger (2006), Summers (2011), Clifton & Halvorson (2001).

## Stage 2 — dedicated QFT interface file

A new file modelled on the structural continuity blueprint, covering:

1. The three-camp landscape (AQFT, Lagrangian, Everettian) and which claims belong to which camp.
2. AQFT locality mapped systematically onto the experiential bubble, history, and trajectory concepts.
3. The Reeh-Schlieder theorem and its implications for entanglement across the bubble boundary.
4. The Unruh effect as observer-dependent ontology — detailed treatment.
5. Wallace's Everettian QFT and the emergence of quasi-classical histories.
6. Where the trajectory ontology requires going beyond anything QFT currently provides (mechanism of lateral movement; the phenomenological layer).

Bibliography additions required for Stage 2: Wallace (2012), Fraser (2009), Wallace (2011), Earman & Fraser (2006).

## Suggested reading order

Priority 1 — read before revising the structural continuity blueprint:

- **Summers (2011)** "Yet More Ado About Nothing" — survey of the relativistic vacuum, Reeh-Schlieder, vacuum entanglement, and modular theory; preprint freely available at arXiv:0802.1854
- **Clifton & Halvorson (2001)** on entanglement and open systems in AQFT

Priority 2 — read before writing the QFT interface file:

- **Halvorson & Müger (2006)** chapter on AQFT (this is the primary secondary source; your abstract algebra and category theory background will be directly useful here)
- **Wallace (2012)** *The Emergent Multiverse*, chapters 2–3 (decoherence) and 8–9 (multiverse structure)

Priority 3 — background and debate:

- **Haag (1996)** *Local Quantum Physics* (primary AQFT source; heavy but precise)
- **Fraser (2009)** and **Wallace (2011)** on the rigorous-vs-Lagrangian debate
- **Earman & Fraser (2006)** on Haag's theorem

## Main open questions after engaging QFT

- Can the experiential bubble be given a fully precise AQFT formulation, or does the phenomenological layer necessarily resist algebraic capture?
- Does the Reeh-Schlieder cyclicity of the vacuum create problems for the quasi-classical separation that the experiential bubble is supposed to support?
- How does the trajectory ontology's lateral movement claim sit relative to Everettian branching? Are they alternatives, or can they be combined?
- Does the observer-dependence of particle content in QFT (Unruh) extend in any structural sense to the observer-dependence of histories claimed by this ontology?
- Is there a category-theoretic formulation of the bubble as a local net restriction that could be made rigorous?
