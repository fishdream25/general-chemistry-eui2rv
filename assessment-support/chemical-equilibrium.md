{{nyml
kind: document
format: 1
title: Chapter 14 Assessment Guide: Chemical Equilibrium
}}

# Chapter 14 Assessment Guide: Chemical Equilibrium

## Source and Format

**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 14 (CC BY 4.0). **Audience:** introductory undergraduate general chemistry, second semester. **Note:** this is design guidance for building assessments — question *guides* an instructor or generator can instantiate into many concrete questions — not a finished question bank or answer key.

## General Assessment Priorities

- Relentlessly test the **Q-vs-K distinction** — same formula, different concentrations — since confusing them (or comparing them without calculating both correctly) is the single most common error in this chapter.
- Require students to **explicitly cross out** any pure solid, pure liquid, or bulk solvent before writing a final equilibrium expression, every time — not just recognize the rule when asked about it directly.
- Pair concentration-stress, pressure/volume-stress, and temperature-stress questions together so students build the habit of identifying *which kind* of stress is being applied before predicting a shift, rather than pattern-matching to a memorized answer.
- Include at least one question per relevant objective that requires students to state whether $K$ itself changes, not just whether the equilibrium position shifts — these are frequently conflated.

## Objective 14.1a: Derive and apply K = k_f/k_r, including the effect of reversing a reaction

### Target understanding

A student can derive the equilibrium constant expression from forward/reverse elementary-step rate laws, calculate $K$ from given rate constants, and correctly invert $K$ when a reaction is written in reverse.

### Question guides

**1. Forward — calculate K from rate constants**
- Variables & ranges: $k_f$, $k_r$ for a single-step reversible elementary reaction.
- Constraint: student must state $K=k_f/k_r$ before substituting.
- Contexts: any simple $\ce{A<=>B}$ or $\ce{A+B<=>C}$ elementary reaction.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($k_f=0.20\ \text{s}^{-1}$, $k_r=0.05\ \text{s}^{-1}$, $K=4.0$).

**2. Inverse — find a rate constant from K**
- Variables & ranges: given $K$ and one rate constant, solve for the other.
- Constraint: correct algebraic rearrangement of $K=k_f/k_r$.
- Contexts: extending the same reaction with a different known rate constant.
- Formats: workout.
- Worked instantiation: given $K=4.0$ and $k_r=0.05\ \text{s}^{-1}$, find $k_f$.

**3. Conceptual — reversing the reaction**
- Variables & ranges: a given $K$ for a forward reaction.
- Constraint: student must state the reciprocal relationship, not recompute from scratch.
- Contexts: any reversible reaction.
- Formats: short-answer.
- Worked instantiation: "A reaction has $K=25$. What is $K$ for the exact reverse reaction, and why?" → $K_{\text{reverse}}=1/25=0.04$, because reversing the reaction swaps which rate constant is "forward" and which is "reverse," inverting the ratio $k_f/k_r$.

**4. Error analysis**
- Variables & ranges: a student claim that equilibrium means the reaction has stopped.
- Constraint: correction must invoke the dynamic (still-occurring, equal-rate) nature of equilibrium.
- Contexts: any equilibrium system.
- Formats: short-answer.
- Worked instantiation: "A student says: 'At equilibrium, the reaction has completely stopped, since concentrations don't change.' What's wrong?" → Both the forward and reverse reactions are still occurring continuously at equilibrium; they simply proceed at equal rates, so their effects on concentration cancel out macroscopically — the reaction has not stopped, it has balanced.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 K-from-rate-constants problems, including at least one reversed reaction. |
| Group discussion | Understand | Debate why "equilibrium" and "no reaction occurring" are different ideas. |
| Quiz | Apply | One K-calculation item, one reversal item. |
| Exam | Analyze | Combine with Objective 14.1b (interpret the resulting K's magnitude). |
| Project/activity | Evaluate | Research a real reaction's forward/reverse rate constants and compute K. |

## Objective 14.1b: Interpret the magnitude of K

### Target understanding

A student can state what $K\gg1$ and $K\ll1$ imply about which side is favored at equilibrium, without over-claiming a precise quantitative product/reactant ratio from $K$ alone.

### Question guides

**1. Forward — classify by magnitude**
- Variables & ranges: several given $K$ values (e.g., $10^{-8}$, 0.5, 50, $10^6$).
- Constraint: classify each as strongly reactant-favored, roughly balanced, or strongly product-favored.
- Contexts: any set of equilibrium reactions.
- Formats: short-answer or multiple-choice.
- Worked instantiation: "A reaction has $K=2.3\times10^{-9}$. What does this tell you about the equilibrium mixture?" → Essentially no product forms — the reaction is overwhelmingly reactant-favored.

**2. Conceptual — what K does NOT tell you**
- Variables & ranges: a prompt about whether K alone gives an exact product/reactant ratio.
- Constraint: answer must note the dependence on stoichiometry and starting amounts.
- Contexts: any reaction with unequal reactant/product coefficients.
- Formats: short-answer.
- Worked instantiation: "Does a larger K always mean a higher percent yield of product, regardless of the reaction's stoichiometry?" → Not necessarily precisely — $K$'s magnitude reliably indicates which side is favored, but the exact quantitative split between reactants and products at equilibrium also depends on the reaction's stoichiometric coefficients and the starting concentrations, not on $K$ alone.

**3. Comparison — two reactions**
- Variables & ranges: two reactions with different K values at the same temperature.
- Constraint: comparison must be justified by K's magnitude alone.
- Contexts: any two unrelated equilibrium reactions.
- Formats: short-answer.
- Worked instantiation: reaction 1 has $K=10^3$; reaction 2 has $K=10^{-3}$. Which reaction goes "more nearly to completion" in the forward direction?

**4. Error analysis**
- Variables & ranges: a claim that $K\gg1$ means the reaction is fast.
- Constraint: correction must distinguish thermodynamic favorability (K) from kinetics (rate), reconnecting to Chapter 13.
- Contexts: any reaction with large K but slow observed rate (e.g., diamond → graphite).
- Formats: short-answer.
- Worked instantiation: "Diamond converting to graphite has a very large K at room temperature, yet diamonds are stable for practical purposes. Explain why this isn't a contradiction." → $K$ describes the equilibrium *position* (thermodynamic favorability), not how *fast* equilibrium is reached; a reaction can be strongly product-favored ($K\gg1$) while still having a negligible rate at a given temperature, exactly as Chapter 13 established with activation energy.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | Classify 3–4 given K values by favored side. |
| Group discussion | Analyze | Discuss the diamond/graphite-style rate-vs-equilibrium distinction. |
| Quiz | Understand | One classification item. |
| Exam | Analyze | Combine with a rate-constant-derivation problem (Objective 14.1a). |
| Project/activity | Evaluate | Look up a real reaction's K and rate, and discuss whether they align with intuition. |

## Objective 14.2a: Write and convert K_c/K_p for homogeneous gas-phase equilibria

### Target understanding

A student can write $K_c$ and $K_p$ expressions for a gas-phase reaction and convert between them using $K_p=K_c(RT)^{\Delta n}$, correctly determining $\Delta n$ from the balanced equation.

### Question guides

**1. Forward — convert K_p to K_c**
- Variables & ranges: a balanced gas-phase equation, given $K_p$ and temperature.
- Constraint: correct sign and value of $\Delta n$.
- Contexts: any gas-phase equilibrium with unequal moles of gas.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{2NH3<=>N2+3H2}$, $K_p=15.6$ at 490 K, $K_c=0.00964$).

**2. Inverse — convert K_c to K_p**
- Variables & ranges: given $K_c$ and temperature, find $K_p$.
- Constraint: correct application of $K_p=K_c(RT)^{\Delta n}$ without inverting the exponent's sign.
- Contexts: a different gas-phase reaction with a different $\Delta n$.
- Formats: workout.
- Worked instantiation: for a reaction with $\Delta n=-1$, given $K_c$ and $T$, find $K_p$.

**3. Conceptual — when does K_p = K_c?**
- Variables & ranges: reactions with $\Delta n=0$ vs. $\Delta n\neq0$.
- Constraint: explanation must reference the exponent in $K_p=K_c(RT)^{\Delta n}$.
- Contexts: e.g., $\ce{H2+I2<=>2HI}$ ($\Delta n=0$) vs. $\ce{2NH3<=>N2+3H2}$ ($\Delta n=2$).
- Formats: short-answer.
- Worked instantiation: "For which of these two reactions does $K_p=K_c$ exactly, regardless of temperature?" → $\ce{H2+I2<=>2HI}$, because $\Delta n=2-(1+1)=0$, making $(RT)^{\Delta n}=1$.

**4. Error analysis**
- Variables & ranges: a flawed $\Delta n$ calculation (e.g., using total moles instead of moles of gas only, or reactants-minus-products instead of products-minus-reactants).
- Constraint: correction must restate $\Delta n=$ (moles of gaseous product) − (moles of gaseous reactant).
- Contexts: any gas-phase reaction.
- Formats: short-answer.
- Worked instantiation: "A student computes $\Delta n$ for $\ce{2NH3<=>N2+3H2}$ as $2-(1+3)=-2$. What's the error, and what should $\Delta n$ be?" → $\Delta n$ is products minus reactants, not reactants minus products; the correct value is $(1+3)-2=+2$.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 K_p/K_c conversions across different Δn values. |
| Group discussion | Understand | Discuss why K_p = K_c(RT)^Δn follows directly from P = cRT (Ch. 5). |
| Quiz | Apply | One conversion problem. |
| Exam | Analyze | Combine with a K_c calculation from equilibrium concentrations (ties to Objective 14.3a). |
| Project/activity | Evaluate | Look up a real industrial gas-phase equilibrium's reported K_p and K_c and verify the conversion. |

## Objective 14.2b: Write equilibrium expressions for liquid-phase and heterogeneous equilibria

### Target understanding

A student can correctly omit bulk solvent (when appropriate) from a liquid-phase equilibrium expression, and correctly omit pure solids and pure liquids from a heterogeneous equilibrium expression — explicitly, every time, not just when reminded.

### Question guides

**1. Forward — write a heterogeneous expression**
- Variables & ranges: a reaction with a mix of solid, liquid, and gas phases.
- Constraint: pure solid/liquid species must be crossed out before the final expression is written.
- Contexts: decomposition reactions, precipitation-adjacent equilibria (preview of Ch. 16's $K_{sp}$).
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{CaCO3(s)<=>CaO(s)+CO2(g)}$, $K_p=P_{\ce{CO2}}$).

**2. Conceptual — why pure solids/liquids are omitted**
- Variables & ranges: a "why" prompt about pure-phase omission.
- Constraint: explanation must reference constant "concentration" (density/molar mass) of a pure solid or liquid.
- Contexts: any heterogeneous equilibrium.
- Formats: short-answer.
- Worked instantiation: "Why doesn't the amount of solid $\ce{CaCO3}$ present affect the equilibrium expression?" → A pure solid's "concentration" is its density divided by molar mass, a constant that doesn't change whether there's a little or a lot of it present — so it can't meaningfully appear as a variable in the expression.

**3. Predict-the-effect — adding more solid**
- Variables & ranges: a heterogeneous equilibrium with a pure solid reactant or product.
- Constraint: prediction must state no shift, referencing the omission rule.
- Contexts: any solid/gas heterogeneous system.
- Formats: short-answer.
- Worked instantiation: given the $\ce{CaCO3}$ system at equilibrium, predict what happens to $P_{\ce{CO2}}$ if half the solid $\ce{CaCO3}$ is removed (as long as some remains).

**4. Error analysis**
- Variables & ranges: a flawed expression that includes a pure solid or the bulk solvent.
- Constraint: correction must identify and remove the incorrectly included species.
- Contexts: any liquid-phase or heterogeneous reaction, including the acetic acid/water example.
- Formats: short-answer.
- Worked instantiation: "A student writes $K_c=\dfrac{[\ce{CH3COO-}][\ce{H3O+}][\ce{H2O}]}{[\ce{CH3COOH}]}$ for acetic acid ionizing in water. What's wrong?" → Water is the bulk solvent, present in large excess with a nearly constant concentration; it should be absorbed into the constant, not written explicitly — the correct expression omits $[\ce{H2O}]$.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 expression-writing problems mixing homogeneous, liquid-phase, and heterogeneous cases. |
| Group discussion | Understand | Discuss why "pure" matters — a solution of CaCO₃ would behave differently than solid CaCO₃. |
| Quiz | Apply | One heterogeneous-expression item. |
| Exam | Analyze | Require identifying and justifying every omitted species in a mixed-phase system. |
| Project/activity | Evaluate | Preview Ch. 16's $K_{sp}$ expressions as heterogeneous equilibria of this same type. |

## Objective 14.2c: Combine equilibrium constants for multi-step reactions

### Target understanding

A student can recognize when a target reaction is the sum of two (or more) given reactions and calculate its equilibrium constant as the product of the individual constants.

### Question guides

**1. Forward — combine two reactions**
- Variables & ranges: two given reactions and their $K$ values, and a target reaction equal to their sum.
- Constraint: verify by addition (species must actually cancel) before multiplying $K$'s.
- Contexts: any pair of reactions summing to a third.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($K_{c1}=490$, $K_{c2}=0.0149$, $K_{c3}=7.30$).

**2. Inverse — find a missing K given the combined result**
- Variables & ranges: given the target reaction's $K$ and one of the two component $K$'s, solve for the other.
- Constraint: correct division rather than multiplication.
- Contexts: the same three-reaction system, rearranged.
- Formats: workout.
- Worked instantiation: given $K_{c3}=7.30$ and $K_{c1}=490$, find $K_{c2}$.

**3. Conceptual — reaction 3 is reaction 1 minus reaction 2**
- Variables & ranges: a target reaction equal to reaction 1 *minus* reaction 2 (i.e., reaction 1 plus the reverse of reaction 2).
- Constraint: student must recognize that subtracting a reaction means using the *reciprocal* of its K.
- Contexts: any three-reaction combination involving a reversed step.
- Formats: short-answer.
- Worked instantiation: "If reaction 3 = reaction 1 − reaction 2, how should $K_{c3}$ be calculated from $K_{c1}$ and $K_{c2}$?" → $K_{c3}=K_{c1}\times(1/K_{c2})=K_{c1}/K_{c2}$, since subtracting reaction 2 is equivalent to adding its reverse, whose $K$ is $1/K_{c2}$.

**4. Error analysis**
- Variables & ranges: a student who adds the two $K$ values instead of multiplying.
- Constraint: correction must connect back to the derivation (rates multiply through the shared intermediate, not add).
- Contexts: the same CoO/CO/Co/H₂O system.
- Formats: short-answer.
- Worked instantiation: "A student computes $K_{c3}=490+0.0149=490.01$. What's the correct method, and why is addition wrong?" → Equilibrium constants for summed reactions *multiply* ($K_{c3}=K_{c1}\times K_{c2}=7.30$), not add — this mirrors Hess's law for enthalpies being additive, but the equilibrium-constant version is multiplicative because $K$ comes from an exponential/ratio relationship, not a directly additive one.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2 multi-step K combination problems. |
| Group discussion | Analyze | Compare this multiplicative rule to Hess's law's additive rule (Ch. 6) and discuss why they differ. |
| Quiz | Apply | One combination problem. |
| Exam | Analyze | Require recognizing a reversed component reaction (subtraction case). |
| Project/activity | Evaluate | Research a real multi-step industrial equilibrium process and its reported step-wise K values. |

## Objective 14.3a: Calculate Q and compare to K to predict reaction direction

### Target understanding

A student can calculate the reaction quotient from a given (possibly non-equilibrium) set of concentrations and correctly predict the reaction's direction by comparing $Q$ to $K$.

### Question guides

**1. Forward — Q < K case**
- Variables & ranges: a set of non-equilibrium concentrations and a known $K$.
- Constraint: student must calculate both $K$ (if not given directly) and $Q$ using the identical expression.
- Contexts: any homogeneous equilibrium.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{2SO2+O2<=>2SO3}$, $Q_c=0.61<K_c=4.3$, proceeds forward).

**2. Inverse — Q > K case**
- Variables & ranges: a different set of concentrations for the same reaction, giving $Q>K$.
- Constraint: student must recognize the reverse-direction case, not just repeat the forward-direction procedure.
- Contexts: same reaction, contrasting mixture.
- Formats: workout.
- Worked instantiation: see the study guide's second worked example ($Q_c=195\gg K_c=4.3$, proceeds in reverse).

**3. Conceptual — Q = K**
- Variables & ranges: a mixture where calculated $Q$ exactly equals a given $K$.
- Constraint: answer must state the system is already at equilibrium, no net shift.
- Contexts: any equilibrium system.
- Formats: short-answer.
- Worked instantiation: "If $Q_c$ calculated from a mixture equals $K_c$ exactly, what happens next?" → Nothing — the system is already at equilibrium, so forward and reverse rates are already equal and no net shift occurs.

**4. Error analysis**
- Variables & ranges: a student who compares $Q$ and $K$ correctly but miscalculates $Q$ by using equilibrium-style stoichiometric assumptions instead of the given concentrations directly.
- Constraint: correction must emphasize that $Q$ uses whatever concentrations are handed to you, not a re-derived equilibrium value.
- Contexts: any Q-vs-K problem.
- Formats: short-answer.
- Worked instantiation: "A student is given non-equilibrium concentrations but sets up an ICE table to 'find' Q instead of substituting the given values directly. What's the error?" → $Q$ is calculated directly from whatever concentrations are given at that moment — no ICE table or equilibrium assumption is needed or appropriate; ICE tables are for finding *unknown* equilibrium concentrations (Objective 14.4a), a different task entirely.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 Q-vs-K problems covering all three comparison cases. |
| Group discussion | Analyze | Debate why Q and K use an identical formula yet serve different diagnostic purposes. |
| Quiz | Apply | One Q-vs-K item per exam form, varying which direction results. |
| Exam | Analyze | Require justifying the predicted direction in terms of the reaction proceeding to relieve the Q/K imbalance. |
| Project/activity | Evaluate | Given a real reaction's K and a proposed non-equilibrium mixture, predict direction and justify. |

## Objective 14.4a: Set up and solve an ICE table for equilibrium concentrations

### Target understanding

A student can build a correct ICE table from a balanced equation and initial concentrations, substitute into the K expression, and solve for equilibrium concentrations — including recognizing when the algebra simplifies to a perfect square.

### Question guides

**1. Forward — perfect-square case**
- Variables & ranges: a reaction where reactant and product stoichiometric coefficients on each side are equal, giving a squared ratio.
- Constraint: student must recognize the perfect-square shortcut (take the square root of both sides) rather than expanding a full quadratic.
- Contexts: esterification-type or similar 1:1:1:1 reactions.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (acetic acid + ethanol, $K_c=4.0$, $x=0.10$).

**2. Inverse — find initial concentration from equilibrium data**
- Variables & ranges: given final equilibrium concentrations and $K$, back-calculate an initial concentration.
- Constraint: correct reconstruction of the ICE table in reverse.
- Contexts: the same or a similar 1:1:1:1 reaction.
- Formats: workout.
- Worked instantiation: given equilibrium concentrations and $K_c=4.0$, find the original initial concentration of acetic acid (assuming equal initial acetic acid and ethanol, no initial products).

**3. Conceptual — why the Change row uses coefficients**
- Variables & ranges: a reaction with unequal stoichiometric coefficients (e.g., 1:3:2 as in ammonia synthesis).
- Constraint: explanation must connect the Change row's multiples of $x$ to the balanced equation's coefficients.
- Contexts: $\ce{N2+3H2<=>2NH3}$-style ICE tables.
- Formats: short-answer.
- Worked instantiation: "In an ICE table for $\ce{N2+3H2<=>2NH3}$, why does $\ce{H2}$'s Change row use $-3x$ while $\ce{N2}$'s uses $-x$?" → The Change row must reflect the reaction's actual stoichiometric ratios — for every 1 mol of $\ce{N2}$ consumed, 3 mol of $\ce{H2}$ are consumed simultaneously, so the same reaction-progress variable $x$ is scaled by each species' own coefficient.

**4. Error analysis**
- Variables & ranges: an ICE table with a sign error (treating a product's Change row as negative) or a coefficient error (forgetting to multiply $x$ by the coefficient).
- Constraint: correction must restate the Change-row sign/coefficient convention.
- Contexts: any ICE-table problem with coefficients other than 1.
- Formats: short-answer.
- Worked instantiation: "A student writes the Change row for a product with coefficient 2 as $+x$ instead of $+2x$. What's the consequence of this error?" → Every downstream equilibrium concentration and the final calculated $x$ will be wrong, because the ICE table no longer reflects the actual reaction stoichiometry — the product's equilibrium concentration would be understated by a factor of 2 relative to how much reactant was actually consumed.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 ICE-table problems, including at least one with unequal coefficients. |
| Group discussion | Analyze | Discuss why some ICE-table equations simplify to a perfect square and others don't. |
| Quiz | Apply | One straightforward ICE-table problem. |
| Exam | Analyze | Require setting up the ICE table explicitly (not just the final answer) for partial credit and error-checking. |
| Project/activity | Evaluate | Given real equilibrium data for a reaction, back-calculate K using an ICE-table-consistent setup. |

## Objective 14.4b: Apply and validate the small-x approximation

### Target understanding

A student can recognize when $K$ is small enough to justify approximating $[\ce{A}]_0-x\approx[\ce{A}]_0$, solve the simplified equation, and check afterward whether the approximation was actually valid.

### Question guides

**1. Forward — apply and check the approximation**
- Variables & ranges: a small $K$ (e.g., $10^{-4}$ to $10^{-6}$ range) and a moderate initial concentration.
- Constraint: student must perform the validity check ($x/[\ce{A}]_0 < 5\%$) explicitly, not just assume it holds.
- Contexts: dissociation-type equilibria with small K (preview of Ch. 15's weak-acid $K_a$ problems).
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{N2O4<=>2NO2}$, $K_c=1.20\times10^{-4}$, valid at 0.77%).

**2. Inverse — recognize when the approximation fails**
- Variables & ranges: a larger $K$ or smaller initial concentration that pushes $x/[\ce{A}]_0$ above 5%.
- Constraint: student must identify the failure and describe the correct next step (exact quadratic).
- Contexts: the same reaction type with a less favorable ratio of $K$ to $[\ce{A}]_0$.
- Formats: workout (partial: identify failure, set up the exact equation without necessarily solving it by hand).
- Worked instantiation: repeat the $\ce{N2O4}$ calculation with $[\ce{N2O4}]_0=0.010$ M instead of 0.500 M, and show that the approximation is no longer valid.

**3. Conceptual — why is 5% the threshold?**
- Variables & ranges: a conceptual prompt about the approximation's purpose.
- Constraint: explanation must reference trading a small, quantifiable error for algebraic simplicity.
- Contexts: any small-K equilibrium.
- Formats: short-answer.
- Worked instantiation: "Why is a 5% threshold used to judge whether the small-x approximation is acceptable, rather than requiring x to be exactly zero?" → No approximation is ever perfectly exact; the 5% threshold is a practical convention balancing algebraic convenience against acceptable error in the final answer — beyond it, the error becomes large enough to noticeably distort the result.

**4. Error analysis**
- Variables & ranges: a student who applies the approximation without ever checking it.
- Constraint: correction must require the explicit validity check as a mandatory last step.
- Contexts: any small-x approximation problem.
- Formats: short-answer.
- Worked instantiation: "A student solves an ICE table using the small-x approximation and reports the answer without checking $x/[\ce{A}]_0$. What step did they skip, and why does it matter?" → They skipped verifying the approximation's validity; without that check, there's no way to know whether the simplified answer is trustworthy or whether the exact quadratic should have been solved instead.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2 small-x approximation problems, one that validates and one that fails. |
| Group discussion | Analyze | Discuss the tradeoff between algebraic convenience and accuracy. |
| Quiz | Apply | One approximation problem with a required validity check. |
| Exam | Analyze | Require both applying the approximation and explicitly justifying (or rejecting) its validity. |
| Project/activity | Evaluate | Preview how this exact technique reappears for weak-acid $K_a$ problems in Chapter 15. |

## Objective 14.5a: Apply Le Chatelier's principle across all stress types

### Target understanding

A student can predict the direction of an equilibrium shift for a concentration, pressure/volume, or temperature change, and can explain that a catalyst affects neither the equilibrium position nor the value of $K$.

### Question guides

**1. Forward — concentration stress**
- Variables & ranges: adding or removing a reactant or product from an equilibrium system.
- Constraint: prediction must be framed as "partially offsetting" the stress, not "completely reversing" it.
- Contexts: any homogeneous or heterogeneous equilibrium.
- Formats: short-answer.
- Worked instantiation: see the study guide's worked example (removing product C from $\ce{A+B<=>C}$ shifts equilibrium forward).

**2. Forward — pressure/volume stress**
- Variables & ranges: a gas-phase reaction with unequal moles of gas on each side, container volume changed.
- Constraint: prediction must reference moles of gas on each side, not just "more pressure = more product."
- Contexts: the Haber process or a similar Δn ≠ 0 reaction.
- Formats: short-answer.
- Worked instantiation: see the study guide's worked example (compressing $\ce{N2+3H2<=>2NH3}$ favors the product side).

**3. Forward — temperature stress**
- Variables & ranges: a reaction with known sign of $\Delta H$, temperature raised or lowered.
- Constraint: prediction must state that increasing T favors the endothermic direction (and that K itself changes), distinct from the other two stress types.
- Contexts: the $\ce{2NO2<=>N2O4}$ system or an analogous reaction.
- Formats: short-answer.
- Worked instantiation: see the study guide's worked example (warming the NO₂/N₂O₄ tubes shifts toward more brown NO₂).

**4. Error analysis — catalyst**
- Variables & ranges: a claim that a catalyst increases equilibrium yield.
- Constraint: correction must state that a catalyst speeds up *both* directions equally, changing neither the equilibrium position nor $K$.
- Contexts: any catalyzed reversible reaction.
- Formats: short-answer.
- Worked instantiation: "A student claims adding a catalyst to a reaction at equilibrium will produce more product. Is this correct?" → No — a catalyst lowers the activation energy for the forward and reverse reactions equally (Chapter 13), so it only speeds up how quickly equilibrium is reached; it does not change the equilibrium position or the value of $K$, and therefore does not increase the ultimate yield.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | One question per stress type (concentration, pressure/volume, temperature, catalyst). |
| Group discussion | Analyze | Debate why temperature is the only stress that changes K itself. |
| Quiz | Understand/Apply | One or two stress-prediction items, mixing types. |
| Exam | Analyze | Require identifying the stress type first, then predicting the shift and stating whether K changes. |
| Project/activity | Evaluate | Research a real industrial or environmental equilibrium system and analyze how each stress type would affect it (e.g., ocean CO₂/carbonate equilibrium under warming). |

## Rubric Themes for Chapter 14

| Evidence of mastery | What to look for |
|---|---|
| Q and K never conflated | Student always states which concentrations (given vs. equilibrium) go into a Q or K calculation before comparing them. |
| Pure solids/liquids/solvent explicitly omitted | Student visibly crosses out or states the omission of pure-phase species before writing a final equilibrium expression, every time. |
| K_p/K_c conversion applied only when needed | Student checks whether the given data's units match before invoking $K_p=K_c(RT)^{\Delta n}$, and gets the sign of $\Delta n$ right. |
| Small-x approximation always checked | Student never reports an approximated answer without an explicit $x/[\ce{A}]_0$ validity check. |
| Stress type identified before predicting a shift | Student names the stress type (concentration/pressure-volume/temperature/catalyst) explicitly before predicting a direction. |
| K changes only with temperature | Student correctly states that concentration, pressure/volume, and catalyst changes shift equilibrium position but never change K, while temperature changes both. |
