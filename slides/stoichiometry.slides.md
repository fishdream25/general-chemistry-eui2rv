{{nyml
kind: document
carrier: slides
uid: doc-6iu02kdjm2tg6bs5
title: Chapter 3: Stoichiometry
ratio: 16:9
theme: paper
}}

<!-- slide template=title -->
# Stoichiometry
## The mole makes chemistry quantitative
**General Chemistry, Chapter 3**

<!-- slide 2col -->
## Chapter Learning Objectives
<!-- @left -->
- **Objective 3.1a** — Calculate average atomic mass and understand the mole concept
- **Objective 3.1b** — Convert between mass, moles, and number of particles
- **Objective 3.1c** — Calculate molecular mass, formula mass, and percent composition
- **Objective 3.1d** — Determine an empirical formula from combustion-analysis data
<!-- @right -->
- **Objective 3.2a** — Balance chemical equations
- **Objective 3.2b** — Convert between quantities of reactants and products using a balanced equation
- **Objective 3.2c** — Determine the limiting reagent
- **Objective 3.2d** — Calculate theoretical yield and percent yield

<!-- slide template=outline -->
## Roadmap
1. Molar mass
2. Balancing chemical reactions

<!-- slide -->
## Chapter Logic
{{mermaid
graph TD
  A["Molar mass:<br/>atomic, molecular, formula mass"] --> B["Mole conversions:<br/>mass, moles, particles"]
  B --> C["Balanced equations:<br/>mole-to-mole ratios"]
  C --> D["Limiting reagent,<br/>theoretical and percent yield"]
}}
**Visual description:** molar mass enables mole conversions; balanced equations give mole-to-mole ratios between substances; limiting reagent and yield calculations apply that ratio to a realistic reaction.

<!-- slide template=section -->
# 1. Molar Mass

<!-- slide -->
## Atomic mass and the mole
- 1 amu = 1/12 the mass of one $\ce{^{12}C}$ atom
- Average atomic mass = weighted average of isotopes
- 1 mol = $N_A = 6.022\times10^{23}$ entities

<!-- slide -->
## How big is a mole?
![Three comparisons for Avogadro's number](../assets/how_big_is_a_mole.svg =760x)
A counting word, like "dozen" — the mole is the bridge between the particle scale and the lab scale

<!-- slide step -->
## Worked example — average atomic mass
Cu: 69.09% at 62.93 amu, 30.91% at 64.9278 amu
- $62.93(0.6909)+64.9278(0.3091)$ {{attrs[.fragment]}}
- **= 63.55 amu**{{attrs[.fragment]}}

<!-- slide -->
## Mole conversions
![Mole conversion triangle](../assets/mole_conversion_triangle.svg =520x)

<!-- slide -->
## Percent composition
![Percent composition of water as a mass bar](../assets/percent_composition_water.svg =760x)
Water is two-thirds hydrogen by **atom count** and only 11% hydrogen by **mass**

<!-- slide -->
## Molecular mass vs. formula mass
- Molecular mass: sum of atomic masses in a molecule
- Formula mass: same idea, for any formula (ionic compounds have no "molecule")
- Both (in amu) are numerically equal to molar mass in g/mol

<!-- slide step -->
## Worked example — molar mass
- $\ce{CH4}$: $12.01+4(1.008)$ {{attrs[.fragment]}}
- **= 16.04 g/mol**{{attrs[.fragment]}}
- $\ce{NaCl}$: $22.99+35.45$ {{attrs[.fragment]}}
- **= 58.44 g/mol** (formula mass){{attrs[.fragment]}}

<!-- slide -->
## Combustion analysis
![Combustion analysis apparatus](../assets/combustion_analysis.svg =620x)
Each absorber's mass gain gives the mass of CO2 or H2O formed; convert to moles of CO2 or H2O with its molar mass, then to moles of C (1 per CO2) or H (2 per H2O)

<!-- slide step -->
## Worked example — ethanol's empirical formula
11.5 g ethanol → 22.0 g CO₂ + 13.5 g H₂O
- C: 0.500 mol; H: 1.50 mol{{attrs[.fragment]}}
- O by difference: 0.25 mol{{attrs[.fragment]}}
- Ratio 2:6:1 → **$\ce{C2H6O}$**{{attrs[.fragment]}}

<!-- slide template=section -->
# 2. Balancing Chemical Reactions

<!-- slide -->
## What coefficients mean
$$\ce{2Mg + O2 -> 2MgO}$$
Means **moles** (or particles) — not grams
![Magnesium burning](../assets/magnesium_burning.jpg =420x)

<!-- slide -->
## Balancing is an atom tally
![Unbalanced and balanced atom tallies](../assets/balancing_atom_tally.svg =760x)
Adjust coefficients only — changing a subscript changes the substance

<!-- slide step -->
## Worked example — balancing
$\ce{C2H6 + O2 -> CO2 + H2O}$
- Balance C, H: coefficients 2, 3{{attrs[.fragment]}}
- O needs a fractional 3.5 coefficient{{attrs[.fragment]}}
- ×2 to clear: **$\ce{2C2H6 + 7O2 -> 4CO2 + 6H2O}$**{{attrs[.fragment]}}

<!-- slide -->
## The stoichiometry road map
![Mass A to moles A to moles B to mass B](../assets/stoichiometry_road_map.svg =840x)
You can only cross from one substance to another in **moles**

<!-- slide -->
## Reactant → product quantity
1. Write balanced equation
2. Convert known mass → moles
3. Use mole ratio (coefficients) → moles of target
4. Convert moles → desired units of target

<!-- slide -->
## Limiting reagent: the idea
![Nuts and bolts analogy](../assets/limiting_reagent_concept.svg =800x)
The limiting reactant is not necessarily the one you have least of — it is the one that runs out first

<!-- slide -->
## Limiting reagent: two methods
- Method 1: least product wins — the limiting reagent gave it
- Method 2 (fewer steps): mol ÷ coefficient — smallest wins
![Limiting reagent bar chart](../assets/limiting_reagent_bar.svg =480x)

<!-- slide step -->
## Worked example — urea synthesis
$\ce{2NH3 + CO2 -> (NH2)2CO + H2O}$; 637.2 g NH₃, 1142 g CO₂
- 37.42 mol NH₃ ÷ 2 = 18.71{{attrs[.fragment]}}
- 25.95 mol CO₂ ÷ 1 = 25.95{{attrs[.fragment]}}
- **NH₃ is limiting** (smaller value){{attrs[.fragment]}}

<!-- slide -->
## Theoretical vs. actual yield
![Yield bars](../assets/theoretical_vs_actual_yield.svg =740x)
Above 100% is not a triumph — it means the product is wet or impure

<!-- slide -->
## Theoretical yield and % yield
$$\%\,\text{Yield}=\frac{\text{Actual Yield}}{\text{Theoretical Yield}}\times100\%$$
Theoretical yield of urea here: 1124 g

<!-- slide step -->
## Worked example — % yield and excess reagent
- Actual yield 1006 g / theoretical 1124 g{{attrs[.fragment]}}
- **89.5% yield**{{attrs[.fragment]}}
- CO₂ remaining: $25.95-18.71=7.24$ mol → **319 g** excess{{attrs[.fragment]}}

<!-- slide template=closing -->
# The mole is the unit of chemistry
Molar mass converts formulas into grams-per-mole; balanced equations convert one substance's amount into another's; limiting-reagent and yield analysis apply that same mole logic to real, imperfect reactions. Every later quantitative chapter assumes this fluency.
