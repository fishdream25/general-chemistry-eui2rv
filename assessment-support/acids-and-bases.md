{{nyml
kind: document
format: 1
title: Chapter 15 Assessment Guide: Acids and Bases
}}

# Chapter 15 Assessment Guide: Acids and Bases

## Source and Format

**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 15 (CC BY 4.0). **Audience:** introductory undergraduate general chemistry, second semester. **Note:** this is design guidance for building assessments — question *guides* an instructor or generator can instantiate into many concrete questions — not a finished question bank or answer key.

## General Assessment Priorities

- Require the **strong-acid/strong-base list check** as an explicit first step of every pH problem — before deciding whether an ICE table is even needed — since skipping straight to an ICE table for a strong acid is the single most common wasted-effort error in this chapter.
- Keep **acid strength ($K_a$, a chemical property) and acid concentration (molarity, an amount)** explicitly separate in at least one question per relevant objective, using paired examples (concentrated weak acid vs. dilute strong acid) so students don't conflate "more acid" with "stronger acid."
- Test the **two oxoacid trends** (same-oxidation-number/different-central-atom vs. same-central-atom/different-oxidation-number) as clearly distinct rules, never interchangeably.
- Require an explicit **hydrolysis-species identification** step ("which ion actually reacts with water?") before any salt-solution pH calculation.

## Objective 15.1a: Identify conjugate acid-base pairs and diprotic acid ionization steps

### Target understanding

A student can identify both conjugate acid-base pairs in a Brønsted reaction — including reactions without water or without an obviously "acidic" reactant — and can write the stepwise ionization equations (with separate $K_a$ expressions) for a diprotic or polyprotic acid.

### Question guides

**1. Forward — identify conjugate pairs**
- Variables & ranges: a Brønsted acid-base reaction, possibly without water as a reactant.
- Constraint: student must identify both pairs, not just the more obvious one.
- Contexts: aqueous and non-aqueous (e.g., gas-phase or amide-ion) reactions.
- Formats: short-answer.
- Worked instantiation: see the study guide's worked example ($\ce{CH3COOH + H2O <=> CH3COO- + H3O+}$).

**2. Forward — an unfamiliar, non-aqueous pair**
- Variables & ranges: a reaction like $\ce{H2S + NH2- <=> HS- + NH3}$.
- Constraint: student must apply the proton-donor/acceptor definition without relying on a memorized "water is always involved" pattern.
- Contexts: any Brønsted reaction without water.
- Formats: short-answer.
- Worked instantiation: "Identify the conjugate acid-base pairs in $\ce{H2S + NH2- <=> HS- + NH3}$." → $\ce{H2S}$/$\ce{HS-}$ is one pair (H₂S is the acid); $\ce{NH2-}$/$\ce{NH3}$ is the other pair ($\ce{NH2-}$ is the base).

**3. Forward — diprotic ionization steps**
- Variables & ranges: a named diprotic or triprotic acid.
- Constraint: each step must be written separately, each with its own correctly formed $K_a$ expression.
- Contexts: $\ce{H2CO3}$, $\ce{H2SO3}$, $\ce{H3PO4}$ (triprotic, three steps).
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{H2CO3}$'s two-step ionization).

**4. Error analysis**
- Variables & ranges: a student who writes only one overall ionization step for a diprotic acid, combining both protons at once.
- Constraint: correction must explain why stepwise ionization (not a single combined step) is the correct model.
- Contexts: any diprotic/polyprotic acid.
- Formats: short-answer.
- Worked instantiation: "A student writes $\ce{H2CO3 <=> 2H+ + CO3^2-}$ as a single step with one $K_a$. What's wrong?" → Diprotic acids ionize in a stepwise manner, each proton removed in its own equilibrium with its own $K_a$; the two ionization constants are typically very different in magnitude ($K_{a_1}\gg K_{a_2}$), so combining them into one step loses the ability to correctly model which species dominate at equilibrium.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | 3–4 conjugate-pair identification problems, including a non-aqueous case. |
| Group discussion | Understand | Debate why every acid-base reaction has exactly two conjugate pairs, never more or fewer. |
| Quiz | Understand | One conjugate-pair item, one diprotic-ionization-writing item. |
| Exam | Analyze | Require both directions: identify pairs AND write stepwise ionizations with correct $K_a$ expressions. |
| Project/activity | Evaluate | Research a real triprotic acid (e.g., $\ce{H3PO4}$) and write all three ionization steps with literature $K_a$ values. |

## Objective 15.1b: Calculate pH/pOH and recognize strong/weak acids and bases

### Target understanding

A student can calculate any one of pH, pOH, $[\ce{H+}]$, or $[\ce{OH-}]$ from any other using $K_w=1.0\times10^{-14}$ and $\ce{pH}+\ce{pOH}=14$, and can recall the short list of common strong acids/bases from memory.

### Question guides

**1. Forward — pH from [OH⁻]**
- Variables & ranges: a given $[\ce{OH-}]$ or $[\ce{H+}]$.
- Constraint: correct use of $K_w$ before taking a logarithm.
- Contexts: any aqueous solution.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($[\ce{OH-}]=2.5\times10^{-3}$ M → pH = 11.40).

**2. Inverse — [H⁺] from pH**
- Variables & ranges: a given pH, solve for $[\ce{H+}]$ (and optionally $[\ce{OH-}]$).
- Constraint: correct inverse-log calculation ($[\ce{H+}]=10^{-\ce{pH}}$).
- Contexts: any aqueous solution.
- Formats: workout.
- Worked instantiation: a solution has pH = 4.20; find $[\ce{H+}]$ and $[\ce{OH-}]$.

**3. Conceptual — classify by memorized list**
- Variables & ranges: a list of acids/bases including at least one from the memorized strong list and at least one common weak one.
- Constraint: classification must come from the memorized list, not a calculation.
- Contexts: $\ce{HClO4}$, $\ce{HF}$, $\ce{NaOH}$, $\ce{NH3}$, etc.
- Formats: short-answer or multiple-choice.
- Worked instantiation: "Classify each as a strong or weak acid/base: $\ce{HNO3}$, $\ce{HNO2}$, $\ce{NH3}$." → $\ce{HNO3}$ strong acid (on the list); $\ce{HNO2}$ weak acid (not on the strong list); $\ce{NH3}$ weak base.

**4. Error analysis**
- Variables & ranges: a student who computes pH directly as $-\log[\ce{OH-}]$.
- Constraint: correction must restate that pH uses $[\ce{H+}]$, not $[\ce{OH-}]$, directly.
- Contexts: any problem starting from $[\ce{OH-}]$.
- Formats: short-answer.
- Worked instantiation: "Given $[\ce{OH-}]=1.0\times10^{-4}$ M, a student computes $\ce{pH}=-\log(1.0\times10^{-4})=4.00$. What's wrong?" → That calculation gives pOH, not pH; the student must either first find $[\ce{H+}]=K_w/[\ce{OH-}]$ and take $-\log$ of that, or compute pOH = 4.00 and then use $\ce{pH}=14-\ce{pOH}=10.00$.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 pH/pOH/[H⁺]/[OH⁻] interconversions. |
| Group discussion | Understand | Quiz each other from memory on the strong acid/base list. |
| Quiz | Apply | One interconversion item, one classification item. |
| Exam | Analyze | Combine interconversion with a strong-vs-weak classification that determines the calculation method (ties to Objective 15.4a). |
| Project/activity | Evaluate | Measure the pH of household liquids (if available) and back-calculate $[\ce{H+}]$. |

## Objective 15.2a: Explain hydrohalic acid and oxoacid strength trends

### Target understanding

A student can rank hydrohalic acid strength by bond strength and oxoacid strength by the two distinct rules (central-atom electronegativity at constant oxidation number; oxidation number at constant central atom), without conflating the two oxoacid rules.

### Question guides

**1. Forward — rank hydrohalic acids**
- Variables & ranges: any subset of $\ce{HF, HCl, HBr, HI}$.
- Constraint: ranking justified by bond strength, not electronegativity of the halogen alone.
- Contexts: any hydrohalic acid comparison.
- Formats: short-answer.
- Worked instantiation: see the study guide's trend ($\ce{HF} \ll \ce{HCl} < \ce{HBr} < \ce{HI}$).

**2. Forward — rank oxoacids, same central atom**
- Variables & ranges: a set of oxoacids of the same central atom, different oxygen counts.
- Constraint: ranking justified by oxidation number/oxygen count.
- Contexts: chlorine oxoacids, or sulfur/nitrogen oxoacid analogues.
- Formats: short-answer.
- Worked instantiation: rank $\ce{HClO}$, $\ce{HClO2}$, $\ce{HClO3}$, $\ce{HClO4}$ by acid strength.

**3. Forward — rank oxoacids, same oxidation number**
- Variables & ranges: oxoacids of different central atoms from the same group, same oxidation number.
- Constraint: ranking justified by central-atom electronegativity, explicitly distinguished from the oxidation-number rule.
- Contexts: $\ce{HClO3}$ vs. $\ce{HBrO3}$; $\ce{H2SO3}$ vs. $\ce{H2SeO3}$.
- Formats: short-answer.
- Worked instantiation: "Which is stronger, $\ce{HClO3}$ or $\ce{HBrO3}$, and why?" → $\ce{HClO3}$ — same oxidation number (+5) on the central atom, so the more electronegative central atom (Cl vs. Br) gives the stronger acid.

**4. Error analysis**
- Variables & ranges: a student applying the electronegativity rule to a same-central-atom comparison (or vice versa).
- Constraint: correction must identify which rule actually applies based on what varies between the two acids.
- Contexts: any oxoacid pair.
- Formats: short-answer.
- Worked instantiation: "A student compares $\ce{HClO2}$ and $\ce{HClO3}$ and says 'Cl has the same electronegativity in both, so they should be equally strong.' What's the error?" → The relevant variable here is oxidation number/oxygen count (same central atom, different oxidation states), not electronegativity — the electronegativity rule only applies when comparing *different* central atoms at the *same* oxidation number.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | 3–4 ranking problems, covering both oxoacid rules separately. |
| Group discussion | Analyze | Discuss why bond strength (not electronegativity) governs the hydrohalic acid trend, contrasting with the oxoacid rules. |
| Quiz | Understand | One hydrohalic ranking, one oxoacid ranking (state which rule applies). |
| Exam | Analyze | Require explicit identification of which rule applies before ranking. |
| Project/activity | Evaluate | Research literature $K_a$ values for a set of oxoacids and verify the trend. |

## Objective 15.2b: Predict salt solution acidity and classify oxides

### Target understanding

A student can predict whether a salt solution is acidic, basic, or neutral from the strength of its parent acid and base (including comparing $K_a$ and $K_b$ for a weak-weak salt), and can classify a given oxide as acidic, basic, or amphoteric.

### Question guides

**1. Forward — classify salts by parent strength**
- Variables & ranges: salts formed from various strong/weak acid-base combinations.
- Constraint: student must identify the parent acid and base first, then apply the strong/weak rule.
- Contexts: any common salt.
- Formats: short-answer.
- Worked instantiation: see the study guide's worked example ($\ce{NaBr}$ neutral, $\ce{NaF}$ basic, $\ce{NH4Cl}$ acidic).

**2. Forward — weak-weak comparison**
- Variables & ranges: a salt from a weak acid and a weak base, with given $K_a$ (cation) and $K_b$ (anion).
- Constraint: comparison of $K_a$ and $K_b$ directly, not a rule of thumb.
- Contexts: e.g., ammonium acetate ($\ce{NH4CH3COO}$).
- Formats: workout/short-answer.
- Worked instantiation: for ammonium acetate, $K_a(\ce{NH4+})\approx K_b(\ce{CH3COO-})$ — predict the solution is nearly neutral, and explain why.

**3. Forward — classify oxides**
- Variables & ranges: a set of metal, nonmetal, and amphoteric oxides.
- Constraint: classification justified by expected reaction with water, acid, or base.
- Contexts: $\ce{Na2O}$, $\ce{SO3}$, $\ce{Al2O3}$.
- Formats: short-answer.
- Worked instantiation: complete $\ce{MgO + H2SO4 -> ?}$ and $\ce{SO3 + KOH -> ?}$.

**4. Error analysis**
- Variables & ranges: a student who assumes any metal cation makes a solution basic.
- Constraint: correction must distinguish spectator cations (from strong bases) from hydrolyzing cations (from weak bases or small highly charged metals).
- Contexts: $\ce{NaCl}$ vs. $\ce{AlCl3}$.
- Formats: short-answer.
- Worked instantiation: "A student assumes $\ce{AlCl3}$ solution is neutral because 'metal chlorides are always neutral, like NaCl.' What's wrong?" → $\ce{Na+}$ is the conjugate acid of a strong base ($\ce{NaOH}$) and does not hydrolyze, but $\ce{Al^3+}$ is a small, highly charged metal cation that *does* hydrolyze (via $\ce{Al(H2O)6^3+}$), making $\ce{AlCl3}$ solutions acidic — not every metal cation behaves like $\ce{Na+}$.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | Classify 4–5 salts; complete 2–3 oxide reactions. |
| Group discussion | Analyze | Debate why small, highly charged cations hydrolyze while alkali metal cations don't. |
| Quiz | Apply | One salt-classification item, one oxide-classification item. |
| Exam | Analyze | Require a weak-weak salt comparison using given $K_a$/$K_b$ values. |
| Project/activity | Evaluate | Research a real amphoteric oxide's use (e.g., $\ce{Al2O3}$ in industry) and both its acid and base reactions. |

## Objective 15.3a: Identify Lewis acids and bases

### Target understanding

A student can identify the Lewis acid (electron-pair acceptor) and Lewis base (electron-pair donor) in a reaction, including reactions where no proton is transferred.

### Question guides

**1. Forward — identify in a non-proton-transfer reaction**
- Variables & ranges: a reaction with clear electron-pair donation/acceptance but no $\ce{H+}$ transfer.
- Constraint: student must justify using electron-pair donation/acceptance, not proton transfer.
- Contexts: metal-ion complexation, boron/aluminum trihalide reactions.
- Formats: short-answer.
- Worked instantiation: see the study guide's worked examples ($\ce{CO2+OH-}$, $\ce{AlCl3+Cl-}$).

**2. Forward — a classic adduct**
- Variables & ranges: $\ce{BF3 + NH3 -> F3B-NH3}$.
- Constraint: identify the empty-orbital acceptor vs. the lone-pair donor.
- Contexts: boron trihalide/amine adducts.
- Formats: short-answer.
- Worked instantiation: see the study guide's self-check.

**3. Conceptual — Lewis vs. Brønsted scope**
- Variables & ranges: a prompt comparing the two definitions' scope.
- Constraint: answer must state the subset relationship correctly (every Brønsted base is a Lewis base, but not vice versa for acids).
- Contexts: any comparison prompt.
- Formats: short-answer.
- Worked instantiation: "Is every Brønsted acid also a Lewis acid? Is every Lewis acid also a Brønsted acid?" → Every Brønsted base is a Lewis base (donating an electron pair to bond a proton is a special case of electron-pair donation), but many Lewis acids (e.g., $\ce{AlCl3}$, $\ce{BF3}$) are not Brønsted acids since they never donate a proton — they accept an electron pair directly.

**4. Error analysis**
- Variables & ranges: a student who claims a reaction has no acid-base character because no proton transfers.
- Constraint: correction must invoke the Lewis definition's broader scope.
- Contexts: any electron-pair-transfer reaction without a proton.
- Formats: short-answer.
- Worked instantiation: "A student says $\ce{AlCl3+Cl- -> AlCl4-}$ isn't an acid-base reaction because nothing donates or accepts a proton. Respond." → Under the Brønsted definition that's true, but the Lewis definition doesn't require proton transfer at all — $\ce{Cl-}$ donates an electron pair (Lewis base) and $\ce{AlCl3}$ accepts it (Lewis acid), so it is very much an acid-base reaction in the more general Lewis sense.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | 3–4 Lewis acid/base identification problems, at least half without proton transfer. |
| Group discussion | Analyze | Debate the Brønsted-vs-Lewis scope relationship using a Venn-diagram framing. |
| Quiz | Understand | One Lewis acid/base identification item. |
| Exam | Analyze | Require justification (which species has the empty orbital vs. the lone pair) not just labeling. |
| Project/activity | Evaluate | Research a real industrial Lewis acid catalyst (e.g., $\ce{AlCl3}$ in Friedel-Crafts reactions) and explain its role. |

## Objective 15.4a: Calculate pH for strong acid/base solutions

### Target understanding

A student can calculate pH or pOH directly from a strong acid or strong base's concentration, without an ICE table, correctly handling bases that release more than one $\ce{OH-}$ per formula unit.

### Question guides

**1. Forward — strong acid**
- Variables & ranges: a given concentration of a strong acid from the memorized list.
- Constraint: $[\ce{H+}]$ = initial concentration directly.
- Contexts: $\ce{HCl}$, $\ce{HNO3}$, etc.
- Formats: workout.
- Worked instantiation: 0.0431 M $\ce{HCl}$ → pH = 1.36.

**2. Forward — strong base with 2 OH⁻**
- Variables & ranges: a base of the form $\ce{B(OH)2}$.
- Constraint: $[\ce{OH-}]$ = 2 × initial concentration.
- Contexts: $\ce{Ca(OH)2}$, $\ce{Ba(OH)2}$.
- Formats: workout.
- Worked instantiation: 0.010 M $\ce{Ca(OH)2}$ → $[\ce{OH-}]=0.020$ M → find pH.

**3. Conceptual — why no ICE table**
- Variables & ranges: a comparison between a strong acid and a weak acid at the same concentration.
- Constraint: explanation must invoke "complete ionization" as the reason no equilibrium calculation is needed.
- Contexts: any strong/weak pair at equal concentration.
- Formats: short-answer.
- Worked instantiation: see the study guide's self-check (0.10 M HCl vs. 0.10 M CH₃COOH).

**4. Error analysis**
- Variables & ranges: a student who sets up an ICE table for a strong acid.
- Constraint: correction must state the strong-acid list check should have come first.
- Contexts: any strong acid problem.
- Formats: short-answer.
- Worked instantiation: "A student sets up an ICE table with an unknown $K_a$ for 0.20 M $\ce{HCl}$. What step did they skip?" → They skipped checking whether $\ce{HCl}$ is on the strong-acid list — it is, so it ionizes completely and $[\ce{H+}]=0.20$ M directly; no ICE table or $K_a$ is needed (or exists) for a strong acid.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 direct pH calculations, including at least one $\ce{B(OH)2}$-type base. |
| Group discussion | Understand | Discuss why "complete ionization" makes the calculation direct. |
| Quiz | Apply | One strong-acid, one strong-base item. |
| Exam | Analyze | Pair with a weak-acid problem at the same concentration to force the strong/weak check (ties to Objective 15.4b). |
| Project/activity | Evaluate | Calculate the pH of a diluted household strong acid/base (e.g., diluted drain cleaner) and discuss safety implications. |

## Objective 15.4b: Calculate pH for weak acid/base solutions and percent ionization

### Target understanding

A student can set up and solve an ICE table using $K_a$ or $K_b$ to find the pH of a weak acid or weak base solution, and can calculate percent ionization from the result.

### Question guides

**1. Forward — weak acid**
- Variables & ranges: a weak acid concentration and $K_a$.
- Constraint: correct ICE table, correctly extracting $[\ce{H+}]$ from $x$.
- Contexts: any monoprotic weak acid.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (0.50 M HF, pH = 1.73, 3.7% ionization).

**2. Forward — weak base**
- Variables & ranges: a weak base concentration and $K_b$.
- Constraint: correct ICE table producing $[\ce{OH-}]$, then converting to pH via pOH.
- Contexts: $\ce{NH3}$ or an amine.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (0.40 M $\ce{NH3}$, pH = 11.43).

**3. Inverse — find concentration from pH**
- Variables & ranges: a given pH and $K_a$, solve backward for initial concentration.
- Constraint: correct algebraic rearrangement of the ICE-table equation.
- Contexts: any weak acid.
- Formats: workout.
- Worked instantiation: a weak acid with $K_a=1.8\times10^{-5}$ has pH = 3.00; find its initial concentration.

**4. Error analysis**
- Variables & ranges: a student who reports percent ionization using the initial concentration in the numerator instead of the equilibrium ionized concentration.
- Constraint: correction must restate the percent-ionization formula correctly.
- Contexts: any weak-acid/base percent-ionization problem.
- Formats: short-answer.
- Worked instantiation: "A student computes percent ionization as $[\ce{HF}]_0/x \times 100\%$ instead of $x/[\ce{HF}]_0\times100\%$. What's wrong?" → Percent ionization is the *ionized* concentration (x, the amount that reacted) divided by the *initial* concentration — the student inverted the ratio, which would give a nonsensical result greater than 100% for a weak acid.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 weak-acid/base pH problems, at least one requiring percent ionization. |
| Group discussion | Analyze | Discuss why percent ionization increases as initial concentration decreases (dilution effect). |
| Quiz | Apply | One weak-acid or weak-base pH item. |
| Exam | Analyze | Require both the pH and percent ionization from a single setup. |
| Project/activity | Evaluate | Compare percent ionization for the same weak acid at two different concentrations and explain the trend. |

## Objective 15.4c: Calculate equilibrium concentrations for a diprotic/polyprotic acid

### Target understanding

A student can solve a diprotic acid's ionization stepwise, recognizing that the first step usually dominates $[\ce{H+}]$ and that the second step's small contribution can often be found using the first step's results.

### Question guides

**1. Forward — full stepwise calculation**
- Variables & ranges: a diprotic acid with $K_{a_1}$ and $K_{a_2}$ given, $K_{a_2}\ll K_{a_1}$.
- Constraint: student must solve step 1 fully before setting up step 2, using step 1's equilibrium concentrations as step 2's initial values.
- Contexts: $\ce{H2C2O4}$, $\ce{H2SO3}$, or similar.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{H2C2O4}$, $[\ce{H+}]\approx0.054$ M, $[\ce{C2O4^2-}]=6.1\times10^{-5}$ M).

**2. Conceptual — why step 1 dominates**
- Variables & ranges: a prompt about the relative sizes of $K_{a_1}$ and $K_{a_2}$.
- Constraint: explanation must connect the size difference to which step controls $[\ce{H+}]$.
- Contexts: any diprotic acid with $K_{a_2}\ll K_{a_1}$.
- Formats: short-answer.
- Worked instantiation: "Why is $[\ce{H+}]$ set almost entirely by the first ionization step for most diprotic acids?" → Because $K_{a_2}$ is typically several orders of magnitude smaller than $K_{a_1}$, the second step ionizes to a much smaller extent, contributing a negligible additional amount of $\ce{H+}$ compared to what the first step already produced.

**3. Predict-the-effect — finding [X²⁻]**
- Variables & ranges: given the first step's result, find the second ionization's product concentration.
- Constraint: recognize that $[\ce{C2O4^2-}]\approx y \approx K_{a_2}$ when $[\ce{H+}]\approx[\ce{HC2O4-}]$ from step 1 (a useful shortcut).
- Contexts: any diprotic acid second-step calculation.
- Formats: workout.
- Worked instantiation: given step 1 results ($[\ce{H+}]=[\ce{HA-}]=0.054$ M) and $K_{a_2}$, find $[\ce{A^2-}]$ at equilibrium.

**4. Error analysis**
- Variables & ranges: a student who solves both steps as if they were simultaneous/independent, ignoring that step 2 starts from step 1's products.
- Constraint: correction must emphasize the sequential nature of the calculation.
- Contexts: any diprotic acid problem.
- Formats: short-answer.
- Worked instantiation: "A student sets up the second ionization step using the *original* initial concentration of the diprotic acid, not the products of step 1. What's wrong?" → Step 2 begins from the equilibrium concentrations produced by step 1 ($[\ce{HA-}]$ and $[\ce{H+}]$ already present), not from the original diprotic acid's initial concentration — the two steps are sequential, not independent.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 1–2 full diprotic-acid stepwise problems. |
| Group discussion | Analyze | Discuss what would change if $K_{a_2}$ were closer in magnitude to $K_{a_1}$. |
| Quiz | Apply | One diprotic-acid step-1 calculation. |
| Exam | Analyze | Require the full two-step calculation, including $[\ce{OH-}]$ at the end. |
| Project/activity | Evaluate | Research a real triprotic acid's three $K_a$ values (e.g., $\ce{H3PO4}$) and discuss how much each step contributes to $[\ce{H+}]$. |

## Objective 15.4d: Calculate the pH of a salt solution using hydrolysis

### Target understanding

A student can identify which ion in a salt hydrolyzes, find the relevant $K_a$ or $K_b$ (using $K_aK_b=K_w$ if necessary), set up an ICE table, and calculate the resulting pH.

### Question guides

**1. Forward — anion hydrolysis (basic salt)**
- Variables & ranges: a salt of a weak acid and strong base, with the anion's $K_b$ given or derivable.
- Constraint: correct identification that the anion (not a spectator cation) hydrolyzes.
- Contexts: $\ce{CH3COONa}$, $\ce{NaF}$, sodium formate.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (0.24 M $\ce{CH3COONa}$, pH = 9.1).

**2. Inverse — find Ka/Kb using KaKb = Kw**
- Variables & ranges: given $K_a$ for a weak acid, find $K_b$ for its conjugate base (or vice versa).
- Constraint: correct application of $K_aK_b=K_w$.
- Contexts: any conjugate acid-base pair.
- Formats: workout.
- Worked instantiation: given $K_a(\ce{HF})=7.1\times10^{-4}$, find $K_b(\ce{F-})$.

**3. Forward — cation hydrolysis (acidic salt)**
- Variables & ranges: a salt of a strong acid and weak base, with the cation's $K_a$ given or derivable.
- Constraint: correct identification that the cation hydrolyzes.
- Contexts: $\ce{NH4Cl}$, $\ce{NH4Br}$.
- Formats: workout.
- Worked instantiation: find the pH of 0.0518 M $\ce{NH4Br}$, given $K_b(\ce{NH3})=1.8\times10^{-5}$.

**4. Error analysis**
- Variables & ranges: a student who tries to hydrolyze the spectator ion (e.g., $\ce{Na+}$ in $\ce{CH3COONa}$) instead of the actual hydrolyzing ion.
- Constraint: correction must state that only the conjugate of a *weak* acid or base hydrolyzes significantly.
- Contexts: any salt with one spectator and one hydrolyzing ion.
- Formats: short-answer.
- Worked instantiation: "A student tries to write a hydrolysis reaction for $\ce{Na+}$ in $\ce{CH3COONa}$ solution. What's wrong?" → $\ce{Na+}$ is the conjugate acid of a strong base ($\ce{NaOH}$) and does not hydrolyze significantly — only $\ce{CH3COO-}$, the conjugate base of the weak acid $\ce{CH3COOH}$, reacts with water to a meaningful extent.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 salt-hydrolysis pH problems, covering both acidic and basic salts. |
| Group discussion | Analyze | Debate which ion hydrolyzes in a list of salts before any calculation begins. |
| Quiz | Apply | One salt-hydrolysis pH item. |
| Exam | Analyze | Require finding the needed $K_a$ or $K_b$ via $K_aK_b=K_w$ as an explicit first step. |
| Project/activity | Evaluate | Research the pH of a common household salt solution (e.g., baking soda) and verify against a hydrolysis calculation. |

## Rubric Themes for Chapter 15

| Evidence of mastery | What to look for |
|---|---|
| Strong/weak check always comes first | Student explicitly checks the memorized strong acid/base list before deciding whether an ICE table is needed. |
| Acid strength vs. concentration kept distinct | Student never conflates "more concentrated" with "stronger acid" — these are independent properties. |
| The two oxoacid trends never conflated | Student states which variable differs (central atom vs. oxidation number) before applying a trend. |
| Hydrolyzing species identified explicitly | Student states which specific ion hydrolyzes (and why the other is a spectator) before setting up a salt-hydrolysis ICE table. |
| Diprotic acids solved sequentially | Student uses step 1's equilibrium concentrations as step 2's initial values, not the original starting concentration. |
| Lewis definition applied beyond proton transfer | Student correctly identifies Lewis acids/bases in reactions with no $\ce{H+}$ transfer. |
