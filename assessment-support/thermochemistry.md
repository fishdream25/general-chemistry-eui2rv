{{nyml
kind: document
format: 1
title: Chapter 6 Assessment Guide: Energy Relationships in Chemical Reactions
}}

# Chapter 6 Assessment Guide: Energy Relationships in Chemical Reactions

## Source and Format

**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 6 (CC BY 4.0). **Audience:** introductory undergraduate general chemistry, first semester. **Note:** this is design guidance for building assessments — question *guides* an instructor or generator can instantiate into many concrete questions — not a finished question bank or answer key.

## General Assessment Priorities

- Enforce sign conventions rigorously: heat absorbed/work done on the system is positive; heat released/work done by the system is negative. Require students to state which convention they're using before substituting numbers.
- Require every calorimetry answer to identify explicitly which is the "reaction" and which is the "surroundings" (water/calorimeter) before writing the $q_{rxn}=-(q_{surroundings})$ relationship.
- Pair Hess's Law problems with a standard-formation-enthalpy problem on the same or a related reaction, since both are two routes to the same kind of answer.
- Never let a $\Delta H$ sign error pass unflagged — losing track of a negative sign (as in the chapter's own FeCl₃ example) is the most consequential and common error type in this chapter.

## Objective 6.1a: Distinguish types of energy, types of systems, and exothermic/endothermic processes

### Target understanding

A student can classify a described scenario as an open, closed, or isolated system, and can classify a process as exothermic or endothermic based on the direction of heat flow.

### Question guides

**1. Forward — classify a system**
- Variables & ranges: a described physical setup (an open beaker, a sealed insulated thermos, a sealed but conducting container).
- Constraint: must justify based on mass AND energy exchange, not just one.
- Contexts: common lab and household setups.
- Formats: multiple-choice.
- Worked instantiation: "A sealed, perfectly insulated thermos is an example of what kind of system?" → an isolated system (no mass or energy exchange).

**2. Inverse — classify a process as exo/endothermic**
- Variables & ranges: a described reaction or phase change.
- Constraint: must reference heat flow direction, not just "gets hot" or "gets cold" colloquially.
- Contexts: combustion, melting, dissolving, freezing.
- Formats: multiple-choice.
- Worked instantiation: see the practice sheet (identifying the exothermic process among several phase-change/reaction options).

**3. Conceptual — why melting is endothermic**
- Variables & ranges: qualitative.
- Constraint: must reference heat absorbed to overcome intermolecular forces, not "getting colder."
- Contexts: ice melting or a similar phase change.
- Formats: short-answer.
- Worked instantiation: "Why is melting ice endothermic, even though the ice itself doesn't feel like it's absorbing anything dramatic?" → Melting requires energy to overcome the intermolecular forces holding the solid's ordered structure together; this energy comes from the surroundings, which is exactly what "endothermic" means.

**4. Error analysis**
- Variables & ranges: a student assumes "exothermic" means "the system feels cold."
- Constraint: correction must clarify the direction of heat flow (system → surroundings), not surface temperature intuition.
- Contexts: any exothermic reaction.
- Formats: short-answer.
- Worked instantiation: "A student thinks exothermic reactions make the surroundings feel cold. What's wrong?" → Exothermic means the system releases heat to the surroundings, which would make the surroundings feel *warmer*, not colder.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | 4–6 system-classification and exo/endo-classification items. |
| Group discussion | Understand | Discuss why a "closed system" is the most common approximation used in lab-scale chemistry. |
| Quiz | Understand | One classification item of each kind. |
| Exam | Analyze | Combine with Objective 6.1b (exothermic/endothermic feeds into the sign of $q$). |
| Project/activity | Understand | Students classify 5 real-world processes (a car engine, a refrigerator, photosynthesis, etc.) as systems and by heat-flow direction. |

## Objective 6.1b: Apply the first law of thermodynamics

### Target understanding

A student can apply $\Delta U=q+w$ with the correct sign convention for heat and work, including the special case $w=-P\Delta V$ for gas expansion/compression.

### Question guides

**1. Forward — calculate ΔU from q and w**
- Variables & ranges: given heat and work values with stated directions (absorbed/released, done on/by).
- Constraint: correct sign assignment before substitution.
- Contexts: any closed-system process.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (gas compression, 679 J work, 185 J heat released).

**2. Inverse — find q or w given ΔU and the other**
- Variables & ranges: given ΔU and either q or w.
- Constraint: correct algebraic rearrangement.
- Contexts: any closed-system process.
- Formats: workout.
- Worked instantiation: "A system's internal energy increases by 300 J while it absorbs 500 J of heat. How much work was done, and in which direction?" → $w=\Delta U-q=300-500=-200$ J; negative work means the system did 200 J of work *on* the surroundings.

**3. Conceptual — why work done on a gas is positive**
- Variables & ranges: qualitative, contrasting compression and expansion.
- Constraint: must connect the sign convention to energy actually entering vs. leaving the system.
- Contexts: gas compression vs. expansion.
- Formats: short-answer.
- Worked instantiation: "Why is $w$ positive when a gas is compressed, but $w=-P\Delta V$ is negative when a gas expands ($\Delta V>0$)?" → Compression means the surroundings do work *on* the system (energy enters, positive by convention); expansion means the system does work *on* the surroundings (energy leaves, so $w$ is negative when $\Delta V$ is positive).

**4. Error analysis**
- Variables & ranges: a student adds q and w without first assigning correct signs based on direction.
- Constraint: correction must show the sign assignment step explicitly.
- Contexts: any first-law problem.
- Formats: short-answer.
- Worked instantiation: "A student computes $\Delta U=185+679=864$ J for the study guide's compression example. What's wrong?" → The 185 J of heat is *released* (to the surroundings), so it must be entered as $q=-185$ J, not $+185$ J; the correct calculation is $\Delta U=-185+679=494$ J.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 4–6 first-law problems with varied sign scenarios. |
| Group discussion | Understand | Discuss why $\Delta U$, but not $q$ or $w$ individually, is a state function. |
| Quiz | Apply | One first-law calculation. |
| Exam | Apply | Combine with Objective 6.2b (first law feeds into the ΔH-ΔU relationship). |
| Project/activity | Understand | Students diagram the sign convention for all four combinations of heat/work direction. |

## Objective 6.2a: Define enthalpy and apply thermochemical-equation rules

### Target understanding

A student can state the relationship between $\Delta H$'s sign and exothermic/endothermic classification, and can correctly scale or reverse a thermochemical equation's $\Delta H$.

### Question guides

**1. Forward — calculate heat from a scaled thermochemical equation**
- Variables & ranges: a thermochemical equation and a given mass of one reactant.
- Constraint: correct division by the equation's stated coefficient.
- Contexts: any thermochemical equation.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{SO2}$/$\ce{SO3}$, 87.9 g → −136 kJ).

**2. Inverse — reverse or scale an equation's ΔH**
- Variables & ranges: a given $\Delta H$ for a forward reaction; find $\Delta H$ for the reverse or a scaled version.
- Constraint: correct sign flip (reverse) or scaling factor (multiply/divide).
- Contexts: any thermochemical equation.
- Formats: short-answer.
- Worked instantiation: see the practice sheet ($\ce{2Al2O3->4Al+3O2}$ reversed and doubled from the formation reaction).

**3. Conceptual — why physical states must be specified**
- Variables & ranges: qualitative, contrasting $\ce{H2O(l)}$ and $\ce{H2O(g)}$ in the same reaction.
- Constraint: must reference that different phases have different enthalpies.
- Contexts: any reaction involving water or another substance with multiple relevant phases.
- Formats: short-answer.
- Worked instantiation: "Why does a thermochemical equation need to specify (l) vs. (g) for water?" → Liquid and gaseous water have different enthalpies (differing by the enthalpy of vaporization); using the wrong phase would give an incorrect $\Delta H$ for the reaction.

**4. Error analysis**
- Variables & ranges: a student forgets to flip the sign of $\Delta H$ when reversing a reaction.
- Constraint: correction must restate the sign-flip rule.
- Contexts: any reversed thermochemical equation.
- Formats: short-answer.
- Worked instantiation: "A student says the reverse of an exothermic reaction is still exothermic. What's wrong?" → Reversing a reaction flips the sign of $\Delta H$; an exothermic forward reaction ($\Delta H<0$) becomes endothermic in reverse ($\Delta H>0$), since energy that was released must now be supplied to run the reaction backward.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 thermochemical-equation scaling/reversing problems. |
| Group discussion | Understand | Discuss why bond-breaking (endothermic) and bond-forming (exothermic) together determine a reaction's overall sign. |
| Quiz | Apply | One thermochemical-equation-scaling problem. |
| Exam | Analyze | Combine with Objective 6.4a/6.4b (thermochemical-equation manipulation is exactly what Hess's Law problems require). |
| Project/activity | Apply | Students find the heat released/absorbed for a real reaction scaled to an industrially relevant quantity. |

## Objective 6.2b: Convert between ΔH and ΔU for a reaction

### Target understanding

A student can convert between $\Delta H$ and $\Delta U$ for a gas-phase reaction using $\Delta U=\Delta H-\Delta nRT$, correctly computing $\Delta n$ as moles of gaseous products minus moles of gaseous reactants.

### Question guides

**1. Forward — calculate ΔU from ΔH**
- Variables & ranges: a balanced equation with a mole-of-gas change, its $\Delta H$, and a temperature.
- Constraint: correct $\Delta n$ (gas only — ignore solids/liquids/aqueous species).
- Contexts: any reaction with $\Delta n_{gas}\ne0$.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{CO}$/$\ce{O2}$/$\ce{CO2}$, $\Delta n=-1$).

**2. Inverse — calculate ΔH from ΔU**
- Variables & ranges: given $\Delta U$, $\Delta n$, and temperature.
- Constraint: correct algebraic rearrangement.
- Contexts: any gas-phase reaction.
- Formats: workout.
- Worked instantiation: "A reaction has $\Delta U=-400.0$ kJ at 300 K with $\Delta n=+2$. Find $\Delta H$." → $\Delta H=\Delta U+\Delta nRT=-400.0+2(8.314\times10^{-3})(300)=-395.0$ kJ.

**3. Conceptual — why ΔH and ΔU are nearly equal for reactions without gas-mole change**
- Variables & ranges: qualitative, contrasting a $\Delta n=0$ reaction with one where $\Delta n\ne0$.
- Constraint: must reference the $\Delta nRT$ term vanishing when $\Delta n=0$.
- Contexts: a reaction with equal moles of gas on both sides.
- Formats: short-answer.
- Worked instantiation: "Why would $\Delta H\approx\Delta U$ for a reaction where the number of moles of gas doesn't change?" → The $\Delta nRT$ correction term is zero when $\Delta n=0$, so $\Delta U=\Delta H-0=\Delta H$ exactly (for gas-phase reactions; solids/liquids contribute negligible $P\Delta V$ regardless).

**4. Error analysis**
- Variables & ranges: a student includes solid or aqueous species when computing $\Delta n$.
- Constraint: correction must restate that only gas-phase species count.
- Contexts: any reaction with a mix of phases.
- Formats: short-answer.
- Worked instantiation: "A student computes $\Delta n$ for $\ce{2CO(g)+O2(g)->2CO2(g)}$ using solid or aqueous species elsewhere in a multi-part problem. What's the rule?" → Only *gas-phase* species contribute to $\Delta n$ in the $\Delta U=\Delta H-\Delta nRT$ relationship, since solids and liquids have negligible volume change compared to gases.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 ΔH-to-ΔU conversion problems. |
| Group discussion | Understand | Discuss why this correction is usually small in magnitude compared to ΔH itself. |
| Quiz | Apply | One ΔH-ΔU conversion. |
| Exam | Analyze | Combine with Objective 6.1b (both use the same first-law framework). |
| Project/activity | Apply | Students find 3 reactions with different $\Delta n$ signs and compare the size of the correction term. |

## Objective 6.3a: Apply specific heat and heat capacity

### Target understanding

A student can apply $q=ms\Delta T$ to relate heat, mass, specific heat, and temperature change, including problems where two objects exchange heat with each other.

### Question guides

**1. Forward — calculate heat for a temperature change**
- Variables & ranges: mass, specific heat, and a temperature change.
- Constraint: correct sign of $\Delta T$ (final − initial).
- Contexts: heating or cooling any single substance.
- Formats: workout.
- Worked instantiation: see the practice sheet (heating 2500 g water).

**2. Inverse — two objects exchanging heat (find an unknown initial temperature)**
- Variables & ranges: two substances reaching a common final temperature, one's initial temperature unknown.
- Constraint: correctly set heat lost by one equal to heat gained by the other (opposite signs).
- Contexts: a hot solid dropped into water, or similar.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (rebar dropped into water, find $T_{i,rebar}$).

**3. Conceptual — why heat capacity, not specific heat, is used for calorimeter parts**
- Variables & ranges: qualitative.
- Constraint: must reference that a calorimeter's mass-specific-heat product varies by design, and is often characterized as a single lumped constant instead.
- Contexts: a bomb or coffee-cup calorimeter.
- Formats: short-answer.
- Worked instantiation: "Why is a calorimeter's own contribution to heat absorption expressed as a heat capacity (J/°C) rather than a specific heat (J/(g·°C))?" → The calorimeter itself is a complex, fixed assembly of parts (not a simple, uniform substance), so it's more practical to characterize its overall heat capacity as a single measured constant rather than track a specific heat and mass for each component.

**4. Error analysis**
- Variables & ranges: a student sets up the heat-exchange equation with both sides having the same sign.
- Constraint: correction must show the required sign difference (heat lost = negative of heat gained).
- Contexts: any two-object heat-exchange problem.
- Formats: short-answer.
- Worked instantiation: "A student writes $q_\text{rebar}=q_\text{water}$ (both positive) for the rebar-in-water problem. What's wrong?" → The rebar *loses* heat while the water *gains* it — these must have opposite signs: $q_\text{rebar}=-q_\text{water}$, not equal positive values.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 specific-heat problems, including at least one two-object exchange. |
| Group discussion | Understand | Discuss why water's unusually high specific heat matters for climate and cooking. |
| Quiz | Apply | One specific-heat calculation. |
| Exam | Apply | Combine with Objective 6.3b (specific heat feeds directly into calorimetry calculations). |
| Project/activity | Apply | Students measure (or research) the specific heat of an everyday material and use it to predict a temperature change. |

## Objective 6.3b: Use constant-volume and constant-pressure calorimetry

### Target understanding

A student can calculate $\Delta U_{rxn}$ from bomb-calorimetry data (accounting for both water and the bomb's own heat capacity) and $\Delta H_{rxn}$ from constant-pressure calorimetry data.

### Question guides

**1. Forward — bomb calorimetry**
- Variables & ranges: sample mass, water mass, bomb heat capacity, temperature change.
- Constraint: both the water term and the bomb term must be included.
- Contexts: any combustion sample burned in a bomb calorimeter.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (glucose combustion, −48.8 kJ).

**2. Inverse — constant-pressure (coffee-cup) calorimetry**
- Variables & ranges: two solution volumes/masses at a common initial temperature, a final temperature.
- Constraint: correct total mass (sum of both solutions) and specific heat assumption.
- Contexts: any neutralization or dissolution reaction in a coffee-cup calorimeter.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (HCl + NaOH neutralization, 2.89×10³ J).

**3. Conceptual — why bomb calorimetry gives ΔU, not ΔH**
- Variables & ranges: qualitative.
- Constraint: must reference the constant-volume condition (no $P\Delta V$ work possible).
- Contexts: the bomb calorimeter's sealed, rigid design.
- Formats: short-answer.
- Worked instantiation: "Why does a bomb calorimeter measure $\Delta U_{rxn}$ rather than $\Delta H_{rxn}$?" → The bomb is a sealed, rigid (constant-volume) container, so no $P\Delta V$ work is possible; by the first law, all the energy change shows up as heat at constant volume, which is exactly the definition of $\Delta U$.

**4. Error analysis**
- Variables & ranges: a student omits the bomb's own heat capacity term in a bomb-calorimetry calculation.
- Constraint: correction must show the missing term.
- Contexts: any bomb-calorimetry problem.
- Formats: short-answer.
- Worked instantiation: "A student computes $q_{rxn}=-q_{water}$ only, ignoring the bomb's heat capacity. What's missing?" → The bomb itself also absorbs heat and warms up; the full relationship is $q_{rxn}=-(q_{water}+q_{bomb})$, and omitting $q_{bomb}$ underestimates the magnitude of the heat released.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 bomb-calorimetry and 2–3 constant-pressure-calorimetry problems. |
| Group discussion | Analyze | Discuss why constant-pressure (coffee-cup) calorimetry is common for classroom labs despite being less precise than a bomb calorimeter. |
| Quiz | Apply | One calorimetry calculation of either type. |
| Exam | Analyze | Combine with Objective 6.2b (the calorimetry result, $\Delta U$ or $\Delta H$, connects back to the ΔH-ΔU relationship). |
| Project/activity | Evaluate | Students design a coffee-cup calorimetry experiment for a reaction of their choosing and predict expected heat output. |

## Objective 6.4a: Apply Hess's Law

### Target understanding

A student can combine two or more thermochemical equations (scaling and/or reversing as needed) to find the enthalpy of a target reaction, correctly tracking the sign through each manipulation.

### Question guides

**1. Forward — combine two given reactions**
- Variables & ranges: two reactions that sum (possibly after scaling) to a target reaction.
- Constraint: student must show the scaling/reversing applied to each given reaction before summing.
- Contexts: any multi-step synthesis pathway.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (FeCl₃ formation from a 2-step path).

**2. Inverse — determine what scaling/reversing was needed**
- Variables & ranges: a target reaction and two given reactions; ask which manipulation converts each given reaction into a piece of the target.
- Constraint: student must state the specific factor and/or reversal for each given reaction.
- Contexts: any Hess's-Law scenario.
- Formats: short-answer.
- Worked instantiation: "To get from the given reaction $\ce{2FeCl2+Cl2->2FeCl3}$ to the target's needed piece $\ce{FeCl2+\frac12Cl2->FeCl3}$, what manipulation is needed?" → Divide the entire given reaction (and its $\Delta H$) by 2.

**3. Conceptual — why Hess's Law works (state-function argument)**
- Variables & ranges: qualitative.
- Constraint: must invoke enthalpy as a state function.
- Contexts: any multi-step reaction pathway.
- Formats: short-answer.
- Worked instantiation: "Why can you add two reactions' $\Delta H$ values to get a third reaction's $\Delta H$, regardless of the actual mechanism?" → Enthalpy is a state function — it depends only on initial and final states, not the path taken — so any valid path (real or hypothetical) connecting the same start and end states gives the same total $\Delta H$.

**4. Error analysis**
- Variables & ranges: a student forgets to scale $\Delta H$ by the same factor used to scale the reaction.
- Constraint: correction must show the matching scale factor applied to $\Delta H$.
- Contexts: any Hess's-Law problem requiring a fractional or multiplied reaction.
- Formats: short-answer.
- Worked instantiation: "A student halves a reaction's coefficients but keeps its original $\Delta H$ unchanged. What's wrong?" → $\Delta H$ must be scaled by the same factor as the reaction's coefficients — halving the reaction requires halving $\Delta H$ as well, since $\Delta H$ is an extensive quantity tied to the stated amounts.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 Hess's-Law combination problems. |
| Group discussion | Analyze | Work through a 3-reaction Hess's-Law cycle as a group, tracking each sign/scale step. |
| Quiz | Apply | One 2-reaction Hess's-Law combination. |
| Exam | Analyze | Combine with Objective 6.4b (Hess's Law and standard-formation-enthalpy methods should give the same answer for the same reaction — an excellent exam cross-check). |
| Project/activity | Evaluate | Students find a real multi-step industrial synthesis and verify Hess's Law using published enthalpy data for each step. |

## Objective 6.4b: Calculate reaction enthalpy from standard enthalpies of formation

### Target understanding

A student can apply $\Delta H_\text{rxn}^\circ=\sum n\Delta H_\text{f}^\circ(\text{products})-\sum m\Delta H_\text{f}^\circ(\text{reactants})$, correctly using zero for elements in their standard state, and can then scale the result to a given mass of reactant.

### Question guides

**1. Forward — calculate ΔH°rxn from formation data**
- Variables & ranges: a balanced equation and formation enthalpies for each species.
- Constraint: elements in standard state correctly assigned $\Delta H_\text{f}^\circ=0$.
- Contexts: any reaction with tabulated formation enthalpies.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (Al/Fe₂O₃ thermite reaction, part a).

**2. Inverse — scale the result to a given mass**
- Variables & ranges: a calculated $\Delta H_\text{rxn}^\circ$ and a given mass of one reactant.
- Constraint: correct mole conversion, then correct division by the reactant's stoichiometric coefficient.
- Contexts: the same reaction as the forward guide, extended.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (part b, 35.0 g Al → −534 kJ).

**3. Conceptual — why "products minus reactants," not the reverse**
- Variables & ranges: qualitative.
- Constraint: must connect the formula's order to the definition of a state-function difference (final minus initial).
- Contexts: any reaction.
- Formats: short-answer.
- Worked instantiation: "Why is the formula 'products minus reactants,' and not 'reactants minus products'?" → $\Delta H_\text{rxn}^\circ$ represents the change going from reactants (initial state) to products (final state) — like any state-function change, it's calculated as (final) − (initial), i.e., products minus reactants.

**4. Error analysis**
- Variables & ranges: a student assigns a nonzero formation enthalpy to a free element.
- Constraint: correction must state the standard-state-element rule.
- Contexts: any reaction with an elemental reactant or product.
- Formats: short-answer.
- Worked instantiation: "A student looks up a nonzero $\Delta H_\text{f}^\circ$ value for solid Fe and uses it in a calculation where Fe is the standard-state element. What's wrong?" → An element in its standard (most stable) state always has $\Delta H_\text{f}^\circ=0$ by definition; a nonzero looked-up value would apply to a different form/phase/allotrope of that element, not the standard-state reference.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 4–6 standard-formation-enthalpy problems, including at least one mass-scaling extension. |
| Group discussion | Understand | Discuss why standard enthalpies of formation are tabulated once and reused across countless reaction calculations. |
| Quiz | Apply | One standard-formation-enthalpy calculation. |
| Exam | Analyze | Combine with Objective 6.4a (cross-check a Hess's-Law answer against a standard-formation-enthalpy calculation for the same reaction). |
| Project/activity | Apply | Students calculate the reaction enthalpy for a real combustion or synthesis reaction using a published table of formation enthalpies. |

## Rubric Themes for Chapter 6

- **Sign conventions are non-negotiable.** A numerically correct magnitude with an incorrect sign is treated as a wrong answer, not a rounding-level deduction — signs carry real physical meaning (direction of heat/energy flow) in this chapter.
- **State explicitly what is system vs. surroundings before writing a calorimetry equation.** This is required scaffolding, not optional context.
- **Hess's Law and standard-formation-enthalpy answers must show every scaling/reversing step**, not just a final combined number.
- **Always double-check a final $\Delta H$'s sign against the reaction's expected exothermic/endothermic direction** — the chapter's own FeCl₃ worked example is a cautionary case where a dropped negative sign would otherwise slip through unnoticed.
