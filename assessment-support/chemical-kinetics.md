{{nyml
kind: document
format: 1
title: Chapter 13 Assessment Guide: Chemical Kinetics
}}

# Chapter 13 Assessment Guide: Chemical Kinetics

## Source and Format

**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 13 (CC BY 4.0). **Audience:** introductory undergraduate general chemistry, second semester. **Note:** this is design guidance for building assessments — question *guides* an instructor or generator can instantiate into many concrete questions — not a finished question bank or answer key.

## General Assessment Priorities

- Relentlessly test the **"rate-law exponents come from data, not coefficients"** rule — this is the single most consequential idea in the chapter, and it is worth testing more than once, in more than one format.
- For every integrated-rate-law or half-life question, require students to **state or confirm the reaction order first**, as an explicit step, before selecting a formula.
- Keep activation energy and $\Delta H$ questions paired or adjacent so students build the habit of distinguishing them, rather than encountering them as isolated ideas in different chapters.
- Include at least one full mechanism-analysis question per relevant objective (identify intermediate, rate-determining step, and resulting rate law together) rather than only testing each piece separately.

## Objective 13.1a: Write rate expressions from a balanced equation

### Target understanding

A student can write the shared rate expression for any balanced equation using stoichiometric coefficients, and can convert a rate of change for one species into the rate of change for any other species in the same reaction.

### Question guides

**1. Forward — convert a rate between species**
- Variables & ranges: a balanced equation with coefficients 1–6, a given rate of change for one species.
- Constraint: student must divide/multiply by the correct coefficient ratio, matching sign conventions (reactants negative, products positive).
- Contexts: gas-phase and solution-phase reactions.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (4PH₃ → P₄ + 6H₂, given rate of H₂ formation).

**2. Inverse — find an unknown coefficient's rate given two others**
- Variables & ranges: a reaction where two species' rates are given and a third is requested.
- Constraint: same conversion method, applied twice or with an unknown to solve for.
- Contexts: combustion or synthesis reactions.
- Formats: workout.
- Worked instantiation: given the rate of $\ce{O2}$ consumption in a combustion reaction, find the rate of $\ce{CO2}$ formation.

**3. Conceptual — why divide by coefficients**
- Variables & ranges: a qualitative "explain why" prompt.
- Constraint: explanation must reference the shared/single rate of reaction, not just restate the formula.
- Contexts: any reaction with unequal coefficients.
- Formats: short-answer.
- Worked instantiation: "Why is the rate of change of a reactant with coefficient 4 divided by 4, but a product with coefficient 1 is not divided at all?" → Dividing by each coefficient normalizes every species' rate of change to the same underlying "rate of reaction," so all expressions describe one consistent pace regardless of stoichiometry.

**4. Error analysis**
- Variables & ranges: a rate expression with a missing negative sign for a reactant, or a missing coefficient division.
- Constraint: correction must identify exactly which convention was violated.
- Contexts: any standard rate-expression setup.
- Formats: short-answer.
- Worked instantiation: "A student writes rate $= \Delta[\ce{A}]/\Delta t$ for a reactant A, without a negative sign. What's wrong?" → Reactant concentration decreases over time, so $\Delta[\ce{A}]/\Delta t$ is negative; a negative sign is needed in front so that "rate" itself is reported as a positive quantity.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 rate-conversion problems across different balanced equations. |
| Group discussion | Understand | Discuss why chemists insist on one shared "rate of reaction" instead of species-specific rates. |
| Quiz | Apply | One direct conversion problem. |
| Exam | Analyze | Combine with Objective 13.1b (use the rate expression inside a rate-law problem). |
| Project/activity | Evaluate | Analyze real experimental concentration-vs-time data for a chosen reaction and compute rates of multiple species. |

## Objective 13.1b: Determine a rate law and rate constant from experimental data

### Target understanding

A student can apply the method of initial rates to determine reaction order in each reactant and overall, and can then calculate the rate constant $k$ with correct units, ==without ever assuming the exponents equal the balanced equation's coefficients==.

### Question guides

**1. Forward — determine order from a data table**
- Variables & ranges: a 3-trial data table (concentrations and rate) for a two-reactant reaction, designed so each trial-pair isolates one exponent.
- Constraint: student must select trial pairs where only one concentration changes.
- Contexts: gas-phase or solution kinetics.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (NO/Cl₂ reaction, three trials).

**2. Inverse — predict rate at a new concentration**
- Variables & ranges: given a determined rate law and $k$, predict the rate at a new, unlisted concentration pair.
- Constraint: correct substitution of the determined exponents (not the coefficients).
- Contexts: extending the same dataset to a hypothetical fourth trial.
- Formats: workout.
- Worked instantiation: using the derived rate $=k[\ce{NO}]^2[\ce{Cl2}]$ and calculated $k$, predict the rate at $[\ce{NO}]=0.20$ M, $[\ce{Cl2}]=0.20$ M.

**3. Conceptual — why coefficients aren't exponents**
- Variables & ranges: a qualitative prompt contrasting an elementary step with an overall reaction.
- Constraint: explanation must state that coefficients equal exponents *only* for elementary steps.
- Contexts: general reaction kinetics vs. mechanism steps (links to Objective 13.4a).
- Formats: short-answer.
- Worked instantiation: "Why can't you predict a rate law's exponents just by looking at the balanced overall equation?" → Because most reactions occur through multiple elementary steps, and only an individual elementary step's rate law is guaranteed to match its own coefficients; the overall equation reflects only the net stoichiometry, not the mechanism.

**4. Error analysis**
- Variables & ranges: a flawed rate-law determination that assumes $x=a$, $y=b$ directly from the balanced equation.
- Constraint: correction must identify that experimental comparison was skipped.
- Contexts: the exact bottleneck flagged in the concept map.
- Formats: short-answer.
- Worked instantiation: "A student writes rate $=k[\ce{NO}]^2[\ce{Cl2}]^1$ for $2\ce{NO}+\ce{Cl2}\rightarrow 2\ce{NOCl}$ purely by copying the balanced-equation coefficients, without checking data. Even though the exponents happen to match in this case, what is wrong with the method?" → The exponents must be verified from experimental data; the balanced-equation coefficients are not a valid shortcut, even when they happen to give the correct numerical answer in a particular case.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 1–2 full rate-law determinations from a 3-trial data table. |
| Group discussion | Analyze | Debate why the method of initial rates requires changing one variable at a time. |
| Quiz | Apply | One order-determination problem from a small data table. |
| Exam | Analyze | Full determination of rate law, $k$ (with units), and a rate prediction at a new concentration. |
| Project/activity | Evaluate | Design (on paper) an experiment to determine a rate law for a novel reaction. |

## Objective 13.2a: Apply integrated rate laws

### Target understanding

Given a reaction's order (stated or determined), a student can apply the correct integrated rate law to solve for an unknown concentration or time, ==first confirming the order before selecting a formula==.

### Question guides

**1. Forward — solve for concentration at time $t$**
- Variables & ranges: a stated order, $k$, $[\ce{A}]_0$, and target time.
- Constraint: correct formula selection based on stated order.
- Contexts: first-order decompositions, second-order dimerizations.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (cyclobutane, first-order, find remaining amount after 180 s).

**2. Inverse — solve for time**
- Variables & ranges: given order, $k$, $[\ce{A}]_0$, and a target $[\ce{A}]_t$, solve for $t$.
- Constraint: correct algebraic rearrangement for the given order.
- Contexts: determining how long a reaction takes to reach a specified conversion.
- Formats: workout.
- Worked instantiation: "How long until a first-order reaction with $k=0.025\ \text{s}^{-1}$ reduces $[\ce{A}]_0=0.80$ M to 0.20 M?" → Solve $\ln([\ce{A}]_0/[\ce{A}]_t)=kt$ for $t$.

**3. Comparison / ranking**
- Variables & ranges: two reactions of the same order but different $k$ values, or the same $k$ but different orders.
- Constraint: comparison must be justified by the formula's structure, not guessed.
- Contexts: comparing decomposition rates of two related compounds.
- Formats: short-answer with justification.
- Worked instantiation: two first-order reactions have $k_1 > k_2$; which reaches 50% completion faster, and why?

**4. Multi-step / synthesis**
- Variables & ranges: combine an integrated-rate-law calculation with a stoichiometry step (e.g., converting moles to mass at the final time).
- Constraint: requires sequencing the kinetics calculation with a Chapter 3-style mass/mole conversion.
- Contexts: any concentration-to-mass conversion after a kinetics calculation.
- Formats: workout.
- Worked instantiation: after finding moles of reactant remaining via the integrated rate law, convert to grams remaining using molar mass.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 integrated-rate-law problems, mixing orders. |
| Group discussion | Analyze | Compare how each order's formula behaves as $t\to\infty$. |
| Quiz | Apply | One integrated-rate-law calculation with the order explicitly stated. |
| Exam | Analyze | Require the student to first justify/confirm the order before solving. |
| Project/activity | Evaluate | Fit real or simulated concentration-vs-time data to find $k$. |

## Objective 13.2b: Calculate half-life and determine order graphically

### Target understanding

A student can calculate half-life for any of the three orders, correctly recognizing that ==only first-order half-life is independent of concentration==, and can determine reaction order by identifying which of three linearized plots ($[\ce{A}]$, $\ln[\ce{A}]$, $1/[\ce{A}]$ vs. $t$) is a straight line.

### Question guides

**1. Forward — calculate half-life**
- Variables & ranges: a stated order, $k$, and (for zero/second order) $[\ce{A}]_0$.
- Constraint: correct formula selection; zero/second order require $[\ce{A}]_0$, first order does not.
- Contexts: any of the three orders.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (cyclobutane half-life = 75 s).

**2. Conceptual — successive half-lives**
- Variables & ranges: a first-order vs. a second-order reaction, asked about successive half-life intervals.
- Constraint: explanation must state that first-order half-lives are equal while second-order half-lives lengthen as the reaction proceeds.
- Contexts: comparing two hypothetical reactions' half-life sequences.
- Formats: short-answer.
- Worked instantiation: "A first-order reaction's first half-life is 20 s. What is its second half-life? Would this answer be the same for a second-order reaction with the same initial half-life?" → 20 s again (constant for first order); no — a second-order reaction's second half-life would be longer than its first, since second-order half-life depends inversely on the (now smaller) concentration.

**3. Graphical — identify order from a plot**
- Variables & ranges: a description or image of which of three plots ($[\ce{A}]$, $\ln[\ce{A}]$, $1/[\ce{A}]$ vs. $t$) is linear.
- Constraint: student must connect linearity of a specific plot to a specific order.
- Contexts: the study guide's own linearization figure, or an analogous dataset.
- Formats: short-answer referencing a figure.
- Worked instantiation: "A plot of $1/[\ce{A}]$ vs. $t$ is a straight line for a given dataset, while $[\ce{A}]$ vs. $t$ and $\ln[\ce{A}]$ vs. $t$ are both curved. What is the reaction order?" → Second order (the integrated rate law $1/[\ce{A}]_t = 1/[\ce{A}]_0 + kt$ is linear only for a second-order reaction).

**4. Inverse — find $[\ce{A}]_0$ from a half-life**
- Variables & ranges: given order (zero or second), $k$, and half-life, solve for $[\ce{A}]_0$.
- Constraint: correct rearrangement of the order-specific half-life formula.
- Contexts: back-calculating a starting concentration from observed decay behavior.
- Formats: workout.
- Worked instantiation: a second-order reaction has $t_{1/2}=25$ s and $k=0.040\ \text{M}^{-1}\text{s}^{-1}$; find $[\ce{A}]_0$.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | Half-life calculations across all three orders. |
| Group discussion | Analyze | Sketch (by hand) how [A] vs. t would look for each order, then discuss why linearization is more useful for identifying order than the raw curve. |
| Quiz | Understand/Apply | One half-life calculation, one graphical-identification item. |
| Exam | Analyze | Require identifying order from a described plot, then completing a full calculation. |
| Project/activity | Evaluate | Plot real or simulated data three ways and identify the order from linearity. |

## Objective 13.3a: Apply collision theory concepts

### Target understanding

A student can state both requirements of collision theory (frequency and sufficient energy), define activation energy and transition state, and ==correctly distinguish activation energy from the reaction's overall enthalpy change==.

### Question guides

**1. Conceptual — state the two requirements**
- Variables & ranges: a "why doesn't every collision react" prompt.
- Constraint: answer must include both frequency and energy-threshold requirements, not just one.
- Contexts: any bimolecular reaction.
- Formats: short-answer.
- Worked instantiation: "Why doesn't every collision between reactant molecules result in a reaction?" → Two conditions must both be met: the molecules must collide (frequency), and the collision must carry at least the activation energy $E_a$ — many collisions are too gentle or poorly oriented to react.

**2. Comparison — Ea vs. ΔH**
- Variables & ranges: a reaction profile description (or sketch) with both $E_a$ and $\Delta H$ marked.
- Constraint: answer must correctly identify each quantity's reference points (reactants→peak vs. reactants→products).
- Contexts: any exothermic or endothermic reaction with a given energy profile.
- Formats: short-answer.
- Worked instantiation: "A reaction has $E_a = 80$ kJ/mol and $\Delta H = -40$ kJ/mol. Sketch (in words) what this reaction's energy profile looks like." → Products lie 40 kJ/mol below reactants (exothermic), but the path between them still passes through a transition state 80 kJ/mol above the reactants — a real energy barrier despite the overall energy release.

**3. Predict-the-trend — temperature and collision energy**
- Variables & ranges: a qualitative temperature-increase scenario.
- Constraint: explanation must connect temperature to the *fraction* of sufficiently energetic collisions, not just "more collisions."
- Contexts: any reaction rate vs. temperature observation.
- Formats: short-answer.
- Worked instantiation: "Why does raising temperature by only 10 °C often roughly double a reaction's rate?" → A modest temperature increase disproportionately increases the fraction of collisions with energy above $E_a$ (an exponential relationship), not just the total collision frequency.

**4. Error analysis**
- Variables & ranges: a flawed claim equating $E_a$ with $\Delta H$.
- Constraint: correction must restate both definitions precisely.
- Contexts: the exact bottleneck flagged in the concept map.
- Formats: short-answer.
- Worked instantiation: "A student claims a reaction with a very negative $\Delta H$ must have a small $E_a$ ('it releases a lot of energy, so it must be easy'). Explain the error." → $E_a$ and $\Delta H$ are independent quantities — a highly exothermic reaction can still have a large activation-energy barrier, meaning it releases a lot of energy overall but still requires significant energy input to get started.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | 2–3 conceptual explain-why items. |
| Group discussion | Analyze | Sketch and compare energy profiles for reactions with different $E_a$/$\Delta H$ combinations. |
| Quiz | Understand | One definition item, one Ea-vs-ΔH distinction item. |
| Exam | Analyze | Require sketching or describing a full energy profile from given $E_a$ and $\Delta H$ values. |
| Project/activity | Evaluate | Research a real reaction's measured $E_a$ and explain what a catalyst would change about its profile. |

## Objective 13.3b: Apply the Arrhenius equation

### Target understanding

A student can use the two-point Arrhenius equation to solve for activation energy or an unknown rate constant, correctly using temperature in kelvin throughout.

### Question guides

**1. Forward — solve for $E_a$**
- Variables & ranges: two (T, k) pairs.
- Constraint: T must be in kelvin; correct substitution into the two-point form.
- Contexts: any two-temperature rate-constant dataset.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (acetaldehyde decomposition, $E_a$ = 190 kJ/mol).

**2. Inverse — solve for $k$ at a new temperature**
- Variables & ranges: $E_a$, one (T, k) pair, and a target temperature.
- Constraint: correct rearrangement to isolate the unknown $k$.
- Contexts: predicting a rate constant at an untested temperature.
- Formats: workout.
- Worked instantiation: given $E_a$ and $k$ at one temperature, predict $k$ at a second, higher temperature.

**3. Conceptual — sign and magnitude reasoning**
- Variables & ranges: a qualitative prompt about which reaction is more temperature-sensitive.
- Constraint: answer must connect larger $E_a$ to greater temperature sensitivity.
- Contexts: comparing two reactions with different $E_a$ values.
- Formats: short-answer.
- Worked instantiation: "Reaction A has $E_a = 40$ kJ/mol; reaction B has $E_a = 120$ kJ/mol. Which reaction's rate is more sensitive to a given temperature increase?" → Reaction B — a larger $E_a$ means the fraction of sufficiently energetic collisions changes more dramatically with temperature.

**4. Multi-step / synthesis**
- Variables & ranges: combine an Arrhenius calculation with a half-life or integrated-rate-law question at the new temperature.
- Constraint: requires first finding $k$ at the new temperature, then using it in a separate kinetics formula.
- Contexts: predicting how a reaction's half-life changes with temperature.
- Formats: workout.
- Worked instantiation: find $k$ at a new temperature via Arrhenius, then use that $k$ to calculate the reaction's half-life at the new temperature.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2 forward/inverse Arrhenius calculations. |
| Group discussion | Analyze | Discuss why T must be in kelvin (ties back to Ch. 5 and Ch. 11 habits). |
| Quiz | Apply | One straightforward $E_a$-solving item. |
| Exam | Synthesize | Combine Arrhenius with an integrated-rate-law or half-life calculation at the new temperature. |
| Project/activity | Evaluate | Look up real Arrhenius parameters for a reaction and predict its rate at a new temperature. |

## Objective 13.4a: Analyze reaction mechanisms

### Target understanding

Given a proposed multi-step mechanism, a student can identify intermediates, write each elementary step's rate law directly from molecularity, identify the rate-determining step, and derive the overall rate law from it.

### Question guides

**1. Forward — full mechanism analysis**
- Variables & ranges: a 2-step mechanism with one step labeled slow/fast (or with relative rate constants given).
- Constraint: student must find the overall reaction (canceling intermediates), name the intermediate, and state the overall rate law from the rate-determining step.
- Contexts: any plausible 2-step gas-phase or solution mechanism.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (NO₂/CO mechanism).

**2. Inverse — propose a mechanism consistent with a given rate law**
- Variables & ranges: an overall reaction and its experimentally-determined rate law (matching neither reactant's coefficient).
- Constraint: proposed mechanism's rate-determining step must reproduce the given rate law exactly.
- Contexts: a reaction whose rate law is known but whose mechanism is not yet given.
- Formats: workout (open-ended, multiple valid answers possible).
- Worked instantiation: given an overall reaction and a rate law that is first-order in one reactant only (despite a coefficient of 2 in the balanced equation), propose a plausible 2-step mechanism consistent with that rate law.

**3. Conceptual — intermediates vs. catalysts**
- Variables & ranges: a mechanism where a species is regenerated (a catalyst) vs. one that is only ever produced-then-consumed (an intermediate).
- Constraint: explanation must distinguish the two based on when each species appears (start vs. mid-mechanism).
- Contexts: catalyzed mechanisms (links to Objective 13.5a).
- Formats: short-answer.
- Worked instantiation: "In a mechanism, species X is consumed in step 1 and regenerated in step 2. Is X an intermediate or a catalyst? What if X were instead produced in step 1 and consumed in step 2?" → If X is present at the start and regenerated at the end, it is a catalyst; if X is produced first and only later consumed (never present at the start), it is an intermediate.

**4. Error analysis**
- Variables & ranges: a flawed rate law written for an elementary step that doesn't match its molecularity, or an overall rate law incorrectly derived from a non-rate-determining step.
- Constraint: correction must identify exactly which step's rate law should have been used.
- Contexts: the exact bottleneck flagged in the concept map (assuming the rate-determining step must be first).
- Formats: short-answer.
- Worked instantiation: "A 3-step mechanism has its largest activation energy in step 2. A student uses step 1's rate law as the overall rate law. What's wrong?" → The rate-determining step is identified by the largest activation energy on the potential-energy profile, which is step 2 here — not necessarily the first step; the overall rate law should come from step 2's rate law instead.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 full mechanism-analysis problems (intermediate, rate law, overall reaction). |
| Group discussion | Analyze | Debate whether a given proposed mechanism is consistent with an experimentally observed rate law. |
| Quiz | Apply | One mechanism-analysis problem. |
| Exam | Analyze | Require both directions: analyze a given mechanism, and propose one consistent with a given rate law. |
| Project/activity | Evaluate | Research a real named reaction mechanism (e.g., SN1/SN2 preview, or an atmospheric ozone reaction) and identify its rate-determining step. |

## Objective 13.4b: Interpret a potential-energy profile

### Target understanding

A student can read a potential-energy profile to identify the number of elementary steps, locate transition states and intermediates, determine each step's activation energy, identify the rate-determining step, and state whether the overall reaction is exothermic or endothermic.

### Question guides

**1. Forward — read a profile**
- Variables & ranges: a described or sketched multi-step profile (2–3 steps) with labeled or unlabeled peaks/valleys.
- Constraint: student must correctly count peaks (transition states) and valleys excluding endpoints (intermediates).
- Contexts: the study guide's own 2-step profile, or an analogous 3-step one.
- Formats: short-answer referencing a figure.
- Worked instantiation: see the study guide's Figure 13.5 discussion (identify TS1, TS2, the intermediate, and the rate-determining step).

**2. Conceptual — exothermic vs. endothermic overall**
- Variables & ranges: a profile where the final product energy is above or below the initial reactant energy.
- Constraint: answer must compare only the reactant and product energy levels, ignoring intermediate peaks/valleys.
- Contexts: any multi-step profile.
- Formats: short-answer.
- Worked instantiation: "In a profile where products end up at higher energy than reactants, despite one very deep intermediate valley, is the overall reaction exothermic or endothermic?" → Endothermic — only the reactant and final product energy levels determine the overall sign of $\Delta H$; the intermediate valley's depth is irrelevant to that comparison.

**3. Graphical — identify the rate-determining step**
- Variables & ranges: a profile with 2–3 peaks of different heights.
- Constraint: student must select the step with the tallest peak *relative to its starting point*, not the tallest peak overall in absolute energy.
- Contexts: a 3-step profile where the highest peak is not the first step.
- Formats: short-answer referencing a figure.
- Worked instantiation: "In a 3-step profile, the second peak is the highest point on the entire diagram, but the activation energy for step 3 (measured from its own starting intermediate) is actually larger than step 2's. Which step is rate-determining?" → Step 3 — activation energy is measured relative to each step's own starting point, not by absolute height on the diagram.

**4. Multi-step / synthesis**
- Variables & ranges: combine profile-reading with a rate-law-writing task (Objective 13.4a).
- Constraint: student must first identify the rate-determining step from the profile, then write its rate law.
- Contexts: a given profile plus the corresponding elementary steps' equations.
- Formats: workout.
- Worked instantiation: given a labeled profile and the balanced elementary steps, identify the rate-determining step from the profile and write the resulting overall rate law.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | 2–3 profile-reading items (count steps, identify intermediates/transition states). |
| Group discussion | Analyze | Sketch a profile from a written mechanism description and compare with classmates. |
| Quiz | Understand | One profile-reading item. |
| Exam | Analyze | Combine profile interpretation with rate-law derivation. |
| Project/activity | Evaluate | Construct a profile (with reasonable relative energies) for a real multi-step reaction from literature data. |

## Objective 13.5a: Explain catalysis and distinguish catalyst types

### Target understanding

A student can explain that a catalyst lowers activation energy for both directions without being consumed or appearing in the overall equation, and can classify a given catalytic process as heterogeneous, homogeneous, or enzyme catalysis.

### Question guides

**1. Forward — classify a catalytic process**
- Variables & ranges: a described catalytic system (phases of catalyst and reactants specified).
- Constraint: classification must be justified by comparing catalyst phase to reactant phase (or noting biological specificity for enzymes).
- Contexts: industrial, environmental, and biological catalysis examples.
- Formats: short-answer or multiple-choice.
- Worked instantiation: "A solid platinum surface catalyzes the reaction of gas-phase CO and O₂. What type of catalysis is this?" → Heterogeneous — the catalyst (solid) is in a different phase from the reactants (gas).

**2. Conceptual — what a catalyst does and doesn't change**
- Variables & ranges: a prompt asking which reaction quantities change with a catalyst and which don't.
- Constraint: answer must state that $E_a$ decreases (both directions) while $\Delta H$, $K$ (equilibrium constant, preview of Ch. 14), and the overall balanced equation are unchanged.
- Contexts: any catalyzed reaction.
- Formats: short-answer.
- Worked instantiation: "Does adding a catalyst change a reaction's $\Delta H$? Does it change its rate constant $k$? Explain both answers." → $\Delta H$ is unchanged (it depends only on reactant/product energies, not the pathway); $k$ increases because the catalyst provides a lower-$E_a$ pathway, directly increasing the rate constant via the Arrhenius equation.

**3. Real-world / applied**
- Variables & ranges: a named real catalytic application (catalytic converter, enzyme, industrial catalyst).
- Constraint: explanation must connect the application to lowered activation energy specifically.
- Contexts: automotive emissions control, digestion, industrial ammonia synthesis.
- Formats: short-answer.
- Worked instantiation: "Explain, in terms of activation energy, why a catalytic converter allows toxic exhaust gases to be converted to less harmful products before leaving the tailpipe." → The catalytic surface provides an alternate reaction pathway with much lower activation energy than the uncatalyzed gas-phase reaction, so the conversion happens fast enough at exhaust-system temperatures and residence times to be effective.

**4. Comparison — catalyst vs. reactant vs. intermediate**
- Variables & ranges: a mechanism where a catalyst appears in an early step and is regenerated later (links to Objective 13.4a).
- Constraint: student must distinguish a catalyst (present at start, regenerated) from an intermediate (produced then consumed, never present at start).
- Contexts: a catalyzed mechanism shown step by step.
- Formats: short-answer.
- Worked instantiation: given a 2-step catalyzed mechanism, identify which species is the catalyst and which (if any) is an intermediate.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand/Apply | Classify 3–4 catalytic examples by type. |
| Group discussion | Analyze | Debate why enzymes are often described as the most "specific" catalysts. |
| Quiz | Understand | One classification item, one conceptual Ea-vs-ΔH-under-catalysis item. |
| Exam | Analyze | Combine catalyst classification with a mechanism-based catalyst/intermediate distinction. |
| Project/activity | Evaluate | Research a real industrial catalytic process (e.g., the Haber process) and identify the catalyst type and its role. |

## Rubric Themes for Chapter 13

| Evidence of mastery | What to look for |
|---|---|
| Rate-law exponents never assumed from coefficients | Student explicitly states or derives exponents from data (or notes "elementary step" as the exception) every time a rate law is written. |
| Correct order confirmed before formula selection | Integrated-rate-law and half-life answers show an explicit order-confirmation step, not a jump straight to a formula. |
| $E_a$ and $\Delta H$ kept conceptually distinct | Any energy-profile discussion correctly separates "barrier height from the start" ($E_a$) from "net energy change, start to finish" ($\Delta H$). |
| Rate-determining step identified by largest activation energy | Student never assumes the first step is automatically rate-determining; they check activation energies (or given "slow/fast" labels) explicitly. |
| Intermediates and catalysts correctly distinguished | Student identifies an intermediate as produced-then-consumed and a catalyst as present-then-regenerated, using the mechanism's actual sequence. |
| Catalyst effects correctly scoped | Student states that a catalyst changes $k$ (via lowering $E_a$) but never changes $\Delta H$ or the overall balanced equation. |
