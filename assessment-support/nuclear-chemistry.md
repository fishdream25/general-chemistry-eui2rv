{{nyml
kind: document
format: 1
title: Chapter 19 Assessment Guide: Nuclear Chemistry
}}

# Chapter 19 Assessment Guide: Nuclear Chemistry

## Source and Format

**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 19 (CC BY 4.0). **Audience:** introductory undergraduate general chemistry, second semester. **Note:** this is design guidance for building assessments — question *guides* an instructor or generator can instantiate into many concrete questions — not a finished question bank or answer key.

## General Assessment Priorities

- Anchor nuclear-equation balancing to its **two conservation rules only** (mass number, charge) — explicitly contrast this with chemical-equation balancing (which conserves each element's atom count) so students don't try to "balance elements" in a nuclear equation.
- Fix the **mass-defect sign convention** explicitly: mass defect = (mass of separate protons + neutrons + electrons) − (actual atomic mass), and a negative ΔE means energy is released on formation — never let the subtraction order drift.
- Reinforce at every opportunity that radioactive decay kinetics is **not new material** — it is Chapter 13's first-order rate law and half-life formula, applied without modification.
- Keep fission (heavy splits) and fusion (light combines) paired with their standard examples (reactors/bombs vs. the Sun/hydrogen bombs) so students build one fixed association rather than confusing the two.

## Objective 19.1a: Distinguish decay types and balance nuclear equations

### Target understanding

A student can distinguish spontaneous radioactive decay from induced nuclear transmutation, and can balance any nuclear equation by conserving mass number and charge.

### Question guides

**1. Conceptual — decay vs. transmutation**
- Variables & ranges: any nuclear process.
- Constraint: explanation must reference spontaneity (decay) vs. bombardment (transmutation).
- Contexts: any radioactive decay vs. any particle-bombardment reaction.
- Formats: short-answer.
- Worked instantiation: "What distinguishes radioactive decay from nuclear transmutation?" → Radioactive decay is spontaneous — an unstable nucleus decays on its own; nuclear transmutation results from deliberately bombarding a nucleus with neutrons, protons, or other nuclei.

**2. Forward — balance given a bombardment product**
- Variables & ranges: a nuclear reaction with one product unknown.
- Constraint: correct use of mass-number and charge conservation to identify the missing nuclide.
- Contexts: any transmutation or decay reaction.
- Formats: workout.
- Worked instantiation: see the study guide's worked examples ($\ce{^125_53I}$ electron capture; Mg-25 + alpha particle).

**3. Inverse — predict the missing particle from a given equation**
- Variables & ranges: $\ce{^6_3Li + ^1_0n -> ? + ^4_2He}$.
- Constraint: correct mass/charge balance to identify both mass number and atomic number of the unknown.
- Contexts: any transmutation with a named unknown product.
- Formats: workout.
- Worked instantiation: mass: $6+1=A+4 \Rightarrow A=3$; charge: $3+0=Z+2 \Rightarrow Z=1$ → $\ce{^3_1H}$ (tritium).

**4. Error analysis**
- Variables & ranges: a student who tries to conserve "atom identity" (as in a chemical equation) rather than mass number and charge.
- Constraint: correction must state the correct nuclear conservation rules explicitly.
- Contexts: any nuclear equation.
- Formats: short-answer.
- Worked instantiation: "A student insists that since Iodine appears on the left of a nuclear equation, an Iodine-containing species must appear on the right too. What's the error?" → Nuclear equations do not conserve element identity — elements can transmute into different elements. Only total mass number and total charge must be conserved; there is no requirement that the same element reappear on both sides.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 nuclear-equation-balancing problems, mixing decay and transmutation. |
| Group discussion | Understand | Contrast nuclear vs. chemical equation conservation rules side by side. |
| Quiz | Apply | One balancing problem with a missing product. |
| Exam | Analyze | Require identifying whether a given reaction is decay or transmutation before balancing. |
| Project/activity | Evaluate | Research a real historical transmutation experiment (e.g., Rutherford's) and balance its equation. |

## Objective 19.1b: Identify patterns of nuclear stability

### Target understanding

A student can identify the patterns that make a nucleus more or less stable: magic numbers, even-even preference, and the universal instability of nuclides with $Z>83$.

### Question guides

**1. Forward — apply the magic-number rule**
- Variables & ranges: a nuclide with a proton or neutron count at or near a magic number.
- Constraint: correct identification of the magic numbers (2, 8, 20, 50, 82, 126).
- Contexts: $\ce{^208_82Pb}$ (both Z=82 and N=126 are magic) or similar.
- Formats: short-answer.
- Worked instantiation: "Why is $\ce{^208_82Pb}$ described as 'doubly magic'?" → It has 82 protons and 126 neutrons — both are magic numbers, giving it exceptional stability even among already-stable heavy nuclides.

**2. Forward — even-even vs. odd-odd**
- Variables & ranges: two nuclides with the same mass number but different proton/neutron parity.
- Constraint: correct application of the even-even-more-stable rule.
- Contexts: any pair of isobars.
- Formats: short-answer.
- Worked instantiation: which is generally more stable, a nuclide with an even number of both protons and neutrons, or one with odd numbers of both?

**3. Predict-the-effect — Z > 83**
- Variables & ranges: any element with atomic number above 83.
- Constraint: prediction must state that ALL isotopes of such elements are radioactive, without exception.
- Contexts: any heavy element (e.g., bismuth, polonium, uranium).
- Formats: short-answer.
- Worked instantiation: "Is it possible for any isotope of an element with Z=90 to be stable (non-radioactive)?" → No — every isotope of every element with atomic number greater than 83 is radioactive, without exception.

**4. Error analysis**
- Variables & ranges: a student who assumes stability depends only on mass number, not proton/neutron counts specifically.
- Constraint: correction must distinguish mass number from the separate proton and neutron counts.
- Contexts: any stability-pattern discussion.
- Formats: short-answer.
- Worked instantiation: "A student says two nuclides with the same mass number A must have the same stability. What's the error?" → Stability patterns (magic numbers, even-even preference) depend on the *specific* proton count (Z) and neutron count (N) separately, not just their sum (A); two isobars with the same A can have very different stability depending on how that mass number is split between protons and neutrons.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | Classify 3–4 nuclides by stability-pattern criteria. |
| Group discussion | Analyze | Discuss why Tc and Pm have no stable isotopes despite modest atomic numbers. |
| Quiz | Understand | One magic-number or even-even classification item. |
| Exam | Analyze | Require justifying a stability comparison using multiple criteria together. |
| Project/activity | Evaluate | Research the table of stable isotopes and verify the even-even/odd-odd stability pattern statistically. |

## Objective 19.1c: Calculate nuclear binding energy from mass defect

### Target understanding

A student can calculate mass defect and the resulting binding energy in J/nucleus, J/mol, MeV/nucleus, and MeV/nucleon, using the correct sign convention throughout.

### Question guides

**1. Forward — full binding energy calculation**
- Variables & ranges: a nuclide's atomic mass, proton/neutron count given.
- Constraint: correct subtraction order for mass defect; correct unit conversions throughout.
- Contexts: any nuclide with a known atomic mass.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{^56_26Fe}$, all four units).

**2. Forward — a second nuclide**
- Variables & ranges: a different nuclide's atomic mass.
- Constraint: same method, independent numbers.
- Contexts: $\ce{^16_8O}$ (atomic mass 15.9949 amu).
- Formats: workout.
- Worked instantiation: calculate binding energy per nucleon for $\ce{^16_8O}$ and compare to Fe-56's.

**3. Conceptual — sign convention**
- Variables & ranges: any binding-energy calculation.
- Constraint: explanation must state that negative ΔE indicates energy release upon nucleus formation.
- Contexts: any mass-defect calculation.
- Formats: short-answer.
- Worked instantiation: "Why is the calculated ΔE for nuclear binding energy negative?" → Mass defect (Δm) is negative because the assembled nucleus has *less* mass than its separate, unbound protons/neutrons/electrons; via $\Delta E=(\Delta m)c^2$, this translates to a negative ΔE, meaning energy is released when the nucleus forms — consistent with the nucleus being a lower-energy, more stable configuration than its separated parts.

**4. Error analysis**
- Variables & ranges: a student who subtracts atomic mass from separate-particle mass in the wrong order, or forgets to include electron mass.
- Constraint: correction must restate the correct subtraction order and the need to include electrons (since atomic mass includes electrons).
- Contexts: any binding-energy calculation.
- Formats: short-answer.
- Worked instantiation: "A student calculates mass defect as (atomic mass) − (mass of protons + neutrons only, no electrons). What's wrong?" → Two issues: the subtraction order is reversed (should be separate-particle mass minus atomic mass, to get a negative Δm), and electron mass must be included in the separate-particle total, since the given atomic mass already includes the atom's electrons.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2 full binding-energy calculations (all four unit forms) for different nuclides. |
| Group discussion | Analyze | Compare binding energy per nucleon across several nuclides and connect to the binding-energy-curve figure. |
| Quiz | Apply | One binding-energy calculation, at least through MeV/nucleon. |
| Exam | Analyze | Require comparing two nuclides' stability using calculated binding energy per nucleon. |
| Project/activity | Evaluate | Calculate binding energy per nucleon for several real nuclides and reconstruct (roughly) the binding-energy curve. |

## Objective 19.2a: Identify types of radioactive decay

### Target understanding

A student can identify alpha, beta, positron, electron capture, and spontaneous fission decay from their emissions, and write correctly balanced equations for each.

### Question guides

**1. Forward — classify by emission**
- Variables & ranges: a nuclear equation showing a specific emitted particle.
- Constraint: correct classification based on the emitted particle's identity.
- Contexts: any of the five decay types.
- Formats: short-answer/multiple-choice.
- Worked instantiation: "What type of decay is $\ce{^212_84Po -> ^4_2He + ^208_82Pb}$?" → Alpha decay (emits a $\ce{^4_2He}$ nucleus).

**2. Forward — write a decay equation from type + parent**
- Variables & ranges: a named decay type and a parent nuclide.
- Constraint: correct mass/charge balance for the specific decay type.
- Contexts: any named parent nuclide undergoing a specified decay type.
- Formats: workout.
- Worked instantiation: write the beta decay equation for $\ce{^14_6C}$.

**3. Conceptual — beta vs. positron decay**
- Variables & ranges: any nuclide capable of either beta or positron decay.
- Constraint: explanation must connect the decay type to whether the nuclide has too many or too few neutrons relative to the band of stability.
- Contexts: neutron-rich vs. proton-rich unstable nuclides.
- Formats: short-answer.
- Worked instantiation: "Why does $\ce{^11_6C}$ undergo positron decay rather than beta decay?" → $\ce{^11_6C}$ has too few neutrons relative to protons (it sits below the band of stability); positron decay converts a proton into a neutron, moving the nuclide toward the stable band, while beta decay would move it the wrong way.

**4. Error analysis**
- Variables & ranges: a student who confuses electron capture with beta decay (both involve an electron).
- Constraint: correction must distinguish which side of the equation the electron appears on.
- Contexts: electron capture vs. beta decay equations.
- Formats: short-answer.
- Worked instantiation: "A student thinks electron capture and beta decay are the same process since both involve electrons. What's the difference?" → In beta decay, an electron is *emitted* (produced, appearing on the product side); in electron capture, an electron is *consumed* (appearing on the reactant side, combining with a proton to form a neutron) — they involve electrons in opposite roles.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | Classify and write equations for 3–4 different decay types. |
| Group discussion | Analyze | Debate why a specific nuclide would prefer beta vs. positron decay, based on its N/Z ratio. |
| Quiz | Understand/Apply | One decay-type classification, one equation-writing item. |
| Exam | Analyze | Require both classification and justification (why this decay type, given the nuclide's position relative to stability). |
| Project/activity | Evaluate | Research a real radioisotope's decay chain (e.g., U-238's decay series) and classify each step. |

## Objective 19.2b: Explain radiocarbon dating

### Target understanding

A student can explain the principle behind radiocarbon dating: continuous atmospheric $\ce{^14C}$ production and biological uptake while alive, followed by pure first-order decay after death.

### Question guides

**1. Conceptual — why dating works at all**
- Variables & ranges: any organism (plant or animal).
- Constraint: explanation must include both the continuous-uptake-while-alive and decay-only-after-death phases.
- Contexts: general radiocarbon dating principle.
- Formats: short-answer.
- Worked instantiation: "Why does an organism's $\ce{^14C}$ content stay roughly constant while it's alive, but only decrease after death?" → While alive, an organism continuously exchanges carbon with its environment (eating, breathing), replenishing $\ce{^14C}$ at the same rate it decays, keeping the ratio roughly constant; after death, no new carbon is taken in, so $\ce{^14C}$ can only decrease via radioactive decay from that point forward.

**2. Predict-the-effect — dating limits**
- Variables & ranges: samples of very different ages, up to and beyond ~50,000 years.
- Constraint: prediction must connect the practical dating limit to the half-life and detectability of remaining $\ce{^14C}$.
- Contexts: very old vs. moderately old samples.
- Formats: short-answer.
- Worked instantiation: "Why can't radiocarbon dating reliably date something 200,000 years old?" → After many half-lives (5730 years each), the remaining $\ce{^14C}$ becomes too small a fraction of the original amount to measure reliably — practical radiocarbon dating tops out around 50,000 years for this reason.

**3. Forward — connect to Chapter 13's method**
- Variables & ranges: any radiocarbon dating calculation.
- Constraint: explicit statement that this reuses Chapter 13's integrated first-order rate law.
- Contexts: any dating problem.
- Formats: short-answer.
- Worked instantiation: "What Chapter 13 concept does radiocarbon dating directly reuse?" → The integrated first-order rate law, $\ln(c_0/c)=kt$, and the half-life relationship $t_{1/2}=\ln2/k$ — exactly the same mathematics as any first-order kinetics problem, just applied to a nuclear decay process instead of a chemical reaction.

**4. Error analysis**
- Variables & ranges: a student who assumes radiocarbon dating works for inorganic materials (rocks, metals).
- Constraint: correction must state the method requires a formerly living (carbon-containing, biologically active) sample.
- Contexts: any non-organic dating scenario.
- Formats: short-answer.
- Worked instantiation: "Could radiocarbon dating be used to date a stone tool's age directly?" → Not directly — the stone itself never participated in the biological carbon cycle; radiocarbon dating requires a sample that was once part of a living organism (wood, bone, charcoal, etc.), which took up $\ce{^14C}$ from the atmosphere while alive.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | Explain the two-phase (alive/dead) principle; identify valid vs. invalid dating samples. |
| Group discussion | Analyze | Debate the practical dating-range limit and why it exists. |
| Quiz | Understand | One conceptual explanation item. |
| Exam | Analyze | Require connecting radiocarbon dating explicitly to Chapter 13's kinetics framework. |
| Project/activity | Evaluate | Research a real archaeological radiocarbon dating result and verify the calculation. |

## Objective 19.2c: Apply first-order kinetics to radioactive decay

### Target understanding

A student can calculate rate constant, half-life, elapsed time, or remaining amount for a radioactive decay problem using Chapter 13's first-order integrated rate law, unmodified.

### Question guides

**1. Forward — age from activity ratio**
- Variables & ranges: initial and current activity (or amount), known half-life.
- Constraint: correct use of $\ln(c_0/c)=kt$ after finding $k$ from $t_{1/2}$.
- Contexts: any radiocarbon or other first-order decay dating problem.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (Dead Sea Scrolls, ~1900 years).

**2. Forward — a second dating problem**
- Variables & ranges: a different activity ratio, same isotope.
- Constraint: same method, independent numbers.
- Contexts: charcoal or other archaeological samples.
- Formats: workout.
- Worked instantiation: charcoal has 0.48 of new wood's $\ce{^14C}$ activity; find its age ($t_{1/2}=5730$ y).

**3. Conceptual — half-lives elapsed**
- Variables & ranges: a sample at exactly $1/2$, $1/4$, or $1/8$ of original activity.
- Constraint: recognize the number of half-lives directly from the fraction remaining, without needing the integrated rate law explicitly.
- Contexts: any clean fractional-remaining scenario.
- Formats: short-answer.
- Worked instantiation: "A sample's activity has dropped to exactly 1/8 of its original value. How many half-lives have passed?" → 3 half-lives ($1/8=(1/2)^3$).

**4. Error analysis**
- Variables & ranges: a student who treats the decay problem as requiring new nuclear-specific formulas.
- Constraint: correction must point back to Chapter 13's identical method.
- Contexts: any radioactive decay kinetics problem.
- Formats: short-answer.
- Worked instantiation: "A student searches for a special 'radioactive decay formula' distinct from Chapter 13's kinetics equations. What should they realize?" → Radioactive decay is always first-order, so it uses the *exact same* $\ln(c_0/c)=kt$ and $t_{1/2}=\ln2/k$ formulas from Chapter 13 — there is no new or different formula to learn; only the physical quantity being tracked (radioactive amount/activity instead of a reactant's molar concentration) has changed.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 radioactive-decay dating/kinetics problems. |
| Group discussion | Understand | Explicitly map each symbol in the decay kinetics equations back to its Chapter 13 meaning. |
| Quiz | Apply | One dating-style kinetics calculation. |
| Exam | Analyze | Require finding $k$ from $t_{1/2}$ as an explicit intermediate step, not skipped. |
| Project/activity | Evaluate | Compare radiocarbon dating to another isotope's dating method (e.g., potassium-argon) using the same kinetics framework. |

## Objective 19.3a: Explain nuclear fission, chain reactions, and critical mass

### Target understanding

A student can define nuclear fission, explain how a chain reaction becomes self-sustaining, and distinguish subcritical, critical, and supercritical mass conditions.

### Question guides

**1. Conceptual — chain reaction mechanics**
- Variables & ranges: the U-235 fission example.
- Constraint: explanation must reference neutron capture triggering further fission events.
- Contexts: U-235 fission or a similar heavy-nuclide fission.
- Formats: short-answer.
- Worked instantiation: see the study guide's fission equation and its discussion of chain reactions.

**2. Forward — classify subcritical/critical/supercritical**
- Variables & ranges: a described amount of fissionable material relative to a stated critical mass.
- Constraint: correct classification based on whether neutrons are mostly captured or mostly escape.
- Contexts: any fissionable-material scenario.
- Formats: short-answer.
- Worked instantiation: "A sample of U-235 is smaller than its critical mass. What happens to most of the neutrons produced by fission, and what's the consequence?" → Most neutrons escape the sample without being captured by another U-235 nucleus, so the chain reaction cannot sustain itself — this is a subcritical mass.

**3. Predict-the-effect — atomic bomb vs. reactor**
- Variables & ranges: the same fissionable material, arranged differently.
- Constraint: prediction must distinguish the explosive (bomb) vs. controlled (reactor) outcomes based on how criticality is managed.
- Contexts: atomic bomb design vs. nuclear reactor design.
- Formats: short-answer.
- Worked instantiation: "Why does a nuclear reactor not explode like an atomic bomb, even though both rely on U-235 fission?" → A reactor keeps several subcritical pieces of fissionable material together with control rods that absorb excess neutrons, moderating the reaction to proceed mildly and controllably; a bomb deliberately merges subcritical pieces to exceed critical mass rapidly, producing an uncontrolled, explosive chain reaction.

**4. Error analysis**
- Variables & ranges: a student who treats critical mass as a fixed universal constant.
- Constraint: correction must state that critical mass depends on the specific material and geometry.
- Contexts: any critical-mass discussion.
- Formats: short-answer.
- Worked instantiation: "A student says 'the critical mass' as if there's one universal number for all fissionable materials. What's the error?" → Critical mass depends on the specific fissionable material and its geometry/density — it is the amount needed so that, on average, enough neutrons are captured (rather than escaping) to sustain a chain reaction for that particular configuration, not a single fixed constant across all materials and shapes.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | Explain chain reactions and classify 2–3 subcritical/critical scenarios. |
| Group discussion | Analyze | Debate why reactor design (control rods) differs fundamentally from bomb design. |
| Quiz | Understand | One chain-reaction or critical-mass explanation item. |
| Exam | Analyze | Require distinguishing bomb vs. reactor outcomes for the same fissionable material. |
| Project/activity | Evaluate | Research the historical development of nuclear reactors and critical-mass calculations. |

## Objective 19.3b: Explain nuclear fusion and its requirements

### Target understanding

A student can define nuclear fusion, explain why very high temperatures are required, and give real examples of where fusion occurs.

### Question guides

**1. Conceptual — why fusion needs extreme temperature**
- Variables & ranges: any fusion reaction.
- Constraint: explanation must reference overcoming electrostatic (Coulomb) repulsion between positively charged nuclei.
- Contexts: any light-nuclide fusion reaction.
- Formats: short-answer.
- Worked instantiation: "Why does nuclear fusion require extremely high temperatures to occur?" → Nuclei are all positively charged and repel each other electrostatically; extremely high temperatures give nuclei enough kinetic energy to overcome this repulsion and get close enough for the (much shorter-range) strong nuclear force to bind them together.

**2. Forward — identify fusion examples**
- Variables & ranges: the Sun vs. a hydrogen bomb.
- Constraint: correct identification of both as fusion, with different temperature-achieving mechanisms.
- Contexts: solar fusion vs. thermonuclear weapon fusion.
- Formats: short-answer.
- Worked instantiation: "What provides the extreme temperature needed for fusion in (a) the Sun and (b) a hydrogen bomb?" → (a) The Sun's own gravitational compression and core pressure generate the needed temperature (~15 million K) continuously; (b) a hydrogen bomb uses a fission "trigger" explosion to briefly generate the extreme temperature needed to ignite fusion.

**3. Predict-the-effect — why controlled fusion power is hard**
- Variables & ranges: any fusion-based energy generation proposal.
- Constraint: prediction must connect the difficulty to sustaining extreme temperatures in a controlled (non-explosive) setting.
- Contexts: fusion power research.
- Formats: short-answer.
- Worked instantiation: "Why has controlled nuclear fusion power been so much harder to achieve than nuclear fission power?" → Fission only requires initiating and moderating a chain reaction at manageable conditions, while fusion requires sustaining extremely high temperatures (tens of millions of degrees) in a controlled, continuous, non-explosive way — an immense engineering challenge not yet solved at commercial scale.

**4. Error analysis**
- Variables & ranges: a student who confuses fusion (combining) with fission (splitting).
- Constraint: correction must restate the fixed pairing (fission=heavy splits, fusion=light combines).
- Contexts: any fission/fusion mix-up.
- Formats: short-answer.
- Worked instantiation: "A student says the Sun's energy comes from nuclear fission. What's the correct process?" → The Sun's energy comes from nuclear *fusion* — light nuclei (hydrogen isotopes) combining into heavier ones (helium); fission is the splitting of heavy nuclei, which is not what powers the Sun.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | Explain the temperature requirement; identify 2 real fusion examples. |
| Group discussion | Analyze | Debate why fusion power remains experimental while fission power is commercially established. |
| Quiz | Understand | One fusion-temperature-requirement explanation item. |
| Exam | Analyze | Require contrasting fission and fusion directly (which splits, which combines, and their real examples). |
| Project/activity | Evaluate | Research a real current fusion research program (e.g., ITER) and its temperature/confinement approach. |

## Objective 19.3c: Explain why fission and fusion both release energy

### Target understanding

A student can explain, using the binding-energy-per-nucleon curve, why both nuclear fission (heavy nuclei splitting) and nuclear fusion (light nuclei combining) release energy — because both move nuclei toward the more stable, higher-binding-energy region near iron.

### Question guides

**1. Conceptual — the shared explanation**
- Variables & ranges: any fission or fusion reaction.
- Constraint: explanation must reference movement toward the Fe-56 peak of the binding-energy curve.
- Contexts: the study guide's own binding-energy-curve figure.
- Formats: short-answer.
- Worked instantiation: "Fission splits heavy nuclei and fusion combines light nuclei — opposite processes. Why do both release energy?" → Both processes move nuclei toward higher binding energy per nucleon, peaking near $\ce{^56_26Fe}$: heavy nuclei (to the right of the peak) release energy by splitting into intermediate-mass products closer to the peak, while light nuclei (to the left of the peak) release energy by combining into heavier products closer to the peak.

**2. Forward — predict which region releases energy**
- Variables & ranges: a nuclide's approximate mass number.
- Constraint: correct identification of whether fission or fusion (not both) would release energy for that mass region.
- Contexts: a very light nuclide (e.g., A≈4) vs. a very heavy one (e.g., A≈235).
- Formats: short-answer.
- Worked instantiation: "Would fusing two $\ce{^56_26Fe}$ nuclei together release energy? Why or why not?" → No — $\ce{^56_26Fe}$ is already at (or essentially at) the peak of the binding-energy curve; combining two iron nuclei would move the product to a *higher* mass number with *lower* binding energy per nucleon, which would require energy input rather than releasing it.

**3. Predict-the-effect — comparing energy release magnitude**
- Variables & ranges: a fusion reaction (light nuclei) vs. a fission reaction (heavy nuclei), by typical per-nucleon energy change.
- Constraint: recognize that fusion of very light nuclei (far from the peak) typically releases more energy per nucleon than fission of heavy nuclei (closer to the peak already).
- Contexts: H-2/H-3 fusion vs. U-235 fission.
- Formats: short-answer.
- Worked instantiation: referencing the binding-energy curve's steepness, explain why fusion reactions (e.g., in the Sun or a hydrogen bomb) tend to release more energy per nucleon than fission reactions.

**4. Error analysis**
- Variables & ranges: a student who treats fission and fusion as releasing energy for unrelated reasons.
- Constraint: correction must unify both under the single binding-energy-curve explanation.
- Contexts: any fission-vs-fusion energy-release discussion.
- Formats: short-answer.
- Worked instantiation: "A student explains fission's energy release using one idea and fusion's using a completely different, unrelated idea. What's the more unified explanation?" → Both are explained by the same binding-energy-per-nucleon curve — energy is released whenever a nuclear process moves the product(s) closer to the Fe-56 peak than the reactant(s) were, regardless of whether that means splitting apart (fission) or combining together (fusion).

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | Explain why both fission and fusion release energy, referencing the same curve. |
| Group discussion | Analyze | Debate why iron is the "end point" nuclei tend toward, and why stars can't fuse past it to release energy. |
| Quiz | Understand | One binding-energy-curve-based explanation item. |
| Exam | Analyze | Require predicting whether a hypothetical reaction near the peak would release or require energy. |
| Project/activity | Evaluate | Research why stellar nucleosynthesis stops producing energy once it reaches iron-group elements. |

## Rubric Themes for Chapter 19

| Evidence of mastery | What to look for |
|---|---|
| Nuclear equations balanced by mass number and charge only | Student never tries to conserve element identity, correctly citing the two nuclear conservation rules. |
| Mass-defect sign convention applied consistently | Student subtracts atomic mass from separate-particle mass (not the reverse) and correctly interprets a negative ΔE as energy release. |
| Radioactive decay treated as ordinary first-order kinetics | Student explicitly reuses Chapter 13's $\ln(c_0/c)=kt$ and $t_{1/2}=\ln2/k$ without treating this chapter as requiring new formulas. |
| Fission and fusion correctly paired with examples | Student never confuses which process splits (fission, heavy) vs. combines (fusion, light), or their standard real-world examples. |
| Critical mass explained as a condition, not a constant | Student explains critical mass in terms of neutron capture vs. escape for a specific material/geometry, not as one universal number. |
| Binding energy per nucleon used to explain fission/fusion energy release | Student connects both processes to moving toward the Fe-56 peak of the binding-energy curve, not as two unrelated facts. |
