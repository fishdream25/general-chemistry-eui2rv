{{nyml
kind: document
format: 1
title: Chapter 18: Redox Reactions and Electrochemistry
}}

# Chapter 18: Redox Reactions and Electrochemistry

:::info
**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 18 (CC BY 4.0)
**Audience:** introductory undergraduate general chemistry, second semester
**Package license:** CC BY 4.0
**Note:** builds on oxidation numbers and redox reactions (Chapter 4), the equilibrium constant (Chapter 14), and Gibbs free energy (Chapter 17); facts checked for accuracy against OpenStax *Chemistry 2e* and Wikipedia (used for reference only — no text or figures adapted from either).
:::

:::success
**Chapter Learning Objectives**
- Assign oxidation numbers and balance redox equations using the half-reaction method.
- Define galvanic cells, electrodes, and cell diagrams.
- Use standard reduction potentials to identify the cathode/anode and calculate standard cell potential.
- Relate $\Delta G^\circ$, K, and $E^\circ$ for a redox reaction, and apply the Nernst equation.
- Explain corrosion, electrolysis, and batteries as applications of this framework.
:::

## Chapter Logic

This chapter is the course's synthesis chapter: it takes redox reactions (Chapter 4), the equilibrium constant (Chapter 14), and free energy (Chapter 17) and unites them through electron transfer. ==A voltmeter reading of the cell potential $E$ is a direct measure of $\Delta G$ (via $\Delta G = -nFE$) — the only place in this course where a free-energy change can be read off an instrument dial.==

{{mermaid
graph TD
  A["Redox half-reactions:<br/>oxidation + reduction"] --> B["Galvanic cells:<br/>anode / cathode"]
  B --> C["Standard reduction<br/>potentials (E-naught)"]
  C --> D["Delta G-naught = -nFE-naught<br/>= -RT ln K"]
  D --> E["Nernst equation:<br/>non-standard conditions"]
  E --> F["Applications:<br/>corrosion, electrolysis, batteries"]
}}

**Visual description:** redox half-reactions combine into a galvanic cell, whose voltage is predicted from standard reduction potentials. That standard potential links directly to free energy (Chapter 17) and the equilibrium constant (Chapter 14). The Nernst equation extends this to non-standard conditions, and the chapter closes with real-world applications.

## 18.1 Redox Reactions{{attrs[#blk-ch18sec01]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 18.1a}} Assign oxidation numbers using the standard rule set.
- {{sp[info] Objective 18.1b}} Balance a redox equation using the half-reaction method, in both acidic and basic solution.
:::

### Oxidation, reduction, and the two agents

A **redox** reaction always pairs **oxidation** (loss of electrons, oxidation number increases) with **reduction** (gain of electrons, oxidation number decreases) — one cannot happen without the other. The **reducing agent** donates electrons (itself oxidized); the **oxidizing agent** accepts electrons (itself reduced).

![One electron moving from a sodium atom to a fluorine atom, labeled as an oxidation and a reduction happening at once](../assets/redox_electron_transfer.svg)
*Figure 18.1 — The electron sodium loses is exactly the electron fluorine gains, so the two half-processes are one event described twice. The box on the right untangles the four terms that students most often swap. Self-generated with matplotlib.*

==The two "agent" names are the ones that trip people up, and the reason is that **an agent is named for what it does to the other species, not for what happens to it.**== The reducing agent is the species that *gets oxidized*; the oxidizing agent is the one that *gets reduced*. Figure 18.1's table is worth reading twice.

:::: tabs
::: tab Problem
In $\ce{2Al(s) + 3Cu^2+(aq) -> 2Al^3+(aq) + 3Cu(s)}$, identify what is oxidized, what is reduced, the reducing agent, and the oxidizing agent. Then verify that electrons balance.
:::
::: tab Solution
**Track the oxidation numbers first.**

| Species | Before | After | Change |
|---|---|---|---|
| Al | 0 (free element) | +3 | **increases** by 3 |
| Cu | +2 (monatomic ion) | 0 (free element) | **decreases** by 2 |

**Aluminum is oxidized** (its oxidation number rises), so **Al is the reducing agent**.

**Copper is reduced** (its oxidation number falls), so **$\ce{Cu^2+}$ is the oxidizing agent**.

**Verify the electron bookkeeping.** Each Al loses 3 electrons and there are 2 of them: $2 \times 3 = 6$ lost. Each $\ce{Cu^2+}$ gains 2 and there are 3: $3 \times 2 = 6$ gained. **Six electrons out, six in** ✓ — which is exactly what the coefficients 2 and 3 exist to arrange.

{{sp[warning] Name the agent, not the atom}} The reducing agent here is **Al**, the species as it appears among the reactants — not $\ce{Al^3+}$, which is the product. An agent is always identified on the reactant side.

**Why this matters for §18.4:** that count of six is $n$, the number of moles of electrons transferred, and $n$ appears in every equation from $\Delta G^\circ = -nFE^\circ$ onward. Getting it wrong scales every subsequent answer.
:::
::::

### Oxidation numbers

An **oxidation number** is the charge an atom would carry if every bond to a different element were fully ionic. It is a bookkeeping device, not a real charge — but it is what makes "who lost electrons" answerable for covalent compounds.

Apply the rules in priority order; when two conflict, the earlier one wins:

| # | Rule |
|---|---|
| 1 | A free element is **0** — including $\ce{O2}$, $\ce{H2}$, $\ce{Na(s)}$ |
| 2 | A monatomic ion equals its **charge** |
| 3 | Group IA is **+1**, Group IIA is **+2**, fluorine is **always −1** |
| 4 | Hydrogen is **+1** (except **−1** in active-metal hydrides such as $\ce{LiH}$) |
| 5 | Oxygen is **−2** (except **−1** in peroxides such as $\ce{H2O2}$, and positive with F) |
| 6 | The oxidation numbers **sum to the overall charge** — zero for a neutral molecule |

Rule 6 is the workhorse: assign everything you know from rules 1–5, then solve for the unknown atom.

:::: tabs
::: tab Problem
Assign the oxidation number of the underlined atom: (a) Mn in $\ce{MnO4^-}$; (b) Cr in $\ce{Cr2O7^2-}$; \(c) S in $\ce{H2SO4}$; (d) O in $\ce{H2O2}$; (e) H in $\ce{NaH}$; (f) C in $\ce{CH4}$.
:::
::: tab Solution
In each case, assign what the rules fix, then solve rule 6 for the unknown.

**(a) $\ce{MnO4^-}$:** four oxygens at −2 give −8; the ion's charge is −1.
$$x + 4(-2) = -1 \quad\Rightarrow\quad x = +7$$

**(b) $\ce{Cr2O7^2-}$:** seven oxygens at −2 give −14; charge −2. Note there are **two** chromiums:
$$2x + 7(-2) = -2 \quad\Rightarrow\quad 2x = 12 \quad\Rightarrow\quad x = +6$$

**\(c) $\ce{H2SO4}$:** two H at +1, four O at −2, neutral overall:
$$2(+1) + x + 4(-2) = 0 \quad\Rightarrow\quad x = +6$$

**(d) $\ce{H2O2}$: oxygen is −1**, not −2 — this is the peroxide exception. Check with rule 6: $2(+1) + 2(-1) = 0$ ✓

**(e) $\ce{NaH}$: hydrogen is −1**, not +1 — the active-metal hydride exception. Sodium is Group IA and takes priority at +1, so hydrogen must be −1.

**(f) $\ce{CH4}$:** four H at +1, neutral overall:
$$x + 4(+1) = 0 \quad\Rightarrow\quad x = -4$$

{{sp[warning] Divide by the subscript}} In (b) the algebra gives $2x = +12$ and the answer is **+6 per chromium**, not +12. Forgetting to divide is the commonest slip in polyatomic ions, and $\ce{Cr2O7^2-}$ is where it usually happens.

**The two exceptions in (d) and (e) are the whole reason the rules are ordered.** A higher-priority rule always wins: in $\ce{NaH}$, "Group IA is +1" outranks "hydrogen is +1", so hydrogen is forced negative.
:::
::::

### Balancing by the half-reaction method

The **half-reaction method** balances any redox equation systematically:

1. Split into oxidation and reduction half-reactions.
2. Balance atoms other than O and H.
3. Balance O with $\ce{H2O}$, then H with $\ce{H+}$ (acidic solution).
4. Balance charge by adding electrons.
5. Multiply each half-reaction so electron counts match, then add them together, cancelling the electrons and any species that appear on both sides.
6. **Basic solution only:** add one $\ce{OH-}$ per $\ce{H+}$ to both sides, combining $\ce{H+}+\ce{OH-}\to\ce{H2O}$.

:::: tabs
::: tab Problem
Balance $\ce{H2O2 + Sn^2+ -> H2O + Sn^4+}$ in (a) acidic and (b) basic solution.
:::
::: tab Solution
**(a) Acidic:** Oxidation: $\ce{Sn^2+ -> Sn^4+ + 2e-}$. Reduction: $\ce{2H+ + H2O2 + 2e- -> 2H2O}$. Electrons already balance (2 each). Adding:

$$\ce{Sn^2+ + 2H+ + H2O2 -> Sn^4+ + 2H2O}$$

**(b) Basic:** add 2 $\ce{OH-}$ to both sides (matching the 2 $\ce{H+}$), then combine $\ce{2H+ + 2OH- -> 2H2O}$:

$$\ce{Sn^2+ + H2O2 -> Sn^4+ + 2OH-}$$

**Check the basic-solution step.** Adding $\ce{OH-}$ to both sides never changes the chemistry — it is like adding the same quantity to both sides of an equation — and the $\ce{H+} + \ce{OH-} \to \ce{H2O}$ combination then removes every proton. The water that appears on both sides cancels, which is why the final equation is shorter than the acidic one.
:::
::::

:::: tabs
::: tab Problem
Balance the oxidation of $\ce{Fe^2+}$ to $\ce{Fe^3+}$ by dichromate, $\ce{Cr2O7^2-}$, in acidic solution. The dichromate is reduced to $\ce{Cr^3+}$.
:::
::: tab Solution
**Step 1 — the two half-reactions.**
$$\text{Oxidation: } \ce{Fe^2+ -> Fe^3+} \qquad \text{Reduction: } \ce{Cr2O7^2- -> Cr^3+}$$

**Step 2 — balance atoms other than O and H.** Two chromiums on the left:
$$\ce{Cr2O7^2- -> 2Cr^3+}$$

**Step 3 — balance O with water, then H with $\ce{H+}$.** Seven oxygens need seven waters, which brings fourteen hydrogens:
$$\ce{Cr2O7^2- -> 2Cr^3+ + 7H2O} \quad\Rightarrow\quad \ce{14H+ + Cr2O7^2- -> 2Cr^3+ + 7H2O}$$

**Step 4 — balance charge with electrons.** Left side: $14(+1) + (-2) = +12$. Right side: $2(+3) = +6$. Add six electrons to the left:
$$\ce{6e- + 14H+ + Cr2O7^2- -> 2Cr^3+ + 7H2O}$$
$$\ce{Fe^2+ -> Fe^3+ + e-}$$

**Step 5 — equalize electrons.** The iron half-reaction releases one; multiply it by six:
$$\ce{6Fe^2+ -> 6Fe^3+ + 6e-}$$

**Step 6 — add and cancel the electrons.**
$$\ce{14H+ + Cr2O7^2- + 6Fe^2+ -> 6Fe^3+ + 2Cr^3+ + 7H2O}$$

**Step 7 — verify both atoms and charge.** Atoms: 14 H each side; 7 O each side; 2 Cr; 6 Fe ✓. Charge: left $14(+1) + (-2) + 6(+2) = +24$; right $6(+3) + 2(+3) = +24$ ✓

**The verification step is not optional.** Charge balance catches errors that atom balance misses — most often a dropped or doubled electron in step 4, which produces an equation that looks perfectly reasonable and is wrong.

**Why chromium needs six electrons:** each Cr goes from +6 in dichromate to +3 in $\ce{Cr^3+}$, a drop of 3, and there are two of them. This is the same count you would get from oxidation numbers alone, which is a useful independent check on step 4.
:::
::::


**Self-check:**
- Why must the number of electrons be equalized between the two half-reactions before adding them?
- In $\ce{H2O2}$ acting as an oxidizing agent, what happens to oxygen's oxidation number?

> **Where this goes next.** §18.1 keeps both half-reactions in the same beaker, where the electrons pass directly from one species to the other and no work is extracted. §18.2 separates them — and forces the electrons through a wire on the way.

## 18.2 Galvanic Cells{{attrs[#blk-ch18sec02]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 18.2a}} Define galvanic cell, electrode, anode, and cathode.
- {{sp[info] Objective 18.2a}} Write the cell diagram for a given set of half-reactions or overall reaction.
:::

### How a galvanic cell works

A **galvanic (voltaic) cell** converts a spontaneous redox reaction's released energy into electricity. ==The anode is where oxidation occurs; the cathode is where reduction occurs== — physically separated so electrons must travel through an external wire to get from one to the other, doing electrical work along the way.

Figure 18.2 is the arrangement §18.1 was building toward: the same electron transfer, but with the two halves separated so the electron must take the long way round.

![Galvanic cell schematic: Zn anode and Cu cathode connected by a wire and salt bridge](../assets/galvanic_cell_diagram.svg)
*Figure 18.2 — Zn is oxidized at the anode (electrons flow out through the wire); $\ce{Cu2+}$ is reduced at the cathode. The salt bridge maintains electrical neutrality: anions migrate toward the anode's solution, cations toward the cathode's, as the reaction proceeds. Self-generated with matplotlib.*

**Why the salt bridge is not optional.** As zinc dissolves, the anode compartment accumulates positive charge; as copper plates out, the cathode compartment loses it. Within seconds that charge imbalance would halt electron flow entirely. The salt bridge lets inert ions migrate — anions toward the anode, cations toward the cathode — keeping both compartments neutral so the reaction can continue. **Remove the salt bridge and the cell stops, even though nothing has been consumed.**

### Cell diagrams

The **cell diagram** notation always runs anode → cathode, with `|` marking a phase boundary and `||` marking the salt bridge:

$$\ce{Zn(s)|Zn^2+}(1\text{ M})||\ce{Cu^2+}(1\text{ M})|\ce{Cu(s)}$$

:::: tabs
::: tab Problem
A solid Mg anode sits in 0.1 M $\ce{MgCl2}$, connected via a salt bridge to a solution with 0.2 M $\ce{Fe^3+}$ and 0.3 M $\ce{Fe^2+}$, with an inert Pt cathode. Overall: $\ce{Mg(s) + 2Fe^3+(aq) -> Mg^2+(aq) + 2Fe^2+(aq)}$. Write the half-reactions and cell diagram.
:::
::: tab Solution
$$\text{Anode: } \ce{Mg(s) -> Mg^2+(aq) + 2e-} \qquad \text{Cathode: } \ce{Fe^3+(aq) + e- -> Fe^2+(aq)}$$

$$\ce{Mg(s)|Mg^2+}(0.1\text{ M})||\ce{Fe^3+}(0.2\text{ M}),\ce{Fe^2+}(0.3\text{ M})|\ce{Pt(s)}$$

Pt appears because an inert electrode is needed — neither $\ce{Fe^3+}$ nor $\ce{Fe^2+}$ is itself a solid conductor.

**Note the comma.** $\ce{Fe^3+}$ and $\ce{Fe^2+}$ are separated by a comma rather than a `|`, because both are dissolved in the same solution — there is no phase boundary between them. A `|` would claim one, wrongly.

The standard hydrogen electrode is written the same way, and is another common case where an inert electrode is required:

$$\ce{Pt(s)|H2}(1\text{ atm})|\ce{H+}(1\text{ M})$$
:::
::::

:::: tabs
::: tab Problem
Write the cell diagram for a cell in which $\ce{Cr(s)}$ is oxidized to $\ce{Cr^3+}$ (0.20 M) and $\ce{Ag+}$ (0.50 M) is reduced to $\ce{Ag(s)}$. Then write both half-reactions and the balanced overall reaction.
:::
::: tab Solution
**Half-reactions.** Chromium is oxidized, so it is the **anode**; silver is reduced, so it is the **cathode**:

$$\text{Anode: } \ce{Cr(s) -> Cr^3+(aq) + 3e-} \qquad \text{Cathode: } \ce{Ag+(aq) + e- -> Ag(s)}$$

**Overall reaction** — equalize electrons by multiplying the silver half-reaction by 3:

$$\ce{Cr(s) + 3Ag+(aq) -> Cr^3+(aq) + 3Ag(s)}$$

**Cell diagram**, anode on the left, cathode on the right, salt bridge in the middle:

$$\ce{Cr(s)|Cr^3+}(0.20\text{ M})||\ce{Ag+}(0.50\text{ M})|\ce{Ag(s)}$$

**Three conventions this example exercises:**

- **Anode always on the left.** The diagram reads in the direction the electrons travel through the external wire.
- **No inert electrode needed here.** Both $\ce{Cr}$ and $\ce{Ag}$ are solid conductors and participate directly, unlike the $\ce{Fe^3+/Fe^2+}$ couple above.
- **$E^\circ$ is not multiplied.** Tripling the silver half-reaction changes the coefficients but not its $E^\circ$ — the reason is in §18.3.
:::
::::

**Self-check:**
- Why does the cell diagram always start with a solid electrode?
- What would happen to the cell current if the salt bridge were removed, and why?

> **Where this goes next.** §18.2 assumed you already knew which half-reaction was the anode. §18.3 supplies the table that decides it — and turns the cell's voltage into something predictable rather than measured.

## 18.3 Standard Reduction Potentials{{attrs[#blk-ch18sec03]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 18.3a}} Define standard reduction potential ($E^\circ$) and the standard hydrogen electrode.
- {{sp[info] Objective 18.3b}} Given two half-reactions, identify cathode/anode and calculate overall cell reaction, diagram, and $E^\circ_\text{cell}$.
:::

### The standard hydrogen electrode and the $E^\circ$ scale

**Standard reduction potential** ($E^\circ$) is measured relative to the **standard hydrogen electrode** (SHE), defined as exactly 0 V. {{sp[warning] Reminder}} changing a half-reaction's stoichiometric coefficients does **not** change its $E^\circ$ — it's an intensive property, not extensive.

Figure 18.3 is the table in visual form — and its vertical order is the whole content of this section.

![Standard reduction potentials for several half-reactions, from Li (most negative) to F2 (most positive)](../assets/reduction_potential_series.svg)
*Figure 18.3 — The half-reaction with the highest $E^\circ$ has the strongest oxidizing agent (its oxidized form) (easiest to reduce); the half-reaction with the lowest $E^\circ$ corresponds to the strongest reducing agent (its reduced form gives up electrons most readily). Self-generated with matplotlib using real, commonly tabulated standard reduction potentials.*

:::warning
**No single electrode potential can be measured on its own.** A voltmeter needs two terminals, so every measurement is a *difference* between two half-cells. The SHE is not special physically — it is a chosen reference point, assigned 0 V by convention, exactly as sea level is assigned zero altitude. Every tabulated $E^\circ$ is really "this half-cell, measured against hydrogen."

The practical consequence: **only differences of $E^\circ$ have physical meaning.** Shifting the whole table by a constant would change no cell voltage anywhere.
:::

:::: tabs
::: tab Problem
(a) What is the standard hydrogen electrode, physically? (b) A cell made from a zinc electrode and a SHE reads 0.76 V, with zinc as the anode. What is $E^\circ$ for $\ce{Zn^2+ + 2e- -> Zn}$? \(c) Why is the answer negative, and what does a negative $E^\circ$ mean?
:::
::: tab Solution
**(a)** A platinum electrode (inert — it conducts but does not react) immersed in 1 M $\ce{H+}$, with $\ce{H2}$ gas bubbled over it at 1 atm:

$$\ce{2H+}(1\text{ M}) + \ce{2e-} \rightleftharpoons \ce{H2}(1\text{ atm}) \qquad E^\circ \equiv 0\ \text{V exactly}$$

Its cell diagram is $\ce{Pt(s)|H2}(1\text{ atm})|\ce{H+}(1\text{ M})$. The 0 V is **assigned, not measured** — it is the origin of the scale.

**(b)** Zinc is stated to be the anode, so hydrogen is the cathode:

$$E^\circ_\text{cell} = E^\circ_\text{cathode} - E^\circ_\text{anode} \quad\Rightarrow\quad 0.76 = 0 - E^\circ_{\ce{Zn^2+/Zn}}$$
$$E^\circ_{\ce{Zn^2+/Zn}} = -0.76\ \text{V}$$

**\(c) Negative means "harder to reduce than $\ce{H+}$."** Zinc metal gives up electrons more readily than hydrogen gas does, so in this pairing zinc is forced into the oxidation role and the tabulated reduction potential comes out below zero.

**The practical reading of the sign:**

- $E^\circ > 0$ — the species is reduced more readily than $\ce{H+}$; it will **oxidize** hydrogen.
- $E^\circ < 0$ — the species is reduced less readily; its metal will **reduce** $\ce{H+}$, releasing $\ce{H2}$.

That second line is why zinc, iron and magnesium all fizz in acid and copper, silver and gold do not: the first three sit below hydrogen on the scale, the last three above it.
:::
::::

:::: tabs
::: tab Problem
A student measures a Cu/Ag cell as $E^\circ_\text{cell} = +0.46$ V and reports "$E^\circ$ of the silver half-cell is +0.46 V." (a) What is wrong with this statement? (b) Suppose every value in the $E^\circ$ table were increased by exactly 2.00 V. Which of these would change: the tabulated potentials, individual cell voltages, $\Delta G^\circ$, or which electrode is the cathode?
:::
::: tab Solution
**(a) $E^\circ_\text{cell}$ is a *difference* between two half-cells, not a property of either one.** The 0.46 V measured for the Cu/Ag cell is $0.80 - 0.34$. Attributing it to silver alone discards the copper half of the measurement.

The deeper point: **no half-cell potential can be measured in isolation at all.** A voltmeter has two leads and always reports a difference. Every tabulated $E^\circ$ is that half-cell measured against the SHE, and the "absolute" value exists only because hydrogen was assigned zero.

**(b) Only the tabulated numbers would change. Everything physical would be identical.**

| Quantity | Changes? | Why |
|---|---|---|
| tabulated $E^\circ$ values | **yes** | every entry shifts by +2.00 V |
| $E^\circ_\text{cell}$ for any cell | **no** | the +2.00 cancels in $E^\circ_\text{cathode} - E^\circ_\text{anode}$ |
| $\Delta G^\circ$ | **no** | it depends on $E^\circ_\text{cell}$, which did not move |
| which electrode is the cathode | **no** | the *ordering* is untouched by a constant shift |

**This is the definition of an arbitrary reference point.** Sea level, the SHE, and $\Delta H^\circ_f = 0$ for elements in their standard states are all the same kind of convention: they fix an origin so that differences — the only things that were ever measurable — can be tabulated as if they were absolute values.
:::
::::

### Building a cell from two half-reactions

Given any two half-reactions combined into a galvanic (spontaneous) cell: the one with the **higher** $E^\circ$ becomes the **cathode** (reduction, exactly as written); the other becomes the **anode**, and its reaction is reversed to an oxidation.

$$E^\circ_\text{cell}=E^\circ_\text{cathode}-E^\circ_\text{anode}$$

==Because the cathode is chosen as the larger of the two, $E^\circ_\text{cell}$ is always positive for a galvanic cell — and a positive $E^\circ_\text{cell}$ is what "spontaneous under standard conditions" means here.== If your answer comes out negative, you assigned the electrodes backwards.

:::: tabs
::: tab Problem
Given $\ce{Ag+ + e- -> Ag}$ ($E^\circ=+0.80$ V) and $\ce{Cu^2+ + 2e- -> Cu}$ ($E^\circ=+0.34$ V), find the cathode, anode, overall reaction, cell diagram, and $E^\circ_\text{cell}$.
:::
::: tab Solution
Ag has the higher $E^\circ$ → **cathode**. Cu → **anode** (reversed): $\ce{Cu -> Cu^2+ + 2e-}$.

Equalizing electrons (Ag needs ×2): overall reaction: $\ce{Cu(s) + 2Ag+(aq) -> Cu^2+(aq) + 2Ag(s)}$

$$\ce{Cu(s)|Cu^2+}(1\text{ M})||\ce{Ag+}(1\text{ M})|\ce{Ag(s)}$$

$$E^\circ_\text{cell}=0.80-0.34=0.46\ \text{V}$$

{{sp[warning] Do not double the silver $E^\circ$}} Multiplying $\ce{Ag+ + e- -> Ag}$ by two to balance electrons does **not** make its $E^\circ$ +1.60 V. Potential is an **intensive** property — energy per unit charge (joules per coulomb), not total energy — so it is unchanged by scaling, exactly as the density of a sample does not change when you take twice as much. The extensive quantity is $\Delta G^\circ = -nFE^\circ$, and *that* does double, because $n$ doubles.
:::
::::

:::: tabs
::: tab Problem
Using $E^\circ$ values $\ce{Zn^2+/Zn} = -0.76$ V, $\ce{Fe^2+/Fe} = -0.44$ V, and $\ce{Cu^2+/Cu} = +0.34$ V: (a) which is the strongest oxidizing agent and which the strongest reducing agent? (b) Will $\ce{Zn(s)}$ reduce $\ce{Fe^2+}$? \(c) Will $\ce{Cu(s)}$ reduce $\ce{Fe^2+}$? (d) Calculate $E^\circ_\text{cell}$ for the Zn/Cu cell.
:::
::: tab Solution
**(a)** The table is written as *reductions*, so a **high** $E^\circ$ means the species on the left is easily reduced — that is, it is a good **oxidizing agent**. A **low** $E^\circ$ means the species on the *right* gives up electrons easily — a good **reducing agent**.

- **Strongest oxidizing agent: $\ce{Cu^2+}$** (highest $E^\circ$, +0.34 V).
- **Strongest reducing agent: $\ce{Zn(s)}$** (lowest $E^\circ$, −0.76 V).

**(b) Yes.** For $\ce{Zn(s)} + \ce{Fe^2+} \to \ce{Zn^2+} + \ce{Fe(s)}$, iron is reduced (cathode, −0.44) and zinc oxidized (anode, −0.76):
$$E^\circ_\text{cell} = -0.44 - (-0.76) = +0.32\ \text{V} > 0 \quad\text{— spontaneous}$$

**\(c) No.** For $\ce{Cu(s)} + \ce{Fe^2+} \to \ce{Cu^2+} + \ce{Fe(s)}$:
$$E^\circ_\text{cell} = -0.44 - (+0.34) = -0.78\ \text{V} < 0 \quad\text{— not spontaneous}$$
The *reverse* runs instead: iron metal dissolves in copper solutions, not the other way round.

**(d)** $E^\circ_\text{cell} = 0.34 - (-0.76) = +1.10$ V — the classic Daniell cell.

**The shortcut this establishes.** A metal will reduce the ion of any metal **above** it in $E^\circ$. Zinc is below iron, which is below copper, so zinc reduces both and copper reduces neither. This single ordering is why zinc is used to protect steel and copper is not.
:::
::::

**Self-check:**
- If you doubled every coefficient in the Ag half-reaction, would $E^\circ_\text{cell}$ change? Would $\Delta G^\circ$?
- Why can no single half-cell potential be measured in isolation?

> **Where this goes next.** §18.3 gives a voltage under standard conditions only — 1 M, 1 atm. §18.4 does two things with that number: connects it to $\Delta G^\circ$ and $K$ from Chapters 14 and 17, and extends it to the non-standard concentrations any real cell actually has.

## 18.4 Nernst Equation{{attrs[#blk-ch18sec04]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 18.4a}} Relate $\Delta G^\circ$, K, and $E^\circ$ for a redox reaction.
- {{sp[info] Objective 18.4b}} Apply the Nernst equation to find E under non-standard conditions.
- {{sp[info] Objective 18.4c}} Calculate the potential of a concentration cell.
:::

### $\Delta G^\circ$, K, and $E^\circ$ — three views of one fact

==$\Delta G^\circ$, $K$ and $E^\circ_\text{cell}$ are one fact in three currencies — and the bridge between them is the only place in this course where a thermodynamic quantity can be read off a voltmeter.== Three quantities describe the same reaction's favorability from three angles, connected by:

$$\Delta G^\circ=-nFE^\circ=-RT\ln K \qquad F=96{,}485\ \text{C/mol (Faraday constant)},\ n=\text{mol }e^-\text{ transferred}$$

| $\Delta G^\circ$ | K | $E^\circ_\text{cell}$ | Meaning |
|---|---|---|---|
| Negative | > 1 | Positive | Favors products |
| 0 | = 1 | 0 | Reactants/products equally favored |
| Positive | < 1 | Negative | Favors reactants |

:::: tabs
::: tab Problem
Find $\Delta G^\circ$ and $K$ at 25 °C for $\ce{Sn(s) + 2Cu^2+(aq) -> Sn^2+(aq) + 2Cu+(aq)}$, given $\ce{Sn^2+ +2e- -> Sn}$ ($E^\circ=-0.1375$ V) and $\ce{Cu^2+ +e- -> Cu+}$ ($E^\circ=0.153$ V). Is it spontaneous?
:::
::: tab Solution
Cu has the higher $E^\circ$ → cathode; Sn → anode (reversed). $n=2$ (equalizing electrons):

$$E^\circ_\text{cell}=0.153-(-0.1375)=0.2905\ \text{V}$$

$$\Delta G^\circ=-nFE^\circ=-2(96{,}485)(0.2905)=-5.606\times10^4\ \text{J/mol}$$

$$K=e^{-\Delta G^\circ/RT}=e^{5.606\times10^4/(8.314\times298)}=6.7\times10^9$$

Negative $\Delta G^\circ$, $K\gg1$ → **spontaneous**, strongly product-favored.

{{sp[warning] K is exquisitely sensitive to $E^\circ$}} $K$ came out near $10^{10}$ from a cell potential of only 0.29 V. At 298 K, **every 0.0592 V of $E^\circ_\text{cell}$ multiplies $K$ by $10^n$, where $n$ is the number of electrons transferred** — so a cell voltage you could barely read on a cheap meter corresponds to an equilibrium constant spanning many orders of magnitude. Carrying an extra digit in $E^\circ$ matters here in a way it rarely does elsewhere — which is why this example kept $E^\circ=0.2905$ V rather than rounding to 0.290. Rounding first would have given $K=6.4\times10^9$, low by about 4%, from a change in the *fourth* digit of a voltage.
:::
::::

:::: tabs
::: tab Problem
For the Daniell cell, $\ce{Zn(s) + Cu^2+(aq) -> Zn^2+(aq) + Cu(s)}$, $E^\circ_\text{cell} = +1.10$ V and $n = 2$. (a) Calculate $\Delta G^\circ$. (b) Calculate $K$. \(c) What does the size of $K$ say about how far the reaction goes?
:::
::: tab Solution
**(a)**
$$\Delta G^\circ = -nFE^\circ = -(2)(96{,}485\ \text{C/mol})(1.10\ \text{V}) = -2.12\times10^{5}\ \text{J/mol} = -212\ \text{kJ/mol}$$

(A coulomb-volt is a joule, so the units work out without conversion.)

**(b)**
$$K = e^{-\Delta G^\circ/RT} = e^{212{,}267/2478} = e^{85.68} = 1.6\times10^{37}$$

**\(c) The reaction goes essentially to completion.** With $K \approx 10^{37}$, the equilibrium ratio $[\ce{Zn^2+}]/[\ce{Cu^2+}]$ is so enormous that no measurable $\ce{Cu^2+}$ remains. Drop excess zinc into copper sulfate solution and the blue color disappears entirely.

**Reading the chain of implications.** A modest 1.10 V — less than the 1.5 V of a single AA cell — corresponds to $-212$ kJ/mol and $K = 10^{37}$. The three numbers are the same fact in three units: **volts for the instrument, kilojoules for the thermodynamicist, and $K$ for the equilibrium chemist.**

**And this is where the chapter's chain closes.** $E^\circ$ came from a table (§18.3), $\Delta G^\circ$ is Chapter 17's spontaneity criterion, and $K$ is Chapter 14's equilibrium constant. Measuring a voltage determines both of the others.
:::
::::

### The Nernst equation

For **non-standard conditions**, the **Nernst equation** extends $E^\circ$ using the reaction quotient $Q$ (Chapter 14):

$$E=E^\circ-\frac{RT}{nF}\ln Q$$

:::: tabs
::: tab Problem
For $\ce{Al(s)|Al^3+}(0.15\text{ M})||\ce{Cu^2+}(0.025\text{ M})|\ce{Cu(s)}$, find $n$, $Q$, and $E$ at 25 °C. ($E^\circ_{\ce{Al^3+/Al}}=-1.662$ V, $E^\circ_{\ce{Cu^2+/Cu}}=0.34$ V)
:::
::: tab Solution
Overall (equalizing electrons, $n=6$): $\ce{3Cu^2+(aq) + 2Al(s) -> 3Cu(s) + 2Al^3+(aq)}$

$$E^\circ=0.34-(-1.662)=2.00\ \text{V} \qquad Q=\frac{[\ce{Al^3+}]^2}{[\ce{Cu^2+}]^3}=\frac{0.15^2}{0.025^3}=1.4\times10^3$$

$$E=2.00-\frac{(8.314)(298)}{6(96{,}485)}\ln(1.4\times10^3)=2.00-0.031=1.97\ \text{V}$$

**Note how small the correction is.** $Q$ is over a thousand, yet the voltage moved by only 0.03 V — because $RT/nF$ is only 4.3 mV here (298 K, $n=6$) and the logarithm compresses everything. **Concentration has a weak effect on cell potential**, which is exactly why a battery holds a nearly constant voltage until it is almost flat, then drops abruptly.
:::
::::

:::: tabs
::: tab Problem
A Daniell cell ($E^\circ = 1.10$ V, $n = 2$) is set up with $[\ce{Zn^2+}] = 1.0$ M and $[\ce{Cu^2+}] = 0.010$ M. (a) Find $E$. (b) Did the potential rise or fall relative to standard, and does that make sense? \(c) What would $E$ be at equilibrium?
:::
::: tab Solution
**(a)** For $\ce{Zn(s) + Cu^2+ -> Zn^2+ + Cu(s)}$, solids are omitted from $Q$:

$$Q = \frac{[\ce{Zn^2+}]}{[\ce{Cu^2+}]} = \frac{1.0}{0.010} = 100$$

$$E = E^\circ - \frac{RT}{nF}\ln Q = 1.10 - \frac{(8.314)(298)}{2(96{,}485)}\ln(100) = 1.10 - (0.01284)(4.605) = 1.10 - 0.059 = 1.04\ \text{V}$$

**(b) It fell, by 0.059 V — and it should have.** The product $\ce{Zn^2+}$ is at its standard concentration while the reactant $\ce{Cu^2+}$ has been depleted a hundredfold, so the cell is closer to equilibrium than a standard cell is, and has less driving force left. **Depleting a reactant always lowers $E$; depleting a product raises it.**

**\(c) At equilibrium, $E = 0$ exactly.** That is what a dead battery is: not a cell that has run out of chemicals, but one that has reached $Q = K$, where there is no remaining driving force. Setting $E = 0$ in the Nernst equation recovers $E^\circ = (RT/nF)\ln K$ — the same relationship as the previous subsection, seen from the other end.

**The factor 0.059 is not a coincidence.** At 298 K, $\frac{RT}{F}\ln 10 = 0.0592$ V, so the Nernst equation is often written $E = E^\circ - \frac{0.0592}{n}\log Q$. Each factor of ten in $Q$ costs $0.0592/n$ volts, and here $n = 2$ with $Q = 10^2$: $2 \times 0.0592/2 = 0.059$ V ✓
:::
::::

### Concentration cells

A **concentration cell** uses the *same* electrode material in both half-cells, differing only in ion concentration — so $E^\circ=0$ and the entire potential comes from $Q$:

Figure 18.4 shows what that means as the two concentrations converge.

![E vs. Q for a Zn2+/Zn concentration cell](../assets/nernst_concentration_cell.svg)
*Figure 18.4 — As the anode/cathode concentration ratio Q approaches 1 (equal concentrations), E approaches zero — there's no driving force left once both half-cells match. Self-generated with matplotlib using the Nernst equation and the worked example's real data point.*

:::: tabs
::: tab Problem
A Zn concentration cell has $[\ce{Zn^2+}]=0.10$ M and 0.50 M in its two half-cells. Find $E$.
:::
::: tab Solution
**Which side is the anode?** The cell runs in whatever direction equalizes the two concentrations, because that is the direction of increasing entropy (Chapter 17). So metal **dissolves** into the dilute side, raising its concentration — that is oxidation, so **the dilute half-cell is the anode**. Metal **plates out** of the concentrated side, lowering its concentration — reduction, so the concentrated half-cell is the cathode. $n = 2$.

$$Q = \frac{[\ce{Zn^2+}]_\text{anode}}{[\ce{Zn^2+}]_\text{cathode}} = \frac{0.10}{0.50} = 0.20$$

$$E=-\frac{RT}{nF}\ln Q=-\frac{(8.314)(298)}{2(96{,}485)}\ln(0.20)=-(0.01284)(-1.609)=0.0207\ \text{V}$$

**Small, and necessarily so.** With $E^\circ = 0$, the entire 21 mV comes from a fivefold concentration difference. A concentration cell can never produce much voltage — but it is exquisitely sensitive to concentration, which is precisely what makes it useful as a *measuring* device rather than a power source.
:::
::::

:::: tabs
::: tab Problem
A pH meter is a concentration cell built around $\ce{H+}$. Consider a cell with $[\ce{H+}] = 1.0\times10^{-3}$ M on one side and $1.0$ M on the other, with hydrogen electrodes and $n = 1$. (a) Find $E$. (b) By how much does $E$ change per pH unit? \(c) Why does this make a usable pH meter?
:::
::: tab Solution
**(a)** The dilute side is the anode, so

$$Q = \frac{1.0\times10^{-3}}{1.0} = 1.0\times10^{-3}$$

$$E = -\frac{RT}{nF}\ln Q = -\frac{(8.314)(298)}{1(96{,}485)}\ln(1.0\times10^{-3}) = -(0.02569)(-6.908) = 0.177\ \text{V}$$

**(b)** Using the base-10 form with $n = 1$:

$$E = -0.0592\log Q = -0.0592\,(\log[\ce{H+}]_\text{dilute} - \log 1.0) = 0.0592 \times \ce{pH}$$

**At 25 °C, each pH unit is worth 0.0592 V — about 59 mV.** Check against (a): pH 3 gives $3 \times 0.0592 = 0.178$ V ✓

**\(c) Because 59 mV per pH unit is easy to measure precisely.** A voltmeter resolving 1 mV resolves pH to about 0.02 units, which is better than any indicator can manage and requires no color judgement at all. The relationship is also perfectly **linear in pH**, so calibrating with two buffer solutions of known pH fixes the whole scale.

**This is the chapter's most useful single result.** A pH meter is not a chemical sensor in any exotic sense — it is a concentration cell, and the number on its display is a voltage divided by 0.0592.
:::
::::

**Self-check:**
- If $E^\circ_\text{cell}=0$ for a reaction, what does that tell you about $K$?
- A battery reads 1.5 V when new and 1.4 V when nearly flat, then falls quickly to 0. Explain both the flatness and the final collapse using the Nernst equation.

> **Where this goes next.** §18.4 completes the theory. §18.5 asks where it shows up — in metal that rusts, in reactions run backwards on purpose, and in the cell powering whatever you are reading this on.

## 18.5 Applications{{attrs[#blk-ch18sec05]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 18.5a}} Explain corrosion as an electrochemical process.
- {{sp[info] Objective 18.5a}} Define electrolysis and distinguish it from a galvanic cell.
- {{sp[info] Objective 18.5a}} Identify common battery types.
:::

### Corrosion

**Corrosion** is the spontaneous electrochemical deterioration of a metal — rust forms when both moisture and oxygen are present: iron is oxidized at an anodic region (often where O2 is scarce, such as under a water drop), the electrons flow through the metal to a cathodic region (where O2 is plentiful, such as the drop's edge) where oxygen is reduced, and the two regions can be some distance apart.

Figure 18.5 shows the result of a galvanic cell nobody built.

![Rust forming on a metal surface](../assets/rust_corrosion.jpg =700x)
*Figure 18.5 — Rust ($\ce{Fe2O3}\cdot x\ce{H2O}$) is the visible product of iron's spontaneous oxidation, with atmospheric $\ce{O2}$ as the oxidizing agent — a galvanic process happening directly on the metal's surface rather than in a separated cell. Source: Georges Grondin, via Wikimedia Commons, public domain.*

:::: tabs
::: tab Problem
Iron rusts; galvanized (zinc-coated) steel does not, even when the coating is scratched through to bare iron. (a) Explain using $E^\circ$ values ($\ce{Fe^2+/Fe} = -0.44$ V, $\ce{Zn^2+/Zn} = -0.76$ V, $\ce{O2}/\ce{H2O} = +1.23$ V). (b) Why is a scratch not fatal? \(c) Tin-plated steel (a "tin can") rusts *faster* once scratched — why?
:::
::: tab Solution
**(a) Rusting is a galvanic cell on the metal's own surface.** Iron is oxidized at one spot (anode) and atmospheric oxygen is reduced at another (cathode):

$$E^\circ_\text{cell} = 1.23 - (-0.44) = +1.67\ \text{V} > 0 \quad\text{— strongly spontaneous}$$

That is why iron rusts at all, and why it needs water present: the electrolyte completes the circuit.

**With zinc present, zinc is the better reducing agent** ($-0.76$ is below $-0.44$), so zinc is oxidized in preference:

$$E^\circ_\text{cell} = 1.23 - (-0.76) = +1.99\ \text{V}$$

**(b) A scratch is not fatal because the zinc protects the iron electrically, not physically.** Even with bare iron exposed, the zinc remains the anode of the couple and corrodes instead — the iron is forced to be the cathode, where nothing dissolves. This is **cathodic protection**, and the zinc is called a **sacrificial anode**. Ships' hulls and buried pipelines carry blocks of zinc or magnesium for exactly this reason.

**\(c) Tin has $E^\circ = -0.14$ V, which is *above* iron's $-0.44$ V.** So in a tin/iron couple, **iron** is the more easily oxidized and becomes the anode. While the coating is intact it works as a physical barrier; once scratched, it creates a galvanic cell that actively drives iron's corrosion — worse than no coating at all.

**The design rule:** a protective metal coating must be **more** easily oxidized than the metal it protects, or a scratch turns it into an accelerant.
:::
::::

### Electrolysis

**Electrolysis** uses external electrical energy to drive a **nonspontaneous** redox reaction — the reverse of what a galvanic cell does spontaneously. {{sp[warning] Reminder}} a negative $E^\circ_\text{cell}$ doesn't mean a reaction "can't happen" — it means external energy input (electrolysis) is required to force it forward under standard conditions. Electrolyzing water yields $\ce{H2}$ and $\ce{O2}$ (the reverse of $\ce{H2}$ combustion); electrolyzing molten $\ce{NaCl}$ yields $\ce{Na}$ metal and $\ce{Cl2}$ gas.

![Side-by-side comparison of a galvanic cell and an electrolytic cell, showing opposite energy conversion and the external power supply](../assets/galvanic_vs_electrolytic.svg)
*Figure 18.6 — The two cell types run the same kind of chemistry in opposite directions. Oxidation is at the anode and reduction at the cathode in **both** — what differs is whether the cell drives the circuit or the circuit drives the cell. Self-generated with matplotlib.*

==Figure 18.6 makes the one comparison worth memorizing: a galvanic cell converts chemical energy into electrical, an electrolytic cell does the reverse, and the anode/cathode definitions never change between them.== What does change is the sign of $E^\circ_\text{cell}$, and therefore whether you need a power supply.

:::: tabs
::: tab Problem
For $\ce{2H2O(l) -> 2H2(g) + O2(g)}$, $E^\circ_\text{cell} = -1.23$ V. (a) Is this spontaneous? (b) What does the negative sign tell you about $\Delta G^\circ$? \(c) What minimum voltage must a power supply provide to electrolyze water? (d) Reconcile this with the fact that hydrogen burning in oxygen is violently spontaneous.
:::
::: tab Solution
**(a) No.** $E^\circ_\text{cell} < 0$, so the reaction does not proceed on its own — water does not spontaneously separate into its elements.

**(b)** From $\Delta G^\circ = -nFE^\circ$ with $n = 4$:

$$\Delta G^\circ = -(4)(96{,}485)(-1.23) = +4.75\times10^{5}\ \text{J/mol} = +475\ \text{kJ/mol}$$

Positive, as a negative $E^\circ$ requires. The two statements are the same statement.

**\(c) At least 1.23 V** must be applied to force the reaction. In practice more is needed — real cells require an **overpotential** on top of the thermodynamic minimum to overcome kinetic barriers at the electrodes, typically bringing the working voltage to 1.5–2.0 V.

**(d) They are the same reaction read in opposite directions.** Hydrogen combustion, $\ce{2H2 + O2 -> 2H2O}$, has $E^\circ_\text{cell} = +1.23$ V and $\Delta G^\circ = -475$ kJ/mol — strongly spontaneous. Electrolysis is that reaction reversed, so every sign flips.

**The accounting is exact.** Electrolyzing water costs at least the 475 kJ/mol of work that burning the hydrogen (e.g., in a fuel cell) can at most return. **Electrolysis is not a way of making energy; it is a way of storing it** — which is the entire principle behind hydrogen as a fuel, and behind every rechargeable battery.
:::
::::

### Batteries

A **battery** is a galvanic cell (or series of them) engineered as a practical, nearly constant-voltage power source.


Figure 18.7 shows the packaging; the chemistry inside is §18.2's.

![AA batteries, close-up of the terminal ends](../assets/batteries.jpg =700x)
*Figure 18.7 — Common battery types include dry cells, mercury batteries, lead storage batteries, lithium-ion batteries, and fuel cells (which require a continuous reactant supply, unlike a sealed battery). Every one of them operates as a galvanic cell when delivering current. Source: ajay_suresh, via Wikimedia Commons, CC BY 2.0.*

**Self-check:**
- Is corrosion more like a galvanic cell or an electrolytic cell? Why?
- A student says a reaction with negative $E^\circ_\text{cell}$ simply never happens. What's the more precise statement?

## Synthesis

==This chapter's central insight is that $\Delta G^\circ$, $K$, and $E^\circ$ are three equivalent descriptions of the same reaction's spontaneity under standard conditions — Chapter 17's free energy, Chapter 14's equilibrium constant, and this chapter's cell potential, all connected by $\Delta G^\circ=-nFE^\circ=-RT\ln K$.== Everything else in the chapter — half-reaction balancing, cell diagrams, the Nernst equation, corrosion, electrolysis, and batteries — is either the mechanics of measuring $E^\circ$ or a practical consequence of this one synthesizing relationship.

## Asset and License Record for This Chapter

| Asset | Source URL | License | Attribution |
|---|---|---|---|
| `assets/redox_electron_transfer.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; released under this package's CC BY 4.0 license. |
| `assets/galvanic_cell_diagram.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; illustrates the study guide's own Zn/Cu worked example; released under this package's CC BY 4.0 license. |
| `assets/reduction_potential_series.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib using real, commonly tabulated standard reduction potentials; released under this package's CC BY 4.0 license. |
| `assets/nernst_concentration_cell.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib using the Nernst equation and the study guide's own real worked-example data point (0.10 M / 0.50 M → $E = 0.0207$ V); released under this package's CC BY 4.0 license. |
| `assets/rust_corrosion.jpg` | https://commons.wikimedia.org/wiki/File:Rust_on_metal.jpg | Public domain | Georges Grondin, via Wikimedia Commons (public domain). Resized from the original for web use. |
| `assets/galvanic_vs_electrolytic.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; released under this package's CC BY 4.0 license. |
| `assets/batteries.jpg` | https://commons.wikimedia.org/wiki/File:AA_Batteries_(51825378856).jpg | CC BY 2.0 | ajay_suresh, via Wikimedia Commons, CC BY 2.0. Resized from the original for web use. |
