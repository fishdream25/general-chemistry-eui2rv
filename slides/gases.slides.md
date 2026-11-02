{{nyml
kind: document
carrier: slides
uid: doc-cjvn43y0cn7lrwes
title: Chapter 5: Gases
ratio: 16:9
theme: paper
}}

<!-- slide template=title -->
# Gases
## One equation, three laws, and why it works
**General Chemistry, Chapter 5**

<!-- slide 2col -->
## Chapter Learning Objectives
<!-- @left -->
- **Objective 5.1a** — Convert between pressure units
- **Objective 5.2a** — Apply the ideal gas equation
- **Objective 5.2b** — Calculate gas density and molar mass
- **Objective 5.3a** — Apply Dalton's law of partial pressures and mole fraction
<!-- @right -->
- **Objective 5.3b** — Correct for water vapor pressure when a gas is collected over water
- **Objective 5.4a** — State the kinetic molecular theory and use it to explain gas-law behavior
- **Objective 5.4b** — Apply Graham's law of effusion and diffusion
- **Objective 5.5a** — Explain why and when real gases deviate from ideal behavior

<!-- slide template=outline -->
## Roadmap
1. General concepts and pressure
2. The gas laws
3. Partial pressures
4. Kinetic molecular theory
5. Deviations from ideal behavior
6. Exit ticket: one gas-law question (critic)

<!-- slide -->
## Chapter Logic
{{mermaid
graph TD
  A["Boyle's, Charles's, Avogadro's laws"] --> B["Ideal gas equation:<br/>PV = nRT"]
  B --> C["Partial pressures,<br/>density and molar mass"]
  C --> D["Kinetic molecular theory:<br/>explains WHY the laws hold"]
  D --> E["Real gases:<br/>deviations at high P, low T"]
}}
**Visual description:** three empirical laws combine into PV=nRT; that equation extends to partial pressures and density/molar mass; kinetic theory explains why it works; real gases deviate at high pressure and low temperature.

<!-- slide template=section -->
# 1. General Concepts and Pressure

<!-- slide -->
## Gases: general properties
- Take the shape and volume of their container
- Highly compressible; mix completely
- Much lower density than liquids/solids

<!-- slide -->
## What pressure is, and how it is measured
![Force over area, and a mercury barometer](../assets/pressure_and_barometer.svg =820x)
The height of the mercury column **is a direct measure of** the pressure (P = ρgh) — which is why mmHg became a unit

<!-- slide -->
## Pressure units
$$1\,\text{atm}=101325\,\text{Pa}=760\,\text{mmHg}=760\,\text{torr}$$

<!-- slide step -->
## Worked example — pressure conversion
489 mmHg to Pa
- $489\times\dfrac{101325}{760}$ {{attrs[.fragment]}}
- **= $6.52\times10^{4}$ Pa**{{attrs[.fragment]}}

<!-- slide template=section -->
# 2. The Gas Laws

<!-- slide -->
## Three laws combine
![Gas laws panels](../assets/gas_laws_panels.svg =680x)

<!-- slide -->
## The ideal gas equation
$$PV=nRT \qquad R=0.0821\ \text{L·atm/(K·mol)}$$
STP (0 °C, 1 atm): 1 mol occupies 22.41 L
![Hot air balloon](../assets/hot_air_balloon.jpg =380x)

<!-- slide step -->
## Worked example — pressure from PV=nRT
1.92 mol, 4.50 L, 25.6 °C
- $P=\dfrac{nRT}{V}$ {{attrs[.fragment]}}
- **= 10.5 atm**{{attrs[.fragment]}}

<!-- slide step -->
## Worked example — molar mass from density
$d=7.71$ g/L, 36.0 °C, 2.88 atm
- $\mathcal{M}=\dfrac{dRT}{P}$ {{attrs[.fragment]}}
- **= 68.0 g/mol**{{attrs[.fragment]}}

<!-- slide -->
## Gas stoichiometry: one extra step
![Mass of A to moles to volume of gas B](../assets/gas_stoichiometry_road_map.svg =840x)
Chapter 3's road map, with $V = nRT/P$ replacing the final molar-mass step

<!-- slide template=section -->
# 3. Partial Pressures

<!-- slide -->
## Dalton's law
$$P=P_1+P_2+\dots \qquad P_i=X_iP,\ X_i=\frac{n_i}{n}$$

<!-- slide -->
## Collected over water is never dry
![Collecting a gas over water](../assets/gas_collected_over_water.svg =800x)
$P_{\mathrm{gas}} = P_{\mathrm{total}} - P_{\mathrm{water}}$ — forgetting this always overstates the yield

<!-- slide step -->
## Worked example — gas collected over water
153 mL $\ce{H2}$, 758 mmHg total, water vapor 22.0 mmHg
- $P_{H_2}=758-22.0=736$ mmHg{{attrs[.fragment]}}
- **$n = 6.08\times10^{-3}$ mol**{{attrs[.fragment]}}

<!-- slide template=section -->
# 4. The Kinetic Molecular Theory

<!-- slide -->
## KMT assumptions
1. Point particles, far apart
2. Random motion, elastic collisions
3. No attraction/repulsion between molecules
4. Average KE ∝ T (absolute temperature, in K) (same for any gas at same T)

<!-- slide -->
## The molecular picture
![Molecular pictures behind Boyle and Charles](../assets/kmt_explains_gas_laws.svg =820x)
Pressure is molecules hitting walls — change the rate or force of the hits and the pressure changes

<!-- slide -->
## KMT explains every gas law
- Boyle's: smaller V → more collisions → higher P
- Charles's: higher T → higher KE → expansion
- Dalton's: no interaction → independent partial pressures

<!-- slide -->
## Graham's Law: effusion and diffusion
$$\frac{r_1}{r_2}=\sqrt{\frac{\mathcal{M}_2}{\mathcal{M}_1}}$$
![Graham's law effusion](../assets/grahams_law_effusion.svg =460x)

<!-- slide template=section -->
# 5. Deviations from Ideal Behavior

<!-- slide -->
## Why real gases deviate
- Real molecules have finite volume (matters at high P)
- Real molecules attract each other (matters at low T)
![Real gas deviation](../assets/real_gas_deviation.svg =480x)

<!-- slide -->
## Molecules do not all move at one speed
![Maxwell-Boltzmann distributions](../assets/molecular_speed_distribution.svg =840x)
Same $T$: heavier is slower · Higher $T$: the whole distribution shifts right and flattens

<!-- slide -->
## The van der Waals equation
$$\left(P+\frac{an^2}{V^2}\right)(V-nb)=nRT$$
$a$ corrects for attraction · $b$ corrects for molecular volume

<!-- slide template=closing -->
# From three laws to one equation, and why it holds
Boyle's, Charles's, and Avogadro's laws combine into PV=nRT; kinetic molecular theory explains why it works at the particle level; and real-gas deviations show precisely where its assumptions (negligible particle volume, no intermolecular attraction) break down.
