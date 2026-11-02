{{nyml
kind: document
format: 1
title: Chapter 10 Assessment Guide: Molecular Geometry and Bonding Theories
}}

# Chapter 10 Assessment Guide: Molecular Geometry and Bonding Theories

## Source and Format

**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 10 (CC BY 4.0). **Audience:** introductory undergraduate general chemistry, first semester. **Note:** this is design guidance for building assessments — question *guides* an instructor or generator can instantiate into many concrete questions — not a finished question bank or answer key.

## General Assessment Priorities

- Require a correct Lewis structure (or at least a correct electron-domain count) as an explicit first step in every VSEPR question — geometry predictions built on a wrong domain count are wrong regardless of the final shape name.
- Test polarity questions with the "two-part test" (polar bonds AND non-cancelling geometry) made explicit, not just a memorized polar/nonpolar fact about a specific named molecule.
- Pair every hybridization question with the underlying domain-counting logic (same electron-domain count that determines VSEPR shape also determines hybridization) rather than treating hybridization as a separate memorized fact per molecule.
- Require the sigma/pi bond count to be justified from the specific bond type (single/double/triple), not just stated as a final number.

## Objective 10.1a: Predict molecular geometry for a central atom with no lone pairs

### Target understanding

A student can determine the number of bonding electron domains around a central atom (with no lone pairs) and name the resulting VSEPR geometry.

### Question guides

**1. Forward — name the geometry from a formula**
- Variables & ranges: an $\ce{AB_n}$ molecule ($n=2$ to 6) with no lone pairs on A.
- Constraint: correct domain count, including treating a double/triple bond as one domain.
- Contexts: any of the five basic shapes.
- Formats: workout.
- Worked instantiation: see the practice sheet ($\ce{CBr4}$: tetrahedral).

**2. Inverse — name a molecule given a geometry**
- Variables & ranges: one of the five basic geometries.
- Constraint: example must have zero lone pairs on the central atom.
- Contexts: any of the five shapes.
- Formats: short-answer.
- Worked instantiation: "Name a molecule with trigonal bipyramidal geometry." → $\ce{PF5}$ (or any $\ce{AB5}$ molecule with no lone pairs).

**3. Conceptual — why 5 and 6 domains require d-orbital involvement**
- Variables & ranges: qualitative, connecting back to Chapter 9's expanded-octet exceptions.
- Constraint: must reference that only Period 3+ central atoms can have 5 or 6 domains.
- Contexts: $\ce{PF5}$ or $\ce{SF6}$.
- Formats: short-answer.
- Worked instantiation: "Why can't a Period 2 central atom form an AB5 or AB6 molecule?" → Trigonal bipyramidal (5 domains) and octahedral (6 domains) geometries require an expanded octet, which needs accessible $d$ orbitals — only available to Period 3 and beyond central atoms (the same restriction from Chapter 9's octet-rule exceptions).

**4. Error analysis**
- Variables & ranges: a student counts a double bond as two separate domains.
- Constraint: correction must restate VSEPR rule 1.
- Contexts: any molecule with a double or triple bond.
- Formats: short-answer.
- Worked instantiation: "A student analyzing $\ce{CO2}$ counts 4 electron domains around carbon (treating each C=O double bond as 2 domains). What's wrong?" → VSEPR rule 1 treats a double (or triple) bond as a single electron domain for geometry purposes; carbon actually has only 2 domains (one to each oxygen), giving linear geometry, not something based on 4 domains.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 4–6 geometry-prediction items across all five no-lone-pair shapes. |
| Group discussion | Understand | Discuss why trigonal bipyramidal is the only common VSEPR shape with two different bond angles (90° and 120°). |
| Quiz | Apply | One geometry-prediction item. |
| Exam | Analyze | Combine with Objective 10.3a (the same domain count also determines hybridization). |
| Project/activity | Apply | Students predict geometries for 5 molecules relevant to a real application (e.g., common industrial gases). |

## Objective 10.1b: Predict molecular geometry for a central atom with lone pairs

### Target understanding

A student can determine the number of bonding and lone-pair electron domains around a central atom and name the resulting molecular geometry (which differs from the electron-domain arrangement when lone pairs are present).

### Question guides

**1. Forward — name the geometry given bonds and lone pairs**
- Variables & ranges: a central atom with a mix of bonding and lone-pair domains.
- Constraint: correct distinction between electron-domain arrangement and named molecular geometry.
- Contexts: $\ce{H2O}$, $\ce{NH3}$, $\ce{SO2}$, or similar.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{SO2}$: bent).

**2. Inverse — determine lone-pair count from a named geometry**
- Variables & ranges: a named molecular geometry and total domain count.
- Constraint: student must subtract bonding domains from total domains.
- Contexts: any lone-pair-containing shape.
- Formats: short-answer.
- Worked instantiation: see the practice sheet ($\ce{SO2}$'s lone-pair count and geometry).

**3. Conceptual — why lone pairs compress bond angles**
- Variables & ranges: qualitative, comparing $\ce{CH4}$ (109.5°) to $\ce{NH3}$ (~107°) to $\ce{H2O}$ (~104.5°).
- Constraint: must reference that lone pairs occupy more angular space than bonding pairs.
- Contexts: the isoelectronic-ish $\ce{CH4}$/$\ce{NH3}$/$\ce{H2O}$ comparison.
- Formats: short-answer.
- Worked instantiation: "Why does the H-N-H bond angle in $\ce{NH3}$ (~107°) differ from the ideal tetrahedral angle (109.5°)?" → A lone pair occupies more angular space than a bonding pair (it's held by only one nucleus, so it spreads out more), pushing the three N-H bonding pairs slightly closer together than the ideal tetrahedral angle.

**4. Error analysis**
- Variables & ranges: a student names a molecule's geometry using the electron-domain arrangement instead of the molecular (atoms-only) shape.
- Constraint: correction must distinguish the two naming conventions.
- Contexts: $\ce{NH3}$ or similar.
- Formats: short-answer.
- Worked instantiation: "A student says $\ce{NH3}$ is tetrahedral, since it has 4 electron domains. What's wrong?" → The *electron-domain arrangement* is tetrahedral, but the named *molecular geometry* only describes the positions of atoms (not lone pairs) — with 3 bonds and 1 lone pair, $\ce{NH3}$'s molecular geometry is trigonal pyramidal, not tetrahedral.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 4–6 geometry-prediction items involving lone pairs. |
| Group discussion | Analyze | Compare bond angles across CH₄/NH₃/H₂O and connect to lone-pair count. |
| Quiz | Apply | One lone-pair geometry-prediction item. |
| Exam | Analyze | Combine with Objective 10.2b (geometry determines whether the molecule is polar). |
| Project/activity | Apply | Students predict and sketch the geometry of 5 lone-pair-containing molecules. |

## Objective 10.2a: Determine polarity of diatomic molecules

### Target understanding

A student can determine whether a diatomic molecule is polar based on whether its two atoms are the same or different elements.

### Question guides

**1. Forward — classify a list of diatomic molecules**
- Variables & ranges: 4–6 diatomic molecules, mixing same-element and different-element pairs.
- Constraint: include at least one of each type.
- Contexts: common diatomic molecules.
- Formats: multiple-choice.
- Worked instantiation: see the practice sheet (identifying the polar molecule among BeCl₂, Br₂, BF₃, IBr, CO₂ — note IBr is the diatomic case here).

**2. Inverse — name a polar and a nonpolar diatomic molecule**
- Variables & ranges: open-ended.
- Constraint: correct classification justification.
- Contexts: any diatomic molecule.
- Formats: short-answer.
- Worked instantiation: "Name one polar and one nonpolar diatomic molecule." → Polar: e.g., HCl (different elements); nonpolar: e.g., N₂ (same element).

**3. Conceptual — why same-element diatomics are always nonpolar**
- Variables & ranges: qualitative.
- Constraint: must reference zero electronegativity difference.
- Contexts: any homonuclear diatomic molecule.
- Formats: short-answer.
- Worked instantiation: "Why is O₂ necessarily nonpolar?" → Both atoms are identical, so their electronegativities are exactly equal — the electronegativity difference is zero, meaning neither atom pulls the shared electrons more than the other.

**4. Error analysis**
- Variables & ranges: a student assumes any diatomic molecule with a "big" atom and a "small" atom must be polar.
- Constraint: correction must clarify that only electronegativity difference (not size) determines diatomic polarity.
- Contexts: a same-element diatomic with very different atomic sizes on the two "sides" being confused (not directly applicable, so reframe as any misconception about size vs. electronegativity).
- Formats: short-answer.
- Worked instantiation: "A student assumes Cl₂ might be slightly polar since chlorine atoms are 'large.' What's the actual determining factor?" → Diatomic polarity depends entirely on electronegativity *difference* between the two atoms, not atomic size; since both atoms in Cl₂ are identical, the electronegativity difference is exactly zero, making it strictly nonpolar regardless of atomic size.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Remember | 4–6 diatomic polarity-classification items. |
| Group discussion | Understand | Discuss why diatomic polarity is the simplest possible case of the general polarity rule. |
| Quiz | Remember | One diatomic classification item. |
| Exam | Apply | Combine with Objective 10.2b (extend the same electronegativity-difference logic to polyatomic molecules). |
| Project/activity | Understand | Students classify 5 real diatomic molecules relevant to atmospheric chemistry. |

## Objective 10.2b: Determine polarity of polyatomic molecules

### Target understanding

A student can determine whether a polyatomic molecule is polar by checking both bond polarity and whether the molecular geometry causes those bond dipoles to cancel.

### Question guides

**1. Forward — determine polarity from geometry and bonds**
- Variables & ranges: a molecule with polar bonds and a given (or derivable) geometry.
- Constraint: both conditions (polar bonds; non-cancelling geometry) must be checked explicitly.
- Contexts: $\ce{CO2}$, $\ce{H2O}$, $\ce{BF3}$, $\ce{NH3}$, or similar.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{BeCl2}$ vs. $\ce{ClNO}$).

**2. Inverse — identify the most polar molecule in a related series**
- Variables & ranges: a series of related molecules (e.g., methyl halides) with varying bond polarity.
- Constraint: student must reason about relative electronegativity differences.
- Contexts: the methyl halide series or similar.
- Formats: multiple-choice.
- Worked instantiation: see the practice sheet (largest dipole moment among CH₃F, CH₃Cl, CH₃Br, CH₃I).

**3. Conceptual — why symmetric molecules with polar bonds can be nonpolar**
- Variables & ranges: qualitative, using $\ce{CO2}$ or $\ce{BF3}$ as the anchor example.
- Constraint: must explain the vector-cancellation idea concretely (not just state the rule).
- Contexts: $\ce{CO2}$ or $\ce{BF3}$.
- Formats: short-answer.
- Worked instantiation: see the study guide's $\ce{CO2}$/$\ce{H2O}$ contrast.

**4. Error analysis**
- Variables & ranges: a student assumes any molecule with polar bonds must be polar overall.
- Constraint: correction must invoke the geometry/cancellation condition.
- Contexts: $\ce{CO2}$ or $\ce{BF3}$.
- Formats: short-answer.
- Worked instantiation: "A student says $\ce{CO2}$ must be polar since C=O bonds are polar. What's missing from this reasoning?" → Having polar bonds is necessary but not sufficient — the molecule's geometry also matters; $\ce{CO2}$'s linear shape places its two identical, oppositely-directed C=O bond dipoles exactly opposite each other, so they cancel and the overall molecule is nonpolar.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 4–6 polyatomic-polarity-determination items. |
| Group discussion | Analyze | Debate a borderline case (a molecule with polar bonds and low, but nonzero, symmetry). |
| Quiz | Apply | One polyatomic-polarity item. |
| Exam | Analyze | Combine with Objective 10.1b (geometry prediction feeds directly into the polarity determination). |
| Project/activity | Evaluate | Students predict and then (via reference data) check the polarity of 5 real molecules. |

## Objective 10.3a: Determine hybridization using valence bond theory

### Target understanding

A student can determine the hybridization (sp, sp², sp³) of a central atom from its electron-domain count, and can explain valence bond theory's potential-energy argument for bond formation.

### Question guides

**1. Forward — determine hybridization from domain count**
- Variables & ranges: a central atom with 2, 3, or 4 electron domains (bonding + lone pair).
- Constraint: correct domain-to-hybridization mapping (2→sp, 3→sp², 4→sp³).
- Contexts: any molecule.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{PCl3}$: $sp^3$).

**2. Inverse — name a molecule with a given hybridization**
- Variables & ranges: sp, sp², or sp³.
- Constraint: example's central atom must actually match the stated hybridization.
- Contexts: any hybridization type.
- Formats: short-answer.
- Worked instantiation: "Name a molecule whose central atom is $sp^2$-hybridized." → e.g., $\ce{BF3}$.

**3. Conceptual — why hybridization and VSEPR domain-counting agree**
- Variables & ranges: qualitative.
- Constraint: must connect that both are describing the same underlying electron-domain geometry.
- Contexts: any molecule analyzed both ways.
- Formats: short-answer.
- Worked instantiation: "Why does a tetrahedral VSEPR shape always correspond to $sp^3$ hybridization?" → Both descriptions come from the same underlying fact — 4 electron domains arranged as far apart as possible — VSEPR names the resulting geometry, while hybridization describes the orbital mixing (one $s$ + three $p$) that produces exactly 4 equivalent directional orbitals matching that same tetrahedral arrangement.

**4. Error analysis**
- Variables & ranges: a student determines hybridization by memorizing specific molecules rather than counting domains.
- Constraint: correction must redirect to the domain-counting method.
- Contexts: an unfamiliar molecule.
- Formats: short-answer.
- Worked instantiation: "A student says they can't determine the hybridization of an unfamiliar molecule like $\ce{OF2}$ since they haven't memorized it. What should they do instead?" → Count electron domains around the central atom (for $\ce{OF2}$: 2 bonds + 2 lone pairs = 4 domains) and apply the general domain-to-hybridization rule ($sp^3$ for 4 domains) — the same method works for any molecule, not just memorized examples.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 4–6 hybridization-determination items. |
| Group discussion | Understand | Discuss valence bond theory's potential-energy curve and why there's a specific minimum-energy bond distance. |
| Quiz | Apply | One hybridization-determination item. |
| Exam | Analyze | Combine with Objective 10.1a/b (the same domain count drives both VSEPR geometry and hybridization). |
| Project/activity | Apply | Students determine hybridization for every central atom in a moderately complex real molecule (e.g., aspirin). |

## Objective 10.3b: Identify sigma and pi bonds and apply the multiple-bond hybridization rule

### Target understanding

A student can count the sigma and pi bonds in a molecule containing single, double, and/or triple bonds, and can apply the rule that one double bond means $sp^2$ while two double bonds or a triple bond means $sp$ (for second-period central atoms).

### Question guides

**1. Forward — count sigma and pi bonds**
- Variables & ranges: a molecule with a mix of single, double, and/or triple bonds.
- Constraint: correct count (every bond has exactly one $\sigma$; a double bond adds one $\pi$, a triple bond adds two $\pi$).
- Contexts: any molecule with multiple bonds.
- Formats: workout.
- Worked instantiation: see the practice sheet (number of $\sigma$ and $\pi$ bonds in a given molecule).

**2. Inverse — determine hybridization from bond type**
- Variables & ranges: a central atom forming one double bond, two double bonds, or a triple bond.
- Constraint: correct application of the multiple-bond rule.
- Contexts: $\ce{CH2=CH2}$, $\ce{CO2}$, $\ce{CH#CH}$.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (each C in $\ce{CH2=CH2}$: $sp^2$).

**3. Conceptual — why a triple bond isn't simply "three sigma bonds"**
- Variables & ranges: qualitative.
- Constraint: must reference that only one bond in any multiple bond can be end-to-end (sigma); the rest must be sideways (pi).
- Contexts: $\ce{N2}$ or $\ce{CH#CH}$.
- Formats: short-answer.
- Worked instantiation: "Why is a triple bond described as 1 σ + 2 π, rather than 3 σ bonds?" → Only one orbital overlap between two atoms can be directly end-to-end (along the bond axis) at a time; the other two bonding interactions in a triple bond must come from sideways ($\pi$) overlap of the remaining unhybridized $p$ orbitals, perpendicular to each other.

**4. Error analysis**
- Variables & ranges: a student assigns $sp^3$ hybridization to a carbon forming a double bond.
- Constraint: correction must restate the multiple-bond rule.
- Contexts: any carbon in a double bond.
- Formats: short-answer.
- Worked instantiation: "A student says a carbon forming one double bond is $sp^3$-hybridized, 'since carbon is usually $sp^3$.' What's wrong?" → A carbon forming one double bond is $sp^2$-hybridized (3 hybrid orbitals for 3 $\sigma$-bonding directions, leaving one unhybridized $p$ orbital for the $\pi$ bond) — $sp^3$ only applies when carbon forms four single bonds with no multiple-bond character.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 sigma/pi-bond-counting and multiple-bond-hybridization problems. |
| Group discussion | Analyze | Work through $\ce{CH2=CH2}$ and $\ce{CH#CH}$ side by side, comparing bond counts and hybridization. |
| Quiz | Apply | One sigma/pi-bond-counting item. |
| Exam | Analyze | Combine with Objective 10.3a (full hybridization analysis of a molecule with mixed bond types). |
| Project/activity | Apply | Students count total σ and π bonds in a real, moderately complex molecule (e.g., aspirin or caffeine). |

## Rubric Themes for Chapter 10

- **Electron-domain counting is the mandatory first step** for VSEPR, polarity, and hybridization questions alike — since all three trace back to the same underlying domain count.
- **Molecular geometry (atoms only) must be distinguished from electron-domain arrangement (including lone pairs)** — using the wrong one is treated as a conceptual error, not a naming slip.
- **Polarity determinations require both conditions checked explicitly**: polar bonds, and a geometry where they don't cancel. Stating only one is incomplete.
- **σ/π bond counts must be justified by bond type**, not just stated as a final number — one bond of any order has exactly one σ, with any additional bond order coming entirely from π bonds.
