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
- **Objective 18.4a** — Relate ΔG°, K, and E° for a redox reaction
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
- Reducing agent donates e⁻ (itself oxidized); oxidizing agent accepts e⁻ (itself reduced)

<!-- slide -->
## Oxidation number rules
:::warning
1. Free element = 0. 2. Monatomic ion = its charge. 3. H=+1, O=−2 (usual). 4. Group IA=+1, IIA=+2, F=−1. 5. Sum = overall charge.
:::

<!-- slide -->
## Half-reaction method
1. Split into oxidation / reduction
2. Balance atoms (not O, H)
3. Balance O with H₂O, H with H⁺
4. Balance charge with e⁻
5. Equalize electrons, add half-reactions
6. Basic solution: add OH⁻ to both sides (one per H⁺), combine H⁺ + OH⁻ → H₂O, cancel excess H₂O

<!-- slide step -->
## Worked example — acidic & basic balancing
H₂O₂ + Sn²⁺ → H₂O + Sn⁴⁺
- Acidic: Sn²⁺ + 2H⁺ + H₂O₂ → Sn⁴⁺ + 2H₂O{{attrs[.fragment]}}
- Basic: add 2 OH⁻ both sides, combine H⁺+OH⁻→H₂O{{attrs[.fragment]}}
- **Sn²⁺ + H₂O₂ → Sn⁴⁺ + 2OH⁻**{{attrs[.fragment]}}

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
Mg(s) + 2Fe³⁺(aq) → Mg²⁺(aq) + 2Fe²⁺(aq), Pt cathode
- Anode: Mg → Mg²⁺ + 2e⁻{{attrs[.fragment]}}
- Cathode: Fe³⁺ + e⁻ → Fe²⁺{{attrs[.fragment]}}
- **Mg(s)|Mg²⁺(0.1M)||Fe³⁺(0.2M),Fe²⁺(0.3M)|Pt(s)**{{attrs[.fragment]}}

<!-- slide template=section -->
# 3. Standard Reduction Potentials

<!-- slide -->
## E°: referenced to the SHE (0 V)
![Reduction potential series](../assets/reduction_potential_series.svg =620x)

<!-- slide -->
## Which electrode is which?
:::warning
In a galvanic cell: Higher E° → CATHODE (reduction as written). Lower E° → ANODE (reverse it — oxidation). E°cell = E°cathode − E°anode.
:::

<!-- slide step -->
## Worked example — Cu/Ag cell
Ag⁺+e⁻→Ag (E°=0.80V); Cu²⁺+2e⁻→Cu (E°=0.34V)
- Ag = cathode, Cu = anode (reversed){{attrs[.fragment]}}
- Cu(s) + 2Ag⁺(aq) → Cu²⁺(aq) + 2Ag(s){{attrs[.fragment]}}
- **E°cell = 0.80 − 0.34 = 0.46 V**{{attrs[.fragment]}}

<!-- slide template=section -->
# 4. Nernst Equation

<!-- slide -->
## Three views, one reaction
$$\Delta G^\circ = -nFE^\circ = -RT\ln K$$
| ΔG° | K | E°cell |
|---|---|---|
| Negative | >1 | Positive |
| 0 | =1 | 0 |
| Positive | <1 | Negative |

<!-- slide step -->
## Worked example — ΔG°, K from E°
Sn²⁺+2e⁻→Sn (−0.1375V); Cu²⁺+e⁻→Cu⁺ (0.153V)
- E°cell = 0.153−(−0.1375) = 0.2905 V, n=2{{attrs[.fragment]}}
- ΔG° = −2(96485)(0.2905) = −5.61×10⁴ J/mol{{attrs[.fragment]}}
- **K = 6.7×10⁹ — spontaneous**{{attrs[.fragment]}}

<!-- slide -->
## Non-standard conditions: Nernst equation
$$E = E^\circ - \frac{RT}{nF}\ln Q$$

<!-- slide step -->
## Worked example — Al/Cu cell, Nernst
Al(s)|Al³⁺(0.15M)||Cu²⁺(0.025M)|Cu(s)
- n=6, Q = 0.15²/0.025³ = 1.4×10³{{attrs[.fragment]}}
- E° = 0.34−(−1.662) = 2.00 V{{attrs[.fragment]}}
- **E = 2.00 − (RT/6F)ln(1.4×10³) = 1.97 V**{{attrs[.fragment]}}

<!-- slide -->
## Concentration cells: E° = 0
![Nernst concentration cell](../assets/nernst_concentration_cell.svg =600x)

<!-- slide step -->
## Worked example — Zn concentration cell
[Zn²⁺] = 0.10 M and 0.50 M, n=2
- Dilute side = anode; concentrated side = cathode{{attrs[.fragment]}}
- E = −(RT/2F)ln(0.10/0.50){{attrs[.fragment]}}
- **E = 0.0207 V**{{attrs[.fragment]}}

<!-- slide template=section -->
# 5. Applications

<!-- slide -->
## Corrosion: electrochemistry in the wild
![Rust](../assets/rust_corrosion.jpg =480x)
Iron oxidizes spontaneously; O₂ is the oxidizing agent — O₂ is reduced where it is plentiful (near the air/water edge), while iron is oxidized at anodic sites where O₂ is scarce.

<!-- slide -->
## Electrolysis: forcing the nonspontaneous
:::warning
Negative E°cell does NOT mean "never happens" — external energy (electrolysis) can drive it. Electrolysis of water: reverse of H₂ combustion. Electrolysis of molten NaCl: makes Na(s) and Cl₂(g).
:::

<!-- slide main-side -->
## Galvanic vs electrolytic
<!-- @main -->
![Side-by-side galvanic and electrolytic cells with opposite energy conversion](../assets/galvanic_vs_electrolytic.svg =740x)
<!-- @side -->
Galvanic: $E^\circ_{cell} > 0$, chemical → electrical, **no supply needed**.

Electrolytic: $E^\circ_{cell} < 0$, electrical → chemical, **supply required**.

**Oxidation is at the anode in BOTH.** Only the sign painted on the electrode flips.

<!-- slide -->
## Batteries: engineered galvanic cells
![Batteries](../assets/batteries.jpg =480x)
Dry cell, mercury, lead storage, lithium-ion, fuel cell — all fundamentally galvanic cells.

<!-- slide template=closing -->
# Three views, one framework
ΔG°, K, and E° are three descriptions of the same reaction's favorability, unified by ΔG° = −nFE° = −RT ln K. This is the course's synthesis: kinetics, equilibrium, thermodynamics, and electrochemistry are one connected story.
