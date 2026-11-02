{{nyml
kind: document
format: 1
title: Chapter 17: Entropy, Free Energy, and Equilibrium
}}

# Chapter 17: Entropy, Free Energy, and Equilibrium

:::info
**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 17 (CC BY 4.0)
**Audience:** introductory undergraduate general chemistry, second semester
**Package license:** CC BY 4.0
**Note:** builds on standard enthalpies of formation and Hess's law (Chapter 6) and the equilibrium constant (Chapter 14); facts checked for accuracy against OpenStax *Chemistry 2e* and Wikipedia (used for reference only — no text or figures adapted from either).
:::

:::success
**Chapter Learning Objectives**
- Define entropy in terms of microstates, predict the sign of $\Delta S$, and calculate $\Delta S^\circ_\text{rxn}$ from tabulated values.
- State the four laws of thermodynamics, especially the second law as the criterion for spontaneity.
- Define Gibbs free energy, calculate $\Delta G^\circ_\text{rxn}$, find phase-transition/reaction-onset temperatures, and relate $\Delta G^\circ$ to K.
:::

## Chapter Logic

Chapter 6 tracked energy as heat ($\Delta H$). This chapter asks a deeper question: not how much heat a reaction releases, but *why* it happens at all — and the answer reconnects directly to Chapter 14's equilibrium constant. ==Every reaction in this course has had a $K$; this chapter finally explains where that number comes from.==

{{mermaid
graph TD
  A["Entropy (S = k ln W):<br/>microstates & disorder"] --> B["Second law:<br/>total universe entropy increases"]
  B --> C["Gibbs free energy:<br/>G = H - TS"]
  C --> D["Delta G = Delta H - T Delta S<br/>sign determines spontaneity"]
  D --> E["Delta G-naught = -RT ln K<br/>links back to Ch. 14's K"]
}}

**Visual description:** entropy's microstate definition leads to the second law (spontaneity requires increasing universe entropy), which motivates Gibbs free energy as a system-only spontaneity criterion (at constant temperature and pressure). Free energy's sign determines spontaneity, and its standard value connects directly back to the equilibrium constant from Chapter 14.

## 17.1 Entropy{{attrs[#blk-ch17sec01]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 17.1a}} Define entropy in terms of microstates (S = k ln W).
- {{sp[info] Objective 17.1a}} Predict the sign of $\Delta S$ for a physical or chemical process.
- {{sp[info] Objective 17.1b}} Calculate the standard entropy of a reaction from tabulated values.
:::

### Spontaneity: two competing tendencies

A **spontaneous** process is one that occurs by itself under the given conditions, without being driven. Two separate tendencies decide whether it does:

1. **Does it release or absorb heat?** Systems tend toward lower energy.
2. **Does it increase or decrease disorder?** Systems tend toward more disorder.

When both point the same way the answer is settled before any calculation. When they disagree, ==the winner depends on temperature — and that single fact is what the rest of the chapter makes quantitative.==

![Four quadrants of enthalpy and entropy sign combinations, showing which are spontaneous always, never, or only above or below a crossover temperature](../assets/spontaneity_quadrants.svg)
*Figure 17.1 — The top-left and bottom-right cells need no arithmetic: both tendencies agree. The other two are a contest between $\Delta H$ and $T\Delta S$, and the crossover sits at $T = \Delta H/\Delta S$. Self-generated with matplotlib.*

Figure 17.1 is worth returning to after §17.3, because everything in that section is a way of putting numbers on these four boxes. Notice already that "exothermic" is **not** the same as "spontaneous" — the bottom-left cell is exothermic and still fails above its crossover temperature, and the top-right cell is endothermic and succeeds above its own.

### Entropy and microstates

**Entropy** ($S$) measures disorder — precisely, a logarithmic measure of the number of equivalent ways ($W$, the number of **microstates**) a system's particles can be arranged:

$$S=k\ln W \qquad k=1.38\times10^{-23}\ \text{J/K (Boltzmann constant)}$$

![Distributing 4 particles between 2 boxes: 5 distributions with 1, 4, 6, 4, and 1 microstates](../assets/microstates_distribution.svg)
*Figure 17.2 — Four particles distributed between two boxes have $2^4=16$ total microstates, grouped into 5 distributions with 1, 4, 6, 4 and 1 microstates respectively. Self-generated with matplotlib.*

Read Figure 17.2 carefully, because it contains the whole idea in miniature. A **distribution** is what you can actually see — how many particles are in each box, ignoring which particle is which. A **microstate** is a specific labeled arrangement. The even split has **six** microstates while "all four on the left" has only **one**, so the even split is six times more likely to be found. **Systems drift toward high-entropy arrangements for no deeper reason than that there are more ways to be in them.**

With four particles the bias is mild. With a mole of them the most probable distribution outnumbers the extremes by a factor so large that the extreme is never observed at all — which is why entropy behaves like a law rather than a tendency.

**Entropy is a state function** — like enthalpy (Chapter 6), $\Delta S=S_f-S_i$ depends only on initial and final states, never on the path taken:

$$\Delta S=k\ln W_f-k\ln W_i=k\ln\frac{W_f}{W_i}$$

:::: tabs
::: tab Problem
A system of 3 particles is distributed between 2 boxes. (a) How many microstates in total? (b) List the distributions and the number of microstates in each. \(c) Which distribution has the highest entropy, and by what factor is it more probable than the least? (d) What changes when the system has $6\times10^{23}$ particles?
:::
::: tab Solution
**(a)** Each particle independently chooses one of two boxes, so $2^3 = 8$ microstates.

**(b)** Group them by what is observable — how many are on the left:

| Distribution | Microstates | Count |
|---|---|---|
| 3 left, 0 right | LLL | 1 |
| 2 left, 1 right | LLR, LRL, RLL | 3 |
| 1 left, 2 right | LRR, RLR, RRL | 3 |
| 0 left, 3 right | RRR | 1 |

Total $1+3+3+1 = 8$ ✓ — and these are the binomial coefficients, which is why Figure 17.2's four-particle case gives 1, 4, 6, 4, 1.

**\(c) The even-as-possible splits (2:1 and 1:2) tie for highest**, at 3 microstates each:

$$S = k\ln W = (1.38\times10^{-23})\ln 3 = 1.52\times10^{-23}\ \text{J/K}$$

against $S = k\ln 1 = 0$ for the all-on-one-side case. The even split is **3 times more probable**.

**(d) The ratio becomes unimaginable.** With $N$ particles the most probable distribution outnumbers the extreme by roughly $N!/[(N/2)!]^2$, and at $N = 6\times10^{23}$ that number has more than $10^{23}$ digits. **The tendency stops being a tendency and becomes, in practice, an absolute rule** — you will never see all the air in a room drift into one corner, not because it is forbidden but because the odds are beyond astronomical.

**Why this matters for the rest of the chapter:** the second law is not a separate law of nature so much as a statement about counting. Systems end up in high-entropy states because there are overwhelmingly more of them.
:::
::::

### Predicting the sign of $\Delta S$

**General trends:** for a given substance, gas ≫ liquid > solid (more accessible microstates as freedom of motion increases); at the same state, more complex molecules have higher entropy (more ways to distribute energy among more atoms/bonds).

![Bar chart of standard molar entropies for four solids, three liquids and six gases](../assets/entropy_trends.svg)
*Figure 17.3 — Both trends in one chart. Phase dominates: even the most complex liquid here sits below the simplest gas. Within a phase, complexity raises entropy; across the whole chart, values run from diamond (solid) at 2.4 to butane (gas) at 310 $\text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$, a factor of 130. Self-generated with matplotlib from commonly cited standard thermodynamic data.*

Two details in Figure 17.3 repay a second look. **Diamond has the lowest entropy on the chart** (2.4 $\text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$) because every carbon is locked rigidly in place — graphite, whose sheets can slide, is already more than twice as high. And **water appears twice**: 69.9 as a liquid and 188.8 as a gas. Same substance, same temperature (298 K), nearly a threefold jump — the phase change is by far the largest single entropy effect in the chapter.

To predict the sign of an entropy change, you will usually not need a table at all. **Count the moles of gas on each side**; if that changes, it dominates everything else.

### Standard entropy of reaction


For a reaction, standard entropy of reaction is calculated the same way as Chapter 6's $\Delta H^\circ_\text{rxn}$, but using absolute standard entropies $S^\circ$, which are not zero for elements:

$$\Delta S^\circ_\text{rxn}=\sum n S^\circ(\text{products})-\sum m S^\circ(\text{reactants})$$

{{sp[warning] Reminder}} more gas moles produced → $\Delta S^\circ_\text{rxn}$ is generally positive; fewer gas moles → generally negative; no net change in gas moles → small in magnitude, either sign.

:::: tabs
::: tab Problem
Calculate $\Delta S^\circ_\text{rxn}$ for $\ce{4Fe(s) + 3O2(g) -> 2Fe2O3(s)}$ at 25 °C. ($S^\circ$: $\ce{Fe(s)}=27.3$, $\ce{O2(g)}=205.2$, $\ce{Fe2O3(s)}=87.4$ J/K·mol)
:::
::: tab Solution
$$\Delta S^\circ_\text{rxn}=2(87.4)-[4(27.3)+3(205.2)]=174.8-(109.2+615.6)=-550\ \text{J/K·mol}$$

This makes sense: 3 mol of gas are consumed and 0 mol of gas are produced, so $\Delta S^\circ_\text{rxn}$ should be — and is — strongly negative.

{{sp[warning] Two things that differ from $\Delta H^\circ$}} **Elements do not have $S^\circ = 0$.** $\ce{Fe(s)}$ contributes 27.3 and $\ce{O2(g)}$ contributes 205.2 — unlike $\Delta H^\circ_f$, where elements in their standard states are defined as zero. And **$S^\circ$ values are in J**, not kJ; mixing them with kJ enthalpies is the single commonest error in §17.3.
:::
::::

:::: tabs
::: tab Problem
Predict the sign of $\Delta S$ for each, without any table: (a) $\ce{H2O(l) -> H2O(g)}$; (b) $\ce{2SO2(g) + O2(g) -> 2SO3(g)}$; \(c) $\ce{NH4NO3(s) -> NH4+(aq) + NO3-(aq)}$; (d) $\ce{N2(g) + O2(g) -> 2NO(g)}$; (e) a gas expanding into a vacuum.
:::
::: tab Solution
Work down a fixed priority list: **phase change first, then moles of gas, then dissolving, then complexity.**

**(a) Positive, and large.** A liquid becoming a gas is one of the biggest entropy increases available — Figure 17.3 shows the jump for water is 69.9 → 188.8 $\text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$.

**(b) Negative.** Count gas moles: 3 on the left, 2 on the right. Fewer gas particles means fewer accessible microstates.

**\(c) Positive.** An ordered crystal becomes free ions dispersed through a solvent. (This is the instant cold pack from Chapter 12 — endothermic, and spontaneous only because $\Delta S$ is positive enough to overcome it.)

**(d) Small, sign not obvious.** Two moles of gas become two moles of gas, so the dominant effect is absent. What remains is a minor difference in molecular complexity, and the value happens to be $+24.8\ \text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$ — small, as predicted.

**(e) Positive.** More volume means more positions available to each particle, so $W$ rises. No chemistry occurs at all; this is entropy in its purest form.

**The rule that decided (a) and (b):** if the number of moles of gas changes, that change sets the sign and nothing else matters much. Only when gas moles are balanced and no phase change, dissolving, or expansion occurs, as in (d), do you need finer reasoning — and then the magnitude will be small.
:::
::::

:::: tabs
::: tab Problem
Calculate $\Delta S^\circ_\text{rxn}$ for $\ce{CaCO3(s) -> CaO(s) + CO2(g)}$. ($S^\circ$: $\ce{CaCO3}=92.9$, $\ce{CaO}=39.8$, $\ce{CO2}=213.8\ \text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$.) Check the sign against the gas-mole rule.
:::
::: tab Solution
$$\Delta S^\circ_\text{rxn} = [S^\circ(\ce{CaO}) + S^\circ(\ce{CO2})] - S^\circ(\ce{CaCO3})$$
$$= (39.8 + 213.8) - 92.9 = 253.6 - 92.9 = +160.7\ \text{J K}^{-1}\text{mol}^{-1}$$

**Check against the rule:** zero moles of gas on the left, one on the right. Gas moles increase, so $\Delta S^\circ$ should be positive and substantial — and $+160.7$ is both.

**Where the number comes from, roughly.** Almost all of it is the $\ce{CO2}$ term: 213.8 of the 253.6 on the product side. The two solids only partly offset each other (39.8 against 92.9, a net −53.1). **Releasing a gas is the entropy story here, and the solids are bookkeeping.**

This is the reaction §17.3 returns to, and its positive $\Delta S^\circ$ paired with a positive $\Delta H^\circ$ puts it squarely in Figure 17.1's top-right quadrant — nonspontaneous cold, spontaneous hot.
:::
::::

**Self-check:**
- Without calculating, would you expect $\Delta S^\circ$ for $\ce{2H2(g) + O2(g) -> 2H2O(l)}$ to be positive or negative? Why?
- Rank $\ce{Al(s)}$, $\ce{H2O(l)}$, and $\ce{HF(g)}$ in order of increasing standard molar entropy.

> **Where this goes next.** §17.1 defined entropy and showed how to compute its change *for the system*. But the tendency toward disorder is a statement about the **universe**, not about any one beaker. §17.2 states that properly, and §17.3 turns it into something you can calculate without ever leaving the system.

## 17.2 The Laws of Thermodynamics{{attrs[#blk-ch17sec02]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 17.2a}} State the zeroth, first, second, and third laws of thermodynamics.
- {{sp[info] Objective 17.2a}} Explain the second law as the criterion for spontaneity.
- {{sp[info] Objective 17.2b}} Explain the third law's role in assigning absolute entropy values.
:::

### The four laws

- **Zeroth law:** if A and B are each in thermal equilibrium with C, then A and B are in thermal equilibrium with each other (this is what makes "temperature" a consistent, transitive concept).
- **First law:** energy is conserved — it changes form (heat, work) but is never created or destroyed (Chapter 6).
- **Second law:** ==in any spontaneous process, the total entropy of the universe (system + surroundings) increases.== This is the chapter's organizing principle.
- **Third law:** a perfect crystalline substance at absolute zero (0 K) has zero entropy — this is what lets us tabulate *absolute* entropy values (unlike enthalpy, which we only ever measure as a *change*, $\Delta H$).

### The second law as the criterion for spontaneity

The second law is the chapter's engine, and it is worth stating precisely because the loose version misleads. It does **not** say that disorder always increases everywhere. It says the **total** entropy of system plus surroundings increases:

$$\Delta S_\text{univ} = \Delta S_\text{sys} + \Delta S_\text{surr} > 0 \qquad \text{for any spontaneous process}$$

:::warning
A system's own entropy can fall during a perfectly spontaneous process — as long as the surroundings gain more than the system loses. Water freezing below 0 °C, a plant growing, a crystal forming from solution: all decrease the entropy of the thing you are looking at, and all are spontaneous, because each dumps enough heat into the surroundings to more than compensate. **"Entropy always increases" is guaranteed only for the universe (or any isolated system), not for an arbitrary chosen system.**
:::

That is also the practical problem with the second law: it requires knowing $\Delta S_\text{surr}$, which means tracking the rest of the universe. §17.3 exists to eliminate that requirement.

**Where it ends.** If every spontaneous process increases the universe's entropy, then the universe is running toward a maximum — a state in which no further entropy-increasing process, including computation and life, can be sustained. That endpoint has a name, the **heat death of the universe**, and it is the second law's long-range prediction.

:::: tabs
::: tab Problem
A student claims: "Life violates the second law — organisms build ordered structures from disordered raw materials, so entropy decreases." Rebut this precisely.
:::
::: tab Solution
**The claim misapplies the law to the wrong system.** The second law constrains $\Delta S_\text{univ}$, not $\Delta S$ of any chosen piece of the universe. An organism is not an isolated system.

**What actually happens.** Building ordered structures does lower the organism's own entropy — that part of the claim is correct. But doing so requires continuously consuming energy-rich, low-entropy inputs (food, or sunlight) and expelling high-entropy outputs: heat, $\ce{CO2}$, water, waste. The entropy exported to the surroundings exceeds the entropy reduction inside:

$$\Delta S_\text{univ} = \underbrace{\Delta S_\text{organism}}_{<0} + \underbrace{\Delta S_\text{surroundings}}_{\gg 0} > 0$$

**A number for scale.** A resting adult radiates roughly 100 W. Over a day that is about $8.6\times10^{6}$ J dumped into surroundings near 300 K, giving $\Delta S_\text{surr} \approx 8.6\times10^{6}/300 \approx 2.9\times10^{4}$ J/K — vastly more than the entropy decrease from any tissue built in that time.

**The general form of this rebuttal, which recurs:** *every* apparent violation of the second law turns out to be a local decrease paid for by a larger increase elsewhere. Water freezing, a crystal growing, a refrigerator cooling its interior, a cell dividing — same structure, same resolution. **Ask what the surroundings received.**

**And note what the law does not forbid:** it never says a system cannot become more ordered. It says the bill must be paid, in heat, somewhere else.
:::
::::

### The third law and absolute entropy

Figure 17.4 shows the substance that sits at the bottom of Figure 17.3's scale, and the third law is what lets its entropy be quoted as an absolute number at all.

![A cut diamond, a highly ordered crystalline solid](../assets/diamond.jpg =450x)
*Figure 17.4 — Diamond's standard entropy is $S^\circ=2.4$ J/K·mol at 25 °C — small because carbon atoms are locked into a highly ordered crystal lattice with few accessible microstates. The third law is what allows this to be reported as an absolute value (entropy relative to a perfect crystal at 0 K, where $S=0$) rather than only as a *change*.*

:::: tabs
::: tab Problem
Water freezing at −10 °C is spontaneous, yet the water's own entropy decreases. (a) Show how this is consistent with the second law. (b) At 0 °C, $\Delta H_\text{fus} = 6.01$ kJ/mol and $\Delta S_\text{fus} = 22.0\ \text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$ for melting. Compute $\Delta S_\text{sys}$, $\Delta S_\text{surr}$ and $\Delta S_\text{univ}$ for **freezing** one mole at 263 K (assume $\Delta H$ and $\Delta S$ are approximately independent of temperature), using $\Delta S_\text{surr} = -\Delta H_\text{sys}/T$.
:::
::: tab Solution
**(a)** The second law constrains the **universe**, not the beaker. Freezing releases heat into the surroundings, and that heat raises the surroundings' entropy. If the gain outside exceeds the loss inside, the total rises and the process is spontaneous.

**(b) Freezing is the reverse of melting**, so both quantities change sign:

$$\Delta H_\text{sys} = -6.01\ \text{kJ/mol} \qquad \Delta S_\text{sys} = -22.0\ \text{J K}^{-1}\text{mol}^{-1}$$

The system's entropy falls — liquid becoming an ordered crystal, exactly as expected.

$$\Delta S_\text{surr} = -\frac{\Delta H_\text{sys}}{T} = -\frac{-6010\ \text{J/mol}}{263\ \text{K}} = +22.85\ \text{J K}^{-1}\text{mol}^{-1}$$

$$\Delta S_\text{univ} = -22.0 + 22.85 = +0.85\ \text{J K}^{-1}\text{mol}^{-1} > 0$$

**Positive — so freezing at −10 °C is spontaneous**, despite the system becoming more ordered.

**Now repeat at 283 K (+10 °C)**, changing nothing but the temperature:

$$\Delta S_\text{surr} = \frac{6010}{283} = +21.24 \quad\Rightarrow\quad \Delta S_\text{univ} = -22.0 + 21.24 = -0.76 < 0$$

**Negative — freezing is not spontaneous at +10 °C**, which is the everyday observation this whole calculation had to reproduce.

**Why temperature is the deciding factor.** $\Delta S_\text{surr} = -\Delta H/T$ has $T$ in the denominator, so the *same* released heat buys **more** entropy in cold surroundings than in warm ones. Dumping 6 kJ into a cold room disturbs it more than dumping 6 kJ into a warm one. That single asymmetry is why ice forms in winter and melts in summer — and, as §17.3 shows, it is where the $T$ in $\Delta G = \Delta H - T\Delta S$ comes from.
:::
::::

:::: tabs
::: tab Problem
(a) Why can $\Delta H^\circ_f$ for an element in its standard state be *defined* as zero, while $S^\circ$ for that same element is a measured non-zero number? (b) Diamond has $S^\circ = 2.4\ \text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$ at 298 K. What is its entropy at 0 K, and how do you know? \(c) What would a *non*-crystalline solid such as glass have at 0 K?
:::
::: tab Solution
**(a) The difference is that entropy has a natural zero and enthalpy does not.**

Enthalpy is only ever measurable as a *change*; there is no experiment that returns the absolute enthalpy of a substance. So chemistry adopts a convention — elements in their standard states are assigned $\Delta H^\circ_f = 0$ — and every tabulated value is relative to that arbitrary choice.

Entropy needs no convention, because the **third law** supplies a real zero: a perfect crystal at 0 K has exactly one microstate ($W = 1$), and $S = k\ln 1 = 0$. Every $S^\circ$ is measured up from that genuine baseline, which is why they are called **absolute** entropies — and why they are never zero for anything at 298 K.

**(b) Zero.** Diamond is a near-perfect crystal, so at 0 K there is one arrangement and $S = 0$. The 2.4 $\text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$ is the entropy it has *acquired* on being warmed to 298 K — the smallest such value in Figure 17.3, because even at room temperature a diamond lattice barely moves.

**\(c) Slightly greater than zero.** Glass is frozen in a disordered arrangement, and cooling to 0 K does not let it find the single lowest-energy configuration — it is stuck in one of many, so $W > 1$ and $S > 0$. This leftover is called **residual entropy**, and it is exactly why the third law is stated for *perfect crystalline* substances.

**The chain worth holding onto:** third law → absolute entropies exist → $S^\circ$ can be tabulated → $\Delta S^\circ_\text{rxn}$ can be computed by simple subtraction, as in §17.1. Without the third law, §17.1's calculation would be impossible.
:::
::::

:::: tabs
::: tab Problem
Carbon monoxide has a measured residual entropy of about 4.6 $\text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$ at 0 K, while $\ce{N2}$ has essentially none. (a) Why does the third law permit this? (b) Show that $4.6\ \text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$ is consistent with roughly two orientations per molecule, using $S = k\ln W$. \(c) What does this imply for tabulated $S^\circ$ values of CO?
:::
::: tab Solution
**(a) The third law applies to a *perfect* crystal.** CO is very nearly symmetric — the two ends are almost indistinguishable in size and polarity — so as the crystal forms, molecules freeze in whichever way round they happened to be pointing. The result is a crystal with a frozen-in random pattern of CO and OC, which is not perfect. $\ce{N2}$ has genuinely identical ends, so no such disorder is possible.

**(b)** If each of $N_A$ molecules has 2 equally likely orientations, the crystal has $W = 2^{N_A}$ arrangements:

$$S = k\ln(2^{N_A}) = N_A k\ln 2 = R\ln 2 = (8.314)(0.693) = 5.76\ \text{J K}^{-1}\text{mol}^{-1}$$

The measured 4.6 is somewhat lower, which says the orientations are not *quite* equally likely — there is a slight energetic preference — but the order of magnitude confirms the two-orientation picture.

**Note the elegant step:** $N_A k = R$. Boltzmann's microscopic constant times Avogadro's number is the ordinary gas constant, which is the bridge between $S = k\ln W$ and every molar quantity in this chapter.

**\(c) $S^\circ$ values for CO obtained purely calorimetrically are slightly too low.** They are measured by integrating heat capacity upward from 0 K, which assumes $S = 0$ there. For CO that baseline is really 4.6, so every derived value inherits the same small offset.

**Why this rarely matters in practice:** the offset is constant, so it cancels in $\Delta S^\circ_\text{rxn}$ whenever CO appears on both sides with the same coefficient — and when it does not, 4.6 $\text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$ is small beside typical reaction entropies of tens to hundreds. It is a real limitation, and a minor one.
:::
::::

**Self-check:**
- A process decreases the entropy of a system. Can it still be spontaneous? Under what condition?
- Why is $\Delta S_\text{surr}$ larger in magnitude for the same released heat when the surroundings are colder?

> **Where this goes next.** The second law is the correct criterion but an awkward one — it demands the surroundings. §17.3 does the algebra that folds the surroundings into a system-only quantity (at constant temperature and pressure), and everything after that is arithmetic.

## 17.3 Free Energy{{attrs[#blk-ch17sec03]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 17.3a}} Define Gibbs free energy and derive the spontaneity criterion $\Delta G < 0$ at constant temperature and pressure.
- {{sp[info] Objective 17.3b}} Calculate standard free energy of reaction from standard free energies of formation.
- {{sp[info] Objective 17.3c}} Determine the temperature at which a reaction or phase transition becomes spontaneous.
- {{sp[info] Objective 17.3d}} {{sp[info] Objective 17.3e}} Relate $\Delta G^\circ$ to K, and calculate $\Delta G$ under non-standard conditions.
:::

### From the second law to Gibbs free energy

At constant temperature and pressure, the second law ($\Delta S_\text{univ}>0$) can be rewritten using only the **system's** properties. Since $\Delta S_\text{surr}=-\Delta H_\text{sys}/T$:

$$\Delta S_\text{sys}-\frac{\Delta H_\text{sys}}{T}>0 \quad\Rightarrow\quad \Delta H_\text{sys}-T\Delta S_\text{sys}<0$$

Defining **Gibbs free energy** $G=H-TS$, this becomes the spontaneity criterion ==$\Delta G=\Delta H-T\Delta S<0$== — no need to ever calculate the surroundings' entropy directly:

| Sign of $\Delta G$ | Meaning |
|---|---|
| $\Delta G<0$ | Spontaneous in the forward direction |
| $\Delta G>0$ | Nonspontaneous forward; reverse is spontaneous |
| $\Delta G=0$ | System at equilibrium |

**What the algebra bought.** At constant temperature and pressure, $\Delta G < 0$ and $\Delta S_\text{univ} > 0$ say exactly the same thing — the derivation above is a rearrangement, not a new law. The gain is entirely practical: $\Delta G$ is built from $\Delta H_\text{sys}$ and $\Delta S_\text{sys}$, both of which are properties of the beaker in front of you. The surroundings have been absorbed into the $\Delta H$ term and need never be mentioned again.

The minus sign is worth noting too: $\Delta S_\text{univ} > 0$ became $\Delta G < 0$ because, at constant temperature and pressure, the two are related by $\Delta G = -T\Delta S_\text{univ}$. Spontaneity looks like "energy going downhill" only because we flipped the sign of an entropy statement.

:::: tabs
::: tab Problem
For each, decide from the signs alone whether the reaction is spontaneous always, never, only at high $T$, or only at low $T$ — then name the quadrant of Figure 17.1: (a) $\Delta H = -120$ kJ/mol, $\Delta S = +150\ \text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$; (b) $\Delta H = +85$ kJ/mol, $\Delta S = -60\ \text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$; \(c) $\Delta H = +178$ kJ/mol, $\Delta S = +161\ \text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$; (d) $\Delta H = -92$ kJ/mol, $\Delta S = -199\ \text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$.
:::
::: tab Solution
Apply $\Delta G = \Delta H - T\Delta S$ and ask what each term contributes.

**(a) Spontaneous at every temperature.** $\Delta H < 0$ makes the first term negative; $\Delta S > 0$ makes $-T\Delta S$ negative too. Both push the same way, so $\Delta G < 0$ regardless of $T$. **Top-left quadrant.**

**(b) Never spontaneous.** $\Delta H > 0$ and $-T\Delta S > 0$ — both terms positive at any temperature. **Bottom-right quadrant.**

**\(c) Spontaneous only at high $T$.** The terms disagree. At low $T$ the $+178$ dominates; as $T$ rises, $-T\Delta S$ grows until it wins:
$$T > \frac{\Delta H}{\Delta S} = \frac{178{,}000}{161} = 1105\ \text{K}$$
**Top-right quadrant** — and this is the $\ce{CaCO3}$ decomposition, as the worked example below confirms.

**(d) Spontaneous only at low $T$.** Again the terms disagree, in the opposite direction:
$$T < \frac{\Delta H}{\Delta S} = \frac{-92{,}000}{-199} = 462\ \text{K}$$
**Bottom-left quadrant** — this is ammonia synthesis, which is why the Haber process fights a thermodynamic headwind at its operating temperature of ~700 K (Chapter 14).

{{sp[warning] Convert the units first}} $\Delta H$ is in kJ and $\Delta S$ in J. Dividing 178 by 161 gives 1.1 K instead of 1105 K — an answer wrong by a factor of 1000 that still looks like a temperature.

**Note that $\Delta H/\Delta S$ gives the crossover in all four cases** — it is just that in (a) and (b) the ratio is negative, meaning the crossover lies at a temperature that does not exist, which is another way of saying the outcome never changes.
:::
::::

:::: tabs
::: tab Problem
A reaction has $\Delta H^\circ = +30.0$ kJ/mol and $\Delta S^\circ = +100.0\ \text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$. (a) Find $\Delta G^\circ$ at 250 K and at 350 K. (b) Find the crossover temperature. \(c) Sketch in words how $\Delta G^\circ$ behaves as a function of $T$, and say what the slope and intercept mean.
:::
::: tab Solution
**(a)** Convert $\Delta S^\circ$ to kJ (0.1000 $\text{kJ}\,\text{K}^{-1}\,\text{mol}^{-1}$) and substitute:

$$T = 250\ \text{K}: \quad \Delta G^\circ = 30.0 - (250)(0.1000) = 30.0 - 25.0 = +5.0\ \text{kJ/mol} \quad (\text{nonspontaneous})$$
$$T = 350\ \text{K}: \quad \Delta G^\circ = 30.0 - (350)(0.1000) = 30.0 - 35.0 = -5.0\ \text{kJ/mol} \quad (\text{spontaneous})$$

**(b)** Set $\Delta G^\circ = 0$:

$$T = \frac{\Delta H^\circ}{\Delta S^\circ} = \frac{30{,}000}{100.0} = 300\ \text{K}$$

Consistent with (a): positive below 300 K, negative above.

**\(c) $\Delta G^\circ = \Delta H^\circ - T\Delta S^\circ$ is a straight line in $T$** — compare $y = b + mx$:

- **Intercept** ($T = 0$): $\Delta G^\circ = \Delta H^\circ = +30.0$ kJ/mol. At absolute zero the entropy term vanishes and enthalpy alone decides.
- **Slope**: $-\Delta S^\circ = -0.1000\ \text{kJ}\,\text{K}^{-1}\,\text{mol}^{-1}$. **The slope of the line *is* the negative of the entropy change**, so a steeply falling line means a large positive $\Delta S^\circ$.
- **Root**: $T = \Delta H^\circ/\Delta S^\circ = 300$ K, where the line crosses zero.

Figure 17.5 is exactly this line drawn for the $\ce{CaCO3}$ decomposition, and reading a slope and an intercept off such a plot is the standard way to extract $\Delta H^\circ$ and $\Delta S^\circ$ from measurements at several temperatures.

{{sp[warning] The straight line assumes constancy}} $\Delta H^\circ$ and $\Delta S^\circ$ do vary slowly with temperature, so the line is really a very gentle curve. Over a few hundred kelvin the approximation is good; extrapolating from 298 K to 2000 K is not.
:::
::::

### Standard free energy of reaction

Like $\Delta H^\circ_\text{rxn}$ and $\Delta S^\circ_\text{rxn}$, standard free energy of reaction is additive:

$$\Delta G^\circ_\text{rxn}=\sum n\Delta G^\circ_f(\text{products})-\sum m\Delta G^\circ_f(\text{reactants})$$

:::: tabs
::: tab Problem
Calculate $\Delta G^\circ_\text{rxn}$ for $\ce{4Fe(s) + 3O2(g) -> 2Fe2O3(s)}$. ($\Delta G^\circ_f$: $\ce{Fe(s)}=0$, $\ce{O2(g)}=0$, $\ce{Fe2O3(s)}=-742.2$ kJ/mol)
:::
::: tab Solution
$$\Delta G^\circ_\text{rxn}=2(-742.2)-[4(0)+3(0)]=-1484.4\ \text{kJ/mol}$$

**As with $\Delta H^\circ_f$ — and unlike $S^\circ$ — elements in their standard states are zero**, which is why iron and oxygen contribute nothing here. Comparing this with §17.1's $\Delta S^\circ_\text{rxn} = -550\ \text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$ for the same reaction shows the pattern of Figure 17.1's bottom-left cell: strongly exothermic, entropy-decreasing, spontaneous at ordinary temperatures. Iron rusts, and it does so despite the entropy penalty.
:::
::::

:::: tabs
::: tab Problem
For $\ce{2SO2(g) + O2(g) -> 2SO3(g)}$: $\Delta H^\circ = -197.8$ kJ/mol and $\Delta S^\circ = -188.0\ \text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$. (a) Calculate $\Delta G^\circ$ at 298 K. (b) Is the reaction spontaneous at 298 K? \(c) Above what temperature does it stop being so?
:::
::: tab Solution
**(a)** Convert $\Delta S^\circ$ to kJ before combining:

$$\Delta G^\circ = \Delta H^\circ - T\Delta S^\circ = -197.8 - (298)(-0.1880) = -197.8 + 56.0 = -141.8\ \text{kJ/mol}$$

**(b) Yes — $\Delta G^\circ < 0$.** Note what the two terms did: the reaction is strongly exothermic ($-197.8$), and the entropy term *opposed* it by $+56.0$ because three moles of gas became two. Enthalpy wins comfortably at room temperature.

**\(c)** Both quantities are negative, so this is Figure 17.1's bottom-left cell — spontaneous below a crossover:

$$T = \frac{\Delta H^\circ}{\Delta S^\circ} = \frac{-197{,}800}{-188.0} = 1052\ \text{K} = 779\ \text{°C}$$

Above 1052 K, $\Delta G^\circ$ turns positive and the reaction reverses.

**The industrial consequence.** This is the key step in sulfuric acid manufacture, and the calculation explains the plant design: the reaction is thermodynamically excellent when cold and kinetically hopeless when cold. Operating near 700 K is a compromise, and it is the same trade — yield against rate — that Chapter 14 identified for ammonia. **Thermodynamics tells you the ceiling; it never tells you how long you will wait.**
:::
::::

### When temperature flips the sign

Free energy is also a **state function**: $\Delta G^\circ_3=\Delta G^\circ_1+\Delta G^\circ_2$ when reaction 3 is the sum of reactions 1 and 2 — the same Hess's-law-style addition from Chapter 6.

Since $\Delta G$ combines $\Delta H$ and $\Delta S$, and $T$ appears explicitly, **temperature can flip the sign of $\Delta G$** whenever $\Delta H$ and $\Delta S$ have the same sign:

:::: tabs
::: tab Problem
For $\ce{CaCO3(s) <=> CaO(s) + CO2(g)}$, $\Delta H^\circ=177.8$ kJ/mol and $\Delta S^\circ=160.5$ J/K·mol at 25 °C. Show this reaction is nonspontaneous at 25 °C, and find the temperature at which it becomes spontaneous.
:::
::: tab Solution
At 298 K: $\Delta G^\circ=177.8\ \text{kJ/mol}-(298\ \text{K})(0.1605\ \text{kJ/K·mol})=130.0\ \text{kJ/mol}>0$ — nonspontaneous, consistent with Le Chatelier's principle (Chapter 14) favoring the reactant side at low T for this endothermic decomposition.

Setting $\Delta G^\circ=0$ and solving for $T$ (isolate $T$ algebraically first, to avoid sign slips):

$$T=\frac{\Delta H^\circ}{\Delta S^\circ}=\frac{177{,}800\ \text{J/mol}}{160.5\ \text{J/K·mol}}=1108\ \text{K} = 835\ °\text{C}$$

Above 835 °C, $\Delta G^\circ<0$ and the decomposition becomes spontaneous.
:::
::::

Figure 17.5 plots that calculation as a line, which is the picture the next worked example asks you to read.

![Chart of Delta G-standard vs. temperature for CaCO3 decomposition, crossing zero at 1108 K](../assets/gibbs_temperature_crossover.svg)
*Figure 17.5 — Because $\Delta H^\circ>0$ and $\Delta S^\circ>0$ here, $\Delta G^\circ=\Delta H^\circ-T\Delta S^\circ$ decreases linearly as $T$ increases, crossing zero at exactly the temperature found above. Self-generated with matplotlib using the worked example's own real data.*

The same $\Delta G=0$ logic applies to **phase transitions**: at the melting or boiling point, both phases are in equilibrium, so $\Delta S=\Delta H/T$ exactly.

:::: tabs
::: tab Problem
Calculate the normal boiling point of dichloromethane, $\ce{CH2Cl2}$, from formation data alone. ($\Delta H^\circ_f$: liquid $-124.2$, gas $-95.4$ kJ/mol. $S^\circ$: liquid 177.8, gas 270.2 $\text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$.) Assume $\Delta H^\circ_\text{vap}$ and $\Delta S^\circ_\text{vap}$ are temperature-independent.
:::
::: tab Solution
**Step 1 — treat the phase change as a reaction**, $\ce{CH2Cl2(l) -> CH2Cl2(g)}$, and take products minus reactants:

$$\Delta H^\circ_\text{vap} = -95.4 - (-124.2) = +28.8\ \text{kJ/mol}$$
$$\Delta S^\circ_\text{vap} = 270.2 - 177.8 = +92.4\ \text{J K}^{-1}\text{mol}^{-1}$$

Both positive, as they must be: vaporizing costs energy and produces a gas.

**Step 2 — at the boiling point the two phases are at equilibrium**, so $\Delta G = 0$:

$$0 = \Delta H^\circ_\text{vap} - T\Delta S^\circ_\text{vap} \quad\Rightarrow\quad T = \frac{\Delta H^\circ_\text{vap}}{\Delta S^\circ_\text{vap}} = \frac{28{,}800\ \text{J/mol}}{92.4\ \text{J K}^{-1}\text{mol}^{-1}} = 312\ \text{K} = 39\ \text{°C}$$

**The measured value is 39.6 °C** — remarkably close, given that the calculation used nothing but two tables and never went near a thermometer.

**What is quietly remarkable here.** Vaporization sits in Figure 17.1's top-right quadrant, spontaneous only above a crossover — and for a phase transition, that crossover *is* the boiling point. The same equation that decides whether limestone decomposes decides when a liquid boils, because both are asking when $\Delta H$ and $T\Delta S$ balance.

**Why the assumption is safe enough.** $\Delta H_\text{vap}$ and $\Delta S_\text{vap}$ do drift with temperature, but the tabulated values are for 298 K and the answer is 312 K — a 14 K extrapolation. Predicting the boiling point of something that boils at 800 K from 298 K data would be far less reliable.
:::
::::


Figure 17.6 is the most familiar $\Delta G = 0$ in chemistry.

![Ice partially melted, liquid water pooling around it](../assets/ice_melting.jpg =450x)
*Figure 17.6 — At exactly 0 °C and 1 atm, ice and liquid water coexist at equilibrium ($\Delta G=0$): for this transition, $\Delta H=6.01$ kJ/mol and $\Delta S=22.0$ J/K·mol, and indeed $6010/22.0 = 273\ \text{K}$ = 0 °C. Source: Rebecca Partington, via Wikimedia Commons, CC BY-SA 2.0.*

### Free energy and the equilibrium constant

Finally, free energy connects directly back to Chapter 14's equilibrium constant:

Figure 17.7 shows why equilibrium is where it is: free energy falls from *either* starting side and bottoms out at one composition.

![Free energy vs. reaction progress, with a minimum at equilibrium](../assets/free_energy_vs_reaction_progress.svg)
*Figure 17.7 — Free energy decreases as the reaction proceeds toward equilibrium from either direction, reaching a minimum exactly where $Q=K$ and $\Delta G=0$. Self-generated with matplotlib; schematic illustration.*

$$\Delta G=\Delta G^\circ+RT\ln Q \qquad \text{at equilibrium: } \Delta G=0,\ Q=K \Rightarrow \boxed{\Delta G^\circ=-RT\ln K}$$

{{sp[warning] Reminder}} **$\Delta G^\circ$ is a single fixed number for a reaction at a given temperature; $\Delta G$ changes as the reaction proceeds and $Q$ changes.** If $Q<K$, $\Delta G<0$ (proceeds forward); if $Q>K$, $\Delta G>0$ (proceeds in reverse) — exactly Chapter 14's $Q$-vs-$K$ rule, now expressed in energy terms.

:::: tabs
::: tab Problem
Calculate $K_p$ for $\ce{N2O4(g) <=> 2NO2(g)}$ at 25 °C. ($\Delta G^\circ_f$: $\ce{N2O4}=97.9$, $\ce{NO2}=51.3$ kJ/mol)
:::
::: tab Solution
$$\Delta G^\circ_\text{rxn}=2(51.3)-97.9=4.7\ \text{kJ/mol}$$

$$K_p=e^{-\Delta G^\circ/RT}=e^{-4700/(8.314\times298)}=0.150$$

Predict qualitatively first: since $\Delta G^\circ>0$ (small and positive), $K$ should be below 1, though not by orders of magnitude — and 0.150 confirms it.

**The correspondence worth memorizing.** $\Delta G^\circ = -RT\ln K$ makes the sign of $\Delta G^\circ$ and the size of $K$ two views of one fact:

| $\Delta G^\circ$ | $K$ | at equilibrium |
|---|---|---|
| large and negative | $K \gg 1$ | almost all product |
| $\approx 0$ | $K \approx 1$ | comparable amounts |
| large and positive | $K \ll 1$ | almost all reactant |

At 298 K the conversion factor is $RT = 2.48$ kJ/mol, so **every 5.7 kJ/mol of $\Delta G^\circ$ moves $K$ by a factor of ten.** A $\Delta G^\circ$ of $-34$ kJ/mol — unremarkable for a chemical reaction — already means $K \approx 10^{6}$.
:::
::::

:::: tabs
::: tab Problem
(a) A reaction has $K = 4.5\times10^{8}$ at 298 K. Find $\Delta G^\circ$. (b) Another has $\Delta G^\circ = +42.0$ kJ/mol at 298 K. Find $K$. \(c) What is $\Delta G^\circ$ when $K = 1$, and what does that mean physically?
:::
::: tab Solution
**(a)** Substitute directly into $\Delta G^\circ = -RT\ln K$:

$$\Delta G^\circ = -(8.314)(298)\ln(4.5\times10^{8}) = -(2478)(19.92) = -4.94\times10^{4}\ \text{J/mol} = -49.4\ \text{kJ/mol}$$

Large $K$, strongly negative $\Delta G^\circ$ — the expected pairing.

**(b)** Rearrange to $K = e^{-\Delta G^\circ/RT}$:

$$K = e^{-42{,}000/2478} = e^{-16.95} = 4.3\times10^{-8}$$

**\(c) $\Delta G^\circ = 0$ exactly**, since $\ln 1 = 0$.

This is the most misread case in the chapter, so state it carefully. $K = 1$ does **not** mean "nothing happens". It means that when every species is at its standard state — 1 M, or 1 atm — the mixture is *already at equilibrium*, so there is no net drive in either direction from that particular starting point. Start from any mixture with Q ≠ 1 and the reaction will proceed, toward whichever side brings $Q$ to 1.

{{sp[warning] $\Delta G^\circ = 0$ is not $\Delta G = 0$}} $\Delta G^\circ = 0$ says $K = 1$, a fact about the reaction. $\Delta G = 0$ says $Q = K$, a fact about the *particular mixture* in front of you. Every reaction reaches $\Delta G = 0$ at its own equilibrium; almost none has $\Delta G^\circ = 0$.
:::
::::

:::: tabs
::: tab Problem
For $\ce{2NH3(g) -> 3H2(g) + N2(g)}$, $\Delta G^\circ=33.0$ kJ/mol. Find $\Delta G$ at 25 °C when $P_{\ce{N2}}=0.870$ atm, $P_{\ce{H2}}=0.250$ atm, $P_{\ce{NH3}}=0.129$ atm.
:::
::: tab Solution
$$Q=\frac{P_{\ce{H2}}^3 P_{\ce{N2}}}{P_{\ce{NH3}}^2}=\frac{0.250^3\times0.870}{0.129^2}=0.817$$

$$\Delta G=\Delta G^\circ+RT\ln Q=33{,}000+(8.314)(298)\ln(0.817)=33{,}000-501=32{,}500\ \text{J/mol}=32.5\ \text{kJ/mol}$$

**Reading the result properly.** $\Delta G = +32.5$ kJ/mol is positive, so the forward reaction is nonspontaneous under these conditions and ammonia will not decompose — the *reverse* reaction is what proceeds.

**Check it against $Q$ and $K$**, which must agree:

$$K = e^{-\Delta G^\circ/RT} = e^{-33{,}000/2478} = 1.6\times10^{-6}$$

$Q = 0.817$ is about **500,000 times larger than $K$**, so the system is overwhelmingly on the product side of where it belongs and must run backwards. That is Chapter 14's $Q > K$ rule, and it gives the same verdict as the sign of $\Delta G$ — as it always must.

**Notice how little $Q$ mattered here.** The $RT\ln Q$ term contributed only $-0.5$ kJ/mol against a standard value of $+33.0$. When $\Delta G^\circ$ is large, non-standard conditions rarely change the verdict; they shift the number slightly. It is when $\Delta G^\circ$ is small — within a few kJ/mol of zero — that $Q$ can flip the sign, and those are the cases worth checking carefully.
:::
::::

:::: tabs
::: tab Problem
For $\ce{N2O4(g) <=> 2NO2(g)}$, $\Delta G^\circ = +4.7$ kJ/mol at 298 K (so $K_p = 0.150$). A vessel contains $P_{\ce{N2O4}} = 2.00$ atm and $P_{\ce{NO2}} = 0.100$ atm. (a) Find $\Delta G$. (b) Which way does the reaction run? \(c) Confirm with $Q$ versus $K$.
:::
::: tab Solution
**(a)** First $Q$, then the correction term:

$$Q = \frac{P_{\ce{NO2}}^2}{P_{\ce{N2O4}}} = \frac{(0.100)^2}{2.00} = 5.00\times10^{-3}$$

$$\Delta G = \Delta G^\circ + RT\ln Q = 4700 + (2478)\ln(5.00\times10^{-3}) = 4700 + (2478)(-5.298)$$

$$= 4700 - 13{,}130 = -8{,}430\ \text{J/mol} = -8.4\ \text{kJ/mol}$$

**(b) $\Delta G < 0$, so the reaction runs forward** — $\ce{N2O4}$ dissociates to $\ce{NO2}$.

**\(c)** $Q = 5.0\times10^{-3}$ against $K = 0.150$. $Q < K$, so the system must make more product to raise $Q$ toward $K$ — forward. ✓ Same answer, arrived at without any energy calculation.

**The point this example exists to make.** $\Delta G^\circ$ is **positive** (+4.7 kJ/mol), which under standard conditions would mean nonspontaneous. But these are not standard conditions — the vessel is loaded with reactant and nearly empty of product — and $\Delta G$ comes out **negative**. **A positive $\Delta G^\circ$ never means a reaction cannot proceed; it means it cannot proceed *starting from standard conditions*.**

This is exactly the case flagged after the ammonia example: $\Delta G^\circ$ is small (4.7 kJ/mol against an $RT\ln Q$ term of $-13$ kJ/mol), so $Q$ dominates and flips the sign.
:::
::::

**Self-check:**
- If a reaction has $\Delta G^\circ<0$, must $K>1$ or $K<1$? Why?
- Two reactions have the same $\Delta H^\circ$ but different $\Delta S^\circ$. Could one be spontaneous at room temperature while the other isn't? Explain using $\Delta G=\Delta H-T\Delta S$.

## Synthesis

==This chapter answers "why do reactions happen" by combining two ideas: enthalpy (Chapter 6) and entropy, weighted by temperature, into a single number — the Gibbs free energy change, $\Delta G$ — whose sign alone determines spontaneity at constant temperature and pressure.== Its biggest payoff is $\Delta G^\circ=-RT\ln K$, which explains, in energetic terms, why equilibrium constants (Chapter 14) have the values they do — a strongly negative $\Delta G^\circ$ is exactly why some reactions have enormous $K$ values. This same $\Delta G^\circ$ reappears in Chapter 18 as $\Delta G^\circ=-nFE^\circ$, connecting thermodynamics directly to electrochemistry.

## Asset and License Record for This Chapter

| Asset | Source URL | License | Attribution |
|---|---|---|---|
| `assets/spontaneity_quadrants.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; entropy values are commonly cited standard thermodynamic data; released under this package's CC BY 4.0 license. |
| `assets/microstates_distribution.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; illustrates the study guide's own worked description ($2^{4} = 16$ microstates); released under this package's CC BY 4.0 license. |
| `assets/entropy_trends.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; entropy values are commonly cited standard thermodynamic data; released under this package's CC BY 4.0 license. |
| `assets/diamond.jpg` | https://commons.wikimedia.org/wiki/File:Apollo_synthetic_diamond.jpg | CC BY 2.0 | Steve Jurvetson, via Wikimedia Commons, CC BY 2.0. |
| `assets/gibbs_temperature_crossover.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib using the study guide's own real worked-example data (deltaH=177.8 kJ/mol, deltaS=160.5 J/K mol); released under this package's CC BY 4.0 license. |
| `assets/ice_melting.jpg` | https://commons.wikimedia.org/wiki/File:Melting_-_Flickr_-_Trinity.jpg | CC BY-SA 2.0 | Rebecca Partington from Seattle, Washington, USA, via Wikimedia Commons, CC BY-SA 2.0. |
| `assets/free_energy_vs_reaction_progress.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; schematic illustration of the G-vs-progress relationship, not a specific reaction's real data; released under this package's CC BY 4.0 license. |
