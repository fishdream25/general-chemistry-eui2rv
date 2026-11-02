{{nyml
kind: document
carrier: slides
uid: doc-701vs3kkmi7k9otj
title: Chapter 19: Nuclear Chemistry
ratio: 16:9
theme: paper
}}

<!-- slide template=title -->
# Nuclear Chemistry
## Where chemistry meets the nucleus
**General Chemistry, Chapter 19**

<!-- slide 2col -->
## Chapter Learning Objectives
<!-- @left -->
- **Objective 19.1a** — Distinguish decay types and balance nuclear equations
- **Objective 19.1b** — Identify patterns of nuclear stability
- **Objective 19.1c** — Calculate nuclear binding energy from mass defect
- **Objective 19.2a** — Identify types of radioactive decay
- **Objective 19.2b** — Explain radiocarbon dating
<!-- @right -->
- **Objective 19.2c** — Apply first-order kinetics to radioactive decay
- **Objective 19.3a** — Explain nuclear fission, chain reactions, and critical mass
- **Objective 19.3b** — Explain nuclear fusion and its requirements
- **Objective 19.3c** — Explain why fission and fusion both release energy

<!-- slide template=outline -->
## Roadmap
1. The nature of nuclear reactions
2. Radioactive decay
3. Nuclear fission and nuclear fusion

<!-- slide -->
## Chapter Logic
{{mermaid
graph TD
  A["Z and A notation (Ch. 2):<br/>balance nuclear equations"] --> B["Nuclear stability and binding energy:<br/>mass defect, E=mc^2"]
  B --> C["Radioactive decay:<br/>types plus first-order kinetics (Ch. 13)"]
  B --> D["Fission and fusion:<br/>move toward higher binding energy per nucleon"]
}}
**Visual description:** atomic notation lets you balance nuclear equations. Binding energy quantifies stability, explaining both radioactive decay and why fission/fusion release energy.

<!-- slide template=section -->
# 1. The Nature of Nuclear Reactions

<!-- slide -->
## Notation and conservation rules
$$\ce{^{A}_{Z}X}$$
- Radioactive decay: spontaneous. Nuclear transmutation: induced by bombardment.
- Nuclear equations conserve MASS NUMBER and CHARGE — not atom identity

<!-- slide step -->
## Worked example — balancing
$\ce{^{125}_{53}I}$ captures an electron
- Mass: 125+0=125. Charge: 53−1=52 (Te){{attrs[.fragment]}}
- **$\ce{^{125}_{53}I + ^0_{-1}e -> ^{125}_{52}Te}$**{{attrs[.fragment]}}

<!-- slide -->
## The band of stability
![Band of stability](../assets/band_of_stability.svg =560x)

<!-- slide -->
## Nuclear stability patterns
:::warning
Magic numbers (2,8,20,28,50,82,126) are extra-stable. Even-even nuclei > odd-odd. EVERY isotope with Z>83 is radioactive.
:::

<!-- slide -->
## Binding energy: $E = mc^2$
$$\Delta m = (\text{mass of parts}) - (\text{atomic mass}) \qquad \Delta E = (\Delta m)c^2$$
Larger (more positive) binding energy per nucleon → more stable nucleus

<!-- slide step -->
## Worked example — Fe-56 binding energy
Atomic mass 55.9349 amu
- $\Delta m = 55.9349 - 56.4651 = -0.5302$ amu{{attrs[.fragment]}}
- $\Delta E = -7.913\times10^{-11}$ J/nucleus = −494 MeV/nucleus{{attrs[.fragment]}}
- **−8.82 MeV/nucleon**{{attrs[.fragment]}}

<!-- slide template=section -->
# 2. Radioactive Decay

<!-- slide -->
## Types of decay
| Type | Emission |
|---|---|
| Alpha | $^4_2He$ nucleus |
| Beta | electron |
| Positron | positron |
| Electron capture | captures $\ce{e-}$ |
| Spontaneous fission | splits + neutrons |

<!-- slide main-side -->
## Which decay, and why
<!-- @main -->
![How each decay mode moves a nuclide on the neutron-proton chart, and which mode a nuclide chooses](../assets/decay_modes_nz.svg =760x)
<!-- @side -->
A nucleus decays in whichever way moves it **toward the band**.

- above the band (neutron-rich) → **$\beta^-$**
- below the band (proton-rich) → **$\beta^+$ or EC**
- $Z > 83$ (too big) → **α**

Locate $N$ vs. $Z$ relative to the band of stability first; the mode follows.

<!-- slide -->
## Always first-order — reuse Ch. 13 exactly
$$\ln\frac{N_0}{N}=kt \qquad t_{1/2}=\frac{\ln2}{k}$$
Nothing new mathematically — N replaces concentration

<!-- slide -->
## Radiocarbon dating
![Carbon-14 decay](../assets/carbon14_decay.svg =560x)

<!-- slide step -->
## Worked example — Dead Sea Scrolls
Activity 10.8 (now) vs. 13.6 (fresh) disintegrations/min/g, t½=5730 y
- k = ln2/5730 = $1.210\times10^{-4}\ \text{y}^{-1}${{attrs[.fragment]}}
- t = ln(13.6/10.8)/k{{attrs[.fragment]}}
- **t ≈ 1900 years**{{attrs[.fragment]}}

<!-- slide template=section -->
# 3. Nuclear Fission and Nuclear Fusion

<!-- slide -->
## Fission: heavy nuclei split
$$\ce{^235_92U + ^1_0n -> ^90_38Sr + ^143_54Xe + 3\,^1_0n}$$
1 neutron captured, 3 released → CHAIN REACTION if critical mass is present

<!-- slide main-side -->
## Chain reaction, and critical mass
<!-- @main -->
![The branching structure of a fission chain reaction, and subcritical versus critical samples](../assets/fission_chain_reaction.svg =760x)
<!-- @side -->
One neutron in, three out (in this example; typically 2–3), and if every neutron triggers another fission — so fissions go **1, 3, 9, 27**, growing as $3^n$.

Whether that happens depends on **capture versus escape**.

**Critical mass** is the minimum mass at which enough neutrons are captured, rather than escaping, to keep the chain going. It is a *condition*, not a constant — shape, density and purity all change it.

<!-- slide -->
## Why both fission AND fusion release energy
![Binding energy curve](../assets/binding_energy_curve.svg =620x)
Both move nuclei TOWARD the Fe-56 peak — from opposite directions

<!-- slide -->
## Fission in practice
![Nuclear power plant](../assets/nuclear_power_plant.jpg =520x)
Atomic bomb: 2 subcritical pieces merge, explosive chain reaction. Reactor: subcritical fuel rods assembled into a critical core + control rods, mild controlled fission.

<!-- slide -->
## Fusion: light nuclei combine
$$\ce{^1_1H + ^2_1H -> ^3_2He} \qquad \ce{^1_1H + ^1_1H -> ^2_1H + ^0_{+1}\beta}$$
Requires extremely high temperature to overcome electrostatic repulsion between the positively charged nuclei

<!-- slide -->
## Fusion in the Sun
![The Sun](../assets/the_sun.jpg =460x)
In the Sun's core, H fuses into He at ~15 million K — the Sun's energy source; fusion of hydrogen isotopes (deuterium and tritium) into He is the basis of a hydrogen bomb.

<!-- slide template=closing -->
# The course's last idea, and its first
Nuclear stability (binding energy per nucleon) explains decay, fission, and fusion (equation balancing rests on conservation of mass number and atomic number) — while decay's kinetics reuse Chapter 13's first-order rate law completely unchanged. A fitting close: this course's very last calculation is its earliest kinetics tool, applied one final time.
