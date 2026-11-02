{{nyml
kind: document
carrier: slides
uid: doc-a34cg029dytne24h
title: Chapter 11: Intermolecular Forces, Liquids, and Solids
ratio: 16:9
theme: paper
}}

<!-- slide template=title -->
# Intermolecular Forces, Liquids, and Solids
## Why molecular attraction explains bulk matter
**General Chemistry, Chapter 11**

<!-- slide 2col -->
## Chapter Learning Objectives
<!-- @left -->
- **Objective 11.1a** — Identify intermolecular forces from molecular structure
- **Objective 11.1b** — Rank intermolecular forces by relative strength
- **Objective 11.2a** — Relate surface tension, viscosity, cohesion, and adhesion to intermolecular force strength
- **Objective 11.2b** — Explain water's anomalous properties via hydrogen bonding
- **Objective 11.3a** — Classify solids and predict their properties
<!-- @right -->
- **Objective 11.3b** — Count atoms per unit cell and determine coordination number
- **Objective 11.4a** — Apply heat-of-phase-change calculations and define equilibrium vapor pressure
- **Objective 11.4b** — Apply the Clausius–Clapeyron equation
- **Objective 11.4c** — Interpret a phase diagram

<!-- slide template=outline -->
## Roadmap
1. Intermolecular forces
2. Properties of liquids
3. Solids
4. Phase changes and diagrams

<!-- slide -->
## Chapter Logic
{{mermaid
graph TD
  A["Molecular polarity & structure"] --> B["Type & strength of<br/>intermolecular (interparticle) force"]
  B --> C["Liquid properties"]
  B --> D["Solid classification"]
  B --> E["Phase-change energetics"]
}}
**Visual description:** polarity and structure set the intermolecular force; that force drives liquid behavior, solid type, and phase-change energetics.

<!-- slide template=section -->
# 1. Intermolecular Forces

<!-- slide -->
## Inter- vs. intramolecular
- **Intramolecular** = covalent bonds *within* a molecule (~150–1,100 kJ/mol)
- **Intermolecular** = attractions *between* neutral molecules (~0.05–40 kJ/mol)
- ==Melting/boiling a molecular substance breaks only the *intermolecular* attractions==
- Every O–H covalent bond in H₂O survives boiling intact

<!-- slide 2col -->
## Polar vs. nonpolar examples
<!-- @left -->
![Polar and nonpolar example molecules](../assets/polar_nonpolar_molecules.svg =480x)
<!-- @right -->
- Polar molecules (H₂O, HF, NH₃): permanent dipole
- Can hydrogen-bond if H is on N, O, or F
- Nonpolar (CH₄, CCl₄, CO₂): no net dipole
- CO₂'s bond dipoles exist but **cancel** by symmetry

<!-- slide -->
## Dispersion forces — even nonpolar molecules attract
- Electron clouds fluctuate → momentary **instantaneous dipole**
- Induces a matching **induced dipole** next door
- **Polarizability** ↑ with more electrons / more diffuse cloud
- Why I₂ is a solid but Cl₂ is a gas at room temperature

<!-- slide main-side -->
## Hydrogen bonding
<!-- @main -->
- H bonded directly to **N, O, or F** → attracted to a nearby lone pair on N, O, or F
- Unusually strong: ~10–40 kJ/mol
- Present in H₂O, NH₃, HF — **not** in CH₄
<!-- @side -->
:::warning
Not every H-containing molecule hydrogen-bonds — check the H is on N/O/F specifically.
:::

<!-- slide main-side -->
## Why water is a liquid and methane a gas
<!-- @main -->
| | M (g/mol) | Shape | Strongest force | 25 °C | bp |
|---|---|---|---|---|---|
| CH₄ | 16.04 | tetrahedral | dispersion | gas | −161 °C |
| H₂S | 34.08 | bent | dipole-dipole | gas | −60 °C |
| **H₂O** | 18.02 | bent | **H-bonding** | **liquid** | **100 °C** |
<!-- @side -->
Water's bent shape (Ch. 10) does two jobs at once:

- bond dipoles **don't cancel** → permanent dipole
- **2 donors + 2 acceptors** → up to **4** H-bonds per molecule

H₂S is bent and twice as heavy — but S is too big and not electronegative enough to H-bond.

<!-- slide -->
## The evidence: hydride boiling points
![Boiling points of main-group hydrides](../assets/hydride_boiling_points.svg =620x)
NH₃, H₂O, and HF sit far above their own group's trend — hydrogen bonding is the extra lift.

<!-- slide 2col -->
## Ranking the forces
<!-- @left -->
$$\text{ion-dipole} > \text{H-bond} >$$
$$\text{dipole-dipole} >$$
$$\text{dispersion}$$
- Ranking holds for *comparable size*
- A huge nonpolar molecule can out-attract a small polar one
<!-- @right -->
{{chart
type: bar
title: Typical energy (kJ/mol, order of magnitude)
labels: H-bond, Dipole-dipole, Dispersion
series: kJ/mol = 25, 5, 2
}}
**Data summary:** approximate order-of-magnitude energies — hydrogen bonds (~25 kJ/mol) exceed dipole-dipole (~5 kJ/mol), which exceed dispersion forces between small molecules (~2 kJ/mol).

<!-- slide step -->
## Worked example — which force, which boils higher?
Compare CH₃OH (methanol) and CH₃SH (methanethiol). Which has hydrogen bonding? Which boils higher?
- Methanol: O–H bond → hydrogen bonding + dipole-dipole + dispersion{{attrs[.fragment]}}
- Methanethiol: S–H bond → S is *not* N/O/F → dipole-dipole + dispersion only{{attrs[.fragment]}}
- **Methanol boils higher** (64.7 °C vs. 6.2 °C) — the extra hydrogen bonding wins{{attrs[.fragment]}}

<!-- slide template=section -->
# 2. Properties of Liquids

<!-- slide main-side -->
## Surface tension
<!-- @main -->
- Resistance to increasing surface area
- Surface molecules pulled only inward/sideways → net inward force
- **Stronger IMF → higher surface tension**
<!-- @side -->
![A water strider standing on water](../assets/water_strider_surface_tension.jpg =360x)
*Supported entirely by surface tension*

<!-- slide -->
## Cohesion, adhesion, and capillary action
- **Cohesion** = like-molecule attraction (water–water)
- **Adhesion** = unlike-molecule attraction (water–glass)
- Adhesion > cohesion → liquid climbs a narrow tube
- This is how paper towels wick, and it helps trees move water upward

<!-- slide -->
## Viscosity
- Resistance to flow
- Stronger IMF → higher viscosity (honey vs. water vs. gasoline)
- Higher temperature → lower viscosity (easier to slip past neighbors)

<!-- slide -->
## Water's anomalies — all one cause
- Each H₂O forms up to **4 hydrogen bonds**
- Unusually high melting/boiling point for its size
- Unusually high specific heat (4.184 J/g·°C) — moderates climate
- **Maximum density at 4 °C**, not at freezing; ice is less dense than liquid water — ice floats

<!-- slide template=section -->
# 3. Solids

<!-- slide -->
## Four types of crystalline solids
| Type | Bonds | Hardness | Melting pt. | Conducts? |
|---|---|---|---|---|
| Molecular | IMF | Soft | Low | Poor |
| Covalent network | Covalent | Hard | High | Poor* |
| Ionic | Ionic | Hard, brittle | High | Poor (good when molten or dissolved) |
| Metallic | Metallic | Soft–hard | Low–high | Good |

<!-- slide 2col -->
## Ionic vs. covalent-network, in real crystals
<!-- @left -->
![NaCl ionic lattice](../assets/nacl_ionic_lattice.png =420x)
*NaCl: each ion has 6 neighbors*
<!-- @right -->
![Quartz crystal](../assets/quartz_crystal.jpg =420x)
*Quartz (SiO₂): one continuous covalent network*

<!-- slide -->
## The three cubic unit cells
![Simple cubic, body-centered cubic, face-centered cubic unit cells](../assets/cubic_unit_cells.svg =900x)

<!-- slide -->
## Counting atoms and coordination number
| Cell | Atoms/cell | Coordination # |
|---|---|---|
| SCC | 1 | 6 |
| BCC | 2 | 8 |
| FCC | 4 | 12 |
- Corner atom → counts $\tfrac{1}{8}$ · Face atom → counts $\tfrac{1}{2}$ · Body atom → counts 1

<!-- slide step -->
## Worked example — BCC atom count
BCC has 8 corner atoms + 1 body-centered atom. Total atoms per cell?
- Corners: $8 \times \tfrac{1}{8} = 1$ atom{{attrs[.fragment]}}
- Center: $1 \times 1 = 1$ atom{{attrs[.fragment]}}
- **Total = 2 atoms per BCC cell**{{attrs[.fragment]}}

<!-- slide template=section -->
# 4. Phase Changes and Diagrams

<!-- slide -->
## Evaporation ⇌ condensation
- Evaporation and condensation reach equal rates → **dynamic equilibrium**
- Vapor pressure at that point = **equilibrium vapor pressure**
- **Molar heat of vaporization** ($\Delta H_\text{vap}$): energy to vaporize 1 mole

<!-- slide 2col -->
## Clausius–Clapeyron equation
<!-- @left -->
$$\ln\frac{P_1}{P_2} = \frac{\Delta H_\text{vap}}{R}\left(\frac{T_1-T_2}{T_1T_2}\right)$$
- Relates vapor pressure at two temperatures
- Needs $\Delta H_\text{vap}$ for the substance
<!-- @right -->
![Vapor pressure of diethyl ether vs temperature](../assets/vapor_pressure_diethyl_ether.svg =480x)

<!-- slide step -->
## Worked example — diethyl ether at 30.0 °C
442 mmHg at 20.0 °C, $\Delta H_\text{vap}$ = 26.5 kJ/mol. Find P at 30.0 °C.
- $\ln(442/P_2) = \tfrac{26{,}500}{8.314}\left(\tfrac{1}{303.15}-\tfrac{1}{293.15}\right) = -0.3587$ {{attrs[.fragment]}}
- $442/P_2 = e^{-0.3587} = 0.6986$ {{attrs[.fragment]}}
- **$P_2 = 633$ mmHg** — up more than 40% in ten degrees (measured: about 640 mmHg){{attrs[.fragment]}}

<!-- slide main-side -->
## Phase diagram of water
<!-- @main -->
![Phase diagram of water](../assets/water_phase_diagram.svg =520x)
<!-- @side -->
- **Triple point**: all 3 phases coexist
- **Critical point**: liquid/vapor become indistinguishable
- Solid–liquid line slopes **negative** — unusual — water is one of the few substances with this behavior

<!-- slide template=closing -->
# One thread: the intermolecular force decides everything
Liquid behavior, solid type, and phase energetics all trace back to a single fact — the force between particles.
