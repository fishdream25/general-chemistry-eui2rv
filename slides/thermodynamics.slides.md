{{nyml
kind: document
carrier: slides
uid: doc-1mogplhrgld2mkx6
title: Chapter 17: Entropy, Free Energy, and Equilibrium
ratio: 16:9
theme: paper
}}

<!-- slide template=title -->
# Entropy, Free Energy, and Equilibrium
## Why reactions happen
**General Chemistry, Chapter 17**

<!-- slide 2col -->
## Chapter Learning Objectives
<!-- @left -->
- **Objective 17.1a** — Define entropy via microstates and predict the sign of ΔS
- **Objective 17.1b** — Calculate the standard entropy of a reaction
- **Objective 17.2a** — State the laws of thermodynamics and explain the second law as the spontaneity criterion
- **Objective 17.2b** — Explain the third law's role in absolute entropy
- **Objective 17.3a** — Define Gibbs free energy and apply the spontaneity criterion
<!-- @right -->
- **Objective 17.3b** — Calculate standard free energy of reaction
- **Objective 17.3c** — Determine transition temperatures by setting ΔG = 0
- **Objective 17.3d** — Relate ΔG° to the equilibrium constant K
- **Objective 17.3e** — Calculate ΔG under non-standard conditions and predict reaction direction

<!-- slide template=outline -->
## Roadmap
1. Entropy
2. The laws of thermodynamics
3. Free energy

<!-- slide -->
## Chapter Logic
{{mermaid
graph TD
  A["Entropy (S = k ln W):<br/>microstates & disorder"] --> B["Second law:<br/>total universe entropy increases in a spontaneous process"]
  B --> C["Gibbs free energy:<br/>G = H - TS"]
  C --> D["Delta G = Delta H - T Delta S<br/>sign determines spontaneity"]
  D --> E["Delta G-naught = -RT ln K<br/>links back to Ch. 14's K"]
}}
**Visual description:** entropy's microstate definition leads to the second law, motivating Gibbs free energy. The sign of ΔG determines spontaneity, and ΔG° connects back to Chapter 14's K.

<!-- slide main-side -->
## Two tendencies, four outcomes
<!-- @main -->
![Four quadrants of enthalpy and entropy sign combinations](../assets/spontaneity_quadrants.svg =700x)
<!-- @side -->
Systems tend toward **lower energy** and toward **more disorder**.

When both agree, the answer is settled before any calculation.

When they disagree, **temperature decides** — and the crossover is at $T = \Delta H/\Delta S$.

<!-- slide template=section -->
# 1. Entropy

<!-- slide -->
## Entropy: a microstate definition
$$S = k \ln W$$
- k = Boltzmann constant, W = number of microstates
- More accessible microstates → higher entropy

<!-- slide -->
## 4 particles, 2 boxes: 16 microstates
![Microstates](../assets/microstates_distribution.svg =900x)
Distribution \(c), 2-2 split, has the MOST microstates → highest entropy, most probable

<!-- slide -->
## Entropy trends
- Gas ≫ Liquid > Solid
- More complex molecules (same state) → higher entropy
- Entropy is a state function: ΔS = Sf − Si

<!-- slide main-side -->
## Both entropy trends, in one chart
<!-- @main -->
![Standard molar entropies for four solids, three liquids and six gases](../assets/entropy_trends.svg =740x)
<!-- @side -->
**Phase dominates.** The most complex liquid here still sits below the simplest gas.

**Across the whole chart, phase and complexity combine** — diamond (solid) 2.4, butane (gas) 310, a factor of 130.

Water appears twice: 69.9 as liquid, 188.8 as gas. The phase change is the largest single effect in the chapter.

<!-- slide step -->
## Worked example — ΔS°rxn
4Fe(s) + 3O₂(g) → 2Fe₂O₃(s). S°: Fe=27.3, O₂=205.2, Fe₂O₃=87.4 J/K·mol
- ΔS° = 2(87.4) − [4(27.3)+3(205.2)]{{attrs[.fragment]}}
- **= −550 J/K·mol** (3 mol gas consumed → strongly negative, as expected){{attrs[.fragment]}}

<!-- slide template=section -->
# 2. The Laws of Thermodynamics

<!-- slide -->
## Four laws
- **Zeroth:** thermal equilibrium is transitive
- **First:** energy is conserved (Ch. 6)
- **Second:** total universe entropy increases in any spontaneous process
- **Third:** a perfect crystal at 0 K has zero entropy

<!-- slide -->
## The third law in action
![Diamond](../assets/diamond.jpg =420x)
Diamond's S° = 2.4 J/K·mol — small because of its highly ordered lattice; the third law lets us report this as an ABSOLUTE value.

<!-- slide -->
## The second law, precisely
:::warning
The system's OWN entropy can decrease in a spontaneous process — only the universe's total entropy must increase.
:::

<!-- slide template=section -->
# 3. Free Energy

<!-- slide -->
## Gibbs free energy
$$G = H - TS \qquad \Delta G = \Delta H - T\Delta S$$
| ΔG | Meaning |
|---|---|
| < 0 | Spontaneous forward |
| > 0 | Spontaneous reverse |
| = 0 | Equilibrium |

<!-- slide step -->
## Worked example — ΔG°rxn
4Fe(s) + 3O₂(g) → 2Fe₂O₃(s). ΔG°f: Fe=0, O₂=0, Fe₂O₃=−742.2 kJ/mol
- ΔG° = 2(−742.2) − 0{{attrs[.fragment]}}
- **= −1484.4 kJ/mol**{{attrs[.fragment]}}

<!-- slide -->
## Temperature can flip the sign of ΔG
![Gibbs temperature crossover](../assets/gibbs_temperature_crossover.svg =620x)

<!-- slide step -->
## Worked example — transition temperature
CaCO₃(s) ⇌ CaO(s) + CO₂(g). ΔH°=177.8 kJ/mol, ΔS°=160.5 J/K·mol
- At 298 K: ΔG°=130.0 kJ/mol > 0 (nonspontaneous){{attrs[.fragment]}}
- Set ΔG°=0: T = ΔH°/ΔS°{{attrs[.fragment]}}
- **T = 1108 K = 835°C**{{attrs[.fragment]}}

<!-- slide -->
## Phase transitions: the same ΔG=0 logic
![Ice melting](../assets/ice_melting.jpg =420x)
At 0°C, 1 atm: ice/water equilibrium. ΔH=6.01 kJ/mol, ΔS=22.0 J/K·mol → ΔH/ΔS = 273 K ✓

<!-- slide -->
## Free energy vs. reaction progress
![Free energy vs reaction progress](../assets/free_energy_vs_reaction_progress.svg =560x)

<!-- slide -->
## Free energy meets equilibrium
$$\Delta G = \Delta G^\circ + RT\ln Q \qquad \Delta G^\circ = -RT\ln K$$
:::warning
ΔG° is ONE fixed number (for a given reaction at a given temperature). ΔG changes as Q changes during the reaction.
:::

<!-- slide step -->
## Worked example — ΔG° → K
N₂O₄(g) ⇌ 2NO₂(g). ΔG°f: N₂O₄=97.9, NO₂=51.3 kJ/mol
- ΔG°rxn = 2(51.3) − 97.9 = 4.7 kJ/mol{{attrs[.fragment]}}
- Predict: ΔG°>0 (small) → K below 1, not by orders of magnitude{{attrs[.fragment]}}
- **K_p = e^(−4700/(8.314×298)) = 0.150** ✓{{attrs[.fragment]}}

<!-- slide step -->
## Worked example — ΔG under real conditions
2NH₃(g) → 3H₂(g) + N₂(g), ΔG°=33.0 kJ/mol. P: N₂=0.870, H₂=0.250, NH₃=0.129 atm
- Q = (0.250³×0.870)/(0.129²) = 0.817{{attrs[.fragment]}}
- ΔG = 33,000 + RT ln(0.817){{attrs[.fragment]}}
- **= 32.5 kJ/mol** (still nonspontaneous forward){{attrs[.fragment]}}

<!-- slide template=closing -->
# One number explains it all
Gibbs free energy combines enthalpy and entropy into a single spontaneity criterion. ΔG° = −RT ln K explains, in energy terms, why equilibrium constants (Ch. 14) are what they are — and reappears in Chapter 18 as ΔG° = −nFE°.
