{{nyml
kind: document
format: 1
title: Chapter 19: Nuclear Chemistry
}}

# Chapter 19: Nuclear Chemistry

Nuclear marker 05:16:34 (review r2)

Nuclear marker2 05:25:26 (review r2)

:::info
**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 19 (CC BY 4.0)
**Audience:** introductory undergraduate general chemistry, second semester
**Package license:** CC BY 4.0
**Note:** builds on atomic number/mass number notation (Chapter 2) and first-order kinetics/half-life (Chapter 13); facts checked for accuracy against OpenStax *Chemistry 2e* and Wikipedia (used for reference only — no text or figures adapted from either).
:::

:::success
**Chapter Learning Objectives**
- Balance nuclear equations by conserving mass number and charge, and identify patterns of nuclear stability.
- Calculate nuclear binding energy from mass defect.
- Identify types of radioactive decay and apply first-order kinetics to decay problems, including radiocarbon dating.
- Explain nuclear fission, nuclear fusion, chain reactions, and critical mass.
:::

## Chapter Logic

Every prior chapter changed how electrons are arranged. This final chapter changes the site of chemistry itself — to the nucleus — while reusing two tools you already have: Chapter 2's atomic notation and Chapter 13's first-order kinetics. ==Nuclear energies are about a million times larger than chemical ones, and they can be measured by a single number: the mass that goes missing when a nucleus forms.==

{{mermaid
graph TD
  A["Z and A notation (Ch. 2):<br/>balance nuclear equations"] --> B["Nuclear stability and binding energy:<br/>mass defect, E=mc^2"]
  B --> C["Radioactive decay:<br/>types plus first-order kinetics (Ch. 13)"]
  B --> D["Fission and fusion:<br/>move toward higher binding energy per nucleon"]
}}

**Visual description:** atomic notation (Z, A) lets you balance nuclear equations. Binding energy, from mass defect, quantifies nuclear stability. That same stability concept explains both why radioactive decay happens and why fission/fusion release energy — while decay's timing reuses Chapter 13's first-order kinetics unchanged.

## 19.1 The Nature of Nuclear Reactions{{attrs[#blk-ch19sec01]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 19.1a}} Distinguish radioactive decay from nuclear transmutation.
- {{sp[info] Objective 19.1a}} Balance a nuclear equation by conserving mass number and charge.
- {{sp[info] Objective 19.1b}} Identify patterns of nuclear stability.
- {{sp[info] Objective 19.1c}} Calculate nuclear binding energy from mass defect.
:::

### Nuclear reactions are not chemical reactions

An atom is written $\ce{^{A}_{Z}X}$, where $Z$ (atomic number) counts protons and $A$ (mass number) counts protons plus neutrons. **Radioactive decay** is spontaneous; **nuclear transmutation** results from bombarding a nucleus with particles.

**The difference from every previous chapter is not a matter of degree.** Chemical reactions rearrange electrons and leave nuclei untouched, so elements are conserved and each atom's identity survives. Nuclear reactions change the nucleus itself, so **one element can become another** — and the conservation rules change accordingly:

| | Chemical reaction | Nuclear reaction |
|---|---|---|
| What changes | electron arrangement | the nucleus |
| Elements | conserved | **transmuted** |
| Conserved quantities | atoms of each element | **mass number $A$ and charge $Z$** |
| Isotopes | behave nearly identically | behave **completely** differently |
| Energy scale | ~$10^{2}$ kJ/mol | ~$10^{8}$ kJ/mol |
| Affected by T, P, catalysts | yes | **no** |

The last row is worth pausing on: nothing you learned in Chapters 13–18 about speeding a reaction up applies here. A radioactive nucleus decays at its own rate regardless of temperature, pressure, chemical state, or what it is bonded to.

### Balancing nuclear equations

Balance by conserving exactly two things: **mass number $A$** (the superscripts) and **charge $Z$** (the subscripts). ==Atom identity is *not* conserved — that is precisely what makes it a nuclear reaction.==

:::: tabs
::: tab Problem
$\ce{^{125}_{53}I}$ captures an electron, producing one new nucleus. Write the equation.
:::
::: tab Solution
Mass number: $125+0=125$. Charge: $53+(-1)=52$ (element 52 = Te):

$$\ce{^{125}_{53}I + ^0_{-1}e -> ^{125}_{52}Te}$$
:::
::::

:::: tabs
::: tab Problem
An $\alpha$ particle strikes $\ce{^{25}_{12}Mg}$, producing a proton and a new nuclide. Identify it.
:::
::: tab Solution
Mass: $25+4=1+A \Rightarrow A=28$. Charge: $12+2=1+Z \Rightarrow Z=13$ (Al):

$$\ce{^{25}_{12}Mg + ^4_2He -> ^1_1H + ^{28}_{13}Al}$$
:::
::::

### Patterns of nuclear stability

{{sp[warning] Remember these three}} certain "magic numbers" of protons/neutrons (2, 8, 20, 28, 50, 82 for protons; 2, 8, 20, 28, 50, 82, 126 for neutrons) confer extra stability; even-even nuclei (both proton and neutron counts even) are generally more stable than odd-odd; and **every** isotope with $Z>83$ is radioactive.

![The band of stability: neutron number vs. proton number for representative stable nuclides](../assets/band_of_stability.svg)
*Figure 19.1 — Light stable nuclides sit close to N=Z, but the band curves upward as Z increases — heavier stable nuclei need proportionally more neutrons to remain stable, since more protons means more electrostatic repulsion for the strong nuclear force to overcome. Self-generated with matplotlib using real Z/N values.*

:::: tabs
::: tab Problem
Predict whether each nuclide is likely stable or radioactive, and give your reason: (a) $\ce{^{16}_{8}O}$; (b) $\ce{^{226}_{88}Ra}$; \(c) $\ce{^{208}_{82}Pb}$; (d) $\ce{^{43}_{20}Ca}$ versus $\ce{^{40}_{20}Ca}$.
:::
::: tab Solution
Work down the three rules in order: $Z > 83$ first, then magic numbers, then even/odd.

**(a) $\ce{^{16}_{8}O}$ — stable, on three counts.** $Z = 8$ is a magic number, $N = 8$ is a magic number, and both counts are even. It is doubly magic and even-even, which is about as stable as a nuclide gets.

**(b) $\ce{^{226}_{88}Ra}$ — radioactive, guaranteed.** $Z = 88 > 83$, and **every** isotope of every element above bismuth is radioactive without exception. No further reasoning is needed.

**\(c) $\ce{^{208}_{82}Pb}$ — stable, and remarkably so.** $Z = 82$ and $N = 126$ are both magic numbers, and both are even. It is the heaviest stable nuclide known — and note how close it sits to the $Z > 83$ cliff. Radium in (b) is only six protons heavier.

**(d) $\ce{^{40}_{20}Ca}$ is stable; $\ce{^{43}_{20}Ca}$ is much less favored.** Calcium-40 has $Z = 20$ (magic) and $N = 20$ (magic), even-even — doubly magic again. Calcium-43 has $N = 23$: odd, not magic, and paired with an even $Z$. It is in fact stable but far rarer in nature, at 0.14% abundance against calcium-40's 97%.

**The pattern across all four.** Nuclear stability is overwhelmingly a *counting* phenomenon — like electron shells, but for protons and neutrons separately. The magic numbers 2, 8, 20, 28, 50, 82 (and 126 for neutrons) are closed nuclear shells, and 8 and 20 appear twice in this problem alone.
:::
::::

:::: tabs
::: tab Problem
$\ce{^{14}_{6}C}$ has $N/Z = 8/6 = 1.33$ and is radioactive; $\ce{^{12}_{6}C}$ has $N/Z = 6/6 = 1.00$ and is stable. But $\ce{^{208}_{82}Pb}$ has $N/Z = 126/82 = 1.54$ and *is* stable. Explain, using Figure 19.1.
:::
::: tab Solution
**There is no single "correct" $N/Z$ ratio — the stable value rises with $Z$.** That rise is exactly the upward curve of the band of stability.

**Why it rises.** Two forces compete inside a nucleus. The **strong nuclear force** binds any pair of nucleons but acts only over about a nucleon's diameter, so each nucleon is bound mainly to its immediate neighbors. **Electrostatic repulsion** acts only between protons but reaches across the entire nucleus.

As $Z$ grows, every proton repels every other proton — an effect growing roughly as $Z^2$ — while the attractive binding grows only in proportion to the number of nucleons. **Extra neutrons supply attraction without adding any repulsion**, so heavy nuclei need proportionally more of them to hold together.

**Applying this to the three cases:**

- $\ce{^{12}C}$ at $N/Z = 1.00$ sits on the band, where light nuclides belong.
- $\ce{^{14}C}$ at 1.33 sits **above** it — neutron-rich for its size, so it $\beta^-$ decays, converting a neutron to a proton and moving down toward the band.
- $\ce{^{208}Pb}$ at 1.54 sits **on** the band, because at $Z = 82$ the band has curved up to meet it.

**The rule this yields:** never ask whether $N/Z$ is large; ask whether it is large **for that element**. Position relative to the band, not the absolute ratio, determines both stability and the decay mode — which is §19.2's subject.
:::
::::

### Binding energy and the mass defect


**Nuclear binding energy** is the energy equivalent (via $E=mc^2$) of the **mass defect** — the "missing mass" between a nucleus and its separate, unbound protons and neutrons:

$$\Delta m = (\text{actual atomic mass}) - (\text{mass of separate protons + neutrons + electrons}) \qquad \Delta E=(\Delta m)c^2$$

Written this way, $\Delta m$ comes out negative (the nucleus weighs less than its parts), and so does $\Delta E$.

**A negative $\Delta E$ means energy is released when the nucleus forms from its parts — the more negative (larger in magnitude) the binding energy per nucleon, the more stable the nucleus.**

:::warning
**Sign conventions differ between textbooks, and both are defensible.** Written as $\Delta E = (\Delta m)c^2$ with $\Delta m$ = (actual mass) − (separate parts), the mass defect is negative and so is $\Delta E$ — energy *released* on assembly. Many texts instead define binding energy as a positive quantity: the energy you must *supply* to pull the nucleus apart. The two differ only in sign and describe the same physics. **Say which convention you are using, and compare magnitudes rather than signed values.**
:::

:::: tabs
::: tab Problem
Calculate the binding energy of $\ce{^56_26Fe}$ (atomic mass 55.9349 amu) in (a) J/nucleus, (b) J/mol, \(c) MeV/nucleus, (d) MeV/nucleon.
:::
::: tab Solution
**(a)** $\Delta m = 55.9349-(26\times1.0073+30\times1.0087+26\times0.00055) = 55.9349-56.4651=-0.5302$ amu

$$\Delta E=(-0.5302\ \text{amu})(1.6605\times10^{-27}\ \text{kg/amu})(2.998\times10^8\ \text{m/s})^2=-7.913\times10^{-11}\ \text{J}$$

**(b)** $\Delta E=(-7.913\times10^{-11})(6.02\times10^{23})=-4.76\times10^{13}\ \text{J/mol}$

**\(c)** $\Delta E=(-7.913\times10^{-11}\ \text{J})/(1.602\times10^{-13}\ \text{J/MeV})=-494\ \text{MeV}$

**(d)** $-494/56=-8.82\ \text{MeV/nucleon}$

{{sp[warning] Why atomic masses work}} The tabulated 55.9349 amu is the *atomic* mass, including 26 electrons — so 26 electron masses are added on the other side too, and they cancel. Using the nuclear mass on one side and the atomic mass on the other is the standard error, and it shifts the answer by about 0.014 amu, or 13 MeV.
:::
::::

:::: tabs
::: tab Problem
Calculate the binding energy of $\ce{^{19}_{9}F}$ (atomic mass 18.9984 amu) in MeV per nucleon, and compare it with $\ce{^{56}_{26}Fe}$'s $-8.82$ MeV/nucleon.
:::
::: tab Solution
**Mass defect.** Fluorine-19 has 9 protons, 10 neutrons and 9 electrons:

$$9(1.0073) + 10(1.0087) + 9(0.00055) = 9.0657 + 10.087 + 0.00495 = 19.1577\ \text{amu}$$
$$\Delta m = 18.9984 - 19.1577 = -0.15925\ \text{amu}$$

**Energy.**

$$\Delta E = (-0.15925)(1.6605\times10^{-27}\ \text{kg/amu})(2.998\times10^{8}\ \text{m/s})^2 = -2.377\times10^{-11}\ \text{J}$$

$$= \frac{-2.377\times10^{-11}}{1.602\times10^{-13}} = -148.4\ \text{MeV per nucleus}$$

**Per nucleon**, dividing by 19:

$$\frac{-148.4}{19} = -7.81\ \text{MeV/nucleon}$$

**Comparison: iron wins.** At $-8.82$ MeV/nucleon, $\ce{^{56}Fe}$ is bound more tightly per particle than $\ce{^{19}F}$'s $-7.81$ — so **iron-56 is the more stable nucleus**, a conclusion that rests on the per-nucleon values, not on fluorine's total binding energy being far smaller.

**Total versus per-nucleon is the distinction that matters.** Iron's total binding energy (494 MeV) is more than three times fluorine's (148 MeV), but that is mostly because iron has three times as many nucleons. **Only the per-nucleon figure compares stability across different nuclei** — and its maximum near iron-56 is why §19.3's fission and fusion both release energy.

**Also worth noticing:** the mass defect is under 1% of the atomic mass in both cases, yet it corresponds to hundreds of MeV. A chemical bond is worth a few eV. That factor of roughly a hundred million is the whole difference between chemistry and nuclear physics.
:::
::::

**Self-check:**
- Why does the binding-energy calculation use the *atomic* mass (including electrons) rather than the nuclear mass?
- Why can total binding energy not be used to compare the stability of two different nuclides?

> **Where this goes next.** §19.1 explains which nuclei are unstable and why. §19.2 asks the next two questions: *how* an unstable nucleus fixes itself, and *when* — the second of which needs no new mathematics at all.

## 19.2 Radioactive Decay{{attrs[#blk-ch19sec02]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 19.2a}} Identify types of radioactive decay and write their equations.
- {{sp[info] Objective 19.2b}} Explain radiocarbon dating.
- {{sp[info] Objective 19.2c}} Apply first-order kinetics to radioactive decay problems.
:::

### The five decay modes

| Decay type | Emission | Example |
|---|---|---|
| Alpha ($\alpha$) | $\ce{^4_2He}$ nucleus | $\ce{^212_84Po -> ^4_2He + ^208_82Pb}$ |
| Beta ($\beta$) | electron ($\ce{^0_{-1}e}$) | $\ce{^14_6C -> ^14_7N + ^0_{-1}\beta}$ |
| Positron | positron ($\ce{^0_{+1}e}$) | $\ce{^11_6C -> ^11_5B + ^0_{+1}\beta}$ |
| Electron capture | (captures an electron) | $\ce{^37_18Ar + ^0_{-1}e -> ^37_17Cl}$ |
| Spontaneous fission | splits into two nuclei + neutrons | $\ce{^252_98Cf -> 2\,^125_49In + 2\,^1_0n}$ |

### Which mode, and why

![Two panels: how each decay mode moves a nuclide on the neutron-proton chart, and which mode a nuclide chooses based on where it sits relative to the band of stability](../assets/decay_modes_nz.svg)
*Figure 19.2 — Panel (a): each mode is a specific move in $(Z, N)$ space. Panel (b): a nuclide's position relative to the band decides which move it makes. Self-generated with matplotlib.*

A nucleus does not choose its decay mode at random. ==It decays in whichever way moves it toward the band of stability — so counting neutrons against protons predicts the likely kind of decay before you know anything else about the nuclide.==

- **Above the band** (too many neutrons) → **$\beta^-$ decay**. A neutron becomes a proton plus an emitted electron: $Z$ rises by one, $N$ falls by one, $A$ is unchanged.
- **Below the band** (too many protons) → **positron emission** or **electron capture**. Both convert a proton into a neutron, moving $Z$ down and $N$ up. Electron capture tends to dominate for heavier nuclides, positron emission for lighter ones.
- **Beyond the band entirely** ($Z > 83$) → **$\alpha$ decay**, which is the only mode that reduces $A$ appreciably. Shedding two protons and two neutrons at a time is how a nucleus that is simply too large gets smaller.

{{sp[warning] $\beta^-$ and $\beta^+$ are opposites, not the same thing}} $\beta^-$ emits an **electron** and *increases* $Z$; $\beta^+$ emits a **positron** and *decreases* $Z$. They move a nuclide in opposite directions on Figure 19.2(a), and they are used by nuclides on opposite sides of the band. Reading "beta decay" without the sign is ambiguous.

:::: tabs
::: tab Problem
Predict the likely decay mode and write the equation for: (a) $\ce{^{3}_{1}H}$ ($N/Z = 2$); (b) $\ce{^{22}_{11}Na}$ ($N/Z = 1.0$, but stable Na is $\ce{^{23}Na}$); \(c) $\ce{^{238}_{92}U}$; (d) $\ce{^{40}_{19}K}$, which can do two different things.
:::
::: tab Solution
For each, decide which side of the band the nuclide sits on, then read the mode off Figure 19.2(b).

**(a) $\ce{^{3}_{1}H}$ — neutron-rich, so $\beta^-$.** Two neutrons to one proton is far above the band for such a light nuclide, where stability needs $N \approx Z$.
$$\ce{^{3}_{1}H -> ^{3}_{2}He + ^{0}_{-1}\beta}$$

**(b) $\ce{^{22}_{11}Na}$ — proton-rich, so $\beta^+$ or electron capture.** Stable sodium is mass 23, so mass 22 is one neutron short.
$$\ce{^{22}_{11}Na -> ^{22}_{10}Ne + ^{0}_{+1}\beta}$$

**\(c) $\ce{^{238}_{92}U}$ — $\alpha$ decay.** $Z = 92 > 83$, so it is simply too big; alpha emission is the only mode that meaningfully reduces $A$.
$$\ce{^{238}_{92}U -> ^{234}_{90}Th + ^{4}_{2}He}$$

**(d) $\ce{^{40}_{19}K}$ — it does both, and that is why it is interesting.** With $Z = 19$ and $N = 21$, *both* counts are odd, which is the least favorable combination. It sits close enough to the band that either correction works: about 89% $\beta^-$ decay to $\ce{^{40}Ca}$, about 11% electron capture to $\ce{^{40}Ar}$.
$$\ce{^{40}_{19}K -> ^{40}_{20}Ca + ^{0}_{-1}\beta} \qquad \ce{^{40}_{19}K + ^{0}_{-1}e -> ^{40}_{18}Ar}$$

**The branch in (d) has a consequence you can look up.** Argon is nearly 1% of the atmosphere — far more than its cosmic abundance would suggest — because essentially all of it is $\ce{^{40}Ar}$ produced by potassium-40 decaying in rocks over billions of years. The same decay underlies potassium–argon dating, which is widely used to date volcanic rocks from thousands to billions of years old.
:::
::::

:::: tabs
::: tab Problem
Complete each nuclear equation by identifying the missing particle: (a) $\ce{^{27}_{13}Al + ^{4}_{2}He -> ^{30}_{15}P + \;?}$; (b) $\ce{^{235}_{92}U -> ^{231}_{90}Th + \;?}$; \(c) $\ce{^{59}_{27}Co + ^{1}_{0}n -> \;? + ^{0}_{-1}\beta}$.
:::
::: tab Solution
Conserve $A$ (superscripts) and $Z$ (subscripts) — nothing else is needed.

**(a)** $A$: $27 + 4 = 31$, and $30$ is accounted for, so the particle has $A = 1$. $Z$: $13 + 2 = 15$, all accounted for, so $Z = 0$. **A neutron, $\ce{^{1}_{0}n}$.**
$$\ce{^{27}_{13}Al + ^{4}_{2}He -> ^{30}_{15}P + ^{1}_{0}n}$$
(This is the 1934 Joliot-Curie experiment — the first artificially produced radioactive nuclide.)

**(b)** $A$: $235 - 231 = 4$. $Z$: $92 - 90 = 2$. **An alpha particle**, as expected for $Z > 83$.
$$\ce{^{235}_{92}U -> ^{231}_{90}Th + ^{4}_{2}He}$$

**\(c)** $A$: $59 + 1 = 60$, and the beta particle carries $A = 0$, so the nuclide has $A = 60$. $Z$: $27 + 0 = 27$, and the beta carries $Z = -1$, so the nuclide has $Z = 28$ — nickel.
$$\ce{^{59}_{27}Co + ^{1}_{0}n -> ^{60}_{28}Ni + ^{0}_{-1}\beta}$$

**The method never varies.** Sum the superscripts on each side and solve; sum the subscripts and solve; then look up the element from $Z$. **Charge conservation is what identifies the element** — which is worth stating plainly, because in every previous chapter the element was given and the charge was the unknown.
:::
::::

### Kinetics of decay, and radiocarbon dating

**Radioactive decay is always a first-order process** — so Chapter 13's exact tools apply, unchanged: $\ln(N_0/N)=kt$ and $t_{1/2}=\ln2/k$, with $N$ (amount or activity of the radioactive isotope) simply replacing concentration.


**Radiocarbon dating** uses $\ce{^14C}$ (half-life 5730 y), continuously formed in the atmosphere and taken up by living things; once an organism dies, its $\ce{^14C}$ only decreases, giving a clock.

![Radiocarbon decay curve with the Dead Sea Scrolls data point marked](../assets/carbon14_decay.svg)
*Figure 19.3 — The fraction of original $\ce{^14C}$ remaining follows the same first-order exponential decay as any Chapter 13 kinetics problem — just with a very long half-life. Self-generated with matplotlib using the real C-14 half-life and the worked example's data.*

:::: tabs
::: tab Problem
A Dead Sea Scrolls sample has activity 10.8 disintegrations/min/g; fresh material has 13.6. Estimate its age. ($t_{1/2}=5730$ y)
:::
::: tab Solution
$$k=\frac{\ln2}{5730\ \text{y}}=1.210\times10^{-4}\ \text{y}^{-1}$$

$$t=\frac{\ln(c_0/c)}{k}=\frac{\ln(13.6/10.8)}{1.210\times10^{-4}\ \text{y}^{-1}}=1.91\times10^3\ \text{y}$$

About 1900 years old.

**A cross-check that costs nothing.** 1900 years is about a third of one half-life, so the activity should have fallen by rather less than half — from 13.6 to somewhere well above 6.8. It fell to 10.8 ✓. **Estimate the number of half-lives before trusting any decay calculation**; it catches order-of-magnitude errors instantly.

{{sp[warning] Activity is proportional to amount}} The problem gives disintegrations per minute, not concentrations — but activity is directly proportional to the number of radioactive nuclei present, so the ratio $13.6/10.8$ can be used exactly where $c_0/c$ would go. Any quantity proportional to the amount will do: mass, counts, or percentage remaining.
:::
::::

:::: tabs
::: tab Problem
Strontium-90, a fission product, has a half-life of 28.8 years. (a) What fraction of an initial sample remains after 100 years? (b) How long until only 1.0% remains? \(c) Why is $\ce{^{90}Sr}$ considered particularly hazardous compared with isotopes of similar half-life?
:::
::: tab Solution
**Find $k$ first** — everything else follows from it:

$$k = \frac{\ln 2}{t_{1/2}} = \frac{0.693}{28.8\ \text{y}} = 2.41\times10^{-2}\ \text{y}^{-1}$$

**(a)** Use $\ln(N_0/N) = kt$, rearranged as $N/N_0 = e^{-kt}$:

$$\frac{N}{N_0} = e^{-(2.41\times10^{-2})(100)} = e^{-2.41} = 0.090 = \textbf{9.0\%}$$

**Sanity check:** 100 years is $100/28.8 = 3.5$ half-lives, so expect between $1/8$ (12.5%) and $1/16$ (6.25%) ✓

**(b)** Solve for $t$ with $N/N_0 = 0.010$:

$$t = \frac{\ln(1/0.010)}{k} = \frac{\ln 100}{2.41\times10^{-2}} = \frac{4.605}{2.41\times10^{-2}} = 191\ \text{y}$$

Roughly **two centuries**, or about 6.6 half-lives.

**\(c) Because of chemistry, not nuclear physics.** Strontium sits directly below calcium in Group 2A, so the body handles $\ce{Sr^2+}$ much as it handles $\ce{Ca^2+}$ — and deposits it in **bone**, next to the marrow that produces blood cells. A half-life of 28.8 years is long enough to persist for a lifetime and short enough to be intensely radioactive throughout.

**The general lesson, and a fitting one for the last chapter.** Nuclear properties determine *how much* radiation a nuclide emits; **its position in the periodic table determines where in the body it ends up**. Iodine-131 concentrates in the thyroid for the same reason, which is why potassium iodide tablets are stockpiled near reactors — Chapter 8's periodic trends, applied to a nuclear problem.
:::
::::

:::: tabs
::: tab Problem
(a) Why can radiocarbon dating not be used on a 200,000-year-old fossil? (b) Why can it not be used on a diamond, or on a seashell taken from limestone bedrock? \(c) Why does it work on wood, bone and cloth?
:::
::: tab Solution
**(a) The clock runs out.** With $t_{1/2} = 5730$ y, 200,000 years is about 35 half-lives:
$$\frac{N}{N_0} = \left(\tfrac{1}{2}\right)^{35} = 2.9\times10^{-11}$$
Essentially no $\ce{^{14}C}$ remains, and what little does is swamped by background counts. **The practical limit is around 50,000 years**, roughly nine half-lives, where about 0.2% remains — still measurable, barely.

**(b) The clock never started, or started too long ago.** The method assumes the sample **exchanged carbon with the atmosphere while alive** and then stopped at death. A diamond's carbon has been isolated for billions of years, so its $\ce{^{14}C}$ is long gone regardless of when the diamond was mined. A shell taken from limestone bedrock is itself millions of years old, as old as the rock it is in, so its $\ce{^{14}C}$ has long since decayed. (Even living shells can date too old if they took up dissolved carbonate from ancient limestone; this is the "reservoir effect".)

**\(c) Because they were once alive and stopped exchanging at a known moment.** Wood, bone, cloth (from flax or cotton), leather, charcoal — all built their carbon from the atmosphere via photosynthesis, directly or through a food chain, and all stopped at death or harvest.

**Every dating method has the same three requirements**, and this example checks all three: a **known starting value** (atmospheric $\ce{^{14}C}$), a **clean start** (the moment exchange stopped), and a **half-life comparable to the age** being measured. Potassium–argon dating, with $t_{1/2} = 1.25$ billion years, is used on rocks for exactly the reason carbon-14 cannot be.
:::
::::

:::: tabs
::: tab Problem
Iodine-131 ($t_{1/2} = 8.02$ days) is used to treat thyroid conditions. A patient receives a dose. (a) What fraction remains after 32 days? (b) Hospitals often quote "ten half-lives" as the point at which a radioisotope is effectively gone — what fraction is that? \(c) Contrast with $\ce{^{90}Sr}$'s 28.8-year half-life: which is more intensely radioactive per atom, and which is the greater long-term hazard?
:::
::: tab Solution
**(a)** 32 days is $32/8.02 = 3.99 \approx 4$ half-lives:
$$\frac{N}{N_0} = \left(\tfrac{1}{2}\right)^{4} = \frac{1}{16} = 6.3\%$$

**(b)** Ten half-lives leaves $(1/2)^{10} = 1/1024 \approx 0.1\%$ — a thousandfold reduction, and the usual working definition of "decayed away".

**\(c) They trade off against each other, and the trade is exact.**

**Iodine-131 is far more intensely radioactive per atom.** From $k = \ln 2 / t_{1/2}$, a *shorter* half-life means a *larger* decay constant and therefore more disintegrations per second from the same number of atoms. I-131's half-life is about 1,300 times shorter than Sr-90's, so mole for mole it is about 1,300 times more active.

**Strontium-90 is the greater long-term hazard**, for the same reason inverted. I-131 is effectively gone in a few months; Sr-90 persists for centuries, and Group 2A chemistry lodges it in bone the whole time.

**The general principle worth ending on.** **Short half-life means intense but brief; long half-life means weak but persistent.** Neither is simply "worse" — which hazard matters depends on whether you are worried about the next month or the next century. A nuclide with a half-life of billions of years, like $\ce{^{238}U}$, is barely radioactive at all.
:::
::::

**Self-check:**
- Why is $\ce{^{11}_{6}C}$'s decay a *positron* decay rather than a beta (electron) decay, based on its position relative to the band of stability?
- If a sample's activity has dropped to exactly 1/4 of its original value, how many half-lives have elapsed?

> **Where this goes next.** §19.2 covered nuclei that rearrange themselves a little. §19.3 covers the two processes that rearrange them enormously — and shows that both release energy for the *same* reason, visible as a single curve.

## 19.3 Nuclear Fission and Nuclear Fusion{{attrs[#blk-ch19sec03]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 19.3a}} Define nuclear fission, chain reaction, and critical mass.
- {{sp[info] Objective 19.3b}} Define nuclear fusion and its temperature requirement.
- Give examples of each.
- {{sp[info] Objective 19.3c}} Explain why both fission and fusion release energy, using binding energy per nucleon.
:::

### Fission and the chain reaction

**Nuclear fission** splits a heavy nucleus ($A>200$) into smaller nuclei plus neutrons:

$$\ce{^235_92U + ^1_0n -> ^90_38Sr + ^143_54Xe + 3\,^1_0n}$$

One neutron is captured; three are released, each capable of triggering further fission — a **chain reaction**.

![The branching structure of a fission chain reaction, and the difference between a subcritical and a critical sample](../assets/fission_chain_reaction.svg)
*Figure 19.4 — Left: with every neutron captured, the number of fissions goes 1, 3, 9, 27 — $3^n$ after $n$ generations. Right: whether that happens at all depends on whether neutrons are captured before they reach the surface and escape. Self-generated with matplotlib.*

==Whether a chain reaction sustains itself is, for a given fissile material, a question of geometry, not of chemistry: the **critical mass** is simply the size at which enough neutrons are captured, rather than escaping, to keep the chain going.== A neutron born near the center of a large sample has far more nuclei to hit before reaching the surface than one born in a small sample. Below that size (**subcritical**), too many neutrons escape and the chain fizzles out.

**This is why critical mass is a condition rather than a constant.** Compress the same amount of material into a smaller volume and it can become critical; surround it with a neutron-reflecting shell and the critical mass falls further; dilute the fissile isotope and it rises. The number quoted for any material always assumes a particular shape and purity.


An **atomic bomb** merges two subcritical U-235 pieces past critical mass, causing an explosive chain reaction; a **nuclear reactor** keeps several subcritical pieces together, using neutron-absorbing control rods to hold the assembly at exactly critical,, avoiding an explosion.

Figure 19.5 shows what $k = 1$ looks like from outside.

![Cooling towers of a nuclear power plant, with visible steam](../assets/nuclear_power_plant.jpg =700x)
*Figure 19.5 — A nuclear reactor uses controlled fission (not an explosive chain reaction) to generate heat; the plume visible rising from these cooling towers is condensed water droplets (water vapor from the cooling water that has recondensed in the cooler air) that carries away waste heat. Source: Roberto Uderio (retouched by AlMare), via Wikimedia Commons, CC BY-SA 3.0.*

:::: tabs
::: tab Problem
For $\ce{^{235}_{92}U + ^{1}_{0}n -> ^{90}_{38}Sr + ^{143}_{54}Xe + 3^{1}_{0}n}$: (a) verify that $A$ and $Z$ balance. (b) Why is a chain reaction possible here but not for an ordinary chemical reaction? \(c) In a reactor, what must be true of the average number of neutrons that go on to cause further fission?
:::
::: tab Solution
**(a)** Mass numbers: $235 + 1 = 236$ on the left; $90 + 143 + 3(1) = 236$ on the right ✓
Charges: $92 + 0 = 92$ on the left; $38 + 54 + 3(0) = 92$ on the right ✓

**(b) Because the reaction produces more of its own trigger than it consumes.** One neutron in, three out — so each fission can initiate up to three more. A combustion reaction consumes a spark and does not emit sparks; fission consumes a neutron and emits three. **Self-amplification is the whole difference**, and Figure 19.4 shows the consequence: 1, 3, 9, 27, growing as $3^n$.

**\(c) Exactly one, on average.** Define $k$ as the mean number of neutrons from each fission that cause another fission:

- $k < 1$ — **subcritical**; the reaction dies out.
- $k = 1$ — **critical**; a steady, self-sustaining rate. **This is what a power reactor maintains.**
- $k > 1$ — **supercritical**; exponential growth, which, if large and uncontrolled, is a bomb.

Control rods made of neutron-absorbing material (boron or cadmium) are pushed in or withdrawn to hold $k$ at 1.000. **A reactor is not a slow bomb; it is a chain reaction deliberately pinned at the break-even point.**

Note that two of the three neutrons must be absorbed or allowed to escape for $k = 1$ — the control system's job is to waste them accurately.
:::
::::

:::: tabs
::: tab Problem
Natural uranium is 99.3% $\ce{^{238}U}$ and only 0.7% $\ce{^{235}U}$, and only $\ce{^{235}U}$ fissions readily with slow neutrons. (a) Why can natural uranium not sustain a chain reaction on its own? (b) What are the two ways of fixing this? \(c) Why does this make nuclear weapons hard to build?
:::
::: tab Solution
**(a) Too few of the neutrons find a $\ce{^{235}U}$ nucleus.** With 140 atoms of $\ce{^{238}U}$ for every one of $\ce{^{235}U}$, most neutrons are either absorbed by $\ce{^{238}U}$ without causing fission, or escape. The effective $k$ falls below 1 and the chain dies.

**(b) Two routes, and they define the two branches of the industry.**

**Enrichment** — raise the $\ce{^{235}U}$ fraction. Reactor fuel is typically enriched to 3–5%. Because the two isotopes are chemically *identical* (Chapter 2 — isotopes differ only in neutron count), no chemical method can separate them; it has to be done physically, by passing $\ce{UF6}$ gas through cascades of thousands of centrifuges to exploit a 1% mass difference.

**Moderation** — slow the neutrons down. Fission neutrons are born fast, and $\ce{^{235}U}$ captures *slow* neutrons far more readily. A **moderator** (water, heavy water, or graphite) slows them through collisions, raising the capture probability enough that even natural uranium can go critical with a good enough moderator.

**\(c) Because the hard part is isotope separation, not chemistry.** Weapons need enrichment above about 90%, and the only barrier between a reactor program and a weapons program is how many times the centrifuges run. **This is why non-proliferation monitoring focuses on enrichment facilities** — the chemistry is public and straightforward; the physical separation is what is difficult and detectable.
:::
::::

### Fusion

**Nuclear fusion** combines light nuclei into heavier ones, releasing energy for the same binding-energy reason — but requires extremely high temperatures to overcome the mutual repulsion between positively charged nuclei:

$$\ce{^1_1H + ^2_1H -> ^3_2He} \qquad \ce{^3_2He + ^3_2He -> ^4_2He + 2\,^1_1H} \qquad \ce{^1_1H + ^1_1H -> ^2_1H + ^0_{+1}\beta}$$

These reactions power the **Sun**; a **hydrogen bomb** uses similar fusion reactions (e.g., $\ce{^6_3Li + ^2_1H -> 2\,^4_2He}$) at the extreme temperatures generated by a fission trigger.

Figure 19.6 is the only fusion reactor currently working at scale.

![The Sun, showing its glowing surface and solar prominences](../assets/the_sun.jpg =600x)
*Figure 19.6 — The Sun's energy comes from hydrogen fusing into helium at its core, at temperatures near 15 million K — and because Earth lacks the Sun's enormous gravitational pressure, reactors must heat plasma even hotter (around 100 million K) and keep it confined long enough for net energy gain, which is why controlled fusion power remains an active research challenge. Source: NASA/SDO (AIA), via Wikimedia Commons, public domain.*

:::: tabs
::: tab Problem
The deuterium–tritium reaction $\ce{^{2}_{1}H + ^{3}_{1}H -> ^{4}_{2}He + ^{1}_{0}n}$ releases 17.6 MeV. (a) Verify $A$ and $Z$ balance. (b) Compare the energy per nucleon with U-235 fission's ~200 MeV. \(c) Why is fusion harder to achieve than fission despite being more efficient?
:::
::: tab Solution
**(a)** $A$: $2 + 3 = 5$; $4 + 1 = 5$ ✓  $Z$: $1 + 1 = 2$; $2 + 0 = 2$ ✓

**(b) Per nucleon, fusion wins comfortably.**
$$\text{fusion: } \frac{17.6\ \text{MeV}}{5\ \text{nucleons}} = 3.5\ \text{MeV/nucleon} \qquad \text{fission: } \frac{200\ \text{MeV}}{235\ \text{nucleons}} = 0.85\ \text{MeV/nucleon}$$

Fission releases more energy *per event*, but fusion releases about **four times more per unit of fuel mass** — which is what actually matters for a fuel.

**\(c) Because fission needs a neutron and fusion needs to defeat electrostatic repulsion.**

A neutron is uncharged, so it can drift into a $\ce{^{235}U}$ nucleus with no barrier at all — fission needs no activation energy in any meaningful sense.

Fusion requires two **positively charged** nuclei to touch, which means overcoming Coulomb repulsion that rises steeply as they approach. In a laboratory, the kinetic energy needed corresponds to temperatures of around $10^{8}$ K, at which no material container can exist. The Sun, at about $1.5\times10^{7}$ K, makes up for the lower temperature with gravity; laboratories must use magnetic confinement or inertial compression, and holding the plasma stable long enough to break even is the unsolved engineering problem.

**The irony worth stating.** Fusion is cleaner (helium rather than long-lived fission products), the fuel is essentially unlimited (deuterium from seawater), and the yield per kilogram is higher. **It is harder only because the reactants repel each other** — a Chapter 8 fact about charge, standing between us and the better technology.
:::
::::

:::: tabs
::: tab Problem
The Sun's core is at about $1.5\times10^{7}$ K. (a) Why is such a temperature required for fusion, when fission needs no comparable heating? (b) The Sun fuses hydrogen at a rate that has kept it shining for 4.6 billion years — why is the *proton–proton* first step so slow? \(c) Why is a fission bomb used as the trigger for a hydrogen bomb?
:::
::: tab Solution
**(a) Because both nuclei are positively charged.** To fuse, two nuclei must approach within about $10^{-15}$ m, where the strong force can act — but Coulomb repulsion rises steeply all the way in. The kinetic energy needed to overcome it corresponds to temperatures of order $10^{7}$–$10^{8}$ K.

Fission needs nothing comparable because its trigger is a **neutron**, which carries no charge and feels no barrier at all. **The asymmetry is entirely about charge**, not about which process is more energetic.

**(b) Because the first step requires a proton to turn into a neutron as it happens.** In $\ce{^{1}_{1}H + ^{1}_{1}H -> ^{2}_{1}H + ^{0}_{+1}\beta}$, two protons must not only touch but simultaneously undergo a weak-force conversion — an extraordinarily improbable coincidence. An individual proton in the Sun's core waits on the order of a billion years for it.

**And that slowness is why the Sun still exists.** A star is a fusion reactor whose rate is throttled by the improbability of its own first step. If proton–proton fusion were fast, the Sun would have burned out long before life could arise on Earth.

**\(c) To supply the temperature.** No chemical explosive reaches $10^{7}$ K; a fission chain reaction does. The fission stage is a *match* for the fusion stage — which is why a fusion weapon cannot be built without first solving fission, and why fusion power research is difficult for exactly the reason weapons research was not: **a laboratory needs the temperature without the bomb.**
:::
::::

### Why both release energy

![Binding energy per nucleon vs. mass number, showing the Fe-56 peak](../assets/binding_energy_curve.svg)
*Figure 19.7 — Both fission and fusion release energy because they move nuclei toward the Fe-56 peak — the most stable configuration per nucleon. Heavy nuclei (like U-235) climb the curve by splitting apart; light nuclei (like H and He isotopes) climb it by combining. Self-generated with matplotlib; two data points (F-19, Fe-56) match this chapter's own binding-energy worked examples.*

:::: tabs
::: tab Problem
The Sun fuses hydrogen to helium; a supernova is needed to make elements heavier than iron. (a) Why does fusion in a star stop at iron? (b) What does this say about where the iron in your blood came from? \(c) Use Figure 19.7 to explain why both fission and fusion release energy despite being opposite processes.
:::
::: tab Solution
**\(c) first, since it answers the others.** Figure 19.7 plots binding energy per nucleon against mass number, and it **peaks at iron-56**. Any process that moves nuclei *toward* that peak releases energy:

- **Light nuclei climb by fusing.** Hydrogen (as deuterium, H-2) at ~1 MeV/nucleon combining toward helium at ~7 MeV/nucleon releases the difference.
- **Heavy nuclei climb by splitting.** Uranium at ~7.6 MeV/nucleon splitting into fragments near ~8.5 MeV/nucleon releases the difference.

**They are not opposite processes in the relevant sense — they are the same process, approaching the same maximum from opposite sides.**

**(a) Fusion stops at iron because iron *is* the peak.** Fusing iron into anything heavier moves *down* the curve, which **absorbs** energy rather than releasing it. A star fusing iron would be cooling itself, so it can no longer support against gravity — which is precisely what triggers the collapse of a supernova.

**(b) The iron in your hemoglobin was made in a supernova.** Elements up to iron were forged in ordinary stellar fusion; everything heavier was built by neutron capture, in aging stars and in explosive events such as supernovae, and much of the iron itself came from dying massive stars and was scattered into space by the explosion.

**A fitting place to end the course.** The curve in Figure 19.7 explains a nuclear reactor, a hydrogen bomb, why the Sun shines, why it will eventually stop, and the origin of every atom heavier than helium in your body. **One graph, and a single principle: systems move toward greater stability** — which is the same statement, in a different currency, as $\Delta G < 0$ from Chapter 17.
:::
::::

:::: tabs
::: tab Problem
Using Figure 19.7, decide whether each process releases or absorbs energy: (a) $\ce{^{4}He}$ (7.07 MeV/nucleon) fusing to $\ce{^{12}C}$ (7.68); (b) $\ce{^{56}Fe}$ (8.79) fusing to $\ce{^{88}Sr}$ (8.73); \(c) $\ce{^{238}U}$ (7.57) splitting into two fragments near $\ce{^{119}Pd}$ (8.50); (d) $\ce{^{12}C}$ (7.68) splitting into three $\ce{^{4}He}$ (7.07).
:::
::: tab Solution
One test settles all four: **does the binding energy per nucleon go up?** If it does, energy is released.

**(a) Releases.** 7.07 → 7.68 is uphill on the curve. This is helium burning in an aged star, and it is the source of essentially all the carbon in the universe.

**(b) Absorbs.** 8.79 → 8.73 goes *down* — past the iron peak, fusion costs energy. Roughly $88(8.73) - 88(8.79) = -5$ MeV must be supplied. This is why stellar fusion halts at iron, and why heavier elements need a supernova.

**\(c) Releases.** 7.57 → 8.50 is uphill:
$$238(8.50) - 238(7.57) = 238(0.93) \approx 220\ \text{MeV}$$
The right order of magnitude for a fission event, and the basis of every reactor.

**(d) Absorbs.** 7.68 → 7.07 is downhill; splitting carbon costs about $12(0.61) = 7$ MeV. **Fission of a light nucleus is not a source of energy** — only heavy nuclei are on the right-hand slope.

**The one-line rule this establishes.** **Energy is released whenever a process moves nuclei toward iron-56 — fusion from below, fission from above — and absorbed whenever it moves away.** "Fission releases energy" and "fusion releases energy" are both incomplete statements; the complete one is about direction along a single curve.

**Reading the curve as a map.** Everything to the left of iron is fuel for fusion; the heavy nuclei far to the right are fuel for fission; iron itself is ash for both. There is no process that extracts energy from iron-56 — which is why it accumulates at the center of dying stars, and why it is the most abundant heavy element in the Earth's core.
:::
::::

**Self-check:**
- Why does a star's fusion stop at iron rather than continuing to heavier elements?
- Why is critical mass described as a *condition* rather than a fixed universal number?

## Synthesis

==This closing chapter shows that nuclear stability — quantified by binding energy per nucleon — is the single idea explaining radioactive decay and both fission and fusion (while nuclear equations are balanced by conserving mass number and atomic number).== Decay happens because unstable nuclei move toward more stable configurations; fission and fusion both release energy for the identical reason (climbing toward the Fe-56 peak from opposite directions). And the chapter's kinetics — half-life, radiocarbon dating — needed no new mathematics at all: Chapter 13's first-order rate law, unchanged, closes out the course exactly as it began six chapters ago.

## Asset and License Record for This Chapter

| Asset | Source URL | License | Attribution |
|---|---|---|---|
| `assets/band_of_stability.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib using real Z/N values for a representative set of stable nuclides; released under this package's CC BY 4.0 license. |
| `assets/decay_modes_nz.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; released under this package's CC BY 4.0 license. |
| `assets/carbon14_decay.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib using the real C-14 half-life (5730 y) and the study guide's own Dead Sea Scrolls worked-example data; released under this package's CC BY 4.0 license. |
| `assets/fission_chain_reaction.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; released under this package's CC BY 4.0 license. |
| `assets/nuclear_power_plant.jpg` | https://commons.wikimedia.org/wiki/File:Cofrentes_nuclear_power_plant_cooling_towers_retouched.jpg | CC BY SA-3.0 | Roberto Uderio (retouched by AlMare), via Wikimedia Commons, CC BY-SA 3.0. Resized from the original for web use. |
| `assets/the_sun.jpg` | https://commons.wikimedia.org/wiki/File:The_Sun_by_the_Atmospheric_Imaging_Assembly_of_NASA's_Solar_Dynamics_Observatory_-_20100819.jpg | Public domain | NASA/SDO (AIA), via Wikimedia Commons (public domain, U.S. government work). Resized from the original for web use. |
| `assets/binding_energy_curve.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib using real binding-energy-per-nucleon values, two of which (F-19, Fe-56) match the study guide's own worked examples; released under this package's CC BY 4.0 license. |
