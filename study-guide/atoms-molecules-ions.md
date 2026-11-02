{{nyml
kind: document
format: 1
title: Chapter 2: Atoms, Molecules, and Ions
}}

# Chapter 2: Atoms, Molecules, and Ions

:::info
**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 2 (CC BY 4.0)
**Audience:** introductory undergraduate general chemistry, first semester
**Package license:** CC BY 4.0
**Note:** builds on Chapter 1's classification of matter; facts checked for accuracy against OpenStax *Chemistry 2e* and Wikipedia (used for reference only — no text or figures adapted from either).
:::

:::success
**Chapter Learning Objectives**
- Describe atomic structure (protons, neutrons, electrons) and summarize the historical experiments that revealed it.
- Define atomic number, mass number, and isotope, and locate element families on the periodic table.
- Distinguish molecules from ions, and molecular from empirical formulas.
- Name ionic compounds, molecular compounds, acids, bases, and hydrates.
:::

## Chapter Logic

Chapter 1 sorted matter from the outside — you could tell a compound from a mixture by what you could do to it in a lab. This chapter goes inside. It asks what an atom is actually made of, how those parts explain the periodic table, how atoms join into molecules and ions, and finally how chemists name the results. ==The last step matters more than it looks: from Chapter 3 onward, every equation you write starts with a correct formula, and you get the formula from the name.==

{{mermaid
graph TD
  A["Atomic structure:<br/>protons, neutrons, electrons"] --> B["Atomic number, mass number,<br/>isotopes, periodic table"]
  B --> C["Molecules and ions:<br/>how atoms combine"]
  C --> D["Naming compounds:<br/>ionic, molecular, acids, bases, hydrates"]
}}

**Visual description:** A top-down flowchart. Atomic structure (protons, neutrons, electrons) leads to the atomic number/mass number/isotope framework and the periodic table's organization. That framework describes how atoms combine into molecules and ions. Naming compounds is the mechanical skill that closes the chapter, applied to everything built so far.

## 2.1 Atoms{{attrs[#blk-ch02sec01]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 2.1a}} State the four postulates of Dalton's atomic theory.
- {{sp[info] Objective 2.1a}} Describe the subatomic particles and their relative mass and charge.
- Describe alpha, beta, and gamma radiation.
- {{sp[info] Objective 2.1b}} Summarize what Rutherford's gold-foil experiment revealed about atomic structure.
- {{sp[info] Objective 2.1c}} Define atomic number (Z), mass number (A), and isotope, and calculate particle counts.
- {{sp[info] Objective 2.1d}} Identify periods, groups, metals, nonmetals, metalloids, and the named families (alkali metals, alkaline earth metals, halogens, noble gases).
:::

### Dalton's atomic theory

In 1808 John Dalton proposed four ideas that turned "atoms" from a philosophical guess into a working scientific theory:

1. Elements are composed of extremely small particles called **atoms**.
2. All atoms of a given element are identical — same size, same mass, same chemical properties — and different from the atoms of every other element.
3. Compounds contain atoms of more than one element, combined so that the ratio of the numbers of atoms of any two of the elements is a whole number or a simple fraction.
4. A chemical reaction only separates, combines, or rearranges atoms. It never creates or destroys them.

Three of these are still how chemists think. Postulate 4 is why chemical equations must balance, which is the whole of Chapter 3. Postulate 3 is why a compound has a fixed formula.

Postulate 2 turned out to be *not quite* right, and the way it fails is worth noticing now, because you will meet the correction later in this very section. Atoms of the same element are identical in **chemical** behavior, but they are not all identical in **mass**. That discovery is what isotopes are.

### Inside the atom

An **atom** is the smallest unit of an element that still behaves like that element. Atoms are extraordinarily small — a typical atom is about 100 picometers across, so roughly ten million of them side by side would span one millimeter.

Every atom has a **nucleus** at its center, containing **protons** and (except for the most common hydrogen atom) **neutrons**. Protons and neutrons together are called **nucleons**. **Electrons** occupy the space around the nucleus. Protons carry a positive charge, electrons a negative charge, and neutrons no charge at all.

If an atom has equal numbers of protons and electrons, the charges cancel and the atom is electrically neutral. If it has more or fewer electrons than protons, it carries a net charge and is called an **ion** — the subject of §2.2.

| Particle | Mass (g) | Charge \(C) | Charge unit |
|---|---|---|---|
| Electron | $9.10938\times10^{-28}$ | $-1.6022\times10^{-19}$ | $-1$ |
| Proton | $1.67262\times10^{-24}$ | $+1.6022\times10^{-19}$ | $+1$ |
| Neutron | $1.67493\times10^{-24}$ | $0$ | $0$ |

Read that table for the *relationships*, not the digits. Two of them do most of the work in this course:

- A proton and a neutron have almost exactly the same mass, and an electron is about **1800 times lighter** than either (Figure 2.1). So more than 99.94% of an atom's mass sits in the nucleus.
- A proton's charge and an electron's charge are the same size with opposite signs. That exact cancellation is why a neutral atom is possible at all, and why gaining one electron gives a charge of exactly $-1$.

![Bar chart comparing the masses of the electron, proton, and neutron on a log scale](../assets/subatomic_particle_masses.svg =480x)
*Figure 2.1 — A proton or neutron is roughly 1800 times more massive than an electron. Note the logarithmic scale: on a linear scale the electron's bar would be invisible. This ratio is why virtually all of an atom's mass is concentrated in its nucleus.*

![Schematic atom showing the nucleus and electron shells](../assets/atom_structure.svg =420x)
*Figure 2.2 — A schematic atom: a dense central nucleus of protons and neutrons, surrounded by electrons. This diagram is deliberately not to scale. If the nucleus were the size of a marble, the nearest electrons would be about a kilometer away, and everything in between would be empty space.*

:::warning
**A picture worth un-learning later.** Figure 2.2 draws electrons as dots on neat circular orbits, like planets. That image is useful now and wrong in detail — Chapter 7 replaces it with orbitals, which are regions of probability rather than paths. Use the diagram to keep track of *how many* electrons there are and roughly how far out they sit; do not read it as a claim about where an electron is at a given moment.
:::

### Radioactivity: what the experimenters had to work with

Some elements spontaneously emit particles or energy from their nuclei. This is **radioactivity**, and an element that does it is **radioactive**. You need the vocabulary right now for a practical reason: the experiment that revealed the nucleus was performed by firing radioactive emissions at metal foil.

![Comparison of alpha, beta, and gamma radiation showing composition, charge, mass, and penetrating power](../assets/radiation_types.svg =760x)
*Figure 2.3 — The three kinds of radioactive emission. An **alpha ($\alpha$) particle** is a helium-4 nucleus — two protons and two neutrons — so it is heavy and carries a $+2$ charge; being bulky, it is stopped by a sheet of paper. A **beta ($\beta$) particle** is a fast-moving electron (or a positron, its positively charged counterpart), far lighter and more penetrating. **Gamma ($\gamma$) radiation** is not a particle of matter at all but a very high-energy photon — no mass, no charge — and it takes thick lead or concrete to absorb. The colored squares rank penetrating power, not energy or danger.*

**X-rays** are the same physical kind of thing as gamma rays: high-energy electromagnetic radiation. The difference is where they come from and how much energy they carry. X-rays originate from the electrons outside the nucleus and typically span wavelengths from about 0.01 to 10 nanometers; gamma rays come from the nucleus itself and sit at the highest energies observed.

Chapter 19 returns to all of this and writes balanced nuclear equations for each decay type. For now, "an alpha particle is a helium nucleus with a $+2$ charge" is the only fact the next subsection needs.

### How we found out: four experiments

You are being asked to accept a fairly specific claim — a tiny dense positive core, light electrons outside, neutral particles hidden in the core. None of that is visible. Each piece came from an experiment that produced a result nobody could explain any other way.

**J. J. Thomson and the charge-to-mass ratio of the electron.** A *cathode ray* is a beam emitted from the negative electrode of a high-vacuum tube. Thomson put electrically charged plates and a magnet outside such a tube and watched the beam bend. From how much it bent in known electric and magnetic fields, he calculated the ratio of the particle's charge to its mass. The beam behaved identically no matter what the electrode was made of — evidence that this negatively charged particle is a component of *all* matter.

**Robert Millikan and the charge of the electron.** Thomson had a ratio, not a value. Millikan sprayed tiny oil droplets between two parallel charged plates and adjusted the field until a droplet hung motionless, with the electric force exactly balancing gravity. That balance gives the droplet's charge. Repeating it for many droplets, he found every charge was a small whole-number multiple of one base value — about $1.5924\times10^{-19}$ C, within 0.6% of today's accepted $1.602176\times10^{-19}$ C. Charge comes in indivisible units, and combining Millikan's charge with Thomson's ratio gives the electron's mass.

**Ernest Rutherford and the gold-foil experiment.** Rutherford's team fired alpha particles (Figure 2.3) from a radioactive source at very thin gold foil. Most passed straight through, some were deflected slightly — and a very few bounced almost straight back.

![Geiger-Marsden experiment: the Thomson plum-pudding prediction compared with the actual Rutherford result](../assets/geiger_marsden_expectation_result.svg =620x)
*Figure 2.4 — What made the gold-foil experiment decisive was the gap between prediction and result. **Left (Thomson model):** if an atom's positive charge were spread diffusely throughout its volume, every alpha particle should sail through with at most a tiny deflection — the expected outcome. **Right (Rutherford model):** in reality, most particles did pass straight through, but a few were deflected sharply and a rare few bounced almost straight back. Only a tiny, dense, concentrated positive nucleus could produce a repulsion strong enough to reverse an alpha particle — so the diffuse "plum pudding" picture had to be abandoned. The lower panels show the same contrast in the actual apparatus: alpha particles from a source strike a thin gold foil, and detectors record where they end up.*

Figure 2.4 sets the prediction beside the result, which is where the argument lives. Rutherford's reasoning ran in two steps. Most particles pass through undeflected, so most of the atom must be empty space. But a few reverse direction, so somewhere in that space there must be something both highly charged (to repel a $+2$ alpha particle that hard) and very massive (or it would be knocked aside instead of doing the knocking). A small dense positive **nucleus** satisfies both at once.

{{sp[warning] Reminder}} A particle bouncing *straight back* only happens on a rare, nearly head-on approach. That rarity is itself the evidence that the nucleus is tiny — if the positive charge filled the atom, near-misses would be common and reversals would not exist at all.

**James Chadwick and the neutron.** By 1920 the picture had a numerical hole in it. Hydrogen has 1 proton; helium has 2. Since electrons are far too light to matter, a helium atom should weigh about twice as much as a hydrogen atom. It actually weighs about four times as much. Something with mass but no charge had to be in the nucleus. In 1932 Chadwick bombarded beryllium with alpha particles and detected a highly penetrating emission that carried no charge but had a mass slightly greater than a proton's. He named the particles **neutrons**, and the 4:1 ratio was explained: helium's nucleus holds 2 protons *and* 2 neutrons.

### Atomic number, mass number, and isotopes

Two counts describe any nucleus.

The **atomic number (Z)** is the number of protons:

$$Z = \text{number of protons}$$

The **mass number (A)** is the total number of nucleons — protons plus neutrons:

$$A = \text{number of protons} + \text{number of neutrons}$$

$Z$ is the more fundamental of the two. ==The proton count is what makes an atom that element: change $Z$ and you have a different element entirely, while changing the neutron count leaves you with the same element in a slightly heavier or lighter version.==

![Isotope notation with the mass number and atomic number labeled, and the three isotopes of carbon](../assets/isotope_notation.svg =740x)
*Figure 2.5 — The standard notation writes the mass number $A$ as a superscript and the atomic number $Z$ as a subscript, both to the left of the element symbol. Since $A$ counts protons plus neutrons and $Z$ counts protons alone, the difference $A-Z$ gives the neutrons. The three carbon isotopes on the right all have 6 protons — that is what makes them carbon — and differ only in neutron count.*

Atoms with the same atomic number but different mass numbers are **isotopes**. This is the correction to Dalton's second postulate promised earlier: carbon-12 and carbon-14 are chemically the same element, but they are not identical atoms.

:::: tabs
::: tab Problem
An atom of uranium has mass number 235 and atomic number 92. How many protons, neutrons, and electrons does the neutral atom have?
:::
::: tab Solution
The atomic number *is* the proton count, so there are **92 protons**.

Neutrons come from the difference:
$$\text{neutrons} = A - Z = 235 - 92 = \mathbf{143}$$

A neutral atom has as many electrons as protons, so **92 electrons**.
:::
::::

:::: tabs
::: tab Problem
Using the notation of Figure 2.5, write the full symbol $^{A}_{Z}\ce{X}$ for the atom that has 17 protons and 20 neutrons. What element is it?
:::
::: tab Solution
Work in the order the definitions give you. The proton count is $Z$, so $Z=17$. On the periodic table, element 17 is chlorine, $\ce{Cl}$.

The mass number adds the two nucleon counts:
$$A = 17 + 20 = 37$$

So the symbol is $^{37}_{17}\ce{Cl}$, chlorine-37.

Note that you were *given* the neutron count and had to add, whereas the uranium problem gave you $A$ and required subtraction. Read carefully which two of the three numbers you have.
:::
::::

:::: tabs
::: tab Problem
An atom of chlorine (Z = 17) gains one electron to become $\ce{Cl^-}$. How many protons and electrons does the ion have? Is it still chlorine?
:::
::: tab Solution
Gaining or losing electrons never touches the nucleus, so the proton count is unchanged: **17 protons**. It has one more electron than the neutral atom's 17, so it has **18 electrons**.

It is still chlorine, because $Z$ is still 17. An ion is a charged version of an element, not a different element.
:::
::::

:::warning
**The three ways to change an atom, and what each one changes.** Students routinely mix these up.
- Change the **electron** count → same element, now an **ion** (charge changes).
- Change the **neutron** count → same element, now a different **isotope** (mass changes).
- Change the **proton** count → a **different element** entirely. This does not happen in chemical reactions; it takes a nuclear process (Chapter 19).
:::

### The periodic table

The **periodic table** arranges the elements by atomic number so that elements with similar chemical behavior line up. Horizontal rows are **periods**; vertical columns are **groups** (also called families).

![Periodic table showing periods, groups, metal/metalloid/nonmetal categories, and four named families](../assets/periodic_table_overview.svg =900x)
*Figure 2.6 — The periodic table. Reading across a row (a period) walks you through elements in order of increasing atomic number. Reading down a column (a group) collects elements that behave alike chemically — this is the single most useful fact about the table. Background color marks the three broad categories: **metals** (good conductors of heat and electricity, the large blue region on the left), **nonmetals** (poor conductors, upper right), and **metalloids** (properties in between, along the staircase boundary). Four groups have names you will use constantly: Group 1A **alkali metals**, Group 2A **alkaline earth metals**, Group 7A **halogens**, and Group 8A **noble gases**. Hydrogen sits above Group 1A but is a nonmetal and is not an alkali metal. The grey elements at the bottom of the table have been made only a few atoms at a time, so their chemical properties are predicted rather than measured.*

Why does the columns-behave-alike pattern exist? Chapter 7 gives the real answer (elements in a group have the same outer-electron arrangement). For now, take it as an observed regularity and use it — because it is about to save you a great deal of memorization in §2.2.

:::: tabs
::: tab Problem
Locate calcium (Z = 20) on the periodic table. What period and group is it in, what family does it belong to, and is it a metal or a nonmetal? Name one element that should behave similarly.
:::
::: tab Solution
Counting up to element 20 on Figure 2.6 puts calcium in the **fourth period**, **Group 2A**.

Group 2A is the **alkaline earth metals**, so calcium is a **metal**.

Elements in the same group behave alike, so magnesium ($\ce{Mg}$, Group 2A, period 3) or strontium ($\ce{Sr}$, Group 2A, period 5) should behave similarly to calcium. Notice what does *not* work: scandium ($\ce{Sc}$) is calcium's neighbor in the same period, but neighbors across a row do not share chemical behavior the way column-mates do.
:::
::::

:::: tabs
::: tab Problem
Classify each as a metal, nonmetal, or metalloid: $\ce{Br}$, $\ce{Si}$, $\ce{Fe}$, $\ce{Ne}$.
:::
::: tab Solution
- $\ce{Br}$ (bromine), Group 7A — a **nonmetal**, and specifically a halogen.
- $\ce{Si}$ (silicon) — a **metalloid**; it sits on the staircase between the metals and nonmetals, which is exactly why it is useful in semiconductors.
- $\ce{Fe}$ (iron), a transition element — a **metal**.
- $\ce{Ne}$ (neon), Group 8A — a **nonmetal**, and a noble gas.

The quick rule: everything left of the staircase except hydrogen is a metal, which is most of the table. Apart from hydrogen, only the upper-right corner is nonmetal.
:::
::::

> **Where this goes next.** You now know what an atom is made of and how the table organizes atoms. But pure lone atoms are rare in nature — only the noble gases occur that way. Almost everything around you is atoms joined together or atoms carrying a charge, and §2.2 is about those two possibilities.

## 2.2 Molecules and Ions{{attrs[#blk-ch02sec02]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 2.2a}} Distinguish a molecule from an ion, and a cation from an anion.
- {{sp[info] Objective 2.2a}} Distinguish a monatomic ion from a polyatomic ion.
- {{sp[info] Objective 2.2a}} Predict the charge of a main-group monatomic ion from its position in the periodic table.
- {{sp[info] Objective 2.2b}} Distinguish a molecular formula from an empirical formula.
- {{sp[info] Objective 2.2b}} Determine the formula of an ionic compound by balancing charge.
- Recognize common organic functional groups (hydroxyl, amino, carboxyl) at an introductory level.
:::

Of all the elements, only the six noble gases in Group 8A (He, Ne, Ar, Kr, Xe, Rn) exist in nature as single atoms — **monatomic** gases. Most other atoms combine, mainly in one of two ways: atoms share electrons and form **molecules**, or atoms transfer electrons and form **ions** that attract one another.

### Molecules

A **molecule** is an aggregate of at least two atoms in a definite arrangement, held together by chemical bonds.

A molecule with exactly two atoms is **diatomic** — hydrogen gas, $\ce{H2}$, is the simplest. Seven elements occur naturally as diatomic molecules rather than lone atoms: $\ce{H2}$, $\ce{N2}$, $\ce{O2}$, $\ce{F2}$, $\ce{Cl2}$, $\ce{Br2}$, and $\ce{I2}$. Molecules with more than two atoms are **polyatomic**: water $\ce{H2O}$, ammonia $\ce{NH3}$, methane $\ce{CH4}$.

"Definite arrangement" is doing real work in that definition. $\ce{H2O}$ is not just two hydrogens and an oxygen in a container — it is those three atoms bonded in a particular geometry, which is what Chapters 9 and 10 are about.

### Organic compounds and functional groups

**Organic chemistry** is the branch that deals with carbon compounds. The simplest organic compounds are **hydrocarbons**, containing only carbon and hydrogen — methane, $\ce{CH4}$, is the smallest.

The chemistry of an organic molecule is largely set by its **functional groups**: small, specific clusters of atoms that behave the same way wherever they appear. Replace one hydrogen atom of methane with a functional group and you get an entirely different substance:

| Replace an H with | Group name | Product | Familiar as |
|---|---|---|---|
| $\ce{-OH}$ | hydroxyl | methanol, $\ce{CH3OH}$ | wood alcohol |
| $\ce{-NH2}$ | amino | methylamine, $\ce{CH3NH2}$ | a simple amine base |
| $\ce{-COOH}$ | carboxyl | acetic acid, $\ce{CH3COOH}$ | vinegar |

Three compounds built on the same CH3– group behave completely differently — one is a solvent, one is a base, one is an acid — because of one small group. That is the central idea of organic chemistry, and you will meet the carboxyl group again in Chapter 15 as a source of $\ce{H+}$.

### Ions: cations and anions

An **ion** is an atom or group of atoms carrying a net electric charge, produced when the electron count no longer matches the proton count.

- Losing one or more electrons leaves excess positive charge: a **cation**. A sodium atom readily gives up one electron to become $\ce{Na+}$.
- Gaining one or more electrons gives excess negative charge: an **anion**. A chlorine atom takes on one electron to become the chloride ion, $\ce{Cl^-}$.

{{sp[warning] Reminder}} A cation is positive. The name is not intuitive, so tie it to something: the "t" in ca**t**ion can be drawn as a plus sign.

Ions containing a single atom are **monatomic**. Ions containing several atoms bonded together but carrying an overall charge are **polyatomic** — $\ce{OH^-}$ (hydroxide), $\ce{CN^-}$ (cyanide), $\ce{NH4+}$ (ammonium).

When a cation and an anion come together, the result is an **ionic compound**. Sodium chloride, $\ce{NaCl}$ — ordinary table salt — is $\ce{Na+}$ and $\ce{Cl^-}$ in a repeating three-dimensional lattice, and Figure 2.7 shows what that arrangement looks like at a scale you can see.

![Macro photo of sodium chloride (table salt) crystals](../assets/nacl_salt.jpg =480x)
*Figure 2.7 — Sodium chloride, an ionic compound of $\ce{Na+}$ cations and $\ce{Cl^-}$ anions. The cubic shape of the crystals is not decorative — it is the repeating alternating arrangement of the two ions showing itself at a scale you can see. Note also what the photo does **not** show: there are no individual "$\ce{NaCl}$ molecules" here. The formula gives the 1:1 ratio in the lattice, not a discrete particle.*

Now the payoff from §2.1. With very few exceptions, metals form cations and nonmetals form anions — and for main-group elements, ==the group number tells you what charge the ion will carry (e.g., +1 for group 1, +2 for group 2, −2 for group 16, −1 for group 17), so an entire category of memorization collapses into reading a column number.==

![Predictable monatomic ion charges for the main-group elements, arranged by group](../assets/ion_charges_by_group.svg =820x)
*Figure 2.8 — Charges of common monatomic ions by group. Metals on the left lose electrons and become positive; the number lost equals the group number, so Group 1A gives $+1$ and Group 2A gives $+2$. Nonmetals on the right gain electrons and become negative; the number gained is $8$ minus the group number, so Group 7A gives $-1$ and Group 6A gives $-2$. Group 4A sits in the middle and rarely forms simple monatomic ions at all. Noble gases form none: they already have the stable full outer shell that every other atom is gaining or losing electrons to reach. The transition metals are the important exception — many form more than one charge, which is precisely why their names need a Roman numeral.*

:::: tabs
::: tab Problem
Predict the charge on the monatomic ion formed by (a) potassium, (b) sulfur, \(c) aluminum.
:::
::: tab Solution
**(a) Potassium** is in Group 1A. It is a metal, so it loses electrons, and the group number says how many: one. The ion is $\ce{K+}$.

**(b) Sulfur** is in Group 6A. It is a nonmetal, so it gains electrons: $8-6=2$ of them. The ion is $\ce{S^2-}$.

**\(c) Aluminum** is in Group 3A, a metal, so it loses three electrons: $\ce{Al^3+}$.

Sanity check on each: the metals came out positive and the nonmetal came out negative. If you get a negative charge for something on the left of the table, you have gone wrong somewhere.
:::
::::

### Chemical formulas: molecular and empirical

A **chemical formula** expresses composition using chemical symbols and subscripts. There are two kinds, and the difference matters.

A **molecular formula** shows the exact number of atoms of each element in one molecule of the substance. An **empirical formula** shows only the simplest whole-number ratio of atoms of each element in the compound.

Hydrogen peroxide is $\ce{H2O2}$ — that is its molecular formula, and it says each molecule has two hydrogens and two oxygens. Its empirical formula is $\ce{HO}$, the reduced 1:1 ratio. Both are correct; they answer different questions. This distinction becomes practical in Chapter 3, where laboratory analysis gives you the empirical formula and you need additional information to recover the molecular one.

:::: tabs
::: tab Problem
Give the empirical formula for (a) hydrogen peroxide, $\ce{H2O2}$, and (b) glucose, $\ce{C6H12O6}$.
:::
::: tab Solution
**(a)** The ratio is 2 H : 2 O, which reduces to 1:1. The empirical formula is $\ce{HO}$.

**(b)** The ratio is 6 C : 12 H : 6 O. Divide all three by 6: 1 C : 2 H : 1 O. The empirical formula is $\ce{CH2O}$.

Glucose's molecular formula is six times its empirical formula. That multiple is real information — it is the difference between a sugar and formaldehyde, which also has the empirical formula $\ce{CH2O}$.
:::
::::

:::: tabs
::: tab Problem
Is $\ce{H2O}$ already in its empirical form? What about benzene, $\ce{C6H6}$?
:::
::: tab Solution
**Water:** the ratio 2 H : 1 O has no common factor greater than 1, so $\ce{H2O}$ *is* its own empirical formula. Molecular and empirical formulas are often identical — the two only differ when the subscripts share a common factor.

**Benzene:** the ratio 6 C : 6 H reduces to 1:1, so the empirical formula is $\ce{CH}$ while the molecular formula is $\ce{C6H6}$. These two examples are the contrast worth remembering: reduce the subscripts and see whether anything changes.
:::
::::

An **allotrope** is one of two or more distinct forms of the *same* element. Carbon is the standard example: diamond and graphite are both pure carbon, differing only in how the atoms are arranged, and they differ enormously in hardness, appearance, electrical conductivity, and price. Same element, same formula, different structure — a reminder that arrangement is as much a part of a substance's identity as composition.

### Formulas of ionic compounds

Ionic compounds are not made of molecules, so their formulas follow a different logic. Two rules cover it:

- The formula is normally the **empirical** formula — the simplest ratio of cations to anions in the lattice.
- The total charge of all the ions in the formula must **sum to zero**. A bulk sample of an ionic compound is electrically neutral.

The second rule is the whole method. If you know the two ion charges, the formula is forced.

![Building an ionic formula by balancing charge, with a case needing reduction and a case that does not](../assets/ionic_formula_charge_balance.svg =820x)
*Figure 2.9 — The charge-crossing shortcut, and the step people forget. Write each ion with its charge, then move each charge number down to be the *other* ion's subscript. **Left:** $\ce{Ca^2+}$ and $\ce{Cl^-}$ give $\ce{CaCl2}$; a subscript of 1 is never written. **Right:** $\ce{Pb^4+}$ and $\ce{O^2-}$ cross to $\ce{Pb2O4}$, but 2 and 4 share a factor of 2, so the formula must be reduced to $\ce{PbO2}$. Always finish by checking that the charges cancel.*

:::: tabs
::: tab Problem
Determine the formula of the compound formed by aluminum and oxygen.
:::
::: tab Solution
Get the charges from the periodic table first (Figure 2.8). Aluminum is Group 3A: $\ce{Al^3+}$. Oxygen is Group 6A: $\ce{O^2-}$.

Cross the charge numbers into subscripts as in Figure 2.9: $\ce{Al2O3}$.

Check for a common factor: 2 and 3 share none, so no reduction is needed.

Check the charge sum: $2(+3) + 3(-2) = +6 - 6 = 0$. ✓

The formula is $\ce{Al2O3}$.
:::
::::

:::: tabs
::: tab Problem
Determine the formula of the compound formed by calcium and the nitrate ion, $\ce{NO3^-}$.
:::
::: tab Solution
Calcium is Group 2A, so $\ce{Ca^2+}$. Nitrate is a polyatomic ion with charge $-1$.

Crossing gives one $\ce{Ca}$ and two $\ce{NO3}$ units. Here is the new wrinkle: because nitrate is a *group* of atoms, the subscript 2 must apply to the whole group, which requires parentheses:

$$\ce{Ca(NO3)2}$$

Writing $\ce{CaNO32}$ would claim 32 oxygen atoms, and writing $\ce{CaN2O6}$ would hide the fact that the nitrate units stay intact.

Check: $1(+2) + 2(-1) = 0$. ✓
:::
::::

> **Where this goes next.** You can now work out what combines with what, and in what ratio. What you cannot yet do is say the result out loud, or go the other way from a name back to a formula. §2.3 supplies both — and going backwards, name to formula, is the direction Chapter 3 will demand of you constantly.

## 2.3 Naming Compounds{{attrs[#blk-ch02sec03]}}

:::success
**Learning Objectives**
- Decide which naming system a formula requires.
- {{sp[info] Objective 2.3a}} Name ionic compounds, including binary compounds, transition-metal compounds (Roman numerals), and those containing polyatomic ions.
- {{sp[info] Objective 2.3b}} Name binary molecular compounds using Greek numerical prefixes.
- {{sp[info] Objective 2.3c}} Name binary acids and oxoacids, and the oxoanions derived from them.
- {{sp[info] Objective 2.3c}} Name bases and hydrates.
:::

Chemical nomenclature looks like pure memorization at first. It is not: it is three separate systems, each internally consistent, and almost every mistake beginners make comes from applying the wrong system rather than from misremembering a rule.

### First, decide which system

![Decision tree for choosing between the acid, ionic, and molecular naming systems](../assets/naming_decision_tree.svg =860x)
*Figure 2.10 — Answer the questions in order and the formula sorts itself into one of three naming systems, each with its own rules. The two boxes at the bottom are modifiers that can apply on top of whichever branch you landed in.*

==Classify first, name second — Roman numerals and Greek prefixes are never mixed in the same base name (a hydrate modifier like "pentahydrate" is added separately),== and if you find yourself writing "iron(III) trichloride" you have merged two systems that do not belong together.

:::: tabs
::: tab Problem
Working down Figure 2.10, decide which naming system each of these needs: $\ce{SO2}$, $\ce{K2S}$, $\ce{HBr}(aq)$, $\ce{CuCl2}$?
:::
::: tab Solution
- **$\ce{SO2}$** — sulfur and oxygen are both nonmetals, so this is **molecular**: Greek prefixes.
- **$\ce{K2S}$** — potassium is a metal, so this is **ionic**. Potassium is Group 1A with only one possible charge, so no Roman numeral.
- **$\ce{HBr}(aq)$** — starts with H and is dissolved in water, so this is an **acid**. No oxygen present, so it is a binary acid.
- **$\ce{CuCl2}$** — copper is a metal, so this is **ionic**. Copper is a transition metal that forms more than one charge, so this one **does** need a Roman numeral.

Notice that $\ce{K2S}$ and $\ce{CuCl2}$ both landed in the ionic branch but take different treatment. The metal's identity, not the shape of the formula, decides it.
:::
::::

### Ionic compounds

An ionic compound is typically a metal combined with a nonmetal. The rules:

- Name the cation first, using the element name unchanged (for metals that form only one ion).
- Name the monatomic anion second, using the element stem plus **-ide**: chlorine → chlor**ide**, oxygen → ox**ide**, sulfur → sulf**ide**, nitrogen → nitr**ide**.
- Never use Greek prefixes when naming ionic compounds. The charges already fix the ratio, so it needs no announcement.

So $\ce{NaCl}$ is sodium chloride and $\ce{K2S}$ is potassium sulfide — not "dipotassium sulfide."

**Transition metals need a Roman numeral.** Because most of them can form more than one ion, the name has to state which one is present: $\ce{FeCl2}$ is iron(II) chloride and $\ce{FeCl3}$ is iron(III) chloride. The numeral gives the charge on the metal, not the number of metal atoms.

A small set of metals form only one ion and therefore take no numeral: the Group 1A metals ($+1$), the Group 2A metals ($+2$), aluminum ($+3$), zinc ($+2$), and silver ($+1$).

**Polyatomic ions** keep their own names, which have to be learned. These are the ones worth memorizing first:

| Formula | Name | Formula | Name |
|---|---|---|---|
| $\ce{NH4+}$ | ammonium | $\ce{ClO^-}$ | hypochlorite |
| $\ce{OH^-}$ | hydroxide | $\ce{ClO2^-}$ | chlorite |
| $\ce{CN^-}$ | cyanide | $\ce{ClO3^-}$ | chlorate |
| $\ce{NO2^-}$ | nitrite | $\ce{ClO4^-}$ | perchlorate |
| $\ce{NO3^-}$ | nitrate | $\ce{MnO4^-}$ | permanganate |
| $\ce{CO3^2-}$ | carbonate | $\ce{CrO4^2-}$ | chromate |
| $\ce{HCO3^-}$ | hydrogen carbonate (bicarbonate) | $\ce{Cr2O7^2-}$ | dichromate |
| $\ce{SO3^2-}$ | sulfite | $\ce{C2O4^2-}$ | oxalate |
| $\ce{SO4^2-}$ | sulfate | $\ce{CH3CO2^-}$ | acetate |
| $\ce{HSO4^-}$ | hydrogen sulfate (bisulfate) | $\ce{O2^2-}$ | peroxide |
| $\ce{PO4^3-}$ | phosphate | $\ce{SCN^-}$ | thiocyanate |
| $\ce{HPO4^2-}$ | hydrogen phosphate | $\ce{H2PO4^-}$ | dihydrogen phosphate |

The table is less arbitrary than it looks. Read the right-hand chlorine column downward and you will see a pattern in the number of oxygens — that pattern is explained under acids below, and once you have it, four names become one rule.

:::: tabs
::: tab Problem
Name $\ce{MgBr2}$ and $\ce{Li2O}$.
:::
::: tab Solution
**$\ce{MgBr2}$** — magnesium is a Group 2A metal with a fixed $+2$ charge, so no Roman numeral. The anion is bromine → brom**ide**. The name is **magnesium bromide**. The subscript 2 is not mentioned; it is already implied by the charges.

**$\ce{Li2O}$** — lithium is Group 1A, fixed $+1$. Oxygen → ox**ide**. The name is **lithium oxide**.
:::
::::

:::: tabs
::: tab Problem
Name $\ce{Cu2O}$ and $\ce{CuO}$.
:::
::: tab Solution
Copper is a transition metal, so both names need a Roman numeral, and you find it by working backwards from the anion.

**$\ce{Cu2O}$** — oxide is always $\ce{O^2-}$. Two copper ions must supply $+2$ total, so each is $+1$: **copper(I) oxide**.

**$\ce{CuO}$** — one oxide is $-2$, so the single copper must be $+2$: **copper(II) oxide**.

This pair is the reason the Roman numeral system exists. Both compounds are "copper and oxygen," and without the numeral the two names would be identical.
:::
::::

:::: tabs
::: tab Problem
Name $\ce{NH4NO3}$ and $\ce{Fe3(PO4)2}$.
:::
::: tab Solution
**$\ce{NH4NO3}$** — this one has no metal at all, but $\ce{NH4+}$ is a polyatomic cation and it behaves exactly like one. Cation ammonium, anion nitrate: **ammonium nitrate**.

**$\ce{Fe3(PO4)2}$** — iron is a transition metal, so find its charge from the anion. Phosphate is $\ce{PO4^3-}$, and there are two of them, so the anions total $-6$. Three iron ions must supply $+6$, so each is $+2$:
$$3x + 2(-3) = 0 \;\Rightarrow\; x = +2$$
The name is **iron(II) phosphate**.
:::
::::

### Molecular compounds

Molecular compounds are formed between nonmetals, or nonmetals and metalloids. Because no charges fix the ratio, the name must state it explicitly, and that is what the Greek prefixes do.

- Some have common names you simply learn: water $\ce{H2O}$, ammonia $\ce{NH3}$, methane $\ce{CH4}$.
- Otherwise, the element that appears further to the left in a period — or lower in a group — is written and named first.
- The second element takes the **-ide** ending.
- Use a Greek prefix on each element to give the number of atoms.
- The prefix **mono-** is dropped from the *first* element only: $\ce{CO}$ is carbon monoxide, not monocarbon monoxide.

| Prefix | Number | Prefix | Number |
|---|---|---|---|
| mono- | 1 | hexa- | 6 |
| di- | 2 | hepta- | 7 |
| tri- | 3 | octa- | 8 |
| tetra- | 4 | nona- | 9 |
| penta- | 5 | deca- | 10 |

:::: tabs
::: tab Problem
Name $\ce{CO}$ and $\ce{CO2}$. Why do these two need prefixes when $\ce{MgBr2}$ did not?
:::
::: tab Solution
**$\ce{CO}$** is **carbon monoxide** and **$\ce{CO2}$** is **carbon dioxide**. In both, mono- is dropped from carbon but kept on the oxide in $\ce{CO}$.

They need prefixes because carbon and oxygen are both nonmetals with no fixed charges, so carbon and oxygen genuinely can combine in more than one ratio, and the name must distinguish them. In $\ce{MgBr2}$ the charges $+2$ and $-1$ permit exactly one ratio, so stating it would be redundant. **Prefixes appear precisely where the ratio is not already determined.**
:::
::::

:::: tabs
::: tab Problem
Name $\ce{N2O4}$ and $\ce{PCl5}$.
:::
::: tab Solution
**$\ce{N2O4}$** — two nitrogens (di-) and four oxygens (tetra-). Nitrogen is named first because it lies to the left of oxygen in period 2. The name is **dinitrogen tetroxide**. (The "a" of tetra- is conventionally dropped before the vowel in oxide.)

**$\ce{PCl5}$** — one phosphorus, so mono- is omitted on the first element; five chlorines gives penta-. The name is **phosphorus pentachloride**.
:::
::::

### Acids

An **acid** is a substance that yields hydrogen ions, $\ce{H+}$, when dissolved in water. Acid names depend on whether oxygen is present.

**Binary acids** contain hydrogen and one other element. As a pure substance, $\ce{HCl}$ is a gas named hydrogen chloride. Dissolved in water it is an acid, and it takes the pattern *hydro-* + stem + *-ic acid*: **hydrochloric acid**. Likewise $\ce{HBr}(aq)$ is hydrobromic acid and $\ce{H2S}(aq)$ is hydrosulfuric acid.

**Oxoacids** contain hydrogen, one other element, and oxygen, written in that order. Five reference oxoacids anchor the whole system, and all five end in *-ic*:

| Acid | Name | Acid | Name |
|---|---|---|---|
| $\ce{H2CO3}$ | carbonic acid | $\ce{H3PO4}$ | phosphoric acid |
| $\ce{HClO3}$ | chloric acid | $\ce{H2SO4}$ | sulfuric acid |
| $\ce{HNO3}$ | nitric acid | | |

Every other oxoacid of the same central element is named by counting oxygens relative to its reference acid:

1. **One more O** than the "-ic" acid → **per-...-ic** acid. $\ce{HClO3}$ chloric → $\ce{HClO4}$ **per**chlor**ic** acid.
2. **One fewer O** → **-ous** acid. $\ce{HNO3}$ nitric → $\ce{HNO2}$ nitr**ous** acid.
3. **Two fewer O** → **hypo-...-ous** acid. $\ce{HBrO3}$ bromic → $\ce{HBrO}$ **hypo**brom**ous** acid.

The anions left behind when the hydrogens are removed are **oxoanions**, and their endings track the acid's:

1. All H removed from an **-ic** acid → the anion ends in **-ate**. Carbonic acid → carbon**ate**, $\ce{CO3^2-}$.
2. All H removed from an **-ous** acid → the anion ends in **-ite**. Chlorous acid → chlor**ite**, $\ce{ClO2^-}$.
3. If only *some* hydrogens are removed, the name says how many remain.

Chlorine shows the complete pattern in one place:

| Acid | Acid name | Anion | Anion name |
|---|---|---|---|
| $\ce{HClO4}$ | perchloric acid | $\ce{ClO4^-}$ | perchlorate |
| $\ce{HClO3}$ | chloric acid | $\ce{ClO3^-}$ | chlorate |
| $\ce{HClO2}$ | chlorous acid | $\ce{ClO2^-}$ | chlorite |
| $\ce{HClO}$ | hypochlorous acid | $\ce{ClO^-}$ | hypochlorite |

And phosphoric acid shows partial hydrogen removal:

| Species | Name |
|---|---|
| $\ce{H3PO4}$ | phosphoric acid |
| $\ce{H2PO4^-}$ | dihydrogen phosphate |
| $\ce{HPO4^2-}$ | hydrogen phosphate |
| $\ce{PO4^3-}$ | phosphate |

{{sp[warning] Reminder}} "-ic acid" gives "-ate"; "-ous acid" gives "-ite". The -ic acid has one more oxygen than the -ous acid, just as the -ate ion has one more oxygen than the -ite ion.

:::: tabs
::: tab Problem
Name $\ce{HF}(aq)$ and $\ce{HI}(aq)$.
:::
::: tab Solution
Both are binary acids — hydrogen plus a single nonmetal, no oxygen — so both take *hydro-* + stem + *-ic acid*.

$\ce{HF}(aq)$ is **hydrofluoric acid**; $\ce{HI}(aq)$ is **hydroiodic acid**.

Compare with the pure gases, which are named as ordinary binary molecular compounds: hydrogen fluoride and hydrogen iodide. Same formula, different name, depending on whether it is dissolved.
:::
::::

:::: tabs
::: tab Problem
Name $\ce{HBrO}$ and $\ce{H2SO3}$, and give the anion of each.
:::
::: tab Solution
**$\ce{HBrO}$** — bromine's reference "-ic" acid is bromic acid, $\ce{HBrO3}$, following chloric acid's pattern. $\ce{HBrO}$ has two fewer oxygens, which is rule 3: **hypobromous acid**. Removing the H from an "-ous" acid gives an "-ite" anion: $\ce{BrO^-}$, **hypobromite**.

**$\ce{H2SO3}$** — the reference is sulfuric acid, $\ce{H2SO4}$. This has one fewer oxygen, which is rule 2: **sulfurous acid**. Its anion is $\ce{SO3^2-}$, **sulfite** — which is exactly the entry you saw in the polyatomic ion table, now derived rather than memorized.
:::
::::

### Bases and hydrates

A **base** is a substance that yields hydroxide ions, $\ce{OH^-}$, when dissolved in water. Sodium hydroxide, $\ce{NaOH}$, is the standard example. Bases need no separate naming system — $\ce{NaOH}$ is named as the ionic compound it is, with hydroxide as the anion.

**Hydrates** are compounds with a definite number of water molecules incorporated into the solid, written after a centered dot. Name the compound normally, then add a Greek prefix and the word "hydrate" to count the waters.

:::: tabs
::: tab Problem
Name $\ce{CuSO4.5H2O}$ and $\ce{CaCl2.2H2O}$.
:::
::: tab Solution
**$\ce{CuSO4.5H2O}$** — take the compound first. The anion is sulfate, $\ce{SO4^2-}$, so copper must be $+2$: copper(II) sulfate. Five waters gives penta-. The name is **copper(II) sulfate pentahydrate**.

**$\ce{CaCl2.2H2O}$** — calcium is Group 2A with a fixed $+2$ charge, so no numeral: calcium chloride. Two waters: **calcium chloride dihydrate**.

Note that the Greek prefix here counts water molecules, not atoms of an element. Apart from prefixes built into polyatomic ion names (such as dichromate), this is the one place a counting prefix is added to an ionic compound's name.
:::
::::

## Synthesis

==This chapter moves from the atom (protons, neutrons, electrons; atomic and mass number) to the periodic table's organization, to how atoms combine into molecules and ions, and finally to the mechanical skill of naming what forms.== The links run in both directions: the periodic table is what makes ion charges predictable, predictable charges are what make ionic formulas derivable rather than memorized, and correct formulas are what naming operates on.

Every piece is reused almost immediately. Chapter 3 needs correct formulas to calculate molar mass and balance equations. Chapter 4 needs compound names and formulas to read and write reaction equations, and it needs the polyatomic ions from §2.3 constantly. The group-to-charge pattern in §2.2 is explained properly in Chapters 7 and 8, once electron configuration is available. The $^{A}_{Z}\ce{X}$ notation and the alpha/beta/gamma vocabulary established here reappear unchanged in Chapter 19's nuclear equations.

## Asset and License Record for This Chapter

| Asset | Source URL | License | Attribution |
|---|---|---|---|
| `assets/atom_structure.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
| `assets/subatomic_particle_masses.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated from the study guide's own particle-mass data; released under this package's CC BY 4.0 license. |
| `assets/radiation_types.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
| `assets/geiger_marsden_expectation_result.svg` | https://commons.wikimedia.org/wiki/File:Geiger-Marsden_experiment_expectation_and_result.svg | CC BY 3.0 | Kurzon, via Wikimedia Commons. |
| `assets/isotope_notation.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
| `assets/periodic_table_overview.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
| `assets/nacl_salt.jpg` | https://commons.wikimedia.org/wiki/File:Chlorek_sodu_NaCl_Salt.jpg | CC BY-SA 3.0 | Kruczy89, via Wikimedia Commons. |
| `assets/ion_charges_by_group.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
| `assets/ionic_formula_charge_balance.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
| `assets/naming_decision_tree.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
