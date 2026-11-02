{{nyml
kind: document
format: 1
title: Chapter 7 Assessment Guide: The Electronic Structure of Atoms
}}

# Chapter 7 Assessment Guide: The Electronic Structure of Atoms

## Source and Format

**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 7 (CC BY 4.0). **Audience:** introductory undergraduate general chemistry, first semester. **Note:** this is design guidance for building assessments — question *guides* an instructor or generator can instantiate into many concrete questions — not a finished question bank or answer key.

## General Assessment Priorities

- Require unit consistency (meters, not nm, inside $c=\lambda\nu$ and $E=h\nu$) as an explicit checked step — unit slips are the most common error source in this chapter's calculations.
- Test quantum-number validity checks (Objective 7.3a) with at least one item testing each individual rule ($l<n$; $|m_l|\le l$; $m_s=\pm\frac12$ only) rather than one generic "spot the error" item.
- Require electron-configuration answers to show noble-gas-core notation once introduced, not full expansion, to build the habit used in later chapters.
- Pair every quantum-mechanical topic (uncertainty principle, electron density) with a concrete contrast to the Bohr model's definite orbits, so students see what specifically changed.

## Objective 7.1a: Relate wave speed, wavelength, and frequency

### Target understanding

A student can apply $u=\lambda\nu$ (or $c=\lambda\nu$ for light) to find any one quantity given the other two, with correct unit consistency.

### Question guides

**1. Forward — find frequency from wavelength**
- Variables & ranges: any visible or near-visible wavelength.
- Constraint: convert nm to m before substituting.
- Contexts: any electromagnetic wave.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (400 nm → frequency).

**2. Inverse — find wavelength from frequency**
- Variables & ranges: any frequency value.
- Constraint: correct algebraic rearrangement.
- Contexts: any electromagnetic wave.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($5.75\times10^{14}$ Hz → wavelength).

**3. Conceptual — why all EM waves share one speed constant**
- Variables & ranges: qualitative, contrasting radio waves and gamma rays.
- Constraint: must state that $c$ is the same for all EM radiation regardless of wavelength/frequency.
- Contexts: any two very different EM wave types.
- Formats: short-answer.
- Worked instantiation: "A radio wave and a gamma ray have vastly different wavelengths. Do they travel at different speeds in a vacuum?" → No — all electromagnetic radiation travels at the same speed $c$ in a vacuum; only wavelength and frequency differ (inversely) between them.

**4. Error analysis**
- Variables & ranges: a student substitutes a wavelength in nm directly into $c=\lambda\nu$ without converting to meters.
- Constraint: correction must show the unit-conversion step.
- Contexts: any wavelength given in nm.
- Formats: short-answer.
- Worked instantiation: "A student computes $\nu=c/\lambda$ using $\lambda=400$ (nm) directly, without converting to meters. What's wrong?" → $c$ is in m/s, so $\lambda$ must be in meters ($400\times10^{-9}$ m), not left in nm — otherwise the calculated frequency is off by a factor of $10^9$.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 wavelength/frequency conversion problems. |
| Group discussion | Understand | Discuss why radio, microwave, and visible light are all fundamentally the "same thing." |
| Quiz | Apply | One wavelength-frequency conversion. |
| Exam | Apply | Combine with Objective 7.1b (the same wavelength value feeds a photon-energy calculation). |
| Project/activity | Understand | Students identify the EM band for 5 real technologies (Wi-Fi, medical X-ray, remote control, etc.). |

## Objective 7.1b: Calculate photon energy

### Target understanding

A student can calculate a photon's energy from its wavelength or frequency using $E=h\nu=hc/\lambda$.

### Question guides

**1. Forward — energy from wavelength**
- Variables & ranges: any wavelength.
- Constraint: unit consistency (meters).
- Contexts: any photon.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (500 nm → $3.98\times10^{-19}$ J).

**2. Inverse — wavelength from a given energy**
- Variables & ranges: any photon energy value.
- Constraint: correct algebraic rearrangement.
- Contexts: any photon.
- Formats: workout.
- Worked instantiation: "What wavelength corresponds to a photon energy of $4.42\times10^{-19}$ J?" → $\lambda=hc/E=(6.63\times10^{-34})(3.00\times10^8)/(4.42\times10^{-19})=450$ nm.

**3. Conceptual — why higher frequency means higher energy**
- Variables & ranges: qualitative, contrasting a gamma ray photon and a radio wave photon.
- Constraint: must reference the direct proportionality $E=h\nu$.
- Contexts: comparing two EM bands.
- Formats: short-answer.
- Worked instantiation: "Why is a single X-ray photon far more energetic than a single radio-wave photon?" → Energy is directly proportional to frequency ($E=h\nu$); X-rays have far higher frequency than radio waves, so each X-ray photon carries proportionally more energy.

**4. Error analysis**
- Variables & ranges: a student uses $E=h\nu$ but supplies a wavelength value instead of a frequency.
- Constraint: correction must show the missing $\nu=c/\lambda$ conversion, or the direct use of $E=hc/\lambda$.
- Contexts: any wavelength-given photon-energy problem.
- Formats: short-answer.
- Worked instantiation: "A student computes $E=h\lambda$ (using wavelength directly in place of frequency). What's wrong?" → $E=h\nu$ requires *frequency*, not wavelength; either first convert $\lambda$ to $\nu=c/\lambda$, or use the combined form $E=hc/\lambda$ directly.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 photon-energy problems, both directions. |
| Group discussion | Understand | Discuss why UV light (but not visible light) can cause sunburn/skin damage. |
| Quiz | Apply | One photon-energy calculation. |
| Exam | Apply | Combine with Objective 7.2a (photon energy feeds directly into Bohr-transition calculations). |
| Project/activity | Understand | Students rank 4 EM bands by photon energy and connect to real biological/technological effects. |

## Objective 7.1c: Apply the photoelectric effect equation

### Target understanding

A student can apply $E=h\nu=KE+W$ to relate a photon's energy, a metal's work function, and an ejected electron's kinetic energy.

### Question guides

**1. Forward — find kinetic energy of ejected electron**
- Variables & ranges: given photon frequency and a metal's work function.
- Constraint: correct subtraction, and recognition that $KE\ge0$ requires $h\nu\ge W$.
- Contexts: any metal with a known work function.
- Formats: workout.
- Worked instantiation: "A metal has work function $3.5\times10^{-19}$ J. Find the kinetic energy of an electron ejected by a photon of frequency $8.0\times10^{14}$ Hz." → $E=h\nu=(6.63\times10^{-34})(8.0\times10^{14})=5.30\times10^{-19}$ J; $KE=E-W=5.30\times10^{-19}-3.5\times10^{-19}=1.8\times10^{-19}$ J.

**2. Inverse — find the threshold frequency**
- Variables & ranges: a given work function.
- Constraint: recognize the threshold frequency is where $KE=0$.
- Contexts: any metal.
- Formats: workout.
- Worked instantiation: "A metal's work function is $3.5\times10^{-19}$ J. What is its threshold frequency?" → $\nu_\text{threshold}=W/h=3.5\times10^{-19}/6.63\times10^{-34}=5.3\times10^{14}$ Hz.

**3. Conceptual — why no electrons are ejected below the threshold frequency**
- Variables & ranges: qualitative.
- Constraint: must reference the particle (photon) nature of light — one photon interacts with one electron.
- Contexts: light below a metal's threshold frequency, at any intensity.
- Formats: short-answer.
- Worked instantiation: "Why doesn't shining a very bright (but low-frequency) light on a metal eject any electrons, no matter how intense?" → Each photon carries a fixed energy $h\nu$ determined only by frequency; if that energy is less than the work function, no single photon can eject an electron, regardless of how many photons (how bright the light) arrive.

**4. Error analysis**
- Variables & ranges: a student assumes increasing light intensity (not frequency) increases ejected electrons' kinetic energy.
- Constraint: correction must distinguish frequency's role (KE) from intensity's role (number of electrons ejected, given sufficient frequency).
- Contexts: any photoelectric-effect scenario.
- Formats: short-answer.
- Worked instantiation: "A student says a brighter light (same frequency) will eject faster electrons. What's wrong?" → Kinetic energy of ejected electrons depends only on photon energy (frequency) via $KE=h\nu-W$; increasing intensity at the same frequency increases the *number* of ejected electrons, not their individual kinetic energy.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 photoelectric-effect problems. |
| Group discussion | Analyze | Discuss why the photoelectric effect was historically important evidence for light's particle nature. |
| Quiz | Apply | One photoelectric-effect calculation. |
| Exam | Analyze | Combine with Objective 7.1b (photon energy calculation as the first step). |
| Project/activity | Understand | Students research the work functions of 3 common metals and predict which would eject electrons under a given light source. |

## Objective 7.2a: Apply Bohr's theory to hydrogen's energy levels and emission spectrum

### Target understanding

A student can calculate the energy and wavelength of a photon emitted or absorbed during an electron transition between two principal energy levels in hydrogen.

### Question guides

**1. Forward — emission transition**
- Variables & ranges: $n_i>n_f$ (emission).
- Constraint: correctly identify the negative $\Delta E$ as emission, then use its magnitude for wavelength.
- Contexts: hydrogen atom.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($n_i=5\to n_f=2$, 434 nm).

**2. Inverse — absorption transition**
- Variables & ranges: $n_i<n_f$ (absorption).
- Constraint: correctly identify the positive $\Delta E$ as absorption.
- Contexts: hydrogen atom.
- Formats: workout.
- Worked instantiation: "Find the wavelength of light absorbed when a hydrogen electron moves from $n=2$ to $n=4$." → $\Delta E=R_H(1/4-1/16)=2.18\times10^{-18}\times0.1875=4.09\times10^{-19}$ J (positive, absorption); $\lambda=ch/\Delta E=486$ nm.

**3. Conceptual — why emission spectra are line spectra, not continuous**
- Variables & ranges: qualitative.
- Constraint: must reference the quantized (discrete) nature of allowed energy levels.
- Contexts: hydrogen's emission spectrum.
- Formats: short-answer.
- Worked instantiation: "Why does hydrogen's emission spectrum consist of discrete lines rather than a continuous rainbow of colors?" → Only specific, quantized energy differences between allowed levels are possible, so only specific photon energies (and therefore specific wavelengths) can be emitted — producing distinct lines rather than a continuum.

**4. Error analysis**
- Variables & ranges: a student interprets a positive $\Delta E$ as emission.
- Constraint: correction must restate the sign convention.
- Contexts: any Bohr-transition calculation.
- Formats: short-answer.
- Worked instantiation: "A student computes a positive $\Delta E$ for a transition and calls it an emission. What's wrong?" → A positive $\Delta E$ (when $n_i<n_f$) means the atom absorbed energy to move to a higher level; only a negative $\Delta E$ ($n_i>n_f$) corresponds to emission.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 Bohr-transition problems, including at least one absorption case. |
| Group discussion | Understand | Discuss how emission-spectrum "fingerprints" are used in astronomy to identify elements in stars. |
| Quiz | Apply | One Bohr-transition calculation. |
| Exam | Analyze | Combine with Objective 7.1b (the transition energy calculation is itself a photon-energy problem). |
| Project/activity | Evaluate | Students identify which hydrogen spectral series (Lyman, Balmer, Paschen) a given transition belongs to. |

## Objective 7.2b: Calculate an electron's de Broglie wavelength

### Target understanding

A student can apply $\lambda=h/(mu)$ to calculate the wavelength of a moving particle, and can explain the standing-wave condition $2\pi r=n\lambda$.

### Question guides

**1. Forward — calculate de Broglie wavelength**
- Variables & ranges: any particle mass and speed.
- Constraint: consistent SI units (kg, m/s).
- Contexts: an electron or another small particle.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (electron at 68 m/s).

**2. Inverse — find speed from a given wavelength**
- Variables & ranges: a given de Broglie wavelength and particle mass.
- Constraint: correct algebraic rearrangement.
- Contexts: any particle.
- Formats: workout.
- Worked instantiation: "An electron has a de Broglie wavelength of $2.0\times10^{-10}$ m. What is its speed?" → $u=h/(m\lambda)=6.63\times10^{-34}/[(9.11\times10^{-31})(2.0\times10^{-10})]=3.6\times10^6$ m/s.

**3. Conceptual — why macroscopic objects don't show observable wave behavior**
- Variables & ranges: qualitative, contrasting an electron with a thrown baseball.
- Constraint: must reference the inverse relationship between mass and wavelength.
- Contexts: any macroscopic object.
- Formats: short-answer.
- Worked instantiation: "Why don't we observe wave-like diffraction when we throw a baseball, even though de Broglie's equation technically applies to it?" → A baseball's mass is enormously larger than an electron's, making its de Broglie wavelength astronomically small (far smaller than any physically relevant length scale) — too small to produce any observable wave effects.

**4. Error analysis**
- Variables & ranges: a student uses mass in grams instead of kilograms.
- Constraint: correction must show the required unit conversion.
- Contexts: any de Broglie wavelength calculation.
- Formats: short-answer.
- Worked instantiation: "A student uses the electron's mass as $9.11\times10^{-28}$ g directly (without converting to kg) in $\lambda=h/(mu)$. What's wrong?" → Planck's constant $h$ is in J·s, which requires SI units throughout — mass must be in kg ($9.11\times10^{-31}$ kg), not grams.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 de Broglie wavelength problems. |
| Group discussion | Understand | Discuss why electron microscopes can achieve much higher resolution than light microscopes. |
| Quiz | Apply | One de Broglie wavelength calculation. |
| Exam | Analyze | Combine with Objective 7.2a (both connect wave behavior to atomic-scale phenomena). |
| Project/activity | Understand | Students calculate the de Broglie wavelength of a macroscopic object (a thrown ball) and compare it to an electron's. |

## Objective 7.3a: Identify valid quantum-number sets and orbital shapes/energies

### Target understanding

A student can determine whether a given set of four quantum numbers is valid, and can relate quantum numbers to orbital shape (s, p, d, f) and relative energy ordering.

### Question guides

**1. Forward — validate a quantum-number set**
- Variables & ranges: 4–5 sets of quantum numbers, at least one violating a rule ($l\ge n$, $|m_l|>l$, invalid $m_s$).
- Constraint: student must identify *which* rule is violated, not just that one is invalid.
- Contexts: any quantum-number set.
- Formats: multiple-choice.
- Worked instantiation: see the practice sheet (identifying the invalid quantum-number set among five).

**2. Inverse — name the orbital type from l**
- Variables & ranges: any value of $l$ from 0 to 3.
- Constraint: correct s/p/d/f labeling.
- Contexts: any orbital.
- Formats: short-answer.
- Worked instantiation: "What type of orbital has $l=3$?" → an $f$ orbital.

**3. Conceptual — why energy depends only on n for hydrogen but not for many-electron atoms**
- Variables & ranges: qualitative, contrasting hydrogen with a multi-electron atom.
- Constraint: must reference electron-electron repulsion/shielding as the source of the difference.
- Contexts: the $4s$ vs. $3d$ filling order.
- Formats: short-answer.
- Worked instantiation: "Why does a many-electron atom's $4s$ orbital fill before its $3d$ orbital, when hydrogen's orbitals are ordered purely by $n$?" → In hydrogen (one electron, no electron-electron repulsion), energy depends only on $n$; in many-electron atoms, electron-electron repulsion and shielding effects change the relative energies of subshells, so $4s$ ends up lower in energy than $3d$ despite $4>3$.

**4. Error analysis**
- Variables & ranges: a student proposes $l=2$ for $n=2$.
- Constraint: correction must state the $l\le n-1$ constraint.
- Contexts: any invalid $(n,l)$ pairing.
- Formats: short-answer.
- Worked instantiation: "A student proposes the quantum numbers $n=2, l=2$. What's wrong?" → For a given $n$, $l$ can only range from 0 to $n-1$; for $n=2$, the maximum allowed $l$ is 1, so $l=2$ is invalid.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | 4–6 quantum-number validation and orbital-naming items. |
| Group discussion | Understand | Discuss why the maximum number of orbitals in a subshell is $2l+1$. |
| Quiz | Understand | One quantum-number validation item. |
| Exam | Analyze | Combine with Objective 7.3b (valid quantum numbers feed directly into writing an electron configuration). |
| Project/activity | Understand | Students build a table of all valid $(n,l,m_l)$ combinations for $n=1$ through $n=3$. |

## Objective 7.3b: Write ground-state electron configurations

### Target understanding

A student can write a correct ground-state electron configuration for a given element, applying the Aufbau principle, Hund's rule, and the Pauli exclusion principle, and can determine whether an atom is paramagnetic or diamagnetic.

### Question guides

**1. Forward — write a full electron configuration**
- Variables & ranges: any main-group element through the third period (or a straightforward fourth-period element).
- Constraint: correct subshell filling order.
- Contexts: any element.
- Formats: workout.
- Worked instantiation: see the study guide's examples (H through Ne).

**2. Inverse — determine paramagnetic/diamagnetic status**
- Variables & ranges: a given electron configuration.
- Constraint: student must identify unpaired electrons specifically (e.g., via an orbital diagram), not guess.
- Contexts: any element's ground-state configuration.
- Formats: short-answer.
- Worked instantiation: "Is a ground-state nitrogen atom paramagnetic or diamagnetic?" → Paramagnetic — nitrogen's $2p^3$ configuration has three unpaired electrons (one in each $2p$ orbital, per Hund's rule).

**3. Conceptual — why Hund's rule maximizes stability**
- Variables & ranges: qualitative.
- Constraint: must reference reduced electron-electron repulsion from occupying separate orbitals.
- Contexts: the $2p^2$ (carbon) or $2p^3$ (nitrogen) configuration.
- Formats: short-answer.
- Worked instantiation: "Why is it more stable for carbon's two $2p$ electrons to occupy separate $2p$ orbitals (with parallel spins) rather than pairing in the same orbital?" → Electrons in separate orbitals experience less electron-electron repulsion (they're farther apart on average) than two electrons forced into the same, more confined orbital — the parallel-spin, separate-orbital arrangement is lower in energy.

**4. Error analysis**
- Variables & ranges: a student pairs electrons in one $2p$ orbital before filling all three singly.
- Constraint: correction must restate Hund's rule.
- Contexts: any $p$-block element with 2 or 3 $p$ electrons.
- Formats: short-answer.
- Worked instantiation: "A student writes carbon's $2p$ orbital diagram with both electrons paired in the first $2p$ orbital. What's wrong?" → Hund's rule requires electrons to occupy separate degenerate orbitals singly (with parallel spin) before any pairing occurs; carbon's two $2p$ electrons should be in two different $2p$ orbitals, each unpaired.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 4–6 electron-configuration problems across different blocks. |
| Group discussion | Analyze | Debate why paramagnetism/diamagnetism is a directly testable physical prediction of electron configuration. |
| Quiz | Apply | One electron-configuration problem. |
| Exam | Analyze | Combine with Objective 7.3a (valid quantum numbers underlie the configuration). |
| Project/activity | Apply | Students write electron configurations and orbital diagrams for all elements in one full period. |

## Objective 7.3c: Use noble-gas-core notation and recognize transition-metal exceptions

### Target understanding

A student can abbreviate an electron configuration using noble-gas-core notation, and can identify the chromium/copper-type exceptions where a half-filled or fully-filled $d$ subshell is favored.

### Question guides

**1. Forward — write noble-gas-core notation**
- Variables & ranges: any element beyond neon.
- Constraint: correct identification of the preceding noble gas.
- Contexts: any element in periods 3+.
- Formats: workout.
- Worked instantiation: see the study guide's example (potassium, $[\ce{Ar}]4s^1$).

**2. Inverse — identify the exception elements**
- Variables & ranges: a first-row transition metal.
- Constraint: student must recognize which two specific elements (Cr, Cu) are exceptions in this row.
- Contexts: the first transition-metal series.
- Formats: short-answer.
- Worked instantiation: "Which two elements in the first transition-metal series (Sc–Zn) don't follow the 'expected' Aufbau filling pattern?" → Chromium and copper.

**3. Conceptual — why half-filled and fully-filled subshells are extra stable**
- Variables & ranges: qualitative.
- Constraint: must reference the specific electron-exchange/symmetry stabilization argument (at the level expected in this course: extra stability of half-filled/filled subshells, without requiring a full quantum-mechanical exchange-energy derivation).
- Contexts: chromium or copper.
- Formats: short-answer.
- Worked instantiation: see the study guide's explanation (a slightly greater stability is associated with half-filled $3d^5$ and completely filled $3d^{10}$ subshells).

**4. Error analysis**
- Variables & ranges: a student writes chromium's configuration by strictly following the "expected" Aufbau order without checking for the exception.
- Constraint: correction must give the actual configuration and name the reason.
- Contexts: chromium specifically.
- Formats: short-answer.
- Worked instantiation: "A student writes chromium's configuration as $[\ce{Ar}]4s^23d^4$. What's the actual configuration, and why?" → The actual ground-state configuration is $[\ce{Ar}]4s^13d^5$ — one electron moves from $4s$ to $3d$ to achieve the extra stability of a half-filled $3d^5$ subshell.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 noble-gas-core notation problems, including Cr and Cu specifically. |
| Group discussion | Understand | Discuss whether students can predict other possible half-filled/filled-subshell exceptions further down the periodic table. |
| Quiz | Apply | One noble-gas-core notation problem. |
| Exam | Analyze | Combine with Objective 7.3b (write the full configuration, then abbreviate it). |
| Project/activity | Understand | Students research whether any actinide or lanthanide elements show similar half-filled/filled-subshell exceptions. |

## Rubric Themes for Chapter 7

- **Unit consistency is checked explicitly.** Any calculation mixing nm and m (or g and kg) without an explicit conversion step is treated as incomplete, even if the final numeric answer happens to be close.
- **Sign of ΔE must be interpreted correctly** in every Bohr-transition problem — a correct magnitude with the wrong emission/absorption interpretation is not full credit.
- **Electron configurations use noble-gas-core notation once available**, and correctly flag the Cr/Cu-type exceptions rather than defaulting to the "expected" pattern.
- **Quantum-number validity checks must name the specific violated rule**, not just say "this one is wrong."
