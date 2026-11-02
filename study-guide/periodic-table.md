{{nyml
kind: document
format: 1
title: Chapter 8: The Periodic Table
}}

# Chapter 8: The Periodic Table

:::info
**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 8 (CC BY 4.0)
**Audience:** introductory undergraduate general chemistry, first semester
**Package license:** CC BY 4.0
**Note:** builds directly on Chapter 7's electron configurations; facts checked for accuracy against OpenStax *Chemistry 2e* and Wikipedia (used for reference only — no text or figures adapted from either).
:::

:::success
**Chapter Learning Objectives**
- Classify elements by category and write electron configurations for their ions.
- Explain effective nuclear charge and use it to compare atomic and ionic radii.
- Explain and apply the periodic trends in ionization energy and electron affinity.
- Describe the chemical behavior of each main group and classify oxides as basic, acidic, or amphoteric.
:::

## Chapter Logic

Chapter 7 ended with a procedure for writing any atom's electron configuration. On its own that is bookkeeping. This chapter turns it into prediction.

==One quantity does almost all the work: the effective nuclear charge, the pull an outermost electron actually feels. Atomic size, ionization energy, electron affinity, and ultimately an element's whole chemical personality are consequences of it.== Learn to reason from configuration to $Z_\text{eff}$ to behavior, and the periodic table stops being a chart to look things up in and becomes a chart to reason from.

{{mermaid
graph TD
  A["Electron configuration<br/>and element categories"] --> B["Effective nuclear charge"]
  B --> C["Atomic and ionic radius"]
  B --> D["Ionization energy<br/>and electron affinity"]
  C --> E["Chemical behavior of each group"]
  D --> E
}}

**Visual description:** A flowchart. Electron configuration determines effective nuclear charge, which in turn drives both the size trends and the energy trends. Those two together account for the observed chemical behavior of each group.

## 8.1 Electron Configuration and Periodic Classification{{attrs[#blk-ch08sec01]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 8.1a}} Classify elements as representative, noble gas, transition metal, Group 2B, lanthanide, or actinide.
- {{sp[info] Objective 8.1a}} Define valence electrons and relate them to group number.
- {{sp[info] Objective 8.1b}} Write electron configurations for cations and anions of representative elements.
- {{sp[info] Objective 8.1b}} Write electron configurations for transition-metal cations.
- {{sp[info] Objective 8.1b}} Identify isoelectronic species.
:::

### Categories of element

Which subshell is filling sorts every element into one of six categories, laid out in Figure 8.1.

| Category | Groups | Subshell being filled |
|---|---|---|
| **Representative (main-group)** | 1A–7A | outermost $s$ or $p$, incompletely filled |
| **Noble gases** | 8A | $p$ subshell complete, except He ($1s^2$, complete $s$ subshell); $ns^2np^6$ otherwise |
| **Transition metals** | 1B, 3B–8B | $d$, incompletely filled — or forming cations that are |
| **Group 2B** | Zn, Cd, Hg | neither: $d$ is full and $s$ is full |
| **Lanthanides and actinides** | f-block | $f$, incompletely filled |

![Simplified periodic-table-shaped map of element categories](../assets/element_category_map.svg =680x)
*Figure 8.1 — Element categories map directly onto which subshell type is being filled: $s$/$p$ (representative), $p^6$ (noble gas), $d$ (transition metal), or $f$ (lanthanide/actinide).*

==**Valence electrons** are the outer-shell electrons involved in bonding== — and for a representative element they are the only ones that matter chemically. Chapter 7 established the reason elements in a group behave alike: they have the same valence configuration. For a representative element, the group number *is* the valence-electron count — Group 6A elements all have six.

:::: tabs
::: tab Problem
Classify each element by category, using only its electron configuration: (a) $[\ce{Ar}]4s^23d^3$; (b) $[\ce{Kr}]5s^24d^{10}5p^4$; \(c) $[\ce{Xe}]6s^24f^7$; (d) $[\ce{Ne}]3s^23p^6$.
:::
::: tab Solution
Ask which subshell is incomplete — that alone decides the category.

**(a)** The $3d$ is partly filled (3 of 10), so this is a **transition metal**. It is vanadium.

**(b)** The outermost $p$ is partly filled (4 of 6), so this is a **representative element** — Group 6A, since $5s^25p^4$ is six valence electrons. It is tellurium.

**\(c)** The $4f$ is partly filled, so this is a **lanthanide**. It is europium.

**(d)** The outermost $p$ is *complete*: $3s^23p^6$. That is a **noble gas**, argon.

Note that (b) and (d) both end in $p$, and only the count distinguishes them. A complete $ns^2np^6$ is the noble-gas signature.
:::
::::

:::: tabs
::: tab Problem
Zinc is $[\ce{Ar}]4s^23d^{10}$ and copper is $[\ce{Ar}]4s^13d^{10}$. Both have a filled $3d$. Why is copper classified as a transition metal and zinc is not?
:::
::: tab Solution
The definition is not about the *atom* alone: a transition metal has an incompletely filled $d$ subshell **or readily forms cations that do**.

**Copper** forms $\ce{Cu^2+}$, which is $[\ce{Ar}]3d^9$ — an incomplete $d$ subshell. It qualifies on the second clause.

**Zinc** forms only $\ce{Zn^2+}$, which is $[\ce{Ar}]3d^{10}$ — still complete. It never produces an incomplete $d$, so it fails both clauses, and Zn, Cd and Hg are set aside as **Group 2B**.

This is the reason the definition carries that awkward second clause at all: without it, copper would be misclassified.
:::
::::

### Ions of representative elements

Cations and anions form by moving toward the nearest noble-gas configuration.

A **cation** loses electrons from the highest occupied $n$ shell:

$$\ce{Na}: [\ce{Ne}]3s^1 \quad\longrightarrow\quad \ce{Na+}: [\ce{Ne}]$$

An **anion** gains electrons into the highest partly filled shell:

$$\ce{F}: [\ce{He}]2s^22p^5 \quad\longrightarrow\quad \ce{F-}: [\ce{Ne}]$$

Species with the same number of electrons, and hence the same configuration, are **isoelectronic**. $\ce{Na+}$, $\ce{F-}$ and $\ce{Ne}$ are all isoelectronic at ten electrons — which is exactly why Chapter 2 could predict ion charges from group number.

:::: tabs
::: tab Problem
Write the electron configuration of (a) $\ce{Mg^2+}$, (b) $\ce{O^2-}$, and \(c) $\ce{Cl-}$. Which are isoelectronic with each other?
:::
::: tab Solution
**(a) $\ce{Mg^2+}$.** Magnesium is $[\ce{Ne}]3s^2$. Losing both $3s$ electrons empties the third shell: $[\ce{Ne}]$, or $1s^22s^22p^6$ — **10 electrons**.

**(b) $\ce{O^2-}$.** Oxygen is $1s^22s^22p^4$. Gaining two electrons completes the $2p$: $1s^22s^22p^6 = [\ce{Ne}]$ — **10 electrons**.

**\(c) $\ce{Cl-}$.** Chlorine is $[\ce{Ne}]3s^23p^5$. Gaining one completes the $3p$: $[\ce{Ne}]3s^23p^6 = [\ce{Ar}]$ — **18 electrons**.

**(a) and (b) are isoelectronic** — both have neon's configuration. \(c) is not; it has argon's.

Note that a cation and an anion arrived at the same configuration from opposite directions. That is the general pattern for representative elements: everything moves toward the nearest noble gas.
:::
::::

### Ions of transition metals

Transition metals follow a rule that looks backwards at first.

{{sp[warning] Reminder}} Electrons are always removed from $ns$ **before** $(n-1)d$ — even though $ns$ *filled* first. Filling order and removal order are not the same, because adding electrons and adding protons changes the relative energies.

$$\ce{Fe}: [\ce{Ar}]4s^23d^6 \quad\longrightarrow\quad \ce{Fe^2+}: [\ce{Ar}]3d^6 \quad\longrightarrow\quad \ce{Fe^3+}: [\ce{Ar}]3d^5$$

:::: tabs
::: tab Problem
Write the electron configuration of (a) $\ce{Ti^2+}$ ($Z=22$), (b) $\ce{Cu^2+}$ ($Z=29$), and \(c) $\ce{Zn^2+}$ ($Z=30$).
:::
::: tab Solution
Write the neutral atom first, then remove from $4s$ before $3d$.

**(a) Ti** is $[\ce{Ar}]4s^23d^2$. Removing both $4s$ electrons: $\ce{Ti^2+} = [\ce{Ar}]3d^2$.

**(b) Cu** is $[\ce{Ar}]4s^13d^{10}$ — one of Chapter 7's two exceptions. Removing the single $4s$ electron gives $\ce{Cu+} = [\ce{Ar}]3d^{10}$; removing one more must then come from $3d$: $\ce{Cu^2+} = [\ce{Ar}]3d^9$.

**\(c) Zn** is $[\ce{Ar}]4s^23d^{10}$. Removing both $4s$: $\ce{Zn^2+} = [\ce{Ar}]3d^{10}$.

$\ce{Zn^2+}$ has a completely filled $3d$ subshell and no partly filled $d$ at all, which is why, under the definition requiring a partly filled d subshell in the atom or a common ion, zinc is often not counted as a true transition metal even though it sits in Group 2B.
:::
::::

> **Where this goes next.** Configuration tells you how many electrons are in the outermost shell. §8.2 asks how tightly the nucleus holds them — which turns out to control everything else in the chapter.

## 8.2 Effective Nuclear Charge and Size{{attrs[#blk-ch08sec02]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 8.2a}} Define effective nuclear charge and estimate it.
- {{sp[info] Objective 8.2a}} Explain how $Z_\text{eff}$ changes across a period and down a group.
- {{sp[info] Objective 8.2a}} Compare atomic radii within a period and within a group.
- {{sp[info] Objective 8.2b}} Compare ionic radii in an isoelectronic series and for one element at different charges.
:::

### Effective nuclear charge

==An outer electron does not feel the full nuclear charge.== Inner electrons sit between it and the nucleus and cancel part of the pull — an effect called **shielding**. What is left over is the **effective nuclear charge**:

$$Z_\text{eff} \approx Z - (\text{number of shielding electrons})$$

![Shielding and effective nuclear charge for lithium, carbon and fluorine](../assets/effective_nuclear_charge.svg =800x)
*Figure 8.2 — All three atoms have the same two inner electrons doing the shielding, so as protons are added across the period, $Z_\text{eff}$ climbs from about $+1$ to about $+7$. The valence electrons are pulled in harder at every step.*

Figure 8.2 makes the arithmetic visible. **Across a period**, protons are added but the new electrons enter the *same* shell, where they shield each other poorly. $Z_\text{eff}$ therefore rises steadily, and the outer electrons are held more tightly.

**Down a group**, $Z_\text{eff}$ also rises — but each new period adds a whole shell, placing the outer electrons much farther from the nucleus. Distance wins, and atoms get larger.

:::warning
**Two competing effects, and which one wins.** It is tempting to say $Z_\text{eff}$ decreases down a group, since atoms get bigger. It does not — the nuclear charge grows faster than the shielding does, so $Z_\text{eff}$ increases both across a period and down a group. What changes down a group is the *distance*: an added shell moves the valence electrons far enough out that the stronger pull is more than offset. Get this backwards and the ionization-energy trend will look inexplicable.
:::

:::: tabs
::: tab Problem
Estimate $Z_\text{eff}$ for a valence electron in (a) sodium and (b) chlorine, counting only core electrons as shielding. Which atom is larger, and does your estimate explain it?
:::
::: tab Solution
Write each configuration and separate core from valence.

**(a) Na** is $[\ce{Ne}]3s^1$: 11 protons, 10 core electrons, 1 valence.
$$Z_\text{eff} \approx 11 - 10 = +1$$

**(b) Cl** is $[\ce{Ne}]3s^23p^5$: 17 protons, 10 core electrons, 7 valence.
$$Z_\text{eff} \approx 17 - 10 = +7$$

**Sodium is much larger.** Its single valence electron feels a pull of roughly $+1$; chlorine's valence electrons each feel about $+7$ and are drawn in far more tightly.

Both are in period 3, so both have their valence electrons in the same shell. Only $Z_\text{eff}$ differs — which is exactly why the radius trend across a period is so steep.

{{sp[warning] Reminder}} This estimate deliberately ignores shielding *among* the valence electrons, which is real but weak. It is good enough for comparisons, not for absolute values.
:::
::::

### Atomic radius

Figure 8.3 collects all four trends of this chapter and the next section onto one table. The **atomic radius** is half the distance between the nuclei of two adjacent atoms of the element — measured between neighbors in a metal, or between the two bonded atoms of a diatomic molecule like $\ce{I2}$.

![Periodic trends in radius, ionization energy and electron affinity](../assets/periodic_trend_map.svg =820x)
*Figure 8.3 — All three trends follow from $Z_\text{eff}$ and distance. Across a period, rising $Z_\text{eff}$ pulls the same shell in tighter: radius falls, and both energies rise. Down a group, the added shell dominates: radius grows, and both energies fall.*

:::: tabs
::: tab Problem
Arrange each set by increasing atomic radius: (a) Li, C, F; (b) Li, Na, K; \(c) Mg, Si, Ca.
:::
::: tab Solution
**(a) F < C < Li.** All in period 2, so the same shell is being filled while $Z$ climbs. Higher $Z_\text{eff}$ means a tighter grip and a smaller atom, so radius decreases left to right — meaning fluorine, furthest right, is smallest.

**(b) Li < Na < K.** All in Group 1A. Each step down adds a shell, so the atoms grow.

**\(c) Si < Mg < Ca.** This one needs both rules. Mg and Si are both in period 3, and Si is further right, so Si < Mg. Ca is directly below Mg in Group 2A, so Ca > Mg. Chaining them gives Si < Mg < Ca.

Part \(c) is the general case: when two elements share neither a period nor a group, compare each to a common neighbor.
:::
::::

### Ionic radius

Forming an ion changes the electron count, and size changes with it — often dramatically.

**A cation is always smaller than its parent atom.** Removing electrons usually empties the outermost shell entirely and always reduces electron–electron repulsion, so the remaining electrons are drawn in.

**An anion is always larger than its parent atom.** Added electrons increase repulsion in the same shell, swelling the cloud, while the nuclear charge is unchanged.

Two comparison rules follow:

- **Within an isoelectronic series** (same electron count, different $Z$): the greater the nuclear charge, the smaller the ion — the effect plotted in Figure 8.4.
- **For the same element** (same $Z$, different electron count): the more electrons, the larger the ion. So $\ce{Fe^3+} < \ce{Fe^2+} < \ce{Fe}$.

:::: tabs
::: tab Problem
Rank $\ce{N^3-}$, $\ce{O^2-}$, $\ce{F-}$, $\ce{Ne}$, $\ce{Na+}$, $\ce{Mg^2+}$, $\ce{Al^3+}$ by size.
:::
::: tab Solution
First check that they belong to one series: N is $Z=7$ with 3 added, O is 8 with 2 added, F is 9 with 1, Ne is 10, Na is 11 minus 1, Mg is 12 minus 2, Al is 13 minus 3. **All have exactly 10 electrons** — an isoelectronic series.

Since the electron count is fixed, only the nuclear charge distinguishes them, and it climbs from 7 to 13. More protons pulling the same ten electrons means a smaller species:

$$\ce{N^3-} > \ce{O^2-} > \ce{F-} > \ce{Ne} > \ce{Na+} > \ce{Mg^2+} > \ce{Al^3+}$$
:::
::::

![Bar chart of radii for the classic 10-electron isoelectronic series](../assets/isoelectronic_radius_series.svg =560x)
*Figure 8.4 — All seven species have exactly 10 electrons, but radius shrinks steadily as nuclear charge climbs from N ($Z = 7$) to Al ($Z = 13$) — the same 10 electrons are pulled progressively tighter.*

:::: tabs
::: tab Problem
For each pair, say which is larger and why: (a) $\ce{K}$ or $\ce{K+}$; (b) $\ce{S}$ or $\ce{S^2-}$; \(c) $\ce{Ca^2+}$ or $\ce{Cl-}$.
:::
::: tab Solution
**(a) $\ce{K}$ is larger.** Potassium is $[\ce{Ar}]4s^1$; losing that one electron removes the entire fourth shell, so $\ce{K+}$ is $[\ce{Ar}]$ — a whole shell smaller.

**(b) $\ce{S^2-}$ is larger.** Same 16 protons, two more electrons. The extra repulsion in the $3p$ subshell swells the cloud.

**\(c) $\ce{Cl-}$ is larger.** These are isoelectronic — both have 18 electrons — so compare nuclear charges: Cl has 17 protons, Ca has 20. Fewer protons pulling the same 18 electrons means the larger ion.

Each part used a different rule: (a) a lost shell, (b) added repulsion at fixed $Z$, \(c) an isoelectronic comparison. Identify which situation you are in before reaching for a rule.
:::
::::

> **Where this goes next. ** Size is one consequence of $Z_\text{eff}$. §8.3 covers the other: how much energy it takes to remove an electron, and how much is released when one is added.

## 8.3 Ionization Energy and Electron Affinity{{attrs[#blk-ch08sec03]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 8.3a}} Define ionization energy and explain why successive values increase.
- {{sp[info] Objective 8.3a}} Read an element's valence-electron count from its successive ionization energies.
- {{sp[info] Objective 8.3a}} Explain and apply the periodic trend in first ionization energy, including its two exceptions.
- {{sp[info] Objective 8.3b}} Define electron affinity and describe its trend.
:::

### Ionization energy

The **ionization energy (IE)** is the minimum energy, in kJ/mol, needed to remove an electron from a gaseous atom or ion in its ground state. Removing the first electron costs $IE_1$, the second $IE_2$, and so on. These always increase:

$$IE_1 < IE_2 < IE_3 < \dots$$

The reason is immediate: after the first removal you are pulling an electron away from a positive ion, and each subsequent removal fights a larger positive charge.

But the increases are not smooth. One step—removing the first core electron once all valence electrons are gone—is always enormously larger than the steps before it, as Figure 8.5 shows.

![Successive ionization energies of Na, Mg and Al](../assets/successive_ionization_energies.svg =820x)
*Figure 8.5 — The huge jump appears exactly when the valence shell is empty and the next electron must come out of the noble-gas core. Sodium's jump is at $IE_2$, magnesium's at $IE_3$, aluminum's at $IE_4$ — one, two, and three valence electrons respectively.*

==Counting the ionization energies that come before the jump counts the valence electrons, and that count is the main-group (A) group number.== It is a way of reading an element's valence-electron count off nothing but a list of energies.

:::: tabs
::: tab Problem
An element has successive ionization energies (kJ/mol) of 738, 1451, 7733, 10540. Which group does it belong to, and what ion will it most likely form?
:::
::: tab Solution
Look at the ratio between consecutive values rather than the differences:

$$\frac{1451}{738}=2.0 \qquad \frac{7733}{1451}=5.3 \qquad \frac{10540}{7733}=1.4$$

The jump is at $IE_3$ — the third electron is more than five times harder to remove than the second. So the first **two** electrons come from the valence shell and the third would have to breach the core.

**Two valence electrons: Group 2A**, and the element will form a **$2+$ ion**. (These are magnesium's values.)

The point of the method is that it works without knowing the element at all. The pattern of the numbers reveals the configuration.
:::
::::

### The trend, and its two exceptions

Figure 8.6 plots the trend across period 2. First ionization energy **increases across a period** (rising $Z_\text{eff}$ holds electrons tighter) and **decreases down a group** (the outer electron is farther out, so easier to remove). It is the mirror image of the atomic-radius trend, and for exactly the same reason.

![Line chart of first ionization energy across Period 2](../assets/ionization_energy_trend.svg =560x)
*Figure 8.6 — Ionization energy rises overall across Period 2, but with two characteristic dips: Be→B (removing a higher-energy $2p$ electron, partly shielded by the $2s$ electrons, is easier than removing a paired $2s$ electron) and N→O (removing one of the two paired electrons in O's $2p^4$, which repel each other, costs less energy than removing an electron from N's half-filled $2p^3$).*

Both dips come straight from Chapter 7's filling rules, which is why they are worth understanding rather than memorizing:

- **Be → B.** Beryllium is $[\ce{He}]2s^2$ and boron is $[\ce{He}]2s^22p^1$. Boron's outermost electron is in a *higher-energy* $2p$ orbital, partly shielded by the filled $2s$, so it comes off more easily despite boron's larger $Z$.
- **N → O.** Nitrogen is $[\ce{He}]2s^22p^3$ — a half-filled $2p$ subshell, with three unpaired electrons and no pairing repulsion. Oxygen is $2p^4$, so one orbital holds a pair. Removing that paired electron relieves the repulsion, making it cheaper than the trend predicts.

:::: tabs
::: tab Problem
Arrange by increasing first ionization energy: (a) Na, Mg, Al; (b) F, Cl, Br; \(c) N, O, F.
:::
::: tab Solution
**(a) Na < Al < Mg.** The general trend across period 3 would give Na < Mg < Al — but this is the Be→B dip repeated one period down. Aluminum's outermost electron is a $3p$ electron shielded by the filled $3s$, so it comes off more easily than magnesium's paired $3s$ electron.

**(b) Br < Cl < F.** All Group 7A. Down a group, ionization energy falls, so the highest is at the top.

**\(c) O < N < F.** The plain trend would give N < O < F, but this is the N→O dip: nitrogen's half-filled $2p^3$ is unusually stable, so oxygen is easier to ionize than nitrogen despite being further right.

Both irregular cases appear in this one problem, which is why the two exceptions are worth knowing: they are common exam material precisely because the plain trend gets them wrong.
:::
::::

### Electron affinity

The **electron affinity (EA)** is the negative of the energy change when a gaseous atom accepts an electron to form an anion. A large positive EA means the atom releases a lot of energy on gaining an electron — it "wants" one.

The trend is broadly the same as ionization energy: EA **increases across a period** and **decreases down a group**, for the same $Z_\text{eff}$ reason. The halogens have the largest values of all, since one more electron completes their shell.

{{sp[warning] Watch out}} The noble gases are the clean exception — their electron affinities are near zero or negative, because a filled shell has no room and an added electron would have to start a new one. Beyond that, electron affinity has more irregularities than ionization energy does; treat the trend as a tendency rather than a law.

:::: tabs
::: tab Problem
Which of each pair has the more positive electron affinity, and why? (a) F or Ne; (b) Cl or Br; \(c) Li or F.
:::
::: tab Solution
**(a) F.** Fluorine is $2s^22p^5$, one electron short of a filled shell, so gaining one releases a great deal of energy. Neon's shell is already full, so an added electron would have to enter $n=3$ — energetically unfavorable, and neon's EA is near zero.

**(b) Cl.** Both are halogens, and EA falls down a group. The added electron in bromine enters a shell farther from the nucleus and is held less strongly. (Chlorine in fact has the largest EA of any element, slightly exceeding fluorine's, because fluorine's small size makes its $2p$ subshell crowded.)

**\(c) F.** Fluorine is at the right of period 2 with high $Z_\text{eff}$ and needs one electron; lithium is at the left, holds its electrons loosely, and would rather lose one than gain one.
:::
::::

:::: tabs
::: tab Problem
Sodium's first ionization energy is 496 kJ/mol and chlorine's is 1251 kJ/mol. Sodium's electron affinity is 53 kJ/mol and chlorine's is 349 kJ/mol. Use these four numbers to predict what happens when sodium meets chlorine.
:::
::: tab Solution
Compare the two possible transfers.

**Sodium gives, chlorine takes.** Removing sodium's electron costs 496 kJ/mol; chlorine accepting it releases 349 kJ/mol. Net cost: $496 - 349 = +147$ kJ/mol.

**Chlorine gives, sodium takes.** Removing chlorine's electron costs 1251 kJ/mol; sodium accepting it releases only 53 kJ/mol. Net cost: $1251 - 53 = +1198$ kJ/mol.

The first direction is cheaper by more than a factor of eight, so **sodium loses and chlorine gains**, giving $\ce{Na+}$ and $\ce{Cl-}$.

Both routes still show a net cost on paper. What pays the remainder is the enormous attraction between the resulting oppositely-charged ions once they come together — the lattice energy, which Chapter 9 quantifies. The trends decide the *direction* of the transfer; the lattice makes it happen.
:::
::::

> **Where this goes next.** §8.2 and §8.3 built four trends from one cause. §8.4 cashes them in: everything an element does chemically follows from how tightly it holds its valence electrons.

## 8.4 A Survey of Chemical Properties of Elements{{attrs[#blk-ch08sec04]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 8.4a}} Explain why elements in a group share chemical behavior, and when the comparison is weakest.
- {{sp[info] Objective 8.4a}} Describe diagonal relationships.
- {{sp[info] Objective 8.4a}} Summarize the chemical behavior of hydrogen and of each main group.
- {{sp[info] Objective 8.4b}} Classify oxides as basic, acidic, or amphoteric, and relate the classification to structure.
:::

### Why groups behave alike — and where the rule weakens

Elements in a group share a valence configuration, so they share chemistry. But the comparison is not equally reliable everywhere.

It is strongest in **Groups 1A and 2A** (all metals, apart from hydrogen) and **Groups 7A and 8A** (all nonmetals), where every member (hydrogen aside) falls in the same class, metal or nonmetal. In **Groups 3A through 6A** the elements shift from nonmetal (or, in 3A, metalloid) to metalloid to metal going down, so chemical properties vary far more even though the valence configuration is constant.

A second pattern cuts across the columns. **Diagonal relationships** link the first three second-period elements to the element diagonally below-right: Li resembles Mg, Be resembles Al, and B resembles Si. The cause is that these pairs have similar cation charge densities — a similar ratio of charge to size, even though the charges themselves differ.

### Hydrogen, and the eight main groups

Hydrogen belongs to no group comfortably. With one electron it can **lose** it to give $\ce{H+}$ (as in $\ce{HCl}$, $\ce{HBr}$ dissolved in water) or **gain** one to fill its $1s$ orbital and give the hydride ion $\ce{H-}$ (as in $\ce{NaH}$, $\ce{CaH2}$). No other element does both routinely, which is why hydrogen is usually drawn floating above the table.

| Group | Character | Chemistry |
|---|---|---|
| **1A** alkali metals | all metals | lowest ionization energies; form $\ce{M+}$; so reactive they never occur pure in nature; react with water to give $\ce{H2}$ plus the hydroxide; tarnish in air by forming oxides |
| **2A** alkaline earth metals | all metals | form $\ce{M^2+}$; less reactive than 1A, and reactivity rises down the group — Be does not react with water, Mg reacts with steam, Ca/Sr/Ba attack cold water |
| **3A** | B is a metalloid, rest metals | B forms no binary ionic compounds and resists oxygen and water; Al forms a protective oxide coating; heavier members form both $+1$ and $+3$ ions, with $+1$ growing more stable downward |
| **4A** | C nonmetal, Si/Ge metalloids, Sn/Pb metals | oxidation states $+2$ and $+4$; $+4$ favored for C and Si, $+2$ decisively favored for Pb; Sn and Pb react with acids to release $\ce{H2}$ |
| **5A** | N/P nonmetals, As/Sb metalloids, Bi metal | $\ce{N2}$ is a diatomic gas forming many oxides; P exists as $\ce{P4}$; both form important oxoacids, $\ce{HNO3}$ and $\ce{H3PO4}$; N forms the nitride ion $\ce{N^3-}$ |
| **6A** | O/S/Se nonmetals, Te/Po metalloids | O is diatomic, S is $\ce{S8}$, Se is $\ce{Se8}$; all form $2-$ anions; sulfur's key compounds are $\ce{SO2}$, $\ce{SO3}$ and $\ce{H2S}$, and $\ce{SO3}$ with water gives sulfuric acid |
| **7A** halogens | all nonmetals | exist as $\ce{X2}$; high ionization energies and large electron affinities; never found free in nature; halide anions are isoelectronic with the next noble gas; HF is a weak acid while HCl, HBr and HI are strong |
| **8A** noble gases | all nonmetals | monatomic; filled $ns^2np^6$ (helium: $1s^2$); the highest ionization energies in their periods and essentially no tendency to gain electrons |

Figure 8.7 shows the most spectacular case. ==Most entries in that table are consequences of §8.3. Group 1A is reactive because its ionization energy is the lowest; the halogens are reactive because their electron affinity is the highest; the noble gases are inert because they are extreme in both directions at once.==

![High-speed photo of sodium metal reacting violently with water](../assets/sodium_water.png =460x)
*Figure 8.7 — Sodium's single, loosely-held valence electron makes it reactive enough to react violently on contact with water, releasing hydrogen gas that can ignite — a dramatic, visible demonstration of Group 1A's characteristic low ionization energy.*

:::: tabs
::: tab Problem
Predict which member of each pair is more reactive, and give the reason in terms of a trend: (a) Li or Cs, as metals; (b) F or I, as nonmetals.
:::
::: tab Solution
**(a) Cs.** Metallic reactivity means willingness to *lose* an electron, so it tracks ionization energy inversely. IE falls down a group, so cesium's valence electron is the easiest to remove. Cesium reacts explosively with water; lithium reacts briskly but far less violently.

**(b) F.** Nonmetal reactivity means willingness to *gain* an electron, so it tracks electron affinity. EA generally falls down a group (though Cl's EA slightly exceeds F's), and electronegativity is highest for fluorine, whose F–F bond is also unusually weak, so fluorine is the most reactive halogen — reactive enough to attack water and release oxygen.

The two answers point in opposite directions down the table, and that is the whole logic of the periodic table in one comparison: metals get more reactive downward, nonmetals less.
:::
::::

:::: tabs
::: tab Problem
Lithium is the only alkali metal whose carbonate decomposes on heating, and the only one forming a nitride directly with $\ce{N2}$ — behavior otherwise typical of magnesium. Explain using the diagonal relationship, and name the other two classic diagonal pairs.
:::
::: tab Solution
**Lithium and magnesium form a diagonal pair.** Going right across a period increases charge and decreases size; going down a group decreases charge density. Moving diagonally down-right, the two effects roughly cancel, so $\ce{Li+}$ and $\ce{Mg2+}$ end up with similar **charge densities** — a similar ratio of charge to size, even though the charges themselves differ.

Since charge density is what controls how strongly a cation polarizes its neighbors, the two behave alike even though they are in different groups.

The other two classic pairs are **Be with Al** and **B with Si**.

This is why the group rule needs a caveat: valence configuration is the dominant influence, but for the small second-period elements, charge density can outweigh it.
:::
::::

### Oxides across a period

Oxygen combines with almost everything, and as Figure 8.8 shows, the character of the oxide tracks the metallic character of its partner.

![Acid-base and structural character of the period 3 oxides](../assets/oxide_character_period3.svg =820x)
*Figure 8.8 — Across period 3 the oxides shift from high-melting ionic solids, through silicon dioxide's covalent network, to small discrete molecules with low melting points — and their acid-base character shifts with the structure.*

- **Metal oxides are generally basic.** Metals have low ionization energies, so they hand electrons over readily and form ionic oxides such as $\ce{Na2O}$ and $\ce{MgO}$. These react with acids to give a salt and water. Being ionic, they have high melting and boiling points.
- **Nonmetal oxides are generally acidic.** $\ce{SO3}$ and $\ce{Cl2O7}$ react with bases to give a salt and water. They are small discrete molecules with weak attractions between them, so their melting points are low. A few — $\ce{CO}$ and $\ce{NO}$ — are neutral, reacting with neither.
- **$\ce{Al2O3}$ is amphoteric**, reacting with both acids and bases. Aluminum, a metal, sits next to the metal/nonmetal boundary, and its oxide sits at the acid/base boundary.

Silicon dioxide is the structural in-between: no ions, but a huge three-dimensional covalent network rather than small molecules — which is why quartz melts at over 1600 °C while $\ce{SO3}$ melts at 17 °C.

:::: tabs
::: tab Problem
Classify each oxide as basic, acidic, or amphoteric, and predict what it reacts with: $\ce{K2O}$, $\ce{P4O10}$, $\ce{Al2O3}$, $\ce{CaO}$.
:::
::: tab Solution
Identify the partner element's character first, then read off the oxide's.

- **$\ce{K2O}$** — potassium is a Group 1A metal, so this is a **basic** oxide. It reacts with acids: $\ce{K2O + 2HCl -> 2KCl + H2O}$.
- **$\ce{P4O10}$** — phosphorus is a nonmetal, so this is an **acidic** oxide. It reacts with bases, and with water to give phosphoric acid.
- **$\ce{Al2O3}$** — aluminum is a metal sitting next to the metal–nonmetal boundary, so this is the **amphoteric** case. It reacts with both acids and bases.
- **$\ce{CaO}$** — calcium is a Group 2A metal: **basic**. It reacts with acids, and with water to give $\ce{Ca(OH)2}$.

The single rule covering all four: **metal oxide → basic, nonmetal oxide → acidic**, with $\ce{Al2O3}$ as the boundary case to memorize.
:::
::::

:::: tabs
::: tab Problem
$\ce{SO2}$ dissolves in water to give sulfurous acid; $\ce{CaO}$ dissolves to give calcium hydroxide. Predict what $\ce{BaO}$ and $\ce{N2O5}$ give with water, and write which of the four oxides would react with each other.
:::
::: tab Solution
Classify each by its partner element.

- **$\ce{BaO}$** — barium is a Group 2A metal, so this is a **basic** oxide. With water it gives the hydroxide: $\ce{BaO + H2O -> Ba(OH)2}$.
- **$\ce{N2O5}$** — nitrogen is a nonmetal, so this is an **acidic** oxide. With water it gives an oxoacid: $\ce{N2O5 + H2O -> 2HNO3}$.

**Which react with each other:** an acidic oxide reacts with a basic one. So $\ce{SO2}$ and $\ce{N2O5}$ each react with $\ce{CaO}$ and with $\ce{BaO}$ — four combinations in all. Two acidic oxides do not react with each other, and neither do two basic ones.

This is the reaction that scrubs sulfur dioxide from power-station flue gas: $\ce{CaO + SO2 -> CaSO3}$, a basic oxide capturing an acidic one.
:::
::::

## Synthesis

==This chapter turns the periodic table from a filing system into a predictive instrument. Two quantities — the effective nuclear charge an outer electron feels and the shell (n) it occupies — account for atomic radius, ionic radius, ionization energy, and electron affinity; and those four together account for the chemical behavior of every group.==

Backwards, none of it works without Chapter 7. An element's category, its valence count, its ion's configuration, and the two ionization-energy dips are all read directly off an electron configuration. Chapter 2's periodic table was a map with names on it; Chapter 7 supplied the mechanism; this chapter supplies the consequences.

Forwards, these trends are the working vocabulary of the rest of the course. Chapter 9 builds bonding on electronegativity, which is ionization energy and electron affinity combined into one number, and explains ionic bonding as a low-IE metal meeting a high-EA nonmetal. Chapter 10's molecular polarity depends on electronegativity differences. Chapter 15's acid strength follows the same left-to-right logic that governs oxide acidity here. From this point on, "predict the trend" is an instruction you are expected to be able to follow without being told which trend.

## Asset and License Record for This Chapter

| Asset | Source URL | License | Attribution |
|---|---|---|---|
| `assets/element_category_map.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib, schematic; released under this package's CC BY 4.0 license. |
| `assets/effective_nuclear_charge.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; released under this package's CC BY 4.0 license. |
| `assets/periodic_trend_map.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; released under this package's CC BY 4.0 license. |
| `assets/isoelectronic_radius_series.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib using standard tabulated ionic radii, matching the study guide's own isoelectronic-series example; released under this package's CC BY 4.0 license. |
| `assets/successive_ionization_energies.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; released under this package's CC BY 4.0 license. |
| `assets/ionization_energy_trend.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib using real tabulated ionization-energy values; released under this package's CC BY 4.0 license. |
| `assets/sodium_water.png` | https://commons.wikimedia.org/wiki/File:Sodium_and_Water.png | CC BY-SA 3.0 | Tavoromann / Tony Mach, via Wikimedia Commons, CC BY-SA 3.0. |
| `assets/oxide_character_period3.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; released under this package's CC BY 4.0 license. |
