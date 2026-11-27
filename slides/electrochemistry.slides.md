{{nyml
kind: document
carrier: slides
uid: doc-zgjm3jgnxwim590d
title: Chapter 18: Redox Reactions and Electrochemistry
ratio: 16:9
theme: paper
}}

<!-- slide template=title -->
# Redox Reactions and Electrochemistry
## Electron transfer as electricity
**General Chemistry, Chapter 18**

<!-- slide 2col -->
## Chapter Learning Objectives
<!-- @left -->
- **Objective 18.1a** — Assign oxidation numbers
- **Objective 18.1b** — Balance redox equations using the half-reaction method
- **Objective 18.2a** — Define galvanic cells and write cell diagrams
- **Objective 18.3a** — Define standard reduction potential and the SHE
- **Objective 18.3b** — Identify cathode/anode and calculate standard cell potential
<!-- @right -->
- **Objective 18.4a** — Relate $\Delta G^\circ$, K, and $E^\circ$ for a redox reaction
- **Objective 18.4b** — Apply the Nernst equation
- **Objective 18.4c** — Calculate the potential of a concentration cell
- **Objective 18.5a** — Explain corrosion, electrolysis, and batteries

<!-- slide template=outline -->
## Roadmap
1. Redox reactions
2. Galvanic cells
3. Standard reduction potentials
4. Nernst equation
5. Applications

<!-- slide -->
## Chapter Logic
{{mermaid
graph TD
  A["Redox half-reactions:<br/>oxidation + reduction"] --> B["Galvanic cells:<br/>anode / cathode"]
  B --> C["Standard reduction<br/>potentials (E-naught)"]
  C --> D["Delta G-naught = -nFE-naught<br/>= -RT ln K"]
  D --> E["Nernst equation:<br/>non-standard conditions"]
  E --> F["Applications:<br/>corrosion, electrolysis, batteries"]
}}
**Visual description:** redox half-reactions combine into a galvanic cell; standard reduction potentials predict its voltage, which links to free energy and K; the Nernst equation extends to non-standard conditions; applications close the chapter.

<!-- slide main-side -->
## One electron, two half-reactions
<!-- @main -->
![One electron moving from sodium to fluorine, labeled as oxidation and reduction at once](../assets/redox_electron_transfer.svg =700x)
<!-- @side -->
The electron Na **loses** is exactly the electron F **gains**. One event, described twice.

**An agent is named for what it does to the OTHER species:**

- reducing agent = the one *oxidized*
- oxidizing agent = the one *reduced*

<!-- slide template=section -->
# 1. Redox Reactions

<!-- slide -->
## Oxidation and reduction, always paired
- **Oxidation:** loses electrons, oxidation number increases
- **Reduction:** gains electrons, oxidation number decreases
- Reducing agent donates $\ce{e-}$ (itself oxidized); oxidizing agent accepts $\ce{e-}$ (itself reduced)

<!-- slide -->
## Oxidation number rules
:::warning
1. Free element = 0. 2. Monatomic ion = its charge. 3. H=+1, O=−2 (usual). 4. Group IA=+1, IIA=+2, F=−1. 5. Sum = overall charge.
:::

<!-- slide -->
## Half-reaction method
1. Split into oxidation / reduction
2. Balance atoms (not O, H)
3. Balance O with $\ce{H2O}$, H with $\ce{H+}$
4. Balance charge with $\ce{e-}$
5. Equalize electrons, add half-reactions
6. Basic solution: add $\ce{OH-}$ to both sides (one per $\ce{H+}$), combine $\ce{H+ + OH- -> H2O}$, cancel excess $\ce{H2O}$

<!-- slide step -->
## Worked example — acidic & basic balancing
$\ce{H2O2 + Sn2+ -> H2O + Sn4+}$
- Acidic: $\ce{Sn2+ + 2H+ + H2O2 -> Sn4+ + 2H2O}${{attrs[.fragment]}}
- Basic: add $\ce{2OH-}$ both sides, combine $\ce{H+} + \ce{OH-}$→$\ce{H2O}${{attrs[.fragment]}}
- **$\ce{Sn2+ + H2O2 -> Sn4+ + 2OH-}$**{{attrs[.fragment]}}

<!-- slide template=section -->
# 2. Galvanic Cells

<!-- slide -->
## The Zn/Cu galvanic cell
![Galvanic cell](../assets/galvanic_cell_diagram.svg =620x)

<!-- slide -->
## Cell diagram notation
$$\ce{Zn(s)|Zn^2+}(1M)||\ce{Cu^2+}(1M)|\ce{Cu(s)}$$
Anode | anode solution || cathode solution | cathode

<!-- slide step -->
## Worked example — Mg/Fe cell
$\ce{Mg(s) + 2Fe3+(aq) -> Mg2+(aq) + 2Fe2+(aq)}$, Pt cathode
- Anode: $\ce{Mg -> Mg2+ + 2e-}${{attrs[.fragment]}}
- Cathode: $\ce{Fe3+ + e- -> Fe2+}${{attrs[.fragment]}}
- **Mg(s)|$\ce{Mg2+}$(0.1M)||$\ce{Fe3+}$(0.2M),$\ce{Fe2+}$(0.3M)|Pt(s)**{{attrs[.fragment]}}

<!-- slide template=section -->
# 3. Standard Reduction Potentials

<!-- slide -->
## $E^\circ$: referenced to the SHE (0 V)
![Reduction potential series](../assets/reduction_potential_series.svg =620x)

<!-- slide -->
## Which electrode is which?
:::warning
In a galvanic cell: Higher $E^\circ$ → CATHODE (reduction as written). Lower $E^\circ$ → ANODE (reverse it — oxidation). $E^\circ_\text{cell} = E^\circ_\text{cathode} - E^\circ_\text{anode}$.
:::

<!-- slide step -->
## Worked example — Cu/Ag cell
$\ce{Ag+} + \ce{e-}$→Ag ($E^\circ$=0.80V); $\ce{Cu2+} + \ce{2e-}$→Cu ($E^\circ$=0.34V)
- Ag = cathode, Cu = anode (reversed){{attrs[.fragment]}}
- $\ce{Cu(s) + 2Ag+(aq) -> Cu2+(aq) + 2Ag(s)}${{attrs[.fragment]}}
- **$E^\circ_\text{cell} = 0.80 - 0.34 = 0.46$ V**{{attrs[.fragment]}}

<!-- slide template=section -->
# 4. Nernst Equation

<!-- slide -->
## Three views, one reaction
$$\Delta G^\circ = -nFE^\circ = -RT\ln K$$
| $\Delta G^\circ$ | K | $E^\circ_\text{cell}$ |
|---|---|---|
| Negative | >1 | Positive |
| 0 | =1 | 0 |
| Positive | <1 | Negative |

<!-- slide step -->
## Worked example — $\Delta G^\circ$, K from $E^\circ$
$\ce{Sn2+} + \ce{2e-}$→Sn (−0.1375V); $\ce{Cu2+} + \ce{e-}$→$\ce{Cu+}$ (0.153V)
- $E^\circ_\text{cell} = 0.153-(-0.1375) = 0.2905$ V, $n = 2${{attrs[.fragment]}}
- $\Delta G^\circ = -2(96485)(0.2905) = -5.61\times10^{4}$ J/mol{{attrs[.fragment]}}
- **$K = 6.7\times10^{9}$ — spontaneous**{{attrs[.fragment]}}

<!-- slide -->
## Non-standard conditions: Nernst equation
$$E = E^\circ - \frac{RT}{nF}\ln Q$$

<!-- slide step -->
## Worked example — Al/Cu cell, Nernst
Al(s)|$\ce{Al3+}$(0.15M)||$\ce{Cu2+}$(0.025M)|Cu(s)
- $n = 6$, $Q = 0.15^2/0.025^3 = 1.4\times10^{3}${{attrs[.fragment]}}
- $E^\circ = 0.34-(-1.662) = 2.00$ V{{attrs[.fragment]}}
- **$E = 2.00$ − (RT/6F)ln($1.4\times10^{3}$) = 1.97 V**{{attrs[.fragment]}}

<!-- slide -->
## Concentration cells: $E^\circ = 0$
![Nernst concentration cell](../assets/nernst_concentration_cell.svg =600x)

<!-- slide step -->
## Worked example — Zn concentration cell
$[\ce{Zn2+}] = 0.10$ M and 0.50 M, $n = 2$
- Dilute side = anode; concentrated side = cathode{{attrs[.fragment]}}
- E = −(RT/2F)ln(0.10/0.50){{attrs[.fragment]}}
- **$E = 0.0207$ V**{{attrs[.fragment]}}

<!-- slide template=section -->
# 5. Applications

<!-- slide -->
## Corrosion: electrochemistry in the wild
![Rust](../assets/rust_corrosion.jpg =480x)
Iron oxidizes spontaneously; $\ce{O2}$ is the oxidizing agent — $\ce{O2}$ is reduced where it is plentiful (near the air/water edge), while iron is oxidized at anodic sites where $\ce{O2}$ is scarce.

<!-- slide -->
## Electrolysis: forcing the nonspontaneous
:::warning
Negative $E^\circ_\text{cell}$ does NOT mean "never happens" — external energy (electrolysis) can drive it. Electrolysis of water: reverse of $\ce{H2}$ combustion. Electrolysis of molten $\ce{NaCl}$: makes Na(l) and $\ce{Cl2(g)}$.
:::

<!-- slide main-side -->
## Galvanic vs electrolytic
<!-- @main -->
![Side-by-side galvanic and electrolytic cells with opposite energy conversion](../assets/galvanic_vs_electrolytic.svg =740x)
<!-- @side -->
Galvanic: $E^\circ_\text{cell} > 0$, chemical → electrical, **no supply needed**.

Electrolytic: $E^\circ_\text{cell} < 0$, electrical → chemical, **supply required**.

**Oxidation is at the anode in BOTH.** Only the sign painted on the electrode flips.

<!-- slide -->
## Batteries: engineered galvanic cells
![Batteries](../assets/batteries.jpg =480x)
Dry cell, mercury, lead storage, lithium-ion, fuel cell — all fundamentally galvanic cells.

<!-- slide template=closing -->
# Three views, one framework
$\Delta G^\circ$, K, and $E^\circ$ are three descriptions of the same reaction's favorability, unified by $\Delta G^\circ$ = −nFE° = −RT ln K. This is the course's synthesis: kinetics, equilibrium, thermodynamics, and electrochemistry are one connected story.
