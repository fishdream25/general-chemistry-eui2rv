{{nyml
kind: document
format: 1
title: Chapter 17 Assessment Guide: Entropy, Free Energy, and Equilibrium
}}

# Chapter 17 Assessment Guide: Entropy, Free Energy, and Equilibrium

## Source and Format

**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 17 (CC BY 4.0). **Audience:** introductory undergraduate general chemistry, second semester. **Note:** this is design guidance for building assessments — question *guides* an instructor or generator can instantiate into many concrete questions — not a finished question bank or answer key.

## General Assessment Priorities

- Anchor every **ΔS sign prediction** to the two explicit rules (phase change, change in moles of gas) before any other consideration — never let students guess from intuition alone.
- Keep **ΔG°** (one fixed number) and **ΔG** (varies with Q) visually and conceptually distinct in every question that uses both — mislabeling one for the other is the single most common error in this chapter.
- Require students to **isolate T algebraically first** ($T=\Delta H/\Delta S$) before substituting numbers in any transition-temperature problem, to prevent sign slips.
- Pair every ΔG°-to-K question with a **qualitative prediction check** (should K be greater or less than 1, given the sign of ΔG°?) before the numeric answer is accepted.

## Objective 17.1a: Define entropy via microstates and predict the sign of ΔS

### Target understanding

A student can explain entropy as a measure of accessible microstates ($S=k\ln W$) and can predict whether a physical or chemical process increases or decreases entropy, based on phase changes and changes in the number of gas-phase particles.

### Question guides

**1. Conceptual — microstates and probability**
- Variables & ranges: the study guide's own 4-particles/2-boxes example.
- Constraint: explanation must connect "more microstates" to "more probable, higher entropy."
- Contexts: any small system of distinguishable particles in multiple containers.
- Formats: short-answer.
- Worked instantiation: "Why does the 2-2 distribution of 4 particles in 2 boxes have higher entropy than the 4-0 distribution?" → The 2-2 distribution corresponds to 6 microstates, while 4-0 corresponds to only 1; since entropy is $k\ln W$, more microstates means higher entropy, and since probability is proportional to the number of microstates, the 2-2 distribution is also the most probable.

**2. Forward — predict ΔS sign, phase change**
- Variables & ranges: any process changing physical state (melting, vaporizing, freezing, condensing, dissolving a gas).
- Constraint: prediction justified by the gas ≫ liquid > solid rule.
- Contexts: any common phase change.
- Formats: short-answer/multiple-choice.
- Worked instantiation: "Predict the sign of ΔS for $\ce{Br2(l) -> Br2(g)}$." → Positive — going from liquid to gas dramatically increases the number of accessible microstates.

**3. Forward — predict ΔS sign, reaction with changing gas moles**
- Variables & ranges: a balanced reaction with unequal gas moles on each side.
- Constraint: prediction justified by the change in total moles of gas.
- Contexts: any gas-phase or gas-producing/consuming reaction.
- Formats: short-answer/multiple-choice.
- Worked instantiation: predict the sign of ΔS° for $\ce{N2(g)+3H2(g)->2NH3(g)}$ (4 mol gas → 2 mol gas, so ΔS° should be negative).

**4. Error analysis**
- Variables & ranges: a student who predicts ΔS sign based on whether a reaction is exothermic or endothermic instead of state/mole-count changes.
- Constraint: correction must redirect to the two correct rules.
- Contexts: any reaction where enthalpy sign and entropy sign happen to differ.
- Formats: short-answer.
- Worked instantiation: "A student assumes an exothermic reaction always has negative ΔS. Why is this reasoning flawed?" → ΔH and ΔS are independent quantities — enthalpy sign depends on bond energies, while entropy sign depends on phase changes and changes in gas-phase particle count; a reaction can be exothermic while still having a positive ΔS if, for example, it produces more moles of gas than it consumes.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | 3–4 ΔS-sign predictions across phase changes and reactions. |
| Group discussion | Analyze | Debate why the 4-particles-2-boxes example generalizes to real molecular systems. |
| Quiz | Understand | One phase-change and one reaction ΔS-sign prediction. |
| Exam | Analyze | Require justification referencing both rules explicitly (phase and gas-mole count). |
| Project/activity | Evaluate | Research a real reaction's measured ΔS° and check it against the qualitative prediction rules. |

## Objective 17.1b: Calculate the standard entropy of a reaction

### Target understanding

A student can calculate $\Delta S^\circ_{rxn}$ from tabulated standard molar entropies, using the same additive method as Chapter 6's $\Delta H^\circ_{rxn}$.

### Question guides

**1. Forward — calculate ΔS°rxn**
- Variables & ranges: a balanced equation with given $S^\circ$ values for all species.
- Constraint: correct stoichiometric weighting (coefficients as multipliers).
- Contexts: any reaction with tabulated standard entropies.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{4Fe+3O2->2Fe2O3}$, $\Delta S^\circ_{rxn}=-550$ J/K·mol).

**2. Forward — a simple diatomic combustion**
- Variables & ranges: $\ce{S(s)+O2(g)->SO2(g)}$ with given $S^\circ$ values.
- Constraint: same additive method, smaller magnitude expected (no net change in gas moles).
- Contexts: any reaction with equal gas moles on both sides.
- Formats: workout.
- Worked instantiation: given $S^\circ(\ce{S})=31.88$, $S^\circ(\ce{O2})=205.0$, $S^\circ(\ce{SO2})=248.5$ J/K·mol, calculate $\Delta S^\circ_{rxn}$.

**3. Conceptual — magnitude vs. sign**
- Variables & ranges: a reaction with no net change in gas moles.
- Constraint: explanation must state that ΔS° should be small in magnitude (either sign) in this case.
- Contexts: any reaction with equal gas moles on both sides.
- Formats: short-answer.
- Worked instantiation: "Why is $\Delta S^\circ_{rxn}$ typically small in magnitude for a reaction with no net change in gas moles?" → With the same number of gas-phase particles on both sides, the dominant driver of large entropy changes (gas formation/consumption) is absent, so any remaining ΔS° comes from smaller effects (molecular complexity differences) and tends to be modest.

**4. Error analysis**
- Variables & ranges: a student who reverses products and reactants in the summation.
- Constraint: correction must restate "products minus reactants."
- Contexts: any $\Delta S^\circ_{rxn}$ calculation.
- Formats: short-answer.
- Worked instantiation: "A student computes $\Delta S^\circ_{rxn}$ as (reactants) − (products) instead of (products) − (reactants). What's the effect?" → The calculated value will have the opposite sign of the correct answer — the convention for both $\Delta H^\circ_{rxn}$ and $\Delta S^\circ_{rxn}$ is always products minus reactants, each weighted by its stoichiometric coefficient.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 ΔS°rxn calculations from tabulated data. |
| Group discussion | Understand | Compare the method directly to Chapter 6's ΔH°rxn calculation. |
| Quiz | Apply | One ΔS°rxn calculation. |
| Exam | Analyze | Combine with a qualitative sign prediction to check before calculating (Objective 17.1a). |
| Project/activity | Evaluate | Look up real standard entropies for a chosen reaction and calculate ΔS°rxn. |

## Objective 17.2a: State the laws of thermodynamics and explain the second law as the spontaneity criterion

### Target understanding

A student can state all four laws of thermodynamics in their own words and can explain why the second law — total universe entropy must increase — is the fundamental criterion for whether a process is spontaneous.

### Question guides

**1. Forward — state each law**
- Variables & ranges: each of the four laws individually.
- Constraint: statement must be in the student's own words, not memorized verbatim.
- Contexts: general thermodynamics.
- Formats: short-answer.
- Worked instantiation: "State the zeroth law of thermodynamics and explain why it matters for the concept of temperature." → If two systems are each in thermal equilibrium with a third, they are in thermal equilibrium with each other — this transitivity is what makes "temperature" a single, consistent, universally comparable quantity rather than a pairwise relationship.

**2. Conceptual — second law as spontaneity criterion**
- Variables & ranges: a spontaneous process where the system's own entropy decreases.
- Constraint: explanation must reference total (system + surroundings) entropy, not system entropy alone.
- Contexts: water freezing below 0 °C, gas condensing, or similar system-entropy-decreasing spontaneous processes.
- Formats: short-answer.
- Worked instantiation: "Water freezing at −5 °C is spontaneous, yet the system's entropy clearly decreases (liquid → solid). How is this consistent with the second law?" → The second law requires only that the *total* entropy of the universe increases; freezing releases heat to the surroundings, increasing the surroundings' entropy by more than the system's entropy decreases, so the net (universe) entropy change is still positive.

**3. Predict-the-effect — heat death of the universe**
- Variables & ranges: the long-term extrapolation of the second law.
- Constraint: explanation must connect maximum entropy to the cessation of spontaneous processes.
- Contexts: cosmological/big-picture framing of the second law.
- Formats: short-answer.
- Worked instantiation: "What would it mean for the universe to reach its maximum possible entropy?" → No further process that increases entropy (which is every spontaneous process, including the physical processes needed to sustain life) could occur — this hypothetical end state is called the "heat death" of the universe.

**4. Error analysis**
- Variables & ranges: a student who conflates the first and second laws.
- Constraint: correction must distinguish conservation of energy (first law) from directionality of natural processes (second law).
- Contexts: any first-vs-second-law confusion.
- Formats: short-answer.
- Worked instantiation: "A student says the first law explains why heat flows from hot to cold, not cold to hot. What's the actual explanation?" → The first law only says energy is conserved — it doesn't forbid heat flowing from cold to hot in principle. The second law is what forbids it: heat flowing from cold to hot spontaneously would decrease total entropy, which never happens spontaneously.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | State all four laws in your own words; explain one system-entropy-decreasing spontaneous process. |
| Group discussion | Analyze | Debate the "heat death of the universe" as a philosophical/physical consequence of the second law. |
| Quiz | Understand | State the second law and give one example application. |
| Exam | Analyze | Require explaining a system-entropy-decreasing spontaneous process using total (universe) entropy. |
| Project/activity | Evaluate | Research a real irreversible process and analyze its entropy change in both system and surroundings. |

## Objective 17.2b: Explain the third law's role in absolute entropy

### Target understanding

A student can explain why the third law (a perfect crystal at 0 K has zero entropy) enables absolute entropy values to be tabulated, in contrast to enthalpy, which is only ever measured as a change.

### Question guides

**1. Conceptual — why entropy can be absolute**
- Variables & ranges: a comparison between $S^\circ$ (absolute) and $\Delta H^\circ_f$ (relative to elements).
- Constraint: explanation must invoke the third law's zero-point reference.
- Contexts: any standard-entropy or standard-enthalpy table.
- Formats: short-answer.
- Worked instantiation: see the study guide's self-check (why $\Delta H^\circ_f$ of an element is zero by definition, but $S^\circ$ isn't).

**2. Forward — interpreting a real S° value**
- Variables & ranges: diamond's $S^\circ=2.4$ J/K·mol at 25 °C.
- Constraint: interpretation must reference the small number of accessible microstates in a rigid crystal.
- Contexts: diamond, or another highly ordered crystalline solid.
- Formats: short-answer.
- Worked instantiation: "Why is diamond's standard entropy so much smaller than that of a gas like $\ce{O2}$ ($S^\circ=205.2$ J/K·mol)?" → Diamond's carbon atoms are locked into a rigid, highly ordered crystal lattice with very few accessible microstates, while gas molecules can occupy a huge number of positions and momenta — far more microstates, and therefore far higher entropy.

**3. Predict-the-effect — temperature and entropy**
- Variables & ranges: a substance at increasing temperature, starting from near 0 K.
- Constraint: prediction must state that entropy increases with temperature, approaching zero only at 0 K.
- Contexts: any pure crystalline substance.
- Formats: short-answer.
- Worked instantiation: "Would you expect diamond's entropy at 200 °C to be higher, lower, or the same as at 25 °C? Why?" → Higher — increasing temperature increases the number of thermally accessible microstates (more vibrational energy levels populated), so entropy increases with temperature.

**4. Error analysis**
- Variables & ranges: a student who assumes all substances have zero entropy at 25 °C, confusing standard enthalpy of formation's zero-reference convention with entropy.
- Constraint: correction must clarify the third law only applies to the *absolute zero* reference point, not to standard-state conditions generally.
- Contexts: any confusion between ΔH°f's elemental-zero convention and S°'s third-law zero.
- Formats: short-answer.
- Worked instantiation: "A student assumes $S^\circ$ of an element in its standard state must be zero, by analogy with $\Delta H^\circ_f$. What's wrong?" → These are different conventions: $\Delta H^\circ_f$ of an element is *defined* as zero by convention (since formation enthalpies are always relative), but $S^\circ$ is an absolute quantity (via the third law's 0 K reference) and is essentially never zero at 25 °C for any real substance, element or not.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | Explain the third law's significance; interpret 2–3 real S° values. |
| Group discussion | Analyze | Compare the "absolute" nature of S° with the "relative" nature of ΔH°f. |
| Quiz | Understand | One third-law explanation item. |
| Exam | Analyze | Require interpreting a given S° value in terms of microstates and crystal order. |
| Project/activity | Evaluate | Research S° values for several related substances (e.g., diamond vs. graphite) and explain the difference. |

## Objective 17.3a: Define Gibbs free energy and apply the spontaneity criterion

### Target understanding

A student can define $G=H-TS$, derive $\Delta G=\Delta H-T\Delta S$ as the spontaneity criterion from the second law, and correctly interpret the sign of ΔG.

### Question guides

**1. Conceptual — why ΔG combines ΔH and ΔS**
- Variables & ranges: any reaction, framed conceptually.
- Constraint: explanation must state that ΔG lets spontaneity be judged from system properties alone.
- Contexts: general thermodynamics.
- Formats: short-answer.
- Worked instantiation: "Why is Gibbs free energy useful, given that the second law is fundamentally about the entropy of the universe, not just the system?" → $\Delta G=\Delta H-T\Delta S$ is derived directly from $\Delta S_{univ}>0$ by substituting $\Delta S_{surr}=-\Delta H_{sys}/T$ — so checking the sign of $\Delta G$ (a system-only quantity) automatically accounts for the surroundings' entropy change too, without ever calculating it directly.

**2. Forward — classify spontaneity from ΔH and ΔS signs**
- Variables & ranges: all four sign combinations of ΔH and ΔS.
- Constraint: student must correctly identify which combinations are always spontaneous, always nonspontaneous, or temperature-dependent.
- Contexts: any reaction with known signs (not necessarily magnitudes) of ΔH and ΔS.
- Formats: short-answer/multiple-choice.
- Worked instantiation: see the source's own practice item ($\Delta H^\circ<0$, $\Delta S^\circ>0$ → spontaneous at all temperatures, since $\Delta G=\Delta H-T\Delta S$ is negative regardless of $T$).

**3. Predict-the-effect — temperature-dependent spontaneity**
- Variables & ranges: ΔH and ΔS with the same sign (both positive or both negative).
- Constraint: prediction must state that spontaneity depends on temperature in these cases.
- Contexts: any reaction where ΔH and ΔS share a sign.
- Formats: short-answer.
- Worked instantiation: "A reaction has $\Delta H^\circ>0$ and $\Delta S^\circ>0$. Is it always spontaneous, always nonspontaneous, or does it depend on temperature?" → It depends on temperature — at low $T$, the $\Delta H$ term dominates ($\Delta G>0$, nonspontaneous); at sufficiently high $T$, the $-T\Delta S$ term dominates and becomes negative enough to make $\Delta G<0$ (spontaneous).

**4. Error analysis**
- Variables & ranges: a student who assumes only ΔS matters for spontaneity, ignoring ΔH.
- Constraint: correction must reference the combined ΔG criterion.
- Contexts: any reaction with a strongly negative ΔH but negative ΔS (or vice versa).
- Formats: short-answer.
- Worked instantiation: "A student says a reaction with $\Delta S^\circ<0$ can never be spontaneous. What's the flaw?" → Spontaneity depends on the combined quantity $\Delta G=\Delta H-T\Delta S$, not $\Delta S$ alone — a sufficiently negative $\Delta H$ can still make $\Delta G<0$ even when $\Delta S<0$, especially at lower temperatures.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | Classify spontaneity for all four ΔH/ΔS sign combinations. |
| Group discussion | Analyze | Debate why the ΔH/ΔS-same-sign cases are the "interesting" ones (temperature-dependent). |
| Quiz | Understand | One sign-combination classification item. |
| Exam | Analyze | Require deriving the direction of temperature-dependence for a given sign combination. |
| Project/activity | Evaluate | Research a real reaction from each of the four sign-combination categories. |

## Objective 17.3b: Calculate standard free energy of reaction

### Target understanding

A student can calculate $\Delta G^\circ_{rxn}$ from tabulated standard free energies of formation, using the same additive (Hess's-law-style) method as Chapter 6, including combining free energies of multiple summed reactions.

### Question guides

**1. Forward — ΔG°rxn from ΔG°f values**
- Variables & ranges: a balanced equation with given $\Delta G^\circ_f$ values.
- Constraint: correct stoichiometric weighting; elements in standard states contribute zero.
- Contexts: any reaction with tabulated formation free energies.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{4Fe+3O2->2Fe2O3}$, $\Delta G^\circ_{rxn}=-1648.4$ kJ/mol).

**2. Forward — combining summed reactions**
- Variables & ranges: two reactions with known $\Delta G^\circ$ summing to a third.
- Constraint: correct addition (or subtraction, for a reversed component) of free energies.
- Contexts: any multi-step free-energy combination.
- Formats: workout.
- Worked instantiation: given $\Delta G^\circ_1=201.3$ kJ/mol for $\ce{ZnS(s)->Zn(s)+S(s)}$ and $\Delta G^\circ_2=-33.4$ kJ/mol for $\ce{S(s)+H2(g)->H2S(g)}$, find $\Delta G^\circ_3$ for $\ce{ZnS(s)+H2(g)->Zn(s)+H2S(g)}$.

**3. Conceptual — why elements contribute zero**
- Variables & ranges: any reaction involving an element in its standard state.
- Constraint: explanation must reference the formation-reaction definition.
- Contexts: any reaction with an elemental reactant or product.
- Formats: short-answer.
- Worked instantiation: "Why does $\ce{O2(g)}$ contribute zero to a $\Delta G^\circ_{rxn}$ calculation?" → $\Delta G^\circ_f$ is defined as the free-energy change to form a substance from its elements in their standard states; for an element already in its standard state, that "formation" is a null process, so its $\Delta G^\circ_f$ is defined as zero.

**4. Error analysis**
- Variables & ranges: a student who adds ΔG° values for reactions that don't actually sum to the target reaction (species don't cancel correctly).
- Constraint: correction must require verifying the reactions actually add up to the target before combining.
- Contexts: any multi-step free-energy combination.
- Formats: short-answer.
- Worked instantiation: "A student adds two reactions' ΔG° values without checking that the intermediate species actually cancel out. What could go wrong?" → If the given reactions don't sum exactly to the target reaction (species left over, or a needed species missing), the resulting $\Delta G^\circ$ won't correspond to the intended reaction at all — always verify by writing out the sum and canceling species explicitly before adding the energies.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 ΔG°rxn calculations, including one multi-step combination. |
| Group discussion | Understand | Compare this method directly to Chapter 6's Hess's law. |
| Quiz | Apply | One ΔG°rxn calculation from formation values. |
| Exam | Analyze | Require verifying that combined reactions actually sum to the target before calculating. |
| Project/activity | Evaluate | Look up real ΔG°f values for a reaction of interest and calculate ΔG°rxn. |

## Objective 17.3c: Determine transition temperatures by setting ΔG = 0

### Target understanding

A student can find the temperature at which a reaction or phase transition becomes spontaneous (or reaches equilibrium) by setting $\Delta G=\Delta H-T\Delta S=0$ and solving for $T$, assuming ΔH and ΔS are temperature-independent.

### Question guides

**1. Forward — reaction onset temperature**
- Variables & ranges: a reaction with known ΔH° and ΔS° (same sign), find the crossover temperature.
- Constraint: isolate $T$ algebraically ($T=\Delta H/\Delta S$) before substituting numbers.
- Contexts: any endothermic, entropy-increasing decomposition reaction.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{CaCO3<=>CaO+CO2}$, $T=1108$ K).

**2. Forward — phase-transition temperature**
- Variables & ranges: given ΔH and ΔS for a phase transition, find the transition temperature.
- Constraint: same $T=\Delta H/\Delta S$ method, applied to melting/boiling instead of a reaction.
- Contexts: melting point, boiling point, or sublimation point calculations.
- Formats: workout.
- Worked instantiation: benzene has $\Delta H^\circ_{fus}=10.9$ kJ/mol and a melting point of 5.5 °C; find $\Delta S^\circ_{fus}$ (rearranging the same relationship in the other direction).

**3. Conceptual — assumptions behind the calculation**
- Variables & ranges: any transition-temperature calculation.
- Constraint: explanation must state the assumption that ΔH and ΔS don't change with temperature.
- Contexts: any $T=\Delta H/\Delta S$ calculation.
- Formats: short-answer.
- Worked instantiation: "What assumption is required to calculate a transition temperature as $T=\Delta H/\Delta S$ using values measured at 25 °C?" → The calculation assumes $\Delta H$ and $\Delta S$ don't change significantly between 25 °C and the transition temperature — a good approximation over a modest temperature range, but increasingly less accurate the further the transition temperature is from 25 °C.

**4. Error analysis**
- Variables & ranges: a student who substitutes numbers into $\Delta G=\Delta H-T\Delta S=0$ without first isolating $T$, introducing a sign error.
- Constraint: correction must recommend isolating $T$ algebraically first.
- Contexts: any transition-temperature calculation.
- Formats: short-answer.
- Worked instantiation: "A student substitutes numbers directly into $0=\Delta H-T\Delta S$ and solves in one messy step, arriving at a negative temperature. What likely went wrong, and what's the fix?" → A sign error was likely introduced during the substitution; isolating $T$ algebraically first ($T=\Delta H/\Delta S$) before plugging in numbers avoids this — a negative or otherwise physically unreasonable temperature is a strong signal to re-check the algebra.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2 transition-temperature calculations, one reaction-based and one phase-based. |
| Group discussion | Analyze | Discuss why this calculation's accuracy degrades far from 25 °C. |
| Quiz | Apply | One transition-temperature calculation. |
| Exam | Analyze | Require identifying whether the reaction is spontaneous at a *given* temperature before finding the crossover point. |
| Project/activity | Evaluate | Look up ΔH and ΔS for a real phase transition and verify the calculated transition temperature against the known value. |

## Objective 17.3d: Relate ΔG° to the equilibrium constant K

### Target understanding

A student can calculate $\Delta G^\circ$ from $K$ (or $K$ from $\Delta G^\circ$) using $\Delta G^\circ=-RT\ln K$, and can qualitatively predict whether $K$ should be greater or less than 1 from the sign of $\Delta G^\circ$ before calculating.

### Question guides

**1. Forward — ΔG° from ΔG°f values, then K**
- Variables & ranges: a reaction with given $\Delta G^\circ_f$ values, find $\Delta G^\circ_{rxn}$ and then $K$.
- Constraint: qualitative sign check before calculating the numeric $K$.
- Contexts: any gas-phase equilibrium with tabulated formation free energies.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{N2O4<=>2NO2}$, $\Delta G^\circ=2.8$ kJ/mol, $K_p=0.323$).

**2. Inverse — ΔG° from K**
- Variables & ranges: a given equilibrium constant, find $\Delta G^\circ$.
- Constraint: correct sign handling in $\Delta G^\circ=-RT\ln K$.
- Contexts: any reaction with a known $K$.
- Formats: workout.
- Worked instantiation: a reaction has $K=4.2\times10^{-3}$ at 298 K; find $\Delta G^\circ$ and state whether it is positive or negative before calculating.

**3. Conceptual — sign correspondence**
- Variables & ranges: a general prompt about the ΔG°-K relationship.
- Constraint: explanation must state that $K>1 \Leftrightarrow \Delta G^\circ<0$ and vice versa.
- Contexts: any $\Delta G^\circ$-K pair.
- Formats: short-answer.
- Worked instantiation: "Without calculating, would you expect $K>1$ or $K<1$ for a reaction with $\Delta G^\circ=-45$ kJ/mol?" → $K>1$ — a negative $\Delta G^\circ$ always corresponds to $K>1$ (product-favored at equilibrium), since $\Delta G^\circ=-RT\ln K$ requires $\ln K>0$ when $\Delta G^\circ<0$.

**4. Error analysis**
- Variables & ranges: a student who drops or mishandles the negative sign in $\Delta G^\circ=-RT\ln K$.
- Constraint: correction must restate the correct sign relationship.
- Contexts: any ΔG°-K calculation.
- Formats: short-answer.
- Worked instantiation: "A student calculates $\Delta G^\circ=+RT\ln K$ (forgetting the negative sign) for a reaction with $K=10$, getting a positive $\Delta G^\circ$. What's wrong, and what should the sign be?" → The correct relationship is $\Delta G^\circ=-RT\ln K$; since $K=10>1$, $\ln K>0$, so $\Delta G^\circ$ should be *negative* — the student's dropped sign gives the opposite (and qualitatively wrong) conclusion.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2 ΔG°-to-K (or K-to-ΔG°) calculations, each with a qualitative sign check first. |
| Group discussion | Analyze | Debate why a very large K (like for a strong acid's ionization) implies a very negative ΔG°. |
| Quiz | Apply | One ΔG°-K conversion, either direction. |
| Exam | Analyze | Require the qualitative prediction explicitly before the numeric answer for partial credit. |
| Project/activity | Evaluate | Research a real reaction's measured K and calculate its ΔG°, connecting to Ch. 14. |

## Objective 17.3e: Calculate ΔG under non-standard conditions and predict reaction direction

### Target understanding

A student can calculate $\Delta G=\Delta G^\circ+RT\ln Q$ given non-standard concentrations or pressures, and can predict reaction direction from the sign of the resulting $\Delta G$ — connecting directly to Chapter 14's $Q$-vs-$K$ framework.

### Question guides

**1. Forward — ΔG from given pressures**
- Variables & ranges: a reaction with known $\Delta G^\circ$ and given non-standard partial pressures.
- Constraint: correct construction of $Q$ from the given pressures before substituting into the ΔG equation.
- Contexts: any gas-phase reaction with non-equilibrium pressures given.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{2NH3->3H2+N2}$, $\Delta G=32.5$ kJ/mol).

**2. Conceptual — ΔG° vs. ΔG**
- Variables & ranges: a prompt distinguishing the two symbols.
- Constraint: explanation must state ΔG° is fixed while ΔG depends on current Q.
- Contexts: any reaction over the course of its progress toward equilibrium.
- Formats: short-answer.
- Worked instantiation: "As a reaction proceeds toward equilibrium, does ΔG° change? Does ΔG change?" → $\Delta G^\circ$ is a fixed constant for a given reaction and temperature — it never changes during the reaction. $\Delta G$ does change, because it depends on $Q$, which changes continuously as reactant and product concentrations shift toward their equilibrium values; $\Delta G$ approaches zero as the reaction approaches equilibrium.

**3. Predict-the-effect — direction from ΔG sign**
- Variables & ranges: a calculated ΔG value (positive or negative).
- Constraint: prediction must connect the sign of ΔG directly to reaction direction, mirroring Chapter 14's Q-vs-K rule.
- Contexts: any non-standard-condition ΔG calculation.
- Formats: short-answer.
- Worked instantiation: "A calculated ΔG for a reaction is −12 kJ/mol under the given conditions. Which direction does the reaction proceed?" → Forward (left to right) — a negative ΔG means the reaction is spontaneous in the forward direction under these specific conditions, equivalent to saying $Q<K$.

**4. Error analysis**
- Variables & ranges: a student who uses ΔG° in place of ΔG (or vice versa) when predicting direction under non-standard conditions.
- Constraint: correction must state that direction under specific, given (non-standard) conditions requires ΔG, not ΔG°.
- Contexts: any problem giving specific non-standard concentrations/pressures.
- Formats: short-answer.
- Worked instantiation: "A student is given specific non-standard pressures and uses the sign of ΔG° (not ΔG) to predict reaction direction. Why is this incorrect?" → ΔG° only describes spontaneity under standard-state conditions (all species at 1 atm or 1 M); to predict direction under the actual, given non-standard conditions, the reaction quotient Q for those specific conditions must be incorporated via $\Delta G=\Delta G^\circ+RT\ln Q$, and the sign of that ΔG (not ΔG°) determines the true direction.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2 ΔG-under-non-standard-conditions calculations, each requiring a direction prediction. |
| Group discussion | Analyze | Debate why ΔG approaches zero as a reaction nears equilibrium. |
| Quiz | Apply | One ΔG calculation with given non-standard pressures/concentrations. |
| Exam | Analyze | Require distinguishing when ΔG° alone suffices (standard conditions) vs. when ΔG is needed (non-standard). |
| Project/activity | Evaluate | Model how ΔG changes over the course of a reaction as Q evolves from its initial value toward K. |

## Rubric Themes for Chapter 17

| Evidence of mastery | What to look for |
|---|---|
| ΔS sign predicted from the two explicit rules | Student references phase change and/or gas-mole-count change explicitly, not vague intuition. |
| ΔG° and ΔG kept visually and conceptually distinct | Student never uses one symbol's value or meaning in place of the other. |
| Transition temperature solved by isolating T first | Student rearranges $\Delta G=\Delta H-T\Delta S=0$ to $T=\Delta H/\Delta S$ before substituting numbers. |
| Qualitative K-vs-1 prediction made before calculating | Student states whether K should be greater or less than 1 from the sign of ΔG°, then verifies the numeric answer matches. |
| Second law applied to the universe, not just the system | Student correctly explains system-entropy-decreasing spontaneous processes via the surroundings' larger entropy increase. |
| ΔG-Q relationship connected to Chapter 14 | Student explicitly ties Δ G = ΔG° + RT ln Q back to the Q-vs-K reaction-direction rule from Chapter 14. |
