{{nyml
kind: document
format: 1
title: Chapter 3: Stoichiometry
}}

# Chapter 3: Stoichiometry

:::info
**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 3 (CC BY 4.0)
**Audience:** introductory undergraduate general chemistry, first semester
**Package license:** CC BY 4.0
**Note:** builds on Chapter 2's chemical formulas; facts checked for accuracy against OpenStax *Chemistry 2e* and Wikipedia (used for reference only — no text or figures adapted from either).
:::

:::success
**Chapter Learning Objectives**
- Calculate atomic mass, molecular/formula mass, and molar mass; convert among mass, moles, and particle count.
- Calculate percent composition and determine an empirical formula from combustion-analysis data.
- Balance chemical equations and use them to convert between quantities of reactants and products.
- Determine the limiting reagent, theoretical yield, and percent yield.
:::

## Chapter Logic

Chapter 2 taught you to write a correct formula. This chapter makes formulas quantitative. The problem it solves is a practical one: chemistry happens between *particles*, in whole-number ratios, but you cannot count particles — you can only weigh them. ==The mole is the unit that bridges those two worlds, and every calculation in this chapter, and in most of the rest of the course, passes through it.==

{{mermaid
graph TD
  A["Molar mass:<br/>atomic, molecular, formula mass"] --> B["Mole conversions:<br/>mass, moles, particles"]
  B --> C["Balanced equations:<br/>mole-to-mole ratios"]
  C --> D["Limiting reagent,<br/>theoretical and percent yield"]
}}

**Visual description:** A top-down flowchart. Molar mass converts a formula into a number in grams per mole. That number lets you convert between mass, moles, and particle count for any substance. A balanced equation then relates moles of one substance to moles of another. Limiting reagent and yield calculations are the final, most realistic application of that mole-to-mole relationship.

## 3.1 Molar Mass{{attrs[#blk-ch03sec01]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 3.1a}} Understand atomic mass, average atomic mass, molar mass, and the mole.
- {{sp[info] Objective 3.1b}} Calculate mass, moles, and number of particles given one of the three.
- {{sp[info] Objective 3.1c}} Calculate molecular mass, formula mass, and percent composition.
- {{sp[info] Objective 3.1d}} Determine an empirical formula from combustion-analysis data, and a molecular formula from an empirical formula plus a molar mass.
:::

### Atomic mass and average atomic mass

Atoms are far too light to weigh individually in grams, so chemists use a scale built for them. One **atomic mass unit (amu)** is defined as exactly $1/12$ the mass of one $\ce{^{12}C}$ atom. This one *is* still tied to carbon-12 — the 2019 SI revision redefined the mole, not the atomic mass unit.

On this scale the atomic mass of $\ce{^{1}H}$ is 1.008 amu, not exactly 1 amu. The reason is worth knowing: a nucleus weighs slightly less than its separated protons and neutrons would, and by different amounts in different elements; the amu is set by carbon-12, whose nucleons have lost mass this way, while $^1H$'s lone proton has not, so $^1H$ comes out slightly above 1 amu (Chapter 19 explains why — the missing mass is the nuclear binding energy).

The number printed under each element symbol on the periodic table is not any single atom's mass. It is the **average atomic mass**: the weighted average over all the isotopes of that element as they occur in nature. Chapter 2 established that an element's atoms can differ in neutron count; this is the number that accounts for that mixture.

:::: tabs
::: tab Problem
Copper's two stable isotopes are $\ce{^{63}Cu}$ (69.09% abundant, 62.93 amu) and $\ce{^{65}Cu}$ (30.91% abundant, 64.9278 amu). Find copper's average atomic mass.
:::
::: tab Solution
A weighted average multiplies each value by its fractional share and adds. Convert the percentages to decimals first:

$$62.93\,\text{amu}\times0.6909+64.9278\,\text{amu}\times0.3091=63.55\ \text{amu}$$

Check the answer for sense before moving on: 63.55 lies between 62.93 and 64.9278, and it sits much closer to 62.93 — which is right, because the lighter isotope is more than twice as abundant. A weighted average always leans toward the more common value.
:::
::::

:::: tabs
::: tab Problem
Chlorine has two stable isotopes, $\ce{^{35}Cl}$ (34.969 amu) and $\ce{^{37}Cl}$ (36.966 amu). The periodic table gives chlorine's average atomic mass as 35.45 amu. Without calculating, which isotope is more abundant? Then find the abundance of $\ce{^{35}Cl}$.
:::
::: tab Solution
**By inspection:** 35.45 is much closer to 34.969 than to 36.966, so $\ce{^{35}Cl}$ must be the more abundant one.

**By calculation:** let $x$ be the fraction that is $\ce{^{35}Cl}$; then $1-x$ is the fraction that is $\ce{^{37}Cl}$.

$$34.969x + 36.966(1-x) = 35.45$$
$$34.969x + 36.966 - 36.966x = 35.45$$
$$-1.997x = -1.516 \quad\Rightarrow\quad x = 0.759$$

So chlorine is **75.9% $\ce{^{35}Cl}$** and 24.1% $\ce{^{37}Cl}$ — consistent with the inspection.

This is the same relationship as the copper problem, run backwards. Notice which unknown you are solving for before you set up.
:::
::::

**Mass spectrometry** is the experiment behind those abundances. A mass spectrometer ionizes a sample and sorts the ions by their mass-to-charge ratio, producing a spectrum whose peak positions give the isotope masses and whose peak heights give the relative abundances. Every average atomic mass on the periodic table traces back to measurements of this kind.

### The mole

The **mole (mol)** is the amount of substance containing exactly $6.02214076\times10^{23}$ elementary entities. That number is **Avogadro's number**:

$$1\,\text{mol} = N_A = 6.022\times10^{23}\ \text{entities}$$

:::info
**Two definitions, and why you will meet both.** Until 20 May 2019, the mole was defined as *the amount of substance containing as many entities as there are atoms in exactly 12 g of* $\ce{^{12}C}$ — an experimental quantity, so $N_A$ had a measured value with an uncertainty, and older tables give it to eight or nine digits (6.0221415, 6.02214129, and so on) that shift slightly between editions. Since 2019 the SI has run the definition the other way: $N_A$ is **fixed by definition** at exactly $6.02214076\times10^{23}\ \text{mol}^{-1}$, and the mole is defined from it. Carbon-12 is no longer part of the definition.

Nothing you calculate changes. The two definitions agree to well beyond the four significant figures this course uses, and $6.022\times10^{23}$ remains correct under both. What changed is the direction of the definition — from "measure this, then report $N_A$" to "$N_A$ is this number, exactly." Textbooks printed before 2019, including many still in use, give the carbon-12 wording.
:::

A mole is a counting word, exactly like "dozen" or "pair." A dozen eggs is 12 eggs; a mole of atoms is $6.022\times10^{23}$ atoms. What makes it strange is only its size — and Figure 3.1 is worth a moment, because that size is the whole reason the unit is useful.

![Three comparisons giving a sense of the size of Avogadro's number](../assets/how_big_is_a_mole.svg =760x)
*Figure 3.1 — Avogadro's number is inconceivably large, and that is the point. Atoms are so small that a count too big to picture corresponds to an amount you can hold in a spoon. The mole was chosen for exactly this reason: it is the scaling factor that turns particle-level ratios into laboratory-level masses.*

**Molar mass** is the mass of one mole of a substance, in grams. Its definition is arranged so that no conversion factor is needed between atomic mass and molar mass: ==an element's average atomic mass in amu is numerically equal to its molar mass in grams per mole.== Carbon is 12.01 amu per atom and 12.01 g per mole; copper is 63.55 amu per atom and 63.55 g per mole.

### Converting between mass, moles, and particles

![Diagram of mole conversions between mass, moles, and particle count](../assets/mole_conversion_triangle.svg =480x)
*Figure 3.2 — Molar mass (g/mol) converts between mass and moles; Avogadro's number converts between moles and particle count. Moles sit in the middle: to get from a mass to a particle count, you must pass through moles.*

Both conversions are dimensional analysis, the technique from Chapter 1 — write the conversion factor so the unit you have cancels.

:::: tabs
::: tab Problem
How many grams of Zn are in 0.356 mol Zn? How many moles of $\ce{CH4}$ are in 6.07 g?
:::
::: tab Solution
The two questions run in opposite directions, so the same conversion factor is written two different ways.

**Moles → grams.** You have moles and want grams, so molar mass goes on top:
$$0.356\,\text{mol}\,\ce{Zn}\times\frac{65.39\,\text{g}\,\ce{Zn}}{1\,\text{mol}\,\ce{Zn}}=23.3\ \text{g}\,\ce{Zn}$$

**Grams → moles.** Now you have grams and want moles, so molar mass is inverted:
$$6.07\,\text{g}\,\ce{CH4}\times\frac{1\,\text{mol}\,\ce{CH4}}{16.04\,\text{g}\,\ce{CH4}}=0.378\ \text{mol}\,\ce{CH4}$$

{{sp[warning] Reminder}} Do not memorize which way to divide. Write the factor so the unit you are holding cancels, and the arithmetic follows.
:::
::::

:::: tabs
::: tab Problem
How many atoms of carbon are in 2.50 g of carbon?
:::
::: tab Solution
There is no direct gram-to-atom conversion. Go through moles, as Figure 3.2 shows.

$$2.50\,\text{g}\,\ce{C}\times\frac{1\,\text{mol}\,\ce{C}}{12.01\,\text{g}\,\ce{C}}=0.2082\ \text{mol}\,\ce{C}$$
$$0.2082\,\text{mol}\,\ce{C}\times\frac{6.022\times10^{23}\ \text{atoms}}{1\,\text{mol}}=1.25\times10^{23}\ \text{atoms}$$

Sanity check: 2.50 g of carbon is about a fifth of a mole (12.01 g/mol), and the answer is about a fifth of $6.022\times10^{23}$. ✓
:::
::::

### Molecular mass and formula mass

**Molecular mass** is the sum of the atomic masses in a molecule. **Formula mass** is the same sum taken over whatever the chemical formula says — the term used for ionic compounds, which have no discrete molecules to speak of. Both are numerically equal to the molar mass in grams per mole.

The distinction is the one Chapter 2 drew about $\ce{NaCl}$: there is no such thing as an "$\ce{NaCl}$ molecule," only a lattice in a 1:1 ratio, so 58.44 is the formula mass of $\ce{NaCl}$, not its molecular mass. The arithmetic is identical either way.

:::: tabs
::: tab Problem
Find the molar mass of $\ce{H2O}$, of $\ce{CH4}$, and of the ionic compound $\ce{NaCl}$.
:::
::: tab Solution
Add up the atomic masses, counting each atom the number of times the subscript says.

$\ce{H2O}$: $2(1.008)+16.00=18.02\ \text{g/mol}$ (molecular mass — water is molecular).

$\ce{CH4}$: $12.01+4(1.008)=16.04\ \text{g/mol}$ (molecular mass).

$\ce{NaCl}$: $22.99+35.45=58.44\ \text{g/mol}$ (formula mass — $\ce{NaCl}$ is ionic).
:::
::::

:::: tabs
::: tab Problem
Find the molar mass of calcium nitrate, $\ce{Ca(NO3)2}$.
:::
::: tab Solution
The parentheses are the whole difficulty here. The subscript 2 multiplies *everything* inside them, so this formula contains one Ca, two N, and six O.

$$40.08 + 2(14.01) + 6(16.00) = 40.08 + 28.02 + 96.00 = 164.10\ \text{g/mol}$$

A common error is to count only three oxygens, giving 116.10. Whenever a formula has parentheses, expand it explicitly before adding.
:::
::::

### Percent composition

**Percent composition** is the percentage by mass contributed by each element in a compound:

$$\%\ \text{element} = \frac{\text{mass of that element in one mole of compound}}{\text{molar mass of the compound}}\times100\%$$

![Percent composition of water shown as a proportional mass bar](../assets/percent_composition_water.svg =760x)
*Figure 3.3 — Percent composition asks about mass, not about how many atoms there are. Water is two-thirds hydrogen by atom count and only 11% hydrogen by mass, because an oxygen atom is about sixteen times heavier than a hydrogen atom.*

:::: tabs
::: tab Problem
Find the percent composition of water, $\ce{H2O}$.
:::
::: tab Solution
Work with one mole of the compound throughout.

Figure 3.3 shows where the answer has to come out. One mole of $\ce{H2O}$ contains two moles of H atoms, so the hydrogen present weighs $2\times1.008=2.016$ g. It contains one mole of O atoms, weighing 16.00 g. The molar mass is their sum, 18.02 g/mol.

$$\%\,\ce{H}=\frac{2.016}{18.02}\times100\%=11.19\%$$
$$\%\,\ce{O}=\frac{16.00}{18.02}\times100\%=88.79\%$$

Once you have all but one element, the last one can be had by subtraction: $100\%-11.19\%=88.81\%$. Computing every element directly and adding them is the check — **if the percentages do not sum to 100% (within rounding), something is wrong before you go any further.**
:::
::::

:::: tabs
::: tab Problem
A fertilizer is sold on the basis of its nitrogen content. Which supplies more nitrogen per gram, ammonium nitrate ($\ce{NH4NO3}$, 80.05 g/mol) or urea ($\ce{(NH2)2CO}$, 60.06 g/mol)?
:::
::: tab Solution
Percent composition is exactly the right tool, because the question is about nitrogen *per gram* rather than per formula unit.

**Ammonium nitrate** contains 2 N per formula unit:
$$\%\,\ce{N}=\frac{2(14.01)}{80.05}\times100\%=35.00\%$$

**Urea** also contains 2 N per formula unit:
$$\%\,\ce{N}=\frac{2(14.01)}{60.06}\times100\%=46.65\%$$

**Urea** is the richer nitrogen source. Both compounds carry two nitrogen atoms, so the difference comes entirely from urea's smaller molar mass — less non-nitrogen mass is being carried along. This is why percent composition, not formula, is what a fertilizer label reports.
:::
::::

### Empirical formulas from combustion analysis

Chapter 2 defined the empirical formula as the simplest whole-number atom ratio. Percent composition is the bridge to finding one experimentally: a mass ratio can be converted to a mole ratio, and a mole ratio, reduced to simplest whole numbers, *is* the empirical formula.

**Combustion analysis** is the standard method for compounds containing carbon and hydrogen. Burn a weighed sample completely in oxygen, and trap the products separately (Figure 3.4). All the carbon leaves as $\ce{CO2}$ and all the hydrogen leaves as $\ce{H2O}$, so each trap's mass gain reports on one element.

![Schematic of a combustion analysis apparatus](../assets/combustion_analysis.svg =620x)
*Figure 3.4 — Each absorber's mass gain, converted using the product's molar mass and formula (1 C per CO2, 2 H per H2O), gives the moles of one element: all the carbon in the sample ends up as $\ce{CO2}$, and all the hydrogen ends up as $\ce{H2O}$.*

{{sp[warning] Watch out}} Oxygen cannot be measured this way, because the combustion adds oxygen from the air. Any oxygen in the original compound must be found by difference, after the C and H masses are subtracted from the sample mass.

:::: tabs
::: tab Problem
Combusting 11.5 g of ethanol produces 22.0 g $\ce{CO2}$ and 13.5 g $\ce{H2O}$. Find ethanol's empirical formula.
:::
::: tab Solution
**Step 1 — moles of C**, from the $\ce{CO2}$. Each $\ce{CO2}$ carries exactly one C:
$$22.0\,\text{g}\,\ce{CO2}\times\frac{1\,\text{mol}\,\ce{CO2}}{44.0\,\text{g}\,\ce{CO2}}\times\frac{1\,\text{mol}\,\ce{C}}{1\,\text{mol}\,\ce{CO2}}=0.500\ \text{mol}\,\ce{C}$$

**Step 2 — moles of H**, from the $\ce{H2O}$. Each $\ce{H2O}$ carries *two* H, so the ratio is 2:1, not 1:1:
$$13.5\,\text{g}\,\ce{H2O}\times\frac{1\,\text{mol}\,\ce{H2O}}{18.0\,\text{g}\,\ce{H2O}}\times\frac{2\,\text{mol}\,\ce{H}}{1\,\text{mol}\,\ce{H2O}}=1.50\ \text{mol}\,\ce{H}$$

**Step 3 — oxygen by difference.** Convert the C and H to masses and subtract both from the sample:
$$m_\ce{O}=11.5\,\text{g}-(0.500\,\text{mol}\times12.0\,\text{g/mol})-(1.50\,\text{mol}\times1.008\,\text{g/mol})=4.0\ \text{g}\,\ce{O}$$
$$4.0\,\text{g}\,\ce{O}\times\frac{1\,\text{mol}\,\ce{O}}{16.0\,\text{g}\,\ce{O}}=0.25\ \text{mol}\,\ce{O}$$

**Step 4 — divide by the smallest.** The three mole counts are 0.500, 1.50, 0.25; dividing each by 0.25 gives 2 : 6 : 1.

The empirical formula is **$\ce{C2H6O}$**.
:::
::::

:::: tabs
::: tab Problem
A compound is 38.7% C, 9.7% H, and 51.6% O by mass, and its molar mass is 62.07 g/mol. Find its empirical formula and its molecular formula.
:::
::: tab Solution
**Assume a 100 g sample.** Then the percentages read directly as grams — this trick is what makes percent-composition problems tractable.

$$\ce{C}:\ 38.7\,\text{g}\times\frac{1\ \text{mol}}{12.01\ \text{g}}=3.22\ \text{mol}$$
$$\ce{H}:\ 9.7\,\text{g}\times\frac{1\ \text{mol}}{1.008\ \text{g}}=9.62\ \text{mol}$$
$$\ce{O}:\ 51.6\,\text{g}\times\frac{1\ \text{mol}}{16.00\ \text{g}}=3.22\ \text{mol}$$

Divide by the smallest (3.22): C 1.00, H 2.99, O 1.00 → ratio 1 : 3 : 1. The empirical formula is $\ce{CH3O}$.

**Now the molecular formula.** The empirical formula mass is $12.01+3(1.008)+16.00=31.03$ g/mol. Compare with the measured molar mass:
$$\frac{62.07}{31.03}=2.00$$

Multiply every subscript by 2: the molecular formula is **$\ce{C2H6O2}$** (ethylene glycol, automotive antifreeze).

This is the step the previous problem stops short of. Combustion analysis alone can never give a molecular formula — it gives a ratio, and a ratio has no scale. **You need one additional measurement, the molar mass, to know how many times the empirical unit repeats.**
:::
::::

> **Where this goes next.** You can now convert between the mass of a substance and the number of particles in it. That covers one substance at a time. §3.2 adds the piece that connects *different* substances: a balanced equation, which states the fixed mole ratio in which they react.

## 3.2 Balancing Chemical Reactions{{attrs[#blk-ch03sec02]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 3.2a}} Balance a chemical equation by adjusting coefficients (never subscripts).
- {{sp[info] Objective 3.2b}} Convert between quantities of reactants and products using a balanced equation.
- {{sp[info] Objective 3.2c}} Determine the limiting reagent using either the "least product" or "smallest mol/coefficient" method.
- {{sp[info] Objective 3.2d}} Calculate theoretical yield, percent yield, and the amount of excess reagent left over.
:::

### What a chemical equation says

A **chemical reaction** changes one or more substances into new ones, and a **chemical equation** describes it in symbols, reactants on the left and products on the right.

The critical point is what the coefficients mean. They count **particles**, and therefore **moles** — never grams:

$$\ce{2Mg + O2 -> 2MgO}$$

The equation reads as 2 atoms of Mg plus 1 molecule of $\ce{O2}$ give 2 formula units of MgO, or equivalently 2 moles of Mg plus 1 mole of $\ce{O2}$ give 2 moles of MgO. It does **not** say 2 g + 1 g → 2 g. In mass terms this reaction is 48.6 g Mg + 32.0 g $\ce{O2}$ → 80.6 g MgO. Mass is conserved (48.6 + 32.0 = 80.6), but not in the ratio the coefficients state. Figure 3.5 shows this reaction happening, and it is worth looking at with the mass numbers in mind.

![Magnesium ribbon burning in air, producing white magnesium oxide](../assets/magnesium_burning.jpg =520x)
*Figure 3.5 — Magnesium burning in air ($\ce{2Mg + O2 -> 2MgO}$). The white ash left behind weighs more than the ribbon did, because the oxygen that combined with it came from the air — a result that looks like a violation of mass conservation until you account for the reactant you cannot see.*

### Balancing an equation

:::warning
**A balanced equation is a recipe you can scale at will — but it is not a claim about masses either.** The conventional coefficients are the smallest whole numbers that make every atom tally match, and multiplying all of them by the same whole number gives an equally balanced equation ($\ce{2H2 + O2 -> 2H2O}$ and $\ce{4H2 + 2O2 -> 4H2O}$ are both correct). By convention the lowest whole-number set is used. What the coefficients never state is a mass ratio: $\ce{2H2 + O2 -> 2H2O}$ means two moles of hydrogen to one of oxygen, which is 4.0 g to 32.0 g — nothing like 2 to 1.
:::

A balanced equation has the same number of each kind of atom on both sides, as Dalton's fourth postulate requires. Balancing means finding coefficients that make that true, and Figure 3.6 shows what "true" looks like as a tally.

![Atom tallies for an unbalanced and a balanced combustion equation](../assets/balancing_atom_tally.svg =760x)
*Figure 3.6 — Balancing is bookkeeping: tally each element on both sides and adjust the coefficients until every row matches. Only the coefficients in front may change.*

**The procedure:**

1. Write correct formulas for all reactants and products. (This is Chapter 2's job, and it must be done before any balancing — a wrong formula cannot be fixed by balancing.)
2. Adjust the **coefficients** so each element's atom count matches on both sides.
    - Start with elements that appear in only one reactant and one product.
    - Leave for last any element appearing in several species — often oxygen.
3. Check every element.

{{sp[warning] Reminder}} Never adjust a subscript to balance an equation. Changing $\ce{H2O}$ to $\ce{H2O2}$ does not give you more water; it gives you hydrogen peroxide, a different substance entirely.

:::: tabs
::: tab Problem
Balance $\ce{CH4 + O2 -> CO2 + H2O}$.
:::
::: tab Solution
**Carbon** appears in one species on each side and already matches: 1 and 1.

**Hydrogen:** 4 on the left, 2 on the right. Put a 2 in front of $\ce{H2O}$:
$$\ce{CH4 + O2 -> CO2 + 2H2O}$$

**Oxygen last**, because it appears in two products. The right side now has $2+2(1)=4$ O atoms. Put a 2 in front of $\ce{O2}$ to supply 4:
$$\ce{CH4 + 2O2 -> CO2 + 2H2O}$$

**Check:** C 1 = 1, H 4 = 4, O 4 = 4. ✓
:::
::::

:::: tabs
::: tab Problem
Balance $\ce{C2H6 + O2 -> CO2 + H2O}$.
:::
::: tab Solution
Balance C and H first, exactly as before: 2 carbons need a 2 on $\ce{CO2}$, and 6 hydrogens need a 3 on $\ce{H2O}$:
$$\ce{C2H6 + O2 -> 2CO2 + 3H2O}$$

Now oxygen. The right side has $2(2)+3(1)=7$ atoms, but $\ce{O2}$ supplies them two at a time, so it needs a coefficient of $7/2=3.5$.

By convention, balanced equations are written with the smallest whole-number coefficients, so clear the fraction by multiplying every coefficient by 2:
$$\ce{2C2H6 + 7O2 -> 4CO2 + 6H2O}$$

**Check:** C 4 = 4, H 12 = 12, O 14 = 14. ✓

This is the contrast with the methane problem: there the oxygen count came out even and no scaling was needed. Odd oxygen counts are common in hydrocarbon combustion, so expect the doubling step.
:::
::::

### Using an equation to convert quantities

==Once balanced, an equation's coefficients give a mole-ratio conversion factor between substances== — and that single idea is the central algorithm of the chapter.

![The stoichiometry road map from mass of A to mass of B](../assets/stoichiometry_road_map.svg =840x)
*Figure 3.7 — Every stoichiometry problem walks this road. Convert the given mass to moles using A's molar mass, cross to the other substance using the coefficient ratio, then convert back to mass using B's molar mass. The crossing can only happen in the middle, in moles — grams of one substance never convert directly into grams of another.*

:::: tabs
::: tab Problem
In $\ce{C6H12O6 + 6O2 -> 6CO2 + 6H2O}$, how much $\ce{CO2}$ forms from 856 g of $\ce{C6H12O6}$?
:::
::: tab Solution
Chain the three steps of Figure 3.7 into one line, checking that each unit cancels:

$$856\,\text{g}\,\ce{C6H12O6}\times\underbrace{\frac{1\,\text{mol}\,\ce{C6H12O6}}{180.2\,\text{g}\,\ce{C6H12O6}}}_{\text{molar mass of A}}\times\underbrace{\frac{6\,\text{mol}\,\ce{CO2}}{1\,\text{mol}\,\ce{C6H12O6}}}_{\text{mole ratio}}\times\underbrace{\frac{44.01\,\text{g}\,\ce{CO2}}{1\,\text{mol}\,\ce{CO2}}}_{\text{molar mass of B}}=1.25\times10^3\ \text{g}\,\ce{CO2}$$

Note that the product outweighs the reactant. That is not an error — the $\ce{CO2}$ also contains the mass of the oxygen consumed.
:::
::::

:::: tabs
::: tab Problem
Using the same equation, how many grams of $\ce{O2}$ are needed to react completely with 90.0 g of glucose?
:::
::: tab Solution
The road is identical; only the mole ratio and the molar mass of the target change, because the target substance changed.

$$90.0\,\text{g}\,\ce{C6H12O6}\times\frac{1\,\text{mol}}{180.2\,\text{g}}\times\frac{6\,\text{mol}\,\ce{O2}}{1\,\text{mol}\,\ce{C6H12O6}}\times\frac{32.00\,\text{g}\,\ce{O2}}{1\,\text{mol}\,\ce{O2}}=95.9\ \text{g}\,\ce{O2}$$

The mole ratio here happens to be $6:1$, the same as for $\ce{CO2}$, but that is a coincidence of this particular equation. Always read the ratio off the two coefficients you actually need.
:::
::::

### Limiting reagent

The previous problems assumed exactly the right amount of everything. Real reactions are often run with one reactant in excess, so the question becomes: which one runs out first?

The **limiting reagent** is the reactant consumed completely. It sets a ceiling on how much product can form; whatever is left of the others is the **excess reagent**. Figure 3.8 makes the distinction concrete before any arithmetic is involved.

![Nuts-and-bolts analogy for limiting and excess reagent](../assets/limiting_reagent_concept.svg =800x)
*Figure 3.8 — The limiting reactant is not necessarily the one you have least of. It is the one that runs out first given the ratio the reaction demands — which is why the nuts limit the assembly here despite outnumbering the bolts.*

Two methods find it, and they always agree:

- **Method 1 (more arithmetic, easier to see).** Work out how much product each reactant could make if it were used up entirely. The smallest answer is the truth, and the reactant that produced it is limiting.
- **Method 2 (less arithmetic).** Convert each reactant to moles, then divide by its own coefficient. The smallest quotient identifies the limiting reagent.

:::: tabs
::: tab Problem
For $\ce{N2 + 3H2 -> 2NH3}$, you have 2.00 mol $\ce{N2}$ and 3.00 mol $\ce{H2}$. Which is limiting? Use both methods.
:::
::: tab Solution
**Method 1 — how much product could each make alone?**

From $\ce{N2}$: $2.00\ \text{mol}\times\dfrac{2\ \text{mol}\,\ce{NH3}}{1\ \text{mol}\,\ce{N2}}=4.00$ mol $\ce{NH3}$.

From $\ce{H2}$: $3.00\ \text{mol}\times\dfrac{2\ \text{mol}\,\ce{NH3}}{3\ \text{mol}\,\ce{H2}}=2.00$ mol $\ce{NH3}$.

The smaller answer wins, so **$\ce{H2}$ is limiting** and only 2.00 mol $\ce{NH3}$ can form.

**Method 2 — moles divided by coefficient.**

$\ce{N2}$: $2.00/1=2.00$.  $\ce{H2}$: $3.00/3=1.00$.

The smaller quotient is $\ce{H2}$'s, giving the same answer with less work.

Note that there is more $\ce{H2}$ than $\ce{N2}$ by moles, and $\ce{H2}$ is still the limiting reagent — the reaction demands three times as much of it.
:::
::::

### Reaction yield

**Theoretical yield** is the amount of product that would form if the limiting reagent reacted completely. **Actual yield** is what a real experiment produces, which is usually less (Figure 3.9).

$$\%\ \text{Yield}=\frac{\text{actual yield}}{\text{theoretical yield}}\times100\%$$

![Theoretical and actual yield shown as proportional bars](../assets/theoretical_vs_actual_yield.svg =740x)
*Figure 3.9 — Percent yield measures how much of the possible product a real reaction delivered. Reactions fall short through side reactions, incomplete conversion, and losses during transfer and purification. A yield above 100% is not a triumph; it means the product is wet or impure.*

![Bar chart identifying the limiting reagent](../assets/limiting_reagent_bar.svg =520x)
*Figure 3.10 — Method 2 applied to the urea synthesis below: dividing each reactant's moles by its coefficient gives 18.71 for $\ce{NH3}$ against 25.95 for $\ce{CO2}$. The smaller value identifies $\ce{NH3}$ as limiting.*

:::: tabs
::: tab Problem
$\ce{2NH3 + CO2 -> (NH2)2CO + H2O}$. React 637.2 g $\ce{NH3}$ with 1142 g $\ce{CO2}$. (a) Which is the limiting reagent? (b) What is the theoretical yield of $\ce{(NH2)2CO}$? \(c) If 1006 g formed, what is the percent yield? (d) How much excess reagent remains?
:::
::: tab Solution
**(a) Limiting reagent.** Convert both to moles first:
$$637.2\,\text{g}\,\ce{NH3}\times\frac{1\ \text{mol}}{17.03\ \text{g}}=37.42\ \text{mol}\qquad 1142\,\text{g}\,\ce{CO2}\times\frac{1\ \text{mol}}{44.01\ \text{g}}=25.95\ \text{mol}$$

Method 2: $37.42/2=18.71$ versus $25.95/1=25.95$, as plotted in Figure 3.10. The smaller quotient belongs to $\ce{NH3}$, so **$\ce{NH3}$ is limiting**.

**(b) Theoretical yield.** The product yield comes from the limiting reagent only — the $\ce{CO2}$ figure plays no part in this calculation:
$$37.42\,\text{mol}\,\ce{NH3}\times\frac{1\,\text{mol}\,\ce{(NH2)2CO}}{2\,\text{mol}\,\ce{NH3}}\times\frac{60.06\,\text{g}}{1\,\text{mol}}=1124\ \text{g}\,\ce{(NH2)2CO}$$

**\(c) Percent yield.**
$$\%\ \text{Yield}=\frac{1006}{1124}\times100\%=89.5\%$$

**(d) Excess reagent remaining.** Find how much $\ce{CO2}$ was actually consumed, then subtract from what was supplied:
$$\ce{CO2}\ \text{used}=37.42\,\text{mol}\,\ce{NH3}\times\frac{1\,\text{mol}\,\ce{CO2}}{2\,\text{mol}\,\ce{NH3}}=18.71\ \text{mol}$$
$$\ce{CO2}\ \text{left}=25.95-18.71=7.24\ \text{mol}\ \Rightarrow\ 7.24\,\text{mol}\times44.01\,\text{g/mol}=319\ \text{g}\,\ce{CO2}$$

{{sp[warning] Reminder}} Carry unrounded values through to the last step. Here rounded and unrounded inputs both give **319 g** (7.24 mol × 44.01 g/mol = 318.6 g), but in longer calculations early rounding can shift the final digits. Round once, at the end.
:::
::::

## Synthesis

==Every calculation in this chapter routes through the mole: molar mass converts a formula into grams per mole, mole ratios from a balanced equation convert one substance's amount into another's, and limiting-reagent and yield analysis is that same mole-ratio logic applied when reactants are not present in stoichiometric proportions, or when the actual yield falls short of the theoretical yield.==

The dependencies run backwards as much as forwards. This chapter cannot start without Chapter 2's correct formulas, and it cannot proceed without Chapter 1's dimensional analysis — every conversion here is a unit-cancellation problem wearing chemical clothing. Looking forward, it is the single most-reused method in the course: gas-law problems (Chapter 5) convert to moles before applying $PV=nRT$, solution concentrations (Chapter 12) are moles per liter, thermochemistry (Chapter 6) reports energy per mole, and equilibrium constants (Chapter 14) are built from molar concentrations. None of those chapters re-teach the mole; they assume it.

## Asset and License Record for This Chapter

| Asset | Source URL | License | Attribution |
|---|---|---|---|
| `assets/how_big_is_a_mole.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
| `assets/mole_conversion_triangle.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
| `assets/percent_composition_water.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated from the study guide's own worked-example data; released under this package's CC BY 4.0 license. |
| `assets/combustion_analysis.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated, schematic; released under this package's CC BY 4.0 license. |
| `assets/magnesium_burning.jpg` | https://commons.wikimedia.org/wiki/File:Magnesium_ribbon_burning.jpg | CC BY-SA 3.0 | Capt. John Yossarian, via Wikimedia Commons. |
| `assets/balancing_atom_tally.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
| `assets/stoichiometry_road_map.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
| `assets/limiting_reagent_concept.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
| `assets/theoretical_vs_actual_yield.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated from the study guide's own worked-example data; released under this package's CC BY 4.0 license. |
| `assets/limiting_reagent_bar.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated from the study guide's own worked-example data; released under this package's CC BY 4.0 license. |
