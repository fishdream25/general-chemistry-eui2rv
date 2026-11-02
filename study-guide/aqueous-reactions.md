{{nyml
kind: document
format: 1
title: Chapter 4: Reactions in Aqueous Solution
}}

# Chapter 4: Reactions in Aqueous Solution

:::info
**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 4 (CC BY 4.0)
**Audience:** introductory undergraduate general chemistry, first semester
**Package license:** CC BY 4.0
**Note:** builds on Chapter 2's formulas and naming and Chapter 3's stoichiometry; facts checked for accuracy against OpenStax *Chemistry 2e* and Wikipedia (used for reference only — no text or figures adapted from either).
:::

:::success
**Chapter Learning Objectives**
- Classify solutes as strong, weak, or nonelectrolytes.
- Apply solubility rules and write molecular, ionic, and net ionic equations.
- Distinguish Arrhenius and Brønsted acids and bases, and write neutralization net ionic equations.
- Assign oxidation numbers, classify redox reactions, and use the activity series.
- Calculate molarity, apply the dilution equation, and carry out solution stoichiometry.
:::

## Chapter Logic

Almost all the chemistry you meet — in a living cell, in a river, in a beaker — happens in water. This chapter is about what changes when a reaction takes place in solution rather than between dry solids.

The central shift is this: ==in water, a dissolved ionic compound is not present as compounds at all. It is present as separate, freely moving ions.== Once you accept that, three things follow. You need a way to know which combinations of ions stay dissolved and which do not (§4.2). You need to recognize the other two great families of reaction those ions undergo: transferring a proton (§4.3) or transferring an electron (§4.4). And you need a way to say *how much* is dissolved (§4.5), so that Chapter 3's stoichiometry still works when your reactants arrive by the beaker rather than on a balance.

{{mermaid
graph TD
  A["Aqueous solutions:<br/>electrolytes and hydration"] --> B["Precipitation:<br/>solubility rules, net ionic equations"]
  A --> C["Acid-base:<br/>proton transfer, neutralization"]
  A --> D["Redox:<br/>electron transfer, oxidation numbers"]
  B --> E["Solution stoichiometry:<br/>molarity, dilution, titration"]
  C --> E
  D --> E
}}

**Visual description:** A branching flowchart. The properties of aqueous solutions feed into three parallel reaction families — precipitation, acid-base, and redox — and all three then feed into solution stoichiometry, which is the quantitative treatment common to all of them.

## 4.1 General Properties of Aqueous Solutions{{attrs[#blk-ch04sec01]}}

:::success
**Learning Objectives**
- Define solution, solute, and solvent.
- {{sp[info] Objective 4.1a}} Explain why some solutions conduct electricity and others do not.
- {{sp[info] Objective 4.1a}} Classify solutes as strong electrolytes, weak electrolytes, or nonelectrolytes.
- Describe hydration.
:::

### Solutions, solutes, and solvents

A **solution** is a homogeneous mixture of two or more substances — Chapter 1's category, now looked at closely. The **solvent** is the substance present in the larger amount; the **solute** is present in the smaller amount. When the solvent is water, the solution is **aqueous**, written $(aq)$.

### Why some solutions conduct electricity

Pure water barely conducts electricity. Dissolve table salt in it and it conducts well. Dissolve sugar in it and it still barely conducts. The difference is not how much dissolved — it is *what the dissolved particles are*.

Electric current is moving charge. ==A solution can carry current only if it contains charged particles free to move== — neutral molecules, however many of them there are, cannot carry a current.

An **electrolyte** is a substance whose aqueous solution conducts electricity. A **nonelectrolyte** is one whose solution does not. Figure 4.1 shows the standard test and, beneath it, the reason.

![Strong, weak, and nonelectrolyte solutions compared by bulb brightness and by particle picture](../assets/electrolyte_conductivity.svg =820x)
*Figure 4.1 — The conductivity test, and what is happening underneath it. A **strong electrolyte** such as $\ce{NaCl}$ dissociates completely, so every formula unit that dissolves becomes two free ions and the bulb is bright. A **weak electrolyte** such as acetic acid ionizes only partially — most of it stays as intact molecules and only a few ions form, so the bulb glows dimly. A **nonelectrolyte** such as glucose dissolves without producing any ions at all, and the bulb stays dark.*

The three categories are worth memorizing in the form the rest of the course uses them:

| Category | What happens in water | Examples |
|---|---|---|
| **Strong electrolyte** | dissociates or ionizes **completely** | soluble salts ($\ce{NaCl}$, $\ce{KNO3}$), strong acids ($\ce{HCl}$, $\ce{HNO3}$), strong bases ($\ce{NaOH}$, $\ce{KOH}$) |
| **Weak electrolyte** | ionizes only **partially** | weak acids ($\ce{CH3COOH}$, $\ce{HF}$), weak bases ($\ce{NH3}$) |
| **Nonelectrolyte** | dissolves without ionizing at all | sugars ($\ce{C6H12O6}$), ethanol, urea |

{{sp[warning] Watch out}} "Strong" here means *completely dissociated*, not *concentrated* and not *dangerous*. A very dilute hydrochloric acid solution is still a strong electrolyte; a very concentrated acetic acid solution is still a weak one.

:::: tabs
::: tab Problem
Classify each as a strong electrolyte, weak electrolyte, or nonelectrolyte: $\ce{KBr}$, $\ce{CH3COOH}$, $\ce{C2H5OH}$ (ethanol), $\ce{HNO3}$.
:::
::: tab Solution
- **$\ce{KBr}$** — a soluble ionic salt, so it dissociates completely: **strong electrolyte**.
- **$\ce{CH3COOH}$** — acetic acid, a weak acid, ionizes only partially: **weak electrolyte**.
- **$\ce{C2H5OH}$** — ethanol is a molecular compound that dissolves but does not ionize: **nonelectrolyte**.
- **$\ce{HNO3}$** — nitric acid is one of the strong acids, ionizing completely: **strong electrolyte**.

The decision procedure: is it ionic and soluble, or a strong acid or strong base? Then strong. Is it a weak acid or weak base? Then weak. Otherwise, a molecular compound that just dissolves — nonelectrolyte.
:::
::::

:::: tabs
::: tab Problem
Solution A contains 0.1 mol of $\ce{NaCl}$ in 1 L of water. Solution B contains 0.1 mol of glucose in 1 L. Both contain the same number of moles of solute. Which conducts better, and by roughly what factor do their dissolved-particle counts differ?
:::
::: tab Solution
**Solution A conducts; solution B essentially does not.**

$\ce{NaCl}$ dissociates completely, so 0.1 mol of it gives 0.1 mol $\ce{Na+}$ plus 0.1 mol $\ce{Cl^-}$ — **0.2 mol of dissolved particles, all of them charged**.

Glucose dissolves as intact molecules, so 0.1 mol gives **0.1 mol of particles, none of them charged**.

So A has twice as many dissolved particles and, more importantly, all of them can carry current while none of B's can. This particle-count difference returns in Chapter 12 as the reason ionic solutes depress a freezing point more than molecular ones at the same molarity.
:::
::::

### Hydration

Why does an ionic lattice come apart in water at all? The ions in $\ce{NaCl}$ are held together by strong attractions; something must be paying for breaking them.

Water molecules are **polar** — slightly negative at the oxygen end, slightly positive at the hydrogen end (Chapter 10 explains why). A water molecule can therefore turn its negative end toward a cation, or its positive end toward an anion, and be attracted either way. **Hydration** is the process in which an ion becomes surrounded by water molecules arranged in this specific orientation, as in Figure 4.2.

![An ionic lattice dissolving, with oriented water molecules surrounding the freed ions](../assets/hydration_of_ions.svg =800x)
*Figure 4.2 — Dissolution at the particle level. In the dry solid the ions are locked in a lattice and cannot move, which is why solid salt does not conduct. In solution each ion is pulled free and wrapped in a shell of water molecules, all turned the same way: oxygen ends inward toward a cation, hydrogen ends inward toward an anion. Those attractions are what pay for breaking the lattice, and the freed ions are now mobile.*

> **Where this goes next.** If dissolved ionic compounds are really just loose ions, then mixing two solutions is really mixing four kinds of ion. Sometimes two of them find each other and leave the solution as a solid — that is §4.2.

## 4.2 Precipitation Reactions{{attrs[#blk-ch04sec02]}}

:::success
**Learning Objectives**
- Define precipitate and solubility.
- {{sp[info] Objective 4.2a}} Apply solubility rules to predict whether an ionic compound is soluble.
- {{sp[info] Objective 4.2b}} Write molecular, ionic, and net ionic equations for a precipitation reaction.
- {{sp[info] Objective 4.2b}} Identify spectator ions.
:::

### Solubility and precipitates

**Solubility** is the maximum amount of a solute that dissolves in a given quantity of solvent at a given temperature. A **precipitate** is an insoluble solid that separates out of solution.

==A precipitation reaction happens only when one of the NEW cation–anion pairings turns out to be insoluble== — so predicting one comes down to a lookup, and these are the rules to memorize:

| Rule | Soluble? | Exceptions to memorize |
|---|---|---|
| Group 1A metal cations and $\ce{NH4+}$ | always **soluble** | none |
| $\ce{NO3-}$, $\ce{ClO3-}$, $\ce{HCO3-}$ | always **soluble** | none |
| $\ce{Cl-}$, $\ce{Br-}$, $\ce{I-}$ | mostly **soluble** | insoluble with $\ce{Ag+}$, $\ce{Pb^2+}$, $\ce{Hg2^2+}$ — e.g. $\ce{AgCl}$, $\ce{PbI2}$, $\ce{Hg2Cl2}$ |
| $\ce{SO4^2-}$ | mostly **soluble** | insoluble with $\ce{Ba^2+}$, $\ce{Pb^2+}$, $\ce{Hg2^2+}$ — e.g. $\ce{BaSO4}$, $\ce{PbSO4}$; $\ce{CaSO4}$ and $\ce{Ag2SO4}$ are only slightly soluble |
| $\ce{OH-}$, $\ce{CO3^2-}$ | mostly **insoluble** | soluble with Group 1A or $\ce{NH4+}$; $\ce{Ba(OH)2}$ is also soluble |

Read the first two rows first. If either ion in a candidate compound appears there, the compound dissolves and no precipitate forms — which settles a large fraction of all questions immediately.

:::: tabs
::: tab Problem
Predict whether each is soluble in water: $\ce{K2CO3}$, $\ce{BaSO4}$, $\ce{AgNO3}$, $\ce{Mg(OH)2}$.
:::
::: tab Solution
- **$\ce{K2CO3}$** — carbonates are usually insoluble, *but* potassium is a Group 1A metal, and that rule wins. **Soluble.**
- **$\ce{BaSO4}$** — sulfates are usually soluble, but $\ce{Ba^2+}$ is one of the three memorized exceptions. **Insoluble.**
- **$\ce{AgNO3}$** — silver halides are insoluble, but this is a nitrate, and all nitrates are soluble. **Soluble.**
- **$\ce{Mg(OH)2}$** — hydroxides are usually insoluble, and Mg2+ is not among the exceptions (Group 1A, NH4+, and the heavier Group 2A ions Ca2+, Sr2+, Ba2+). **Insoluble.**

Notice the pattern in the first and third: when an "always soluble" rule meets a "usually insoluble" rule, the always-soluble rule wins. Check the cation and the anion against the always-soluble rows first.
:::
::::

### Molecular, ionic, and net ionic equations

The same reaction can be written three ways, and each says something different.

- The **molecular equation** writes every compound as a neutral formula, as if nothing had dissociated. It is useful for bookkeeping and for telling you what to put in the flask.
- The **ionic equation** writes every dissolved (aqueous) *strong electrolyte* as the separate ions it actually exists as. Solids, weak electrolytes, and nonelectrolytes stay written as whole formulas, because that is how they actually exist.
- The **net ionic equation** removes the **spectator ions** — the ones that appear unchanged on both sides — leaving only the species that actually changed. Figure 4.3 tracks a single reaction's ions through all three.

![Schematic of a precipitation reaction, with every dissolved ion labeled and a key](../assets/precipitation_reaction.svg =620x)
*Figure 4.3 — Follow the individual ions, not the compounds. Each solution starts with **two** kinds of dissolved ion (see the key): $\ce{AgNO3}$ supplies $\ce{Ag+}$ and $\ce{NO3-}$; $\ce{NaCl}$ supplies $\ce{Na+}$ and $\ce{Cl-}$. On mixing, only $\ce{Ag+}$ and $\ce{Cl-}$ actually combine — they form insoluble $\ce{AgCl}$, which drops out of solution as a solid. The other two ions, $\ce{Na+}$ and $\ce{NO3-}$, drift through the whole process unchanged, which is exactly what makes them **spectator ions** and why they cancel out of the net ionic equation.*

**The four steps:**

1. Write the balanced molecular equation.
2. Rewrite it as an ionic equation, splitting only the dissolved (aq) strong electrolytes into ions.
3. Cancel the spectator ions — those identical on both sides.
4. Check that both atoms and charge balance in what remains.

:::: tabs
::: tab Problem
Give the ionic and net ionic equations for $\ce{AgNO3(aq) + NaCl(aq) -> AgCl(s) + NaNO3(aq)}$.
:::
::: tab Solution
**Ionic equation.** $\ce{AgNO3}$, $\ce{NaCl}$, and $\ce{NaNO3}$ are all soluble salts and therefore strong electrolytes, so all three split. $\ce{AgCl}$ is a solid and stays whole:

$$\ce{Ag+ + NO3- + Na+ + Cl- -> AgCl(s) + Na+ + NO3-}$$

**Cancel spectators.** $\ce{Na+}$ and $\ce{NO3-}$ appear identically on both sides:

$$\ce{Ag+(aq) + Cl-(aq) -> AgCl(s)}$$

**Check.** One Ag and one Cl on each side; charge is $(+1)+(-1)=0$ on the left and 0 on the right. ✓
:::
::::

:::: tabs
::: tab Problem
Give the net ionic equation for $\ce{Ba(OH)2(aq) + Na2SO4(aq) -> BaSO4(s) + 2NaOH(aq)}$.
:::
::: tab Solution
$\ce{Ba(OH)2}$ is one of the memorized soluble hydroxides, so it does dissociate — and note that it releases **two** hydroxide ions:

$$\ce{Ba^2+ + 2OH- + 2Na+ + SO4^2- -> BaSO4(s) + 2Na+ + 2OH-}$$

Canceling $\ce{Na+}$ and $\ce{OH-}$ leaves:

$$\ce{Ba^2+(aq) + SO4^2-(aq) -> BaSO4(s)}$$

**Check.** Charge is $(+2)+(-2)=0$ on the left, 0 on the right. ✓

The coefficients matter when canceling: two hydroxides on the left cancel two on the right, not one.
:::
::::

:::: tabs
::: tab Problem
Solutions of $\ce{KNO3}$ and $\ce{NaCl}$ are mixed. Write the net ionic equation.
:::
::: tab Solution
Work out the possible new pairings: $\ce{KCl}$ and $\ce{NaNO3}$. Check both against the solubility rules — potassium and sodium are Group 1A, and nitrate is always soluble, so **both are soluble**.

Nothing precipitates. Every ion is a spectator, and **there is no net ionic equation**: no reaction occurs. Mixing the two solutions just gives one solution containing four kinds of ion.

This case is as important as the others. A precipitation reaction only happens if one of the *new* pairings is insoluble, so always check both.
:::
::::

> **Where this goes next.** Precipitation is one thing dissolved ions can do: pair up and leave. §4.3 covers a second, which involves transferring a particle rather than pairing off — specifically, a proton.

## 4.3 Acid-Base Reactions{{attrs[#blk-ch04sec03]}}

:::success
**Learning Objectives**
- List the observable properties of acids and bases.
- {{sp[info] Objective 4.3a}} Distinguish the Arrhenius and Brønsted definitions.
- {{sp[info] Objective 4.3a}} Identify the common strong and weak acids.
- {{sp[info] Objective 4.3b}} Write net ionic equations for neutralization reactions.
:::

### What acids and bases do

Long before anyone could define them, acids and bases were recognized by how they behave.

| Acids | Bases |
|---|---|
| taste sour — vinegar (acetic acid), citrus fruit (citric acid) | taste bitter |
| change the color of plant dyes (e.g., turn blue litmus red) | feel slippery |
| react with certain metals to release $\ce{H2}$ gas | — |
| react with carbonates and bicarbonates to release $\ce{CO2}$ gas | — |
| their aqueous solutions conduct electricity | their aqueous solutions conduct electricity |

{{sp[warning] Watch out}} These are historical observations, not laboratory procedures. Never taste or touch a chemical to identify it.

That last shared row is the clue the definitions had to explain: both acids and bases produce ions in water.

### Two definitions

An **Arrhenius acid** produces $\ce{H+}$ (really $\ce{H3O+}$, the hydronium ion) in water; an **Arrhenius base** produces $\ce{OH-}$. This definition is simple and works well for aqueous solutions, but it is tied to water.

A **Brønsted acid** is a **proton donor**; a **Brønsted base** is a **proton acceptor**. A Brønsted acid must contain at least one ionizable hydrogen. This definition is broader — it does not mention water at all, and it lets a substance be an acid in one reaction and a base in another. Consider:

$$\ce{NH3 + H2O <=> NH4+ + OH-}$$

Going forward, $\ce{H2O}$ donates a proton to $\ce{NH3}$, so water is the acid and ammonia is the base. Going in reverse, $\ce{NH4+}$ donates a proton to $\ce{OH-}$, so the ammonium ion is the acid and hydroxide is the base. ==Being an acid is a role a substance plays in a particular reaction, not a permanent property of the substance.== Chapter 15 builds the whole of acid-base chemistry on this idea.

:::: tabs
::: tab Problem
For each reaction, identify the Brønsted acid and the Brønsted base: (a) $\ce{HCl + H2O -> H3O+ + Cl-}$; (b) $\ce{NH3 + H2O <=> NH4+ + OH-}$. What does comparing the two tell you about water?
:::
::: tab Solution
Ask one question each time: *which species handed over a proton?*

**(a)** $\ce{HCl}$ gives its proton to $\ce{H2O}$. So $\ce{HCl}$ is the **acid** and $\ce{H2O}$ is the **base**.

**(b)** Here $\ce{H2O}$ gives a proton to $\ce{NH3}$. So $\ce{H2O}$ is the **acid** and $\ce{NH3}$ is the **base**.

**Water played both roles**, base in (a) and acid in (b), even though it is the same substance in both. A substance able to do this is called *amphiprotic*, and water is the most important example.

This is exactly what the Arrhenius definition cannot express. Arrhenius asks what a substance *produces in water*, which makes water the fixed background rather than a participant. Brønsted asks who hands the proton to whom in this particular reaction — so the answer is allowed to change from one reaction to the next.
:::
::::

### Strong and weak acids

A **strong acid** ionizes completely in water; a **weak acid** ionizes only partially. This is the electrolyte distinction from §4.1, applied to acids — and it is the single most consequential thing to memorize in this chapter, because it decides how you write every ionic equation from here on.

**The strong acids** — there are only seven in general chemistry, so learn the list and treat everything else as weak:

$\ce{HCl}$ (hydrochloric) · $\ce{HBr}$ (hydrobromic) · $\ce{HI}$ (hydroiodic) · $\ce{HNO3}$ (nitric) · $\ce{H2SO4}$ (sulfuric) · $\ce{HClO4}$ (perchloric) · $\ce{HClO3}$ (chloric)

**Common weak acids:** $\ce{HF}$ (hydrofluoric), $\ce{HNO2}$ (nitrous), $\ce{H2SO3}$ (sulfurous), $\ce{H3PO4}$ (phosphoric), $\ce{HCN}$ (hydrocyanic), $\ce{HSO4-}$ (hydrogen sulfate), and the organic acids containing $\ce{-COOH}$ — acetic ($\ce{CH3COOH}$), formic ($\ce{HCOOH}$), benzoic ($\ce{C6H5COOH}$), and oxalic ($\ce{HOOC-COOH}$). Any acid with a $\ce{-COOH}$ group is a weak acid, which converts a long memorization into one recognizable pattern.

{{sp[warning] Reminder}} Sulfuric acid is a strong acid on its *first* proton only. The $\ce{HSO4-}$ left behind is itself a weak acid, which is why it appears on the weak list above.

:::: tabs
::: tab Problem
Classify each as a strong or weak acid, and write how each is represented in an ionic equation: $\ce{HClO4}$, $\ce{HClO2}$, $\ce{CH3COOH}$, $\ce{HI}$.
:::
::: tab Solution
Check each against the list of seven strong acids; anything absent from it is weak.

- **$\ce{HClO4}$** (perchloric) — on the list, **strong**. In an ionic equation it is split: $\ce{H+ + ClO4-}$.
- **$\ce{HClO2}$** (chlorous) — *not* on the list, **weak**. Written whole: $\ce{HClO2}$.
- **$\ce{CH3COOH}$** (acetic) — has a $\ce{-COOH}$ group, so **weak**. Written whole: $\ce{CH3COOH}$.
- **$\ce{HI}$** (hydroiodic) — on the list, **strong**. Split: $\ce{H+ + I-}$.

The $\ce{HClO4}$/$\ce{HClO2}$ pair is the one to study. They differ by two oxygen atoms and by nothing else you can see, yet one is among the strongest acids known and the other is weak. There is no shortcut here — the list of seven has to be memorized, and everything else treated as weak.
:::
::::

:::warning
**"Strong" does not mean "concentrated", and it does not mean "dangerous".** *Strong* describes how completely an acid ionizes, which is a fixed property of the substance. *Concentrated* describes how much of it is dissolved per liter, which you control. A 0.001 M solution of hydrochloric acid is a strong acid that is very dilute; glacial acetic acid is a weak acid that is nearly pure. The two words answer different questions, and mixing them up will produce wrong ionic equations for the rest of the course.
:::

### Neutralization

A **neutralization reaction** is an acid reacting with a base to give water and a salt. What the net ionic equation looks like depends on whether the acid and the base are strong or weak.

:::: tabs
::: tab Problem
Give the net ionic equation for the strong acid / strong base reaction $\ce{HCl(aq) + NaOH(aq) -> NaCl(aq) + H2O}$.
:::
::: tab Solution
Everything dissolved here is a strong electrolyte, so everything splits except the water:

$$\ce{H+ + Cl- + Na+ + OH- -> Na+ + Cl- + H2O}$$

$\ce{Na+}$ and $\ce{Cl-}$ are spectators:

$$\ce{H+ + OH- -> H2O}$$

Every strong acid / strong base neutralization that forms a soluble salt reduces to this same equation, whichever acid and base you started with — the identities cancel out.
:::
::::

:::: tabs
::: tab Problem
Give the net ionic equation for the weak acid / strong base reaction $\ce{HCN(aq) + NaOH(aq) -> NaCN(aq) + H2O}$.
:::
::: tab Solution
$\ce{HCN}$ is a **weak** acid, so it is mostly intact molecules in solution and must be written whole:

$$\ce{HCN + Na+ + OH- -> Na+ + CN- + H2O}$$

Only $\ce{Na+}$ is a spectator:

$$\ce{HCN + OH- -> CN- + H2O}$$

{{sp[warning] Reminder}} A weak acid or base keeps its molecular formula in an ionic equation. Only *strong* electrolytes get split into ions.

Compare with the previous problem: same base, same kind of reaction, and a completely different net ionic equation — because the acid was weak. Checking the strong-acid list is a step you cannot skip.
:::
::::

:::: tabs
::: tab Problem
Give the net ionic equation for $\ce{2HNO3(aq) + Ba(OH)2(aq) -> Ba(NO3)2(aq) + 2H2O}$.
:::
::: tab Solution
Nitric acid is strong; $\ce{Ba(OH)2}$ is a soluble hydroxide and a strong base; barium nitrate is soluble. All three split:

$$\ce{2H+ + 2NO3- + Ba^2+ + 2OH- -> Ba^2+ + 2NO3- + 2H2O}$$

Canceling $\ce{NO3-}$ and $\ce{Ba^2+}$:

$$\ce{2H+ + 2OH- -> 2H2O} \quad\text{which reduces to}\quad \ce{H+ + OH- -> H2O}$$

The final step matters: a net ionic equation is written in the lowest whole-number coefficients, so the 2s divide out. This confirms the pattern — every strong-acid/strong-base neutralization that forms a soluble salt is $\ce{H+ + OH- -> H2O}$.
:::
::::

> **Where this goes next.** Precipitation moved ions around; neutralization moved a proton. §4.4 covers the third and most general family, where what moves is an electron.

## 4.4 Oxidation-Reduction Reactions{{attrs[#blk-ch04sec04]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 4.4a}} Define oxidation and reduction in terms of electron transfer and oxidation-number change.
- Identify the oxidizing and reducing agents.
- {{sp[info] Objective 4.4a}} Assign oxidation numbers using the standard rule set.
- {{sp[info] Objective 4.4b}} Classify redox reactions (combination, decomposition, combustion, displacement, disproportionation).
- {{sp[info] Objective 4.4b}} Use the activity series to predict displacement reactions.
:::

### Electron transfer

A **redox** reaction — short for reduction–oxidation — is one in which electrons move from one species to another.

- **Oxidation** is the loss of electrons.
- **Reduction** is the gain of electrons.

==The two always happen together, because an electron that leaves one species has to arrive somewhere== — they are not two reactions, but one transfer described from each end.

![Electron-shell diagram of electron transfer from Na to F, before and after](../assets/electron_transfer_naf.svg =520x)
*Figure 4.4 — Why the transfer happens, drawn shell by shell. **Before (top):** sodium has a single, loosely-held valence electron in its third shell (highlighted red), while fluorine is one electron short of a full outer shell. **After (bottom):** that one electron moves from Na to F — and both end up with the same stable neon configuration (2, 8). Sodium is **oxidized** (lost an electron, now $\ce{Na+}$); fluorine is **reduced** (gained one, now $\ce{F-}$). Note there is only ever **one** electron in motion: oxidation and reduction are not two separate events but one transfer, counted from each atom's point of view.*

The agents are named for what they do to the *other* species, which is why they seem backwards at first:

- The **reducing agent** donates electrons — and is itself oxidized.
- The **oxidizing agent** accepts electrons — and is itself reduced.

In Figure 4.4, sodium is the reducing agent (it reduces fluorine) and fluorine is the oxidizing agent.

### Oxidation numbers

Electron transfer is obvious when ions form. It is far less obvious in a reaction like $\ce{CH4 + 2O2 -> CO2 + 2H2O}$, where nothing becomes an ion. The **oxidation number** is a bookkeeping device that makes the transfer visible anyway: it is the charge an atom *would* carry if every bond to a different element were fully ionic. Figure 4.5 places it on a scale, so that "oxidized" and "reduced" become directions rather than definitions to memorize.

![Oxidation number shown on a number line, with a worked assignment for sulfur in sulfate](../assets/oxidation_number_line.svg =800x)
*Figure 4.5 — Oxidation numbers laid out on a number line. Moving right — a more positive number — means electrons were lost, which is oxidation. Moving left means electrons were gained, which is reduction. The panel works through one assignment step by step.*

**The rules, in the order you apply them:**

1. A free element is **0** — this covers $\ce{Na}$, $\ce{O2}$, $\ce{P4}$, and any other uncombined element.
2. A monatomic ion equals its charge: $\ce{Na+}$ is $+1$, $\ce{S^2-}$ is $-2$.
3. Hydrogen is usually $+1$, oxygen usually $-2$. **Exceptions:** hydrogen is $-1$ in metal hydrides such as $\ce{LiH}$; oxygen is $-1$ in peroxides such as $\ce{H2O2}$.
4. In compounds, Group 1A metals are always $+1$, Group 2A always $+2$, fluorine always $-1$.
5. The oxidation numbers in a neutral molecule sum to **0**; in a polyatomic ion they sum to the **ion's charge**.

Rule 5 is the one that does the work — the others give you the known values, and rule 5 solves for the unknown.

{{sp[warning] Reminder}} Oxidation numbers need not be whole numbers. In the superoxide ion $\ce{O2-}$, each oxygen is $-1/2$. Treat the rules as a consistent convention, not as a description of real charges.

:::: tabs
::: tab Problem
Assign the oxidation number of the named element in each: (a) N in $\ce{HNO3}$; (b) Cr in $\ce{Cr2O7^2-}$; \(c) C in $\ce{CH4}$.
:::
::: tab Solution
**(a) N in $\ce{HNO3}$.** H is $+1$, O is $-2$ and there are three. The molecule is neutral, so everything sums to 0:
$$(+1) + x + 3(-2) = 0 \;\Rightarrow\; x = +5$$

**(b) Cr in $\ce{Cr2O7^2-}$.** Seven oxygens at $-2$ give $-14$. This is an ion of charge $-2$, so the sum is $-2$, not 0:
$$2x + 7(-2) = -2 \;\Rightarrow\; 2x = +12 \;\Rightarrow\; x = +6$$
Note the division by 2 at the end — the answer is per chromium atom.

**\(c) C in $\ce{CH4}$.** Four hydrogens at $+1$ give $+4$; the molecule is neutral:
$$x + 4(+1) = 0 \;\Rightarrow\; x = -4$$
Carbon is negative here, which surprises people. It is a consequence of rule 3, not a claim that carbon carries four extra electrons.
:::
::::

:::: tabs
::: tab Problem
For $\ce{Zn + CuSO4 -> ZnSO4 + Cu}$, identify what is oxidized, what is reduced, the oxidizing agent, and the reducing agent.
:::
::: tab Solution
Assign oxidation numbers to the species that change. Sulfate is unchanged on both sides, so ignore it.

- Zn: **0** as a free element → **$+2$** in $\ce{ZnSO4}$. The number went **up**, so zinc was **oxidized**.
- Cu: **$+2$** in $\ce{CuSO4}$ → **0** as free copper. The number went **down**, so copper was **reduced**.

Now the agents, named for their effect on the other species:
- Zinc gave the electrons away, so zinc is the **reducing agent**.
- Copper(II) took them, so $\ce{Cu^2+}$ is the **oxidizing agent**.

The species oxidized is always the reducing agent, and the species reduced is always the oxidizing agent. If that seems backwards, read the name as a job description: the reducing agent's job is to reduce something else.
:::
::::

### Types of redox reaction

| Type | What happens | Example |
|---|---|---|
| **Combination** | two or more reactants form one product | $\ce{2Al + 3Br2 -> 2AlBr3}$ |
| **Decomposition** | one compound breaks into simpler parts | $\ce{2KClO3 -> 2KCl + 3O2}$ |
| **Combustion** | a substance reacts with $\ce{O2}$ | $\ce{2H2 + O2 -> 2H2O}$ |
| **Displacement** | one element replaces another in a compound | $\ce{Zn + 2HCl -> ZnCl2 + H2}$ |
| **Disproportionation** | the *same* element is both oxidized and reduced | $\ce{Cl2 + 2OH- -> ClO- + Cl- + H2O}$ |

Displacement comes in three flavors worth naming separately: **hydrogen displacement** (a metal displaces $\ce{H2}$ from water or acid), **metal displacement** (a more active metal displaces a less active one, e.g. $\ce{TiCl4 + 2Mg -> Ti + 2MgCl2}$), and **halogen displacement**, which follows the order $\ce{F2 > Cl2 > Br2 > I2}$, so that $\ce{Cl2 + 2KBr -> 2KCl + Br2}$ proceeds but the reverse does not.

Disproportionation is the one to look at twice. In $\ce{Cl2 + 2OH- -> ClO- + Cl- + H2O}$, chlorine starts at 0, ends at $+1$ in $\ce{ClO-}$ and at $-1$ in $\ce{Cl-}$. The same element went both up and down.

:::: tabs
::: tab Problem
Classify each reaction and give the oxidation-number changes: (a) $\ce{2N2O -> 2N2 + O2}$; (b) $\ce{6Li + N2 -> 2Li3N}$; \(c) $\ce{Ni + Pb(NO3)2 -> Pb + Ni(NO3)2}$.
:::
::: tab Solution
**(a) Decomposition.** One reactant becomes two products. Both products are free elements, so both are 0. In $\ce{N2O}$, oxygen is $-2$ (rule 3), so the two nitrogens must supply $+2$ between them: N is $+1$. Nitrogen goes $+1 \to 0$ (reduced), oxygen $-2 \to 0$ (oxidized).

**(b) Combination.** Two reactants become one product. Both reactants are free elements, so both are 0. In $\ce{Li3N}$, lithium is $+1$ (rule 4), so nitrogen must be $-3$. Lithium goes $0 \to +1$ (oxidized), nitrogen $0 \to -3$ (reduced).

**\(c) Metal displacement.** Nitrate is unchanged throughout, so ignore it. Ni goes $0 \to +2$ (oxidized); Pb goes $+2 \to 0$ (reduced). Nickel displaced lead, which tells you nickel is the more active of the two.
:::
::::

### The activity series

Whether a displacement reaction actually happens depends on how reactive the metals are. The **activity series** (Figure 4.6) ranks them, and Figure 4.7 shows one displacement in progress.

| Metals | What they react with to give $\ce{H2}$ |
|---|---|
| Li, K, Ba, Ca, Na | **cold water** |
| Mg, Al, Zn, Cr, Fe, Cd | **steam** |
| Co, Ni, Sn, Pb | **acids** only |
| Cu, Ag, Hg, Pt, Au | **nothing** — no $\ce{H2}$ from water or acid |

![Activity series of metals, color-coded by reactivity tier](../assets/activity_series_ladder.svg =360x)
*Figure 4.6 — The activity series orders metals from most reactive (top) to least reactive (bottom); a metal displaces any less-active metal (lower on this list) from its compound in solution.*

![Iron wire displacing copper from a copper chloride solution](../assets/displaced_copper.jpg =420x)
*Figure 4.7 — Iron is more active than copper (higher on the activity series), so it displaces copper metal directly out of copper chloride solution: $\ce{Fe(s) + CuCl2(aq) -> FeCl2(aq) + Cu(s)}$, visible here as reddish copper crystals coating the iron wire.*


:::: tabs
::: tab Problem
Will each of these reactions occur? (a) $\ce{Cu(s)}$ placed in $\ce{HCl(aq)}$; (b) $\ce{Zn(s)}$ placed in $\ce{HCl(aq)}$; \(c) $\ce{Br2}$ added to a solution of $\ce{NaCl}$.
:::
::: tab Solution
**(a) No.** Copper is in the bottom tier of the activity series — it does not release $\ce{H2}$ from water or acid. This is exactly why copper is used for plumbing.

**(b) Yes.** Zinc is in the tier that reacts with steam, and everything above the bottom tier reacts with acid: $\ce{Zn + 2HCl -> ZnCl2 + H2}$.

**\(c) No.** Halogen displacement runs $\ce{F2 > Cl2 > Br2 > I2}$. Bromine is *less* active than chlorine, so it cannot displace chloride. The reverse, $\ce{Cl2}$ added to $\ce{NaBr}$, would work.

The general rule for all three: a displacement happens only when the incoming element is *more* active than the one already in the compound.
:::
::::

> **Where this goes next.** You can now predict which reactions happen in solution. What you cannot yet do is say how much — and in solution, amounts are measured as concentrations rather than masses. §4.5 supplies the conversion.

## 4.5 Solution Stoichiometry{{attrs[#blk-ch04sec05]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 4.5a}} Calculate and use molarity.
- {{sp[info] Objective 4.5b}} Determine the concentration of an individual ion from a compound's molarity.
- {{sp[info] Objective 4.5a}} Apply the dilution equation $M_iV_i=M_fV_f$.
- {{sp[info] Objective 4.5b}} Describe gravimetric analysis and titration, and use titration data.
:::

### Molarity

Chapter 3's stoichiometry runs on moles, and a balance gives you moles by way of mass. A solution does not work that way: you measure out a *volume*. **Molarity** is the conversion factor that closes the gap.

$$M = \text{molarity} = \frac{\text{moles of solute}}{\text{liters of solution}}$$

The unit is mol/L, usually written **M**. ==Read a molarity as a conversion factor and it behaves exactly like molar mass did in Chapter 3:== 0.50 M means "0.50 mol per 1 L," to be written either way up as the cancellation requires.

{{sp[warning] Watch out}} The denominator is liters of **solution**, not liters of solvent. A 1.0 M solution is made by dissolving one mole and then adding water *until the total volume is one liter* — not by adding one liter of water.

:::: tabs
::: tab Problem
How many grams of glucose ($\ce{C6H12O6}$, 180.18 g/mol) are needed to make 250 mL of a 0.283 M solution?
:::
::: tab Solution
Three conversions, chained so each unit cancels:

$$250\,\text{mL}\times\frac{1\,\text{L}}{1000\,\text{mL}}\times\frac{0.283\,\text{mol}}{1\,\text{L}}\times\frac{180.18\,\text{g}}{1\,\text{mol}}=12.7\ \text{g}$$

Carrying full precision through — $0.250\,\text{L}\times0.283\,\text{mol/L}=0.07075\,\text{mol}$, then $\times\,180.18\,\text{g/mol}$ — gives 12.7 g. Rounding the intermediate mole value first would shift the answer.
:::
::::

:::: tabs
::: tab Problem
What is the molarity of a solution made by dissolving 5.85 g of $\ce{NaCl}$ (58.44 g/mol) in enough water to make 500.0 mL?
:::
::: tab Solution
Molarity needs moles on top and liters on the bottom, so convert both.

$$5.85\,\text{g}\times\frac{1\,\text{mol}}{58.44\,\text{g}}=0.1001\ \text{mol}\qquad 500.0\,\text{mL}=0.5000\ \text{L}$$
$$M=\frac{0.1001\ \text{mol}}{0.5000\ \text{L}}=0.200\ \text{M}$$

This is the previous problem run backwards: there you were given a molarity and found a mass; here you are given a mass and find the molarity.
:::
::::

:::: tabs
::: tab Problem
What is the concentration of each ion in a 0.25 M solution of $\ce{Al2(SO4)3}$?
:::
::: tab Solution
The label gives the concentration of the *compound*, but §4.1 established that the compound is not what is actually in solution. Read the formula for how many of each ion one formula unit releases:

$$\ce{Al2(SO4)3 -> 2Al^3+ + 3SO4^2-}$$

$$[\ce{Al^3+}] = 2\times0.25 = 0.50\ \text{M}\qquad [\ce{SO4^2-}] = 3\times0.25 = 0.75\ \text{M}$$

Neither equals 0.25 M. This is a routine exam trap, and the fix is always to write the dissociation equation first.
:::
::::

### Dilution

**Dilution** is preparing a less concentrated solution from a more concentrated one by adding solvent. The key insight is what does *not* change: adding water adds no solute, so the moles of solute are the same before and after.

Since moles $= M \times V$, that conservation is the whole equation, and Figure 4.8 is that sentence drawn:

$$M_iV_i = M_fV_f$$

![Dilution shown as the same solute particles spread through a larger volume](../assets/dilution_same_moles.svg =780x)
*Figure 4.8 — Dilution changes the concentration and the volume but not the amount of solute. Count the particles: twelve before, twelve after. Concentration falls by exactly the same factor that volume rises, so their product holds constant — which is all the dilution equation says.*

:::: tabs
::: tab Problem
How would you prepare 50 mL of 1.00 M HCl from a 3.92 M stock solution?
:::
::: tab Solution
Identify which three of the four quantities you have: $M_i = 3.92$ M, $M_f = 1.00$ M, $V_f = 50$ mL. Solve for $V_i$:

$$V_i=\frac{M_fV_f}{M_i}=\frac{1.00\,\text{M}\times50\,\text{mL}}{3.92\,\text{M}}=12.8\ \text{mL}$$

**In practice:** measure 12.8 mL of the 3.92 M stock, then add water until the *total* volume reaches 50 mL. You do not add 50 mL of water.

Note that the volumes cancel as a ratio, so milliliters may be used on both sides without converting to liters — as long as both volumes use the same unit.
:::
::::

### Gravimetric analysis

**Gravimetric analysis** determines how much of an ion is present by turning it into a weighable solid — a direct application of §4.2.

1. Dissolve the unknown sample in water.
2. React it with a solution known to precipitate the ion of interest.
3. Filter off the precipitate.
4. Dry it, then weigh it.
5. Use the precipitate's formula and mass to work back to the amount of the unknown ion.

Step 5 is Chapter 3's road map run in reverse: mass of precipitate → moles of precipitate → moles of the ion → mass of the ion.

### Titration

In a **titration**, a solution of accurately known concentration is added gradually to a solution of unknown concentration until the reaction between them is complete. Titrations are used for both acid-base and redox analysis.

The **equivalence point** is the point at which exactly enough has been added for complete reaction. An **indicator** is a substance that changes color at or near that point, and the moment you actually observe the change is the **endpoint**. Figure 4.9 shows the apparatus and the distinction.

![Titration apparatus with the indicator stages and the equivalence point defined](../assets/titration_setup.svg =800x)
*Figure 4.9 — A titration. Titrant of known concentration is delivered from the burette into the analyte, and an indicator signals when the reaction is complete. The equivalence point is a fact about the chemistry; the endpoint is what the eye sees. A well-chosen indicator makes them coincide closely enough to ignore the difference.*

:::: tabs
::: tab Problem
It takes 27.4 mL of 0.100 M NaOH to neutralize 25.0 mL of an HCl solution of unknown concentration. What is that concentration?
:::
::: tab Solution
**Step 1 — the balanced equation**, since it supplies the mole ratio:
$$\ce{HCl + NaOH -> NaCl + H2O}$$
The ratio is 1:1.

**Step 2 — moles of the known.** Molarity times volume gives moles:
$$0.0274\,\text{L}\times0.100\,\text{M}=2.74\times10^{-3}\ \text{mol NaOH}$$

**Step 3 — cross to the unknown** using the mole ratio. It is 1:1, so $2.74\times10^{-3}$ mol HCl.

**Step 4 — back to a concentration**, using the analyte's own volume:
$$M=\frac{2.74\times10^{-3}\ \text{mol}}{0.0250\ \text{L}}=0.110\ \text{M}$$

This is Chapter 3's road map with molarity substituted for molar mass at both ends. {{sp[warning] Reminder}} Divide by the volume of the *unknown* solution at the end, not the titrant's volume.
:::
::::

:::: tabs
::: tab Problem
It takes 31.5 mL of 0.150 M NaOH to neutralize 25.0 mL of $\ce{H2SO4}$. What is the sulfuric acid's concentration?
:::
::: tab Solution
**The balanced equation is the whole difficulty here**, because sulfuric acid has two ionizable protons:
$$\ce{H2SO4 + 2NaOH -> Na2SO4 + 2H2O}$$
The ratio is **1 acid to 2 base**, not 1:1.

$$0.0315\,\text{L}\times0.150\,\text{M}=4.725\times10^{-3}\ \text{mol NaOH}$$
$$4.725\times10^{-3}\ \text{mol NaOH}\times\frac{1\,\text{mol}\,\ce{H2SO4}}{2\,\text{mol NaOH}}=2.363\times10^{-3}\ \text{mol}\,\ce{H2SO4}$$
$$M=\frac{2.363\times10^{-3}\ \text{mol}}{0.0250\ \text{L}}=0.0945\ \text{M}$$

Assuming a 1:1 ratio would have given 0.189 M — exactly twice the right answer. Write the balanced equation before touching the numbers.
:::
::::

## Synthesis

==This chapter sorts aqueous reactions into three main families — precipitation, acid-base, and redox — each governed by its own predictive rule: solubility rules, the strong-acid list, and oxidation-number bookkeeping. Molarity and dilution then supply the quantitative language shared by all three.==

The dependencies run in both directions. Everything here rests on Chapter 2 (you cannot apply a solubility rule without recognizing the ions, or write a formula without naming) and Chapter 3 (every solution-stoichiometry problem is the mole road map with molarity in place of molar mass). Looking forward, the strong/weak electrolyte distinction from §4.1 is the foundation of Chapters 15 and 16; oxidation numbers return in Chapter 18 as the basis of electrochemistry; titration is the working method of Chapter 16; and molarity is assumed without comment from Chapter 12 onward.

## Asset and License Record for This Chapter

| Asset | Source URL | License | Attribution |
|---|---|---|---|
| `assets/electrolyte_conductivity.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated, schematic; released under this package's CC BY 4.0 license. |
| `assets/hydration_of_ions.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated, schematic; released under this package's CC BY 4.0 license. |
| `assets/precipitation_reaction.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated, schematic; released under this package's CC BY 4.0 license. |
| `assets/electron_transfer_naf.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated, schematic (replaces a hotlinked source image); released under this package's CC BY 4.0 license. |
| `assets/oxidation_number_line.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
| `assets/activity_series_ladder.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated from the study guide's own activity-series table; released under this package's CC BY 4.0 license. |
| `assets/displaced_copper.jpg` | https://commons.wikimedia.org/wiki/File:Displaced_copper_crystal.jpg | CC BY-SA 4.0 | 2x910, via Wikimedia Commons. |
| `assets/dilution_same_moles.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated from the study guide's own worked-example data; released under this package's CC BY 4.0 license. |
| `assets/titration_setup.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated, schematic; released under this package's CC BY 4.0 license. |
