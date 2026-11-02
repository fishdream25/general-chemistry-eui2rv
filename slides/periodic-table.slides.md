{{nyml
kind: document
carrier: slides
uid: doc-9lgq9cp49j4xthzk
title: Chapter 8: Periodic Relationships Among the Elements
ratio: 16:9
theme: paper
}}

<!-- slide template=title -->
# Periodic Relationships Among the Elements
## From electron configuration to predictive trends
**General Chemistry, Chapter 8**

<!-- slide 2col -->
## Chapter Learning Objectives
<!-- @left -->
- **Objective 8.1a** — Classify elements by category
- **Objective 8.1b** — Write electron configurations for ions and identify isoelectronic species
- **Objective 8.2a** — Explain effective nuclear charge and atomic radius trends
- **Objective 8.2b** — Compare ionic radii (isoelectronic series and same-element different-charge)
<!-- @right -->
- **Objective 8.3a** — Explain and apply the periodic trend in ionization energy
- **Objective 8.3b** — Explain and apply the periodic trend in electron affinity
- **Objective 8.4a** — Describe periodic patterns in chemical behavior and diagonal relationships
- **Objective 8.4b** — Classify oxides as basic, acidic, or amphoteric

<!-- slide template=outline -->
## Roadmap
1. Electron configuration and periodic classification
2. Effective nuclear charge and size
3. Ionization energy and electron affinity
4. A survey of chemical properties

<!-- slide -->
## Chapter Logic
{{mermaid
graph TD
  A["Electron configuration:<br/>categorizes every element"] --> B["Effective nuclear charge:<br/>drives atomic and ionic radius trends"]
  B --> C["Ionization energy and<br/>electron affinity trends"]
  C --> D["Chemical behavior patterns:<br/>groups, diagonal relationships, oxide acidity"]
}}
**Visual description:** electron configuration categorizes elements; effective nuclear charge drives radius trends; the same logic drives ionization energy and electron affinity; all together explain observed chemical behavior patterns.

<!-- slide template=section -->
# 1. Electron Configuration and Periodic Classification

<!-- slide -->
## Element categories
![Element category map](../assets/element_category_map.svg =620x)

<!-- slide step -->
## Worked example — transition-metal cation
$\ce{Fe}$: $[Ar]4s^23d^6$
- Remove $4s$ electrons first{{attrs[.fragment]}}
- $\ce{Fe^2+}$: $[Ar]3d^6${{attrs[.fragment]}}
- $\ce{Fe^3+}$: $[Ar]3d^5${{attrs[.fragment]}}

<!-- slide template=section -->
# 2. Effective Nuclear Charge and Size

<!-- slide -->
## Shielding, and what an outer electron actually feels
![Zeff for Li, C and F](../assets/effective_nuclear_charge.svg =800x)
Same core doing the shielding all across a period, so, if we treat the $1s^2$ core as screening fully and the valence electrons as not screening each other, $Z_\mathrm{eff}$ climbs from about +1 to +7

<!-- slide -->
## Effective nuclear charge ($Z_\text{eff}$)
- Increases left→right across a period (smaller atoms)
- Outweighed by added shells going down a group (larger atoms)

<!-- slide -->
## Three trends, one cause
![Periodic trend arrows](../assets/periodic_trend_map.svg =820x)
Across: radius **down**, IE **up**, EA **up** · Down: radius **up**, IE **down**, EA **down**

<!-- slide -->
## Isoelectronic series
![Isoelectronic radius series](../assets/isoelectronic_radius_series.svg =560x)

<!-- slide step -->
## Worked example — isoelectronic ranking
$\ce{N3-}$, $\ce{O2-}$, $\ce{F-}$, Ne, $\ce{Na+}$, $\ce{Mg2+}$, $\ce{Al3+}$ (all $\ce{10e-}$)
- Nuclear charge increases $Z = 7$→13{{attrs[.fragment]}}
- **Radius decreases in the same order**{{attrs[.fragment]}}

<!-- slide template=section -->
# 3. Ionization Energy and Electron Affinity

<!-- slide -->
## The jump reveals the group number
![Successive ionization energies](../assets/successive_ionization_energies.svg =820x)
Count the ionization energies before the big jump — that is the valence-electron count

<!-- slide -->
## Ionization energy trend
$$IE_1<IE_2<IE_3<\dots$$
Increases left→right across a period, bottom→top in a group
![Ionization energy trend](../assets/ionization_energy_trend.svg =560x)

<!-- slide -->
## Electron affinity
Similar trend to IE, but noble gases have near-zero/negative EA (no room in a filled shell)

<!-- slide template=section -->
# 4. A Survey of Chemical Properties

<!-- slide -->
## Group trends and diagonal relationships
- Same group → similar valence config (e.g., ns1) → similar chemistry
- Most reliable for 1A/2A (metals) and 7A/8A (nonmetals)
- Diagonal relationship: Li~Mg, Be~Al, B~Si

<!-- slide -->
## Alkali metal reactivity
![Sodium and water](../assets/sodium_water.png =340x)
Low ionization energy → violent reaction with water

<!-- slide -->
## Quick group survey
- 1A: low IE, reacts with water
- 2A: forms $\text{M}^{2+}$, reactivity increases down group
- 7A (halogens): high IE, large positive EA, forms $X^-$
- 8A: highest IE, essentially unreactive

<!-- slide -->
## Oxides across period 3
![Oxide character from basic to acidic](../assets/oxide_character_period3.svg =820x)
Metal oxide → basic · nonmetal oxide → acidic · $\mathrm{Al_2O_3}$ on the boundary → amphoteric

<!-- slide -->
## Oxide acidity and basicity
- Metal oxides: generally **basic** ($\ce{Na2O}$, $\ce{MgO}$)
- Nonmetal oxides: generally **acidic** ($\ce{SO3}$, $\ce{Cl2O7}$)
- $\ce{Al2O3}$: **amphoteric** — reacts with both acids and bases

<!-- slide template=closing -->
# The periodic table as a predictive map
Effective nuclear charge, built from electron configuration, explains radius, ionization energy, and electron affinity trends in one unified logic — and those trends explain every group's observed chemical behavior, from alkali-metal reactivity to oxide acidity.
