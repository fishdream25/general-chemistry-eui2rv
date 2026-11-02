{{nyml
kind: document
format: 1
title: Chapter 16 Assessment Guide: Acid-Base Equilibria and Solubility Equilibria
}}

# Chapter 16 Assessment Guide: Acid-Base Equilibria and Solubility Equilibria

## Source and Format

**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 16 (CC BY 4.0). **Audience:** introductory undergraduate general chemistry, second semester. **Note:** this is design guidance for building assessments — question *guides* an instructor or generator can instantiate into many concrete questions — not a finished question bank or answer key.

## General Assessment Priorities

- Require students to **classify which of the three titration regions** (before, at, or after equivalence) a given point falls into *before* selecting a calculation method — never let them default to one method for an entire curve.
- Test the assumption that **every equivalence point is pH 7** directly and repeatedly — this is the single most common misconception carried over from introductory coverage of neutralization.
- Require the **Henderson-Hasselbalch "x is small" precondition** to be stated explicitly at least once, so it's understood as a shortcut valid under specific conditions, not a universally different method from the ICE table.
- Pair every $K_{sp}$-from-solubility question with a stoichiometry check (writing out the dissolution equation and its coefficients *before* squaring or cubing any concentration).

## Objective 16.1a: Explain buffer action and calculate buffer pH

### Target understanding

A student can explain why a buffer resists pH change (both conjugate species present, each able to consume one type of added stress) and can calculate buffer pH using either a full ICE table or the Henderson-Hasselbalch equation, recognizing when the two methods agree.

### Question guides

**1. Conceptual — why buffers resist pH change**
- Variables & ranges: any weak acid/conjugate base buffer pair.
- Constraint: explanation must name both reactions (acid + added base; base + added acid).
- Contexts: any common buffer system.
- Formats: short-answer.
- Worked instantiation: "Explain why a mixture of $\ce{CH3COOH}$ and $\ce{CH3COONa}$ resists pH change when a small amount of strong acid is added." → The $\ce{CH3COO-}$ present reacts with the added $\ce{H+}$ ($\ce{CH3COO- + H+ -> CH3COOH}$), consuming most of the stress before it can change $[\ce{H+}]$ much; if the buffer weren't present, that same added acid would change pH dramatically.

**2. Forward — buffer pH via ICE table**
- Variables & ranges: equal or unequal initial concentrations of a weak acid and its conjugate base, given $K_a$.
- Constraint: correct ICE table with the conjugate base's initial concentration in the "Equilibrium" row alongside the acid's.
- Contexts: any monoprotic weak acid/conjugate base pair.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (1.0 M $\ce{CH3COOH}$/1.0 M $\ce{CH3COONa}$, pH = 4.74).

**3. Forward — buffer pH via Henderson-Hasselbalch**
- Variables & ranges: same scenario as above.
- Constraint: student must recognize this gives the identical answer to the ICE table, faster.
- Contexts: same buffer systems.
- Formats: workout.
- Worked instantiation: redo the above using $\ce{pH}=\ce{p}K_a+\log([\text{base}]/[\text{acid}])$.

**4. Error analysis**
- Variables & ranges: a student who uses Henderson-Hasselbalch with initial (not equilibrium) concentrations without checking that the approximation is valid.
- Constraint: correction must state the "x is small relative to both concentrations" precondition.
- Contexts: any buffer scenario, especially with very dilute buffer components.
- Formats: short-answer.
- Worked instantiation: "A student applies Henderson-Hasselbalch to a buffer where the acid and conjugate base concentrations are both only $1\times10^{-6}$ M, with $K_a=1\times10^{-5}$. Why might this be inaccurate?" → Henderson-Hasselbalch assumes the amount ionized ($x$) is negligible compared to the initial concentrations; when the concentrations are this low relative to $K_a$, that assumption can fail, and a full ICE table (or a check of the assumption) is needed.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 buffer-pH calculations, both by ICE table and Henderson-Hasselbalch. |
| Group discussion | Understand | Discuss why a buffer needs *comparable* amounts of acid and conjugate base, not just any amount of each. |
| Quiz | Apply | One buffer-pH item, either method. |
| Exam | Analyze | Require both methods on the same buffer to show they agree. |
| Project/activity | Evaluate | Research a real biological buffer (e.g., blood's bicarbonate buffer) and its operating pH range. |

## Objective 16.1b: Calculate buffer pH after a stress, and design a buffer at a target pH

### Target understanding

A student can find the new pH after adding a small amount of strong acid or base to a buffer (updating the acid/conjugate-base amounts first), and can choose an appropriate weak acid/conjugate base pair and ratio to achieve a specific target pH.

### Question guides

**1. Forward — pH after adding strong acid**
- Variables & ranges: a buffer, plus a given amount of strong acid added.
- Constraint: student must first update the acid/base amounts (stoichiometric neutralization) before applying Henderson-Hasselbalch.
- Contexts: any buffer with a modest acid addition (not enough to exhaust either component).
- Formats: workout.
- Worked instantiation: see the study guide's worked example (1.0 M/1.0 M acetate buffer + 0.10 mol HCl, pH 4.74 → 4.65).

**2. Inverse — design a buffer at a target pH**
- Variables & ranges: a target pH, a weak base with known $K_b$, solve for the mass of conjugate acid salt needed.
- Constraint: correct use of $K_a=K_w/K_b$ before applying Henderson-Hasselbalch in reverse.
- Contexts: any weak base/conjugate acid buffer.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{NH3}$/$\ce{NH4Cl}$ at pH 9.30, 3.58 g needed).

**3. Conceptual — choosing the right acid**
- Variables & ranges: several weak acids with different $\ce{p}K_a$ values, a target pH.
- Constraint: selection justified by proximity of $\ce{p}K_a$ to the target pH.
- Contexts: any buffer-design scenario (e.g., a physiological pH target).
- Formats: short-answer/multiple-choice.
- Worked instantiation: "Which of these acids would best buffer at pH 7.4: one with $K_a=1.8\times10^{-5}$, or one with $K_a=3.2\times10^{-8}$?" → The one with $K_a=3.2\times10^{-8}$ ($\ce{p}K_a\approx7.5$), since its $\ce{p}K_a$ is much closer to 7.4.

**4. Error analysis**
- Variables & ranges: a student who forgets that added strong acid/base is a *stoichiometric* reaction before any equilibrium is considered.
- Constraint: correction must separate the neutralization step from the equilibrium (Henderson-Hasselbalch) step.
- Contexts: any buffer-plus-strong-acid/base scenario.
- Formats: short-answer.
- Worked instantiation: "A student plugs the original buffer concentrations directly into Henderson-Hasselbalch even after HCl has been added, without adjusting them first. What's the error?" → The added strong acid reacts essentially completely with the conjugate base before any new equilibrium is considered; the acid/base amounts must be updated (moles of conjugate base decrease, moles of acid increase by the same amount) before Henderson-Hasselbalch is applied to the *new* ratio.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2 "pH after adding acid/base" problems; 1 buffer-design problem. |
| Group discussion | Analyze | Debate why buffer capacity is limited — what happens if you add enough acid to exhaust the conjugate base entirely? |
| Quiz | Apply | One "pH after stress" item. |
| Exam | Analyze | Require a full buffer-design calculation, including mass/volume conversions. |
| Project/activity | Evaluate | Design a buffer recipe for a specific target pH using available lab chemicals and their $K_a$ values. |

## Objective 16.2a: Describe titration pH behavior by acid/base strength combination

### Target understanding

A student can state the equivalence-point pH for strong-strong (7), weak acid-strong base (>7), and strong acid-weak base (<7) titrations, and explain why each differs based on whether the product salt hydrolyzes.

### Question guides

**1. Conceptual — why equivalence isn't always pH 7**
- Variables & ranges: any titration type.
- Constraint: explanation must invoke salt hydrolysis (Chapter 15) as the reason equivalence-point pH varies.
- Contexts: strong-strong vs. weak-strong vs. strong-weak.
- Formats: short-answer.
- Worked instantiation: "Why is the equivalence point of an acetic acid/NaOH titration above pH 7, while HCl/NaOH's is exactly 7?" → At equivalence, acetic acid/NaOH produces a solution of pure sodium acetate, whose acetate ion is the conjugate base of a weak acid and hydrolyzes to produce $\ce{OH-}$, raising the pH above 7; HCl/NaOH produces NaCl, whose ions are both spectators (conjugates of a strong acid and strong base) that don't hydrolyze, leaving the solution neutral.

**2. Forward — classify by combination**
- Variables & ranges: several named acid/base titration pairs.
- Constraint: correct classification into one of the three categories.
- Contexts: various common acids and bases.
- Formats: short-answer/multiple-choice.
- Worked instantiation: classify the equivalence-point pH (=7, >7, or <7) for: $\ce{HNO3}$/$\ce{KOH}$; $\ce{HNO2}$/$\ce{KOH}$; $\ce{HCl}$/$\ce{NH3}$.

**3. Predict-the-shape — curve comparison**
- Variables & ranges: strong-strong vs. weak-strong titration curves at the same concentrations.
- Constraint: comparison must reference starting pH, buffer region presence, and equivalence-point pH together.
- Contexts: the study guide's own comparison figure.
- Formats: short-answer.
- Worked instantiation: see the study guide's Figure 16.1 and its self-check.

**4. Error analysis**
- Variables & ranges: a student who assumes a weak acid/strong base titration's equivalence point is always exactly pH 7 "like all titrations."
- Constraint: correction must restate the hydrolysis-dependence rule.
- Contexts: any weak-strong titration.
- Formats: short-answer.
- Worked instantiation: "A student assumes every titration's equivalence point is pH 7 because 'that's where the acid and base are equal.' What's wrong?" → Equal moles of acid and base does not by itself guarantee pH 7 — it guarantees a solution of the resulting *salt*, and that salt's pH depends on whether its ions hydrolyze; only a strong acid-strong base combination reliably gives pH 7 at equivalence.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | Classify 4–5 titration pairs by equivalence-point pH category. |
| Group discussion | Analyze | Debate why the equivalence point rule connects directly back to Chapter 15's salt-hydrolysis rules. |
| Quiz | Understand | One classification item. |
| Exam | Analyze | Require justification linking equivalence-point pH to salt hydrolysis. |
| Project/activity | Evaluate | Sketch (by hand or software) all three curve types for equal concentrations and compare. |

## Objective 16.2b: Calculate pH at any point during a titration

### Target understanding

A student can calculate pH before, at, and after the equivalence point for any acid-base titration, correctly selecting the calculation method for each region.

### Question guides

**1. Forward — strong-strong, all three regions**
- Variables & ranges: a strong acid titrated by a strong base, several titrant volumes spanning before/at/after equivalence.
- Constraint: correct method per region (remaining acid/base directly; pH=7 at equivalence).
- Contexts: any strong-strong titration.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (25.0 mL 0.100 M HCl + 0.100 M NaOH at 10.0/25.0/35.0 mL).

**2. Forward — weak-strong, all three regions**
- Variables & ranges: a weak acid titrated by a strong base, several titrant volumes.
- Constraint: correct method per region (Henderson-Hasselbalch before; salt hydrolysis at; excess base after).
- Contexts: any weak-strong titration.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (25.0 mL 0.100 M $\ce{CH3COOH}$ + 0.100 M NaOH at 10.0/25.0/35.0 mL).

**3. Predict-the-effect — halfway to equivalence**
- Variables & ranges: exactly half the volume needed to reach equivalence in a weak-strong titration.
- Constraint: recognize that at the half-equivalence point, $[\text{acid}]=[\text{conjugate base}]$, so $\ce{pH}=\ce{p}K_a$ exactly.
- Contexts: any weak acid/strong base titration.
- Formats: short-answer.
- Worked instantiation: "In the acetic acid titration above, what is the pH when exactly 12.5 mL of NaOH (half of the 25.0 mL needed for equivalence) has been added, and why is this a particularly easy point to calculate?" → At half-equivalence, exactly half the acid has been converted to its conjugate base, so $[\text{acid}]=[\text{conjugate base}]$ and $\log(1)=0$, giving $\ce{pH}=\ce{p}K_a$ directly — no further calculation needed.

**4. Error analysis**
- Variables & ranges: a student using Henderson-Hasselbalch past the equivalence point, or using strong-acid logic before it for a weak acid.
- Constraint: correction must restate which method belongs to which region.
- Contexts: any titration problem with a region-classification error.
- Formats: short-answer.
- Worked instantiation: "A student uses Henderson-Hasselbalch to calculate pH after the equivalence point in a weak acid/strong base titration. What's wrong?" → Past equivalence, there is no more original weak acid left to form a buffer — the solution is dominated by excess strong base, so pH should be calculated directly from the excess $\ce{OH-}$ concentration, not from the (no-longer-applicable) Henderson-Hasselbalch ratio.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | Full three-region titration calculations for both a strong-strong and a weak-strong case. |
| Group discussion | Analyze | Discuss why the half-equivalence point is a "free" pKa measurement. |
| Quiz | Apply | One titration-point pH calculation, region specified. |
| Exam | Analyze | Require classifying the region first, then calculating — for at least one point in each region. |
| Project/activity | Evaluate | Plot a full titration curve from calculated points and identify the half-equivalence and equivalence points. |

## Objective 16.2c: Select an appropriate acid-base indicator

### Target understanding

A student can select an indicator whose color-change range (≈ $\ce{p}K_a\pm1$) falls within a titration curve's steep region near the equivalence point, and can explain why a mismatched indicator would give an inaccurate endpoint.

### Question guides

**1. Forward — match indicator to equivalence point**
- Variables & ranges: a titration's equivalence-point pH, several candidate indicators with known ranges.
- Constraint: selection based on range overlap with the steep region, not just the equivalence value alone.
- Contexts: any acid-base titration paired with a set of indicators.
- Formats: multiple-choice/short-answer.
- Worked instantiation: for a titration with equivalence at pH 8.72 (matching the study guide's acetic acid/NaOH example), phenolphthalein (range ≈ 8.3–10.0) is an appropriate choice; methyl orange (range ≈ 3.1–4.4) is not.

**2. Conceptual — why the steep region matters**
- Variables & ranges: a prompt about why indicator range must fall in the steep part of the curve.
- Constraint: explanation must connect a small volume change to a large pH change specifically in the steep region.
- Contexts: any titration curve.
- Formats: short-answer.
- Worked instantiation: "Why does an indicator need to change color within the titration curve's steep region, rather than just somewhere near the equivalence point?" → In the steep region, a tiny additional volume of titrant causes a large pH swing, so the indicator changes color at almost exactly the equivalence volume; outside the steep region, the same small volume change causes only a small pH change, so the indicator would change color well before or after the true equivalence point, introducing significant error.

**3. Predict-the-effect — wrong indicator**
- Variables & ranges: a mismatched indicator/titration pairing (e.g., using methyl orange for a weak acid/strong base titration).
- Constraint: prediction must describe the direction and cause of the resulting error.
- Contexts: study guide's own self-check (phenolphthalein vs. a strong-strong titration).
- Formats: short-answer.
- Worked instantiation: see the study guide's self-check on this exact question.

**4. Error analysis**
- Variables & ranges: the classic dinitrophenol practice item — a student who assumes any weak-acid indicator works for any titration.
- Constraint: correction must reference matching the SPECIFIC range to the SPECIFIC equivalence point.
- Contexts: strong acid/weak base titrations especially (acidic equivalence point).
- Formats: short-answer.
- Worked instantiation: "The indicator dinitrophenol has $K_a=1.1\times10^{-4}$ (range ≈ pH 2.9–4.9 approximately). For which titration type — strong acid/strong base, strong acid/weak base, or weak acid/strong base — is it best suited?" → Strong acid/weak base, since that combination's equivalence point falls below pH 7, within dinitrophenol's acidic color-change range; a weak acid/strong base titration's equivalence point (above pH 7) would fall well outside this indicator's range.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | Match 3–4 indicators to 3–4 titration scenarios. |
| Group discussion | Analyze | Debate what happens to the measured endpoint if the wrong indicator is chosen. |
| Quiz | Apply | One indicator-selection item with justification required. |
| Exam | Analyze | Require identifying equivalence-point pH first, then selecting a matching indicator. |
| Project/activity | Evaluate | Research the color-change ranges of 3 real indicators not covered in class and propose titrations they'd suit. |

## Objective 16.3a: Write Ksp expressions and convert between Ksp and molar solubility

### Target understanding

A student can write a correctly exponentiated $K_{sp}$ expression from a dissolution equation and can convert between molar solubility and $K_{sp}$ in both directions, using the correct stoichiometric relationship between ion concentrations.

### Question guides

**1. Forward — Ksp from solubility**
- Variables & ranges: a compound's solubility in g/L or mol/L, with a stoichiometry beyond 1:1.
- Constraint: correctly scale the counted ion's concentration before exponentiating (e.g., double $[\ce{OH-}]$ for a 1:2 salt).
- Contexts: $\ce{Ca(OH)2}$-type and similar compounds.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{Ca(OH)2}$, $K_{sp}=1.31\times10^{-6}$).

**2. Inverse — solubility from Ksp**
- Variables & ranges: a given $K_{sp}$, solve for molar solubility and then mass solubility.
- Constraint: correct stoichiometric relationship (e.g., 1:1 vs. 1:2) before taking a root.
- Contexts: $\ce{CaCO3}$-type (1:1) and $\ce{Ca(OH)2}$-type (1:2) compounds.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{CaCO3}$, solubility = $9.3\times10^{-3}$ g/L).

**3. Conceptual — Ksp comparison pitfall**
- Variables & ranges: two compounds with similar $K_{sp}$ but different stoichiometries (1:1 vs. 1:2).
- Constraint: explanation must state that Ksp values are only directly comparable as a solubility ranking for the *same* stoichiometry.
- Contexts: any 1:1 vs. 1:2 (or 1:3) comparison.
- Formats: short-answer.
- Worked instantiation: "Compound A (1:1 stoichiometry) and Compound B (1:2 stoichiometry) both have $K_{sp}=4\times10^{-9}$. Does this mean they have the same molar solubility?" → No — for compound A, solubility $=\sqrt{K_{sp}}$; for compound B (with $K_{sp}=4s^3$ style relationship), the solubility formula is different, so equal $K_{sp}$ values do not imply equal solubilities when the stoichiometries differ.

**4. Error analysis**
- Variables & ranges: a student who forgets to square/cube the correct ion's concentration.
- Constraint: correction must reference writing the dissolution equation and its coefficients first.
- Contexts: any compound with a coefficient other than 1.
- Formats: short-answer.
- Worked instantiation: "A student computes $K_{sp}$ for $\ce{Ca(OH)2}$ as $[\ce{Ca^2+}][\ce{OH-}]$ (forgetting the exponent of 2). What's the fix?" → Write the dissolution equation first ($\ce{Ca(OH)2(s)<=>Ca^2+ + 2OH-}$), then use its coefficients directly as exponents: $K_{sp}=[\ce{Ca^2+}][\ce{OH-}]^2$.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 Ksp↔solubility conversions, mixing 1:1 and non-1:1 stoichiometries. |
| Group discussion | Analyze | Debate why Ksp ranking only works within the same stoichiometry class. |
| Quiz | Apply | One Ksp-from-solubility item, one solubility-from-Ksp item. |
| Exam | Analyze | Require writing the dissolution equation explicitly before any calculation. |
| Project/activity | Evaluate | Look up real Ksp values for a table of compounds and rank solubilities correctly, accounting for differing stoichiometries. |

## Objective 16.3b: Predict precipitation by comparing Q to Ksp

### Target understanding

A student can calculate the ion product $Q$ from given (possibly post-mixing) concentrations and correctly predict whether precipitation occurs by comparing $Q$ to $K_{sp}$.

### Question guides

**1. Forward — will it precipitate?**
- Variables & ranges: two solutions mixed, with a resulting dilution to account for.
- Constraint: student must correctly account for the volume change (dilution) before comparing $Q$ to $K_{sp}$.
- Contexts: any two ionic solutions mixed together.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (equal volumes of $\ce{AgNO3}$ and $\ce{NaCl}$, $Q>K_{sp}$, precipitates).

**2. Inverse — minimum concentration to begin precipitation**
- Variables & ranges: one ion's concentration given, find the minimum concentration of the other ion needed to just reach $Q=K_{sp}$.
- Constraint: correct algebraic rearrangement, accounting for stoichiometry if not 1:1.
- Contexts: e.g., $\ce{Ag2CO3}$-type (1:2) compounds.
- Formats: workout.
- Worked instantiation: given $[\ce{CO3^2-}]=2.50\times10^{-6}$ M and $K_{sp}(\ce{Ag2CO3})=8.1\times10^{-12}$, find the minimum $[\ce{Ag+}]$ to begin precipitation.

**3. Conceptual — dilution matters**
- Variables & ranges: a prompt about why concentrations must be adjusted after mixing.
- Constraint: explanation must state that mixing two solutions dilutes each below its original concentration.
- Contexts: any two-solution mixing scenario.
- Formats: short-answer.
- Worked instantiation: "Why can't you use the original, pre-mixing concentrations of $\ce{Ag+}$ and $\ce{Cl-}$ directly in the $Q$ calculation after combining two solutions?" → Combining two solutions increases the total volume, diluting each ion's concentration below its original value; $Q$ must be calculated using the concentrations *after* mixing, not before.

**4. Error analysis**
- Variables & ranges: a student who concludes precipitation occurs whenever ions capable of forming an insoluble salt are simply present together, without calculating $Q$.
- Constraint: correction must require the actual $Q$-vs-$K_{sp}$ comparison.
- Contexts: any borderline precipitation scenario.
- Formats: short-answer.
- Worked instantiation: "A student assumes any solution containing both $\ce{Ag+}$ and $\ce{Cl-}$ must precipitate $\ce{AgCl}$, since it's known to be insoluble. What's missing?" → "Insoluble" is a relative term — precipitation only occurs if $Q$ (calculated from the actual concentrations present) exceeds $K_{sp}$; sufficiently dilute solutions of $\ce{Ag+}$ and $\ce{Cl-}$ can coexist without precipitating.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 precipitation-prediction problems, including at least one requiring a dilution calculation. |
| Group discussion | Analyze | Discuss why "insoluble" compounds still have a nonzero, calculable solubility. |
| Quiz | Apply | One Q-vs-Ksp precipitation-prediction item. |
| Exam | Analyze | Require finding a minimum concentration to just avoid (or just cause) precipitation. |
| Project/activity | Evaluate | Research a real water-treatment or geological precipitation process and analyze it via Q vs. Ksp. |

## Objective 16.3c: Calculate solubility with a common ion present

### Target understanding

A student can calculate the solubility of a slightly soluble compound in a solution that already contains one of its constituent ions, correctly setting up the ICE table with the common ion's nonzero initial concentration.

### Question guides

**1. Forward — solubility with a common ion**
- Variables & ranges: a target ion concentration to limit, given $K_{sp}$.
- Constraint: correct ICE table with the common ion's initial concentration included.
- Contexts: any compound dissolving into a solution already containing one of its ions.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{Mn(OH)2}$, limiting $[\ce{Mn^2+}]$ to $1.8\times10^{-6}$ M via pH control).

**2. Conceptual — why solubility decreases**
- Variables & ranges: a comparison of a compound's solubility in pure water vs. in a solution with a common ion.
- Constraint: explanation must invoke Le Chatelier's principle (Chapter 14) explicitly.
- Contexts: any common-ion scenario.
- Formats: short-answer.
- Worked instantiation: "Why is $\ce{AgCl}$ less soluble in a $0.10$ M $\ce{NaCl}$ solution than in pure water?" → The dissolved $\ce{Cl-}$ already present shifts the dissolution equilibrium $\ce{AgCl(s)<=>Ag++Cl-}$ to the left (Le Chatelier's principle, Chapter 14), suppressing further dissolution and lowering $\ce{AgCl}$'s solubility compared to pure water.

**3. Predict-the-effect — comparing two common-ion concentrations**
- Variables & ranges: the same slightly soluble compound in two solutions with different common-ion concentrations.
- Constraint: prediction must correctly rank solubility as inversely related to common-ion concentration.
- Contexts: any $K_{sp}$ compound.
- Formats: short-answer.
- Worked instantiation: would $\ce{PbCl2}$ be more soluble in 0.10 M $\ce{NaCl}$ or in 0.50 M $\ce{NaCl}$? Why?

**4. Error analysis**
- Variables & ranges: a student who solves a common-ion solubility problem using the simple $\sqrt{K_{sp}}$ shortcut without accounting for the common ion's initial concentration.
- Constraint: correction must state that the shortcut only applies in pure water (no common ion present).
- Contexts: any common-ion problem.
- Formats: short-answer.
- Worked instantiation: "A student calculates $\ce{AgCl}$'s solubility in 0.10 M $\ce{NaCl}$ using $\sqrt{K_{sp}}$ directly, the same way they would for pure water. What's wrong?" → That shortcut assumes both ions start at zero concentration (pure water); with 0.10 M $\ce{Cl-}$ already present, the correct approach is an ICE table with $[\ce{Cl-}]_0=0.10$ M, which gives a much smaller solubility than the pure-water shortcut would suggest.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2 common-ion solubility problems, one framed as a pH-control scenario. |
| Group discussion | Analyze | Connect this directly back to Chapter 14's Le Chatelier's principle and common-ion-effect framing. |
| Quiz | Apply | One common-ion solubility calculation. |
| Exam | Analyze | Require comparing solubility in pure water vs. with a common ion side by side. |
| Project/activity | Evaluate | Research how the common ion effect is used industrially (e.g., salting out soap, water softening). |

## Objective 16.4a: Define complex ion/formation constant and solve Kf problems

### Target understanding

A student can define a complex ion and formation constant, connect complex-ion formation to Lewis acid-base theory (Chapter 15), and set up/solve a basic $K_f$ equilibrium problem using the same framework as any other equilibrium constant.

### Question guides

**1. Conceptual — Lewis acid-base connection**
- Variables & ranges: any complex-ion formation reaction.
- Constraint: explanation must identify the metal cation as the Lewis acid and the ligand as the Lewis base.
- Contexts: $\ce{Ag(NH3)2+}$ or similar.
- Formats: short-answer.
- Worked instantiation: "In $\ce{Ag+ + 2NH3 <=> Ag(NH3)2+}$, identify the Lewis acid and Lewis base, connecting to Chapter 15's definitions." → $\ce{Ag+}$ is the Lewis acid (accepts electron pairs); $\ce{NH3}$ is the Lewis base (donates an electron pair from its lone pair on nitrogen), twice.

**2. Forward — write the Kf expression**
- Variables & ranges: any complex-ion formation reaction with given stoichiometry.
- Constraint: correct exponents matching the ligand stoichiometry.
- Contexts: $\ce{Ag(NH3)2+}$, $\ce{Al(OH)4-}$, or similar.
- Formats: workout.
- Worked instantiation: write the $K_f$ expression for $\ce{Al(OH)3(s) + OH-(aq) <=> Al(OH)4-(aq)}$.

**3. Conceptual — larger Kf means more stable**
- Variables & ranges: two complex ions with different $K_f$ values.
- Constraint: explanation must connect larger $K_f$ to the same "product-favored" reasoning as Chapter 14's $K$.
- Contexts: any two complex ions.
- Formats: short-answer.
- Worked instantiation: "Complex A has $K_f=10^{7}$; complex B has $K_f=10^{2}$. Which complex, once formed, is more resistant to falling back apart into free metal ion and ligands?" → Complex A — a much larger $K_f$ means the equilibrium lies far toward the complexed form, exactly analogous to a large $K$ meaning a reaction is strongly product-favored (Chapter 14).

**4. Error analysis**
- Variables & ranges: a student who writes the $K_f$ expression with the metal ion and ligand in the numerator (as if it were a dissociation constant).
- Constraint: correction must restate that $K_f$ describes *formation*, so the complex ion belongs in the numerator.
- Contexts: any $K_f$ expression-writing task.
- Formats: short-answer.
- Worked instantiation: "A student writes $K_f=[\ce{Ag+}][\ce{NH3}]^2/[\ce{Ag(NH3)2+}]$. What's wrong?" → This is backwards — $K_f$ is the *formation* constant, describing the reaction written with the complex ion as the product, so the complex ion belongs in the numerator: $K_f=[\ce{Ag(NH3)2+}]/([\ce{Ag+}][\ce{NH3}]^2)$.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | 2–3 Kf-expression-writing problems; 1 Lewis acid/base identification in a complex-ion context. |
| Group discussion | Analyze | Debate why complex-ion formation is described as an equilibrium (reversible) rather than a one-way reaction. |
| Quiz | Understand | One Kf-expression item. |
| Exam | Analyze | Require both the Lewis acid/base identification and the correct Kf expression for a novel complex ion. |
| Project/activity | Evaluate | Research a real application of complex-ion chemistry (e.g., photographic fixing with thiosulfate, or EDTA in water treatment) and its relevant Kf. |

## Rubric Themes for Chapter 16

| Evidence of mastery | What to look for |
|---|---|
| Henderson-Hasselbalch used as a shortcut, not blindly | Student can also set up the full ICE table and shows the two methods agree, rather than treating HH as an unrelated formula. |
| Titration region identified before method is chosen | Student explicitly states "before/at/after equivalence" before selecting a calculation approach. |
| Equivalence-point pH tied to salt hydrolysis | Student never assumes pH 7 at equivalence without checking whether the product salt hydrolyzes. |
| Ksp stoichiometry applied correctly | Student writes the dissolution equation and its coefficients before exponentiating any concentration in a Ksp expression. |
| Common ion effect explained via Le Chatelier | Student connects reduced solubility with a common ion back to Chapter 14's equilibrium-shift reasoning, not as an isolated rule. |
| Kf treated as an ordinary equilibrium constant | Student sets up Kf problems (including which species goes in the numerator) using the same logic as any other K from Ch. 14. |
