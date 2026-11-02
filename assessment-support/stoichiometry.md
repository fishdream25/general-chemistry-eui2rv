{{nyml
kind: document
format: 1
title: Chapter 3 Assessment Guide: Stoichiometry
}}

# Chapter 3 Assessment Guide: Stoichiometry

## Source and Format

**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 3 (CC BY 4.0). **Audience:** introductory undergraduate general chemistry, first semester. **Note:** this is design guidance for building assessments — question *guides* an instructor or generator can instantiate into many concrete questions — not a finished question bank or answer key.

## General Assessment Priorities

- Treat mole conversions (mass ↔ moles ↔ particles) as the single most important recurring skill in the course — test it more than once, in more than one context, throughout the semester.
- Require every stoichiometric-conversion answer to show the full unit-factor-label chain (mirroring Chapter 1's dimensional analysis), not just a final number.
- For limiting-reagent questions, accept either Method 1 or Method 2 (per the study guide) as long as the reasoning is shown — don't penalize a correct answer reached by the "more calculations" method.
- Always carry full precision through multi-step calculations and round only at the end — the study guide's own excess-reagent example (7.24 mol × 44.01 g/mol) is a cautionary worked instantiation of what goes wrong otherwise.

## Objective 3.1a: Calculate average atomic mass and understand the mole concept

### Target understanding

A student can calculate a weighted-average atomic mass from isotope data, and can state what one mole represents (Avogadro's number of entities).

### Question guides

**1. Forward — calculate average atomic mass**
- Variables & ranges: two (or three) isotopes with given abundances and masses.
- Constraint: abundances must be used as decimal weights, summing to 1.
- Contexts: any element with 2-3 stable isotopes.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (copper, 63.55 amu).

**2. Inverse — infer relative abundance from average atomic mass**
- Variables & ranges: two isotope masses and the known average atomic mass.
- Constraint: student must reason about which isotope the average sits closer to.
- Contexts: boron, chlorine, or similar two-isotope elements.
- Formats: short-answer.
- Worked instantiation: "Boron's isotopes are B-10 (10.013 amu) and B-11 (11.009 amu); average atomic mass is 10.81 amu. Which isotope is more abundant?" → B-11, since 10.81 is closer to 11.009 than to 10.013.

**3. Conceptual — why atomic mass isn't a whole number**
- Variables & ranges: qualitative.
- Constraint: must reference both the isotope-weighting effect and the amu definition.
- Contexts: any element's periodic-table entry.
- Formats: short-answer.
- Worked instantiation: "Why is chlorine's atomic mass listed as 35.45, not a whole number?" → It's a weighted average of chlorine's naturally occurring isotopes (mainly Cl-35 and Cl-37), not the mass of any single atom.

**4. Error analysis**
- Variables & ranges: a student averages two isotope masses with equal (50/50) weighting instead of using actual abundances.
- Constraint: correction must show the abundance-weighted calculation.
- Contexts: any two-isotope element with unequal abundances.
- Formats: short-answer.
- Worked instantiation: "A student averages copper's isotope masses as $(62.93+64.9278)/2=63.93$. What's wrong?" → This ignores the actual abundances (69.09%/30.91%); a weighted average using those percentages gives 63.55 amu instead.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 average-atomic-mass calculations. |
| Group discussion | Understand | Discuss why isotope abundances are typically very stable/consistent in nature. |
| Quiz | Apply | One average-atomic-mass problem. |
| Exam | Analyze | Combine with Objective 3.1b (use the calculated molar mass in a mole conversion). |
| Project/activity | Understand | Students look up 3 elements' isotope data and verify the listed atomic mass. |

## Objective 3.1b: Convert between mass, moles, and number of particles

### Target understanding

A student can convert any one of mass, moles, or particle count into either of the other two, given a substance's molar mass.

### Question guides

**1. Forward — mass to particles**
- Variables & ranges: a mass of any element or compound.
- Constraint: must chain both conversions (mass→moles→particles) explicitly.
- Contexts: any element or compound.
- Formats: workout.
- Worked instantiation: see the practice sheet (3.22 g Mg → atoms).

**2. Inverse — particles or moles to mass**
- Variables & ranges: a mole or particle-count value.
- Constraint: correct direction of the molar-mass and Avogadro's-number factors.
- Contexts: any element or compound.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (0.356 mol Zn → grams).

**3. Conceptual — why moles are needed at all**
- Variables & ranges: qualitative.
- Constraint: must reference the impracticality of counting or weighing individual atoms directly.
- Contexts: any everyday-scale sample.
- Formats: short-answer.
- Worked instantiation: "Why do chemists use moles instead of just atom counts?" → Atom counts are impossibly large for lab-scale samples; the mole rescales that count to a lab-manageable quantity (grams) via molar mass.

**4. Error analysis**
- Variables & ranges: a student multiplies by Avogadro's number when converting mass to moles (instead of dividing by molar mass first).
- Constraint: correction must show the correct two-step chain.
- Contexts: any mass-to-particles conversion.
- Formats: short-answer.
- Worked instantiation: "A student multiplies grams directly by $N_A$ to find atom count. What step is missing?" → Grams must first be converted to moles (divide by molar mass); only then does multiplying by $N_A$ give the correct particle count.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 4–6 mixed-direction mole-conversion problems. |
| Group discussion | Understand | Discuss why Avogadro's number is defined relative to $\ce{^{12}C}$ specifically. |
| Quiz | Apply | One two-step conversion. |
| Exam | Apply | Combine with a stoichiometric conversion (Objective 3.2b) requiring a mole conversion as the first step. |
| Project/activity | Understand | Students estimate how many moles of water are in a typical glass, then convert to molecules. |

## Objective 3.1c: Calculate molecular mass, formula mass, and percent composition

### Target understanding

A student can calculate molecular or formula mass (choosing the correct term for molecular vs. ionic compounds) and can calculate the percent composition by mass of each element in a compound.

### Question guides

**1. Forward — calculate molar mass**
- Variables & ranges: one molecular and one ionic compound.
- Constraint: correct term ("molecular mass" vs. "formula mass") used for each.
- Contexts: any compound.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{CH4}$, $\ce{NaCl}$).

**2. Inverse — calculate percent composition**
- Variables & ranges: any compound with 2–3 elements.
- Constraint: percentages must sum to (approximately) 100%.
- Contexts: any compound.
- Formats: workout.
- Worked instantiation: "Find the percent composition of water, $\ce{H2O}$." → H: $2.016/18.015\times100\%=11.19\%$; O: $16.00/18.015\times100\%=88.81\%$ (or $100\%-11.19\%$).

**3. Conceptual — why formula mass, not molecular mass, for ionic compounds**
- Variables & ranges: qualitative.
- Constraint: must reference the absence of discrete molecules in an ionic lattice.
- Contexts: $\ce{NaCl}$ or similar.
- Formats: short-answer.
- Worked instantiation: see the study guide's caution (no "NaCl molecule" — an extended lattice, hence "formula mass," not "molecular mass").

**4. Error analysis**
- Variables & ranges: a student forgets to multiply an atomic mass by its subscript when computing molar mass.
- Constraint: correction must show the missing multiplication step.
- Contexts: any formula with a subscript > 1.
- Formats: short-answer.
- Worked instantiation: "A student computes $\ce{CH4}$'s molar mass as $12.01+1.008=13.02$. What's wrong?" → The 4 hydrogen atoms must each be counted: $12.01+4(1.008)=16.04$ g/mol, not just one hydrogen.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 molar-mass and 2–3 percent-composition problems. |
| Group discussion | Understand | Discuss why percent composition doesn't depend on sample size (ties back to Ch. 1's intensive properties). |
| Quiz | Apply | One molar-mass or percent-composition problem. |
| Exam | Analyze | Combine with Objective 3.1d (percent composition feeds into empirical-formula determination). |
| Project/activity | Apply | Students calculate the percent composition of a compound from a household product's listed formula. |

## Objective 3.1d: Determine an empirical formula from combustion-analysis data

### Target understanding

A student can convert combustion-analysis mass data (CO₂ and H₂O trapped) into moles of each element, find any remaining element by mass difference, and reduce to the empirical formula.

### Question guides

**1. Forward — full combustion-analysis problem**
- Variables & ranges: a sample mass and its CO₂/H₂O combustion products.
- Constraint: student must find O (or any third element) by mass difference, not by assuming a formula.
- Contexts: hydrocarbons and oxygen-containing organic compounds.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (ethanol).

**2. Inverse — determine composition percentages directly**
- Variables & ranges: element mass percentages are given directly (no combustion apparatus).
- Constraint: assume a 100 g sample to convert percentages directly to grams.
- Contexts: any multi-element compound.
- Formats: workout.
- Worked instantiation: see the practice sheet (thiol compound, C/H/S percentages).

**3. Conceptual — why divide by the smallest mole value**
- Variables & ranges: qualitative.
- Constraint: must reference finding the simplest whole-number ratio.
- Contexts: any empirical-formula calculation.
- Formats: short-answer.
- Worked instantiation: "Why do you divide every element's mole count by the smallest one?" → This rescales the smallest value to exactly 1, revealing the other elements' counts *relative* to it — the simplest whole-number ratio, which is what an empirical formula reports.

**4. Error analysis**
- Variables & ranges: a student assumes there's no third element (e.g., oxygen) just because it isn't directly trapped by the apparatus.
- Constraint: correction must show the mass-difference check.
- Contexts: any oxygen-containing organic compound.
- Formats: short-answer.
- Worked instantiation: "A student finds moles of C and H from combustion data and stops, assuming the formula is just $\ce{C_xH_y}$. What check is missing?" → Checking whether the masses of C and H alone account for the full original sample mass; if not, the difference is another element (commonly O) that combustion analysis doesn't trap directly.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 full combustion-analysis problems. |
| Group discussion | Analyze | Discuss why combustion analysis can't directly detect oxygen (or nitrogen, sulfur, etc. without additional traps). |
| Quiz | Apply | One combustion-analysis or percent-based empirical-formula problem. |
| Exam | Analyze | Combine with Objective 3.1c (percent composition as the starting point). |
| Project/activity | Evaluate | Students verify that a compound's stated empirical formula is consistent with its stated percent composition. |

## Objective 3.2a: Balance chemical equations

### Target understanding

A student can balance a chemical equation by adjusting only coefficients, using the "one reactant/one product first" strategy, and clearing any fractional coefficients.

### Question guides

**1. Forward — balance a straightforward equation**
- Variables & ranges: a combustion or synthesis reaction with 2–4 species.
- Constraint: only coefficients change; subscripts stay fixed.
- Contexts: hydrocarbon combustion, synthesis reactions.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{C2H6}$ combustion).

**2. Inverse — verify a proposed balanced equation**
- Variables & ranges: a given equation, possibly already balanced or with one wrong coefficient.
- Constraint: student must check every element's atom count on both sides.
- Contexts: any equation.
- Formats: short-answer.
- Worked instantiation: "Is $\ce{2H2 + O2 -> 2H2O}$ balanced? Show your check." → Yes: H: 4 = 4; O: 2 = 2.

**3. Conceptual — why subscripts can't change**
- Variables & ranges: qualitative.
- Constraint: must reference that changing a subscript changes the substance's identity.
- Contexts: any balancing exercise.
- Formats: short-answer.
- Worked instantiation: see the study guide's Reminder badge (changing $\ce{H2O}$ to $\ce{H2O2}$ changes the substance itself).

**4. Error analysis**
- Variables & ranges: a student changes a subscript to balance an equation instead of a coefficient.
- Constraint: correction must identify the specific incorrect edit.
- Contexts: any balancing exercise.
- Formats: short-answer.
- Worked instantiation: "A student 'balances' $\ce{H2 + O2 -> H2O}$ by changing the product to $\ce{H2O2}$. What's wrong?" → This changes hydrogen peroxide's formula into a completely different substance; the fix is a coefficient change ($\ce{2H2 + O2 -> 2H2O}$), not a subscript change.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 4–6 balancing problems of increasing complexity. |
| Group discussion | Understand | Discuss why the "balance elements appearing in only one place first" strategy usually converges fastest. |
| Quiz | Apply | One balancing problem. |
| Exam | Apply | Combine with Objective 3.2b (use the balanced equation immediately in a stoichiometric calculation). |
| Project/activity | Apply | Students balance all the combustion equations for a short list of common fuels. |

## Objective 3.2b: Convert between quantities of reactants and products using a balanced equation

### Target understanding

A student can use a balanced equation's mole ratio to convert a given mass (or moles) of one substance into the mass (or moles) of any other substance in the reaction.

### Question guides

**1. Forward — mass of reactant to mass of product**
- Variables & ranges: a balanced equation and a given reactant mass.
- Constraint: full four-step chain (mass→moles→mole ratio→mass) shown explicitly.
- Contexts: combustion or synthesis reactions.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (glucose combustion → CO₂).

**2. Inverse — mass of product to mass of reactant**
- Variables & ranges: a given product mass, reactant mass requested.
- Constraint: same four-step chain, applied in reverse.
- Contexts: any reaction with the direction reversed from the forward guide.
- Formats: workout.
- Worked instantiation: "How much $\ce{C6H12O6}$ must be combusted to produce 500 g of $\ce{CO2}$?" (reverse of the study guide's glucose example).

**3. Conceptual — why moles, not grams, convert directly**
- Variables & ranges: qualitative.
- Constraint: must reference that a balanced equation's coefficients are mole (particle) ratios, not mass ratios.
- Contexts: any balanced equation with unequal reactant/product molar masses.
- Formats: short-answer.
- Worked instantiation: see the study guide's Mg/O₂/MgO caution (2 g Mg + 1 g O₂ does NOT give 2 g MgO).

**4. Error analysis**
- Variables & ranges: a student tries to convert directly from grams of reactant to grams of product without passing through moles.
- Constraint: correction must insert the missing mole-conversion steps.
- Contexts: any stoichiometric conversion.
- Formats: short-answer.
- Worked instantiation: "A student writes $\text{grams product}=\text{grams reactant}\times\frac{\text{coefficient product}}{\text{coefficient reactant}}$. What's missing?" → The equation's coefficients are mole ratios, not mass ratios; grams must first be converted to moles, the mole ratio applied, and the result converted back to grams of the target substance.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 4–6 reactant-to-product conversion problems. |
| Group discussion | Analyze | Debate why the "2 g + 1 g → 2 g" reading of a balanced equation is wrong, using real molar masses. |
| Quiz | Apply | One reactant-to-product conversion. |
| Exam | Analyze | Combine with Objective 3.2c (this conversion is step 1 of a limiting-reagent problem). |
| Project/activity | Apply | Students calculate the mass of product from a reaction relevant to a real industrial or biological process. |

## Objective 3.2c: Determine the limiting reagent

### Target understanding

A student can determine which reactant limits a reaction using either the "least product produced" method or the "moles ÷ coefficient" method, and can identify the amount of excess reagent remaining.

### Question guides

**1. Forward — identify the limiting reagent**
- Variables & ranges: two reactant masses and a balanced equation.
- Constraint: student picks and correctly applies one of the two methods.
- Contexts: any two-reactant reaction.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (NH₃ + CO₂ → urea).

**2. Inverse — calculate excess reagent remaining**
- Variables & ranges: the same reaction, after the limiting reagent is identified.
- Constraint: student must subtract the amount of excess reagent *consumed* from the amount *available*.
- Contexts: any two-reactant reaction.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (CO₂ remaining, 319 g).

**3. Conceptual — why "more reactant mass" doesn't mean "not limiting"**
- Variables & ranges: qualitative, contrasting mass with moles÷coefficient.
- Constraint: must reference that the *required ratio*, not raw mass, determines which reactant runs out.
- Contexts: any reaction where the reactant with greater mass is nonetheless limiting.
- Formats: short-answer.
- Worked instantiation: "In the urea reaction, 637.2 g NH₃ is used vs. 1142 g CO₂ — yet NH₃ is limiting even though its mass is less. Could a reactant with the *larger* mass ever be limiting instead? Explain." → Yes — mass alone doesn't determine limiting status; it depends on moles available relative to the stoichiometric ratio required, which can go either way regardless of which reactant has more raw mass.

**4. Error analysis**
- Variables & ranges: a student picks the limiting reagent by comparing raw reactant masses instead of mol÷coefficient values.
- Constraint: correction must show the proper method.
- Contexts: any two-reactant reaction.
- Formats: short-answer.
- Worked instantiation: "A student says CO₂ must be limiting since less of it (1142 g) was... " (continued: actually NH₃ has less mass but isn't necessarily limiting on mass alone) → Limiting reagent is never determined by comparing raw masses directly; it requires converting to moles and dividing by each reactant's coefficient.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 limiting-reagent problems using both methods across different problems. |
| Group discussion | Analyze | Debate a scenario where the reactant with more mass is nonetheless limiting. |
| Quiz | Apply | One limiting-reagent identification. |
| Exam | Analyze | Combine with Objective 3.2d (limiting reagent feeds directly into theoretical yield). |
| Project/activity | Evaluate | Students design a two-reactant scenario where their initial mass guess for "limiting" turns out wrong, then recompute correctly. |

## Objective 3.2d: Calculate theoretical yield and percent yield

### Target understanding

A student can calculate theoretical yield from the limiting reagent and can calculate percent yield given an actual yield.

### Question guides

**1. Forward — calculate theoretical yield**
- Variables & ranges: a limiting reagent's mass and a balanced equation.
- Constraint: full mole-ratio chain from limiting reagent to product.
- Contexts: any reaction with an identified limiting reagent.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (1124 g $\ce{(NH2)2CO}$).

**2. Inverse — calculate percent yield**
- Variables & ranges: a theoretical yield and an actual yield.
- Constraint: correct ratio direction (actual ÷ theoretical, not the reverse).
- Contexts: any reaction with both yields given.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (89.5%).

**3. Conceptual — why percent yield is virtually always ≤ 100%**
- Variables & ranges: qualitative.
- Constraint: must reference real-world losses (side reactions, incomplete reactions, purification losses).
- Contexts: any real laboratory-scale reaction.
- Formats: short-answer.
- Worked instantiation: "Why is percent yield almost always below 100%, even for a well-run reaction?" → Real reactions rarely go to 100% completion, side reactions can consume some reactant, and physical transfer/purification steps lose some product — theoretical yield assumes none of this loss occurs.

**4. Error analysis**
- Variables & ranges: a student computes theoretical yield using the excess reagent's mass instead of the limiting reagent's.
- Constraint: correction must identify the limiting reagent first.
- Contexts: any two-reactant reaction.
- Formats: short-answer.
- Worked instantiation: "A student calculates theoretical yield starting from the CO₂ mass, in a reaction where NH₃ is limiting. What's wrong?" → Theoretical yield must be calculated from the *limiting* reagent (NH₃ here); starting from the excess reagent (CO₂) overstates the theoretical yield, since not all of the CO₂ can actually react.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 theoretical-yield and percent-yield problems. |
| Group discussion | Understand | Discuss real-world reasons an industrial process might report yields well below 100%. |
| Quiz | Apply | One percent-yield calculation given theoretical and actual yields. |
| Exam | Analyze | Combine all of Objectives 3.2a-d into one full multi-part limiting-reagent/yield problem (see the study guide's and practice sheet's multi-part examples). |
| Project/activity | Evaluate | Students research a real industrial reaction's typical percent yield and discuss why it falls short of 100%. |

## Rubric Themes for Chapter 3

- **Show the full mole-conversion chain.** A correct final numeric answer without the intermediate mass→mole→mole→mass steps shown does not receive full credit — this chain is the single most important habit in the chapter.
- **Never adjust a subscript to balance an equation.** This is treated as a conceptual error, not a minor slip, since it changes chemical identity.
- **Limiting reagent must be justified by moles ÷ coefficient (or equivalent), not by comparing raw masses.** A correct answer reached by comparing masses directly should be flagged for the wrong reasoning even if the identified reagent happens to be right.
- **Carry full precision until the final rounding step.** Multi-step yield/excess-reagent problems are graded on whether intermediate values were rounded prematurely, per the study guide's own 314-vs-319 g caution.
