{{nyml
kind: document
carrier: slides
uid: doc-zrgauk7rghzgm8p8
title: Chapter 6: Thermochemistry
ratio: 16:9
theme: paper
}}

<!-- slide template=title -->
# Thermochemistry
## Tracking heat through a reaction
**General Chemistry, Chapter 6**

<!-- slide 2col -->
## Chapter Learning Objectives
<!-- @left -->
- **Objective 6.1a** — Distinguish types of energy, types of systems, and exothermic/endothermic processes
- **Objective 6.1b** — Apply the first law of thermodynamics
- **Objective 6.2a** — Define enthalpy and apply thermochemical-equation rules
- **Objective 6.2b** — Convert between $\Delta H$ and $\Delta U$ for a reaction
<!-- @right -->
- **Objective 6.3a** — Apply specific heat and heat capacity
- **Objective 6.3b** — Use constant-volume and constant-pressure calorimetry
- **Objective 6.4a** — Apply Hess's Law
- **Objective 6.4b** — Calculate reaction enthalpy from standard enthalpies of formation

<!-- slide template=outline -->
## Roadmap
1. Energy and the first law of thermodynamics
2. Enthalpy
3. Calorimetry
4. Standard enthalpy

<!-- slide -->
## Chapter Logic
{{mermaid
graph TD
  A["First law of thermodynamics:<br/>Delta U = q + w"] --> B["Enthalpy (H):<br/>ΔH = heat at constant pressure (q_p)"]
  B --> C["Calorimetry:<br/>measuring q experimentally"]
  C --> D["Hess's Law and standard<br/>enthalpies of formation:<br/>calculating without measuring"]
}}
**Visual description:** the first law is the general energy-accounting rule; enthalpy specializes it to constant pressure; calorimetry measures it; Hess's Law and formation enthalpies let you calculate it without measuring.

<!-- slide template=section -->
# 1. Energy and the First Law

<!-- slide -->
## System, surroundings, and the boundary
![Open, closed and isolated systems](../assets/system_and_surroundings.svg =820x)
Which kind you have follows from where you choose to draw the boundary and what can cross it, not a fact about the chemistry

<!-- slide -->
## Signs come from the system's point of view
![Sign conventions for q and w](../assets/sign_conventions_q_w.svg =800x)
$q>0$ absorbed · $q<0$ released · $w>0$ done ON the system · $w<0$ done BY it

<!-- slide -->
## Systems and processes
- Open: exchanges mass + energy · Closed: energy only · Isolated: neither
- Exothermic: releases heat · Endothermic: absorbs heat

<!-- slide -->
## First law of thermodynamics
$$\Delta U=q+w \qquad w=-P\Delta V\ \text{(gas expansion or compression against constant external pressure } P\text{)}$$

<!-- slide step -->
## Worked example — internal energy change
679 J work done on gas; 185 J heat released
- $\Delta U=q+w=-185+679$ {{attrs[.fragment]}}
- **= 494 J**{{attrs[.fragment]}}

<!-- slide template=section -->
# 2. Enthalpy

<!-- slide -->
## Enthalpy and sign convention
![Exo/endo diagram](../assets/exo_endo_diagram.svg =560x)

<!-- slide step -->
## Worked example — heat from mass
$\ce{2SO2+O2->2SO3}$, $\Delta H = -198.2$ kJ, 87.9 g $\ce{SO2}$
- $87.9/64.07\times(-198.2/2)$ {{attrs[.fragment]}}
- **= −136 kJ**{{attrs[.fragment]}}

<!-- slide step -->
## $\Delta H$ vs. $\Delta U$ for gas reactions
$$\Delta U=\Delta H-\Delta nRT$$
$\ce{2CO+O2->2CO2}$, $\Delta H = -566.0$ kJ/mol{{attrs[.fragment]}}
$\Delta n = -1$ → **$\Delta U = -563.5$ kJ**{{attrs[.fragment]}}

<!-- slide template=section -->
# 3. Calorimetry

<!-- slide -->
## Water is the outlier
![Specific heats compared](../assets/specific_heat_comparison.svg =760x)
4.184 $\text{J}\,\text{g}^{-1}\,\text{°C}^{-1}$ against gold's 0.129 — about 32 times more heat for the same rise

<!-- slide -->
## Two calorimeters, two quantities
![Constant pressure vs constant volume](../assets/two_calorimeters.svg =800x)
Rigid and sealed → $\Delta U$ · open to the air → $\Delta H$

<!-- slide -->
## Specific heat and heat capacity
$$q=ms\Delta T \qquad C=ms$$

<!-- slide -->
## Bomb calorimetry (constant volume)
$$q_\text{rxn}=-(q_\text{water}+q_\text{bomb})=\Delta U_\text{rxn}$$
![Bomb calorimeter schematic](../assets/bomb_calorimeter.svg =360x)

<!-- slide -->
## A real bomb calorimeter
![Bomb calorimeter photo](../assets/bomb_calorimeter_photo.jpg =420x)

<!-- slide step -->
## Worked example — glucose combustion
3.12 g glucose, 775 g water, bomb C=893 J/°C, $\Delta T = 11.8$°C
- $q=-[(4.184)(775)(11.8)+(893)(11.8)]$ {{attrs[.fragment]}}
- **= −48.8 kJ**{{attrs[.fragment]}}

<!-- slide -->
## Constant-pressure calorimetry
$$q_\text{rxn}=-(q_\text{water}+q_\text{cal})=\Delta H_\text{rxn}$$
Coffee-cup calorimeter: HCl + NaOH neutralization example gives **$q_\text{soln} = 2.9\times10^{3}$ J**, so **$\Delta H_\text{rxn} = -2.9\times10^{3}$ J** for the amounts reacted (exothermic)

<!-- slide template=section -->
# 4. Standard Enthalpy

<!-- slide -->
## Standard enthalpy of formation
- Element in its most stable form: $\Delta H_f^\circ=0$
- $\Delta H_\text{rxn}^\circ=\sum n\Delta H_f^\circ(\text{products})-\sum m\Delta H_f^\circ(\text{reactants})$

<!-- slide -->
## Formation enthalpies are heights from a chosen zero
![Formation enthalpy reference level](../assets/formation_enthalpy_reference.svg =800x)
A reaction enthalpy is a **difference** of heights, so, because a balanced equation conserves each element, the choice of zero always cancels

<!-- slide -->
## Hess's Law
![Hess's law cycle](../assets/hess_law_cycle.svg =560x)

<!-- slide step -->
## Worked example — $\ce{FeCl3}$ formation
$\Delta H_1^\circ=-341.8$, $\Delta H_2^\circ=-115.4$ kJ
- $\Delta H_f^\circ=\Delta H_1^\circ+\tfrac12\Delta H_2^\circ$ {{attrs[.fragment]}}
- **= −399.5 kJ**{{attrs[.fragment]}}

<!-- slide step -->
## Worked example — Al/Fe2O3 thermite reaction
$\Delta H_\text{rxn}^\circ=-826.7$ kJ; 35.0 g Al reacted
- 1.297 mol Al ÷ 2 mol (coefficient){{attrs[.fragment]}}
- **q = −536 kJ**{{attrs[.fragment]}}

<!-- slide template=closing -->
# From general law to calculable numbers
The first law of thermodynamics is a universal accounting rule; enthalpy specializes it to constant pressure; calorimetry measures heat flow directly ($\Delta H$ at constant pressure, $\Delta U$ at constant volume); Hess's Law and standard formation enthalpies let you calculate a reaction's enthalpy from tabulated data without measuring that reaction itself — because enthalpy is a state function.
