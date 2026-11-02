{{nyml
kind: document
carrier: slides
uid: doc-p0shf3h13ks4opnm
title: Chapter 16: Acid-Base Equilibria and Solubility Equilibria
ratio: 16:9
theme: small-press
}}

<!-- slide template=title -->
# Acid-Base Equilibria
## Buffers, titrations, and solubility
**General Chemistry, Chapter 16**

<!-- slide 2col -->
## Chapter Learning Objectives
<!-- @left -->
- **Objective 16.1a** — Explain buffer action and calculate buffer pH
- **Objective 16.1b** — Calculate buffer pH after a stress, and design a buffer at a target pH
- **Objective 16.2a** — Describe titration pH behavior by acid/base strength combination
- **Objective 16.2b** — Calculate pH at any point during a titration
- **Objective 16.2c** — Select an appropriate acid-base indicator
<!-- @right -->
- **Objective 16.3a** — Write Ksp expressions and convert between Ksp and molar solubility
- **Objective 16.3b** — Predict precipitation by comparing Q to Ksp
- **Objective 16.3c** — Calculate solubility with a common ion present
- **Objective 16.4a** — Define complex ion/formation constant and solve Kf problems

<!-- slide template=outline -->
## Roadmap
1. Buffer solutions
2. Titrations
3. Solubility equilibria
4. Complex equilibria

<!-- slide -->
## Chapter Logic
{{mermaid
graph TD
  A["Buffers: weak acid/base<br/>+ its conjugate"] --> B["Henderson-Hasselbalch:<br/>pH = pKa + log(base/acid)"]
  B --> C["Titrations: buffer region,<br/>equivalence point, excess titrant"]
  D["Ksp: same K/Q framework,<br/>applied to dissolution"] --> E["Common ion effect<br/>(Le Chatelier, Ch 14)"]
  C -.reuses ICE tables.-> D
  D --> F["Complex ions:<br/>Kf, same framework again"]
}}
**Visual description:** buffers lead to Henderson-Hasselbalch, extended across a titration curve. Ksp applies the same K/Q framework to dissolution, including the common-ion effect. Complex ions (Kf) close the chapter.

<!-- slide template=section -->
# 1. Buffer Solutions

<!-- slide -->
## Why buffers resist pH change
- Weak acid + its conjugate base, BOTH present at once
- Acid component neutralizes added OH⁻
- Base component neutralizes added H⁺

<!-- slide main-side -->
## Two reservoirs — and a limit
<!-- @main -->
![The buffer's two reservoirs and a computed pH curve showing the buffer holding and then failing](../assets/buffer_action.svg =740x)
<!-- @side -->
The acid reservoir eats added OH⁻; the base reservoir eats added H⁺.

0.10 mol HCl into 1.0 L: buffer **4.74 → 4.65**, pure water **7.00 → 1.00**.

Past 1.0 mol of added HCl every acetate is gone — **capacity exceeded**, and the curve falls off a cliff.

<!-- slide step -->
## Worked example — buffer pH (ICE table)
1.0 M CH₃COOH + 1.0 M CH₃COONa, K_a = 1.8×10⁻⁵
- $x(1.0+x)/(1.0-x)=1.8\times10^{-5} \Rightarrow x=1.8\times10^{-5}$ M{{attrs[.fragment]}}
- **pH = 4.74**{{attrs[.fragment]}}

<!-- slide -->
## The Henderson-Hasselbalch shortcut
$$pH = pK_a + \log\frac{[\text{conjugate base}]}{[\text{acid}]}$$
Same Ka expression, rearranged — skips the ICE table when "x is small" already holds.

<!-- slide step -->
## Worked example — HH, then add HCl
Same buffer. Add 0.10 mol HCl to 1.0 L.
- Original: pH = pKa + log(1.0/1.0) = 4.74{{attrs[.fragment]}}
- After HCl: [CH₃COO⁻]=0.90, [CH₃COOH]=1.1{{attrs[.fragment]}}
- **pH = 4.74 + log(0.90/1.1) = 4.65** (vs. pH 7→1 in pure water!){{attrs[.fragment]}}

<!-- slide step -->
## Worked example — designing a buffer
0.750 L of 0.100 M NH₃, target pH 9.30. K_b(NH₃)=1.8×10⁻⁵
- pKa(NH₄⁺) = 9.25{{attrs[.fragment]}}
- [NH₃]/[NH₄⁺] = 10^0.05 = 1.12 → [NH₄⁺]=0.0893 M{{attrs[.fragment]}}
- **mass NH₄Cl = 0.0670 mol × 53.5 g/mol = 3.58 g**{{attrs[.fragment]}}

<!-- slide template=section -->
# 2. Titrations

<!-- slide -->
## Titration curves: strong vs. weak acid
![Titration curves](../assets/titration_curves.svg =680x)

<!-- slide -->
## Equivalence pH is not always 7
| Titration | Left at equivalence | pH |
|---|---|---|
| strong acid + strong base | neutral salt | **= 7** |
| weak acid + strong base | conjugate **base** | **> 7** |
| strong acid + weak base | conjugate **acid** | **< 7** |

At **half**-equivalence, $[\mathrm{A^-}]=[\mathrm{HA}]$ and $\mathrm{pH}=\mathrm{p}K_a$ — the standard way to measure an unknown $K_a$.

<!-- slide -->
## Three regions, three methods
1. Before equivalence: Henderson-Hasselbalch (weak-strong)
2. At equivalence: pH=7 (strong-strong) or salt hydrolysis (weak-strong)
3. After equivalence: excess strong titrant, direct calculation

<!-- slide step -->
## Worked example — strong acid + strong base
25.0 mL 0.100 M HCl + 0.100 M NaOH: 10.0, 25.0, 35.0 mL added
- 10.0 mL: [H⁺]=0.0428 M → **pH=1.37**{{attrs[.fragment]}}
- 25.0 mL: equal moles → **pH=7** (neutral salt){{attrs[.fragment]}}
- 35.0 mL: [OH⁻]=0.0167 M → **pH=12.2**{{attrs[.fragment]}}

<!-- slide step -->
## Worked example — weak acid + strong base
25.0 mL 0.100 M CH₃COOH (K_a=1.8×10⁻⁵) + same NaOH
- 10.0 mL (buffer region): pH = pKa+log(0.0010/0.0015) = **4.57**{{attrs[.fragment]}}
- 25.0 mL (equivalence): acetate hydrolyzes → **pH=8.72**{{attrs[.fragment]}}
- 35.0 mL (past equivalence): excess OH⁻ sets pH, same as strong acid titration → **pH=12.2**{{attrs[.fragment]}}

<!-- slide -->
## A titration endpoint
![Titration endpoint](../assets/titration_endpoint.jpg =380x)

<!-- slide -->
## Choosing an indicator
![Indicator ranges](../assets/indicator_ranges.svg =680x)
:::warning
The indicator's color-change range (≈pKa±1) must fall within the curve's STEEP region near equivalence.
:::

<!-- slide template=section -->
# 3. Solubility Equilibria

<!-- slide -->
## Ksp: the same K_c framework, new context
$$\text{AgCl(s)} \rightleftharpoons \text{Ag}^+\text{(aq)} + \text{Cl}^-\text{(aq)} \qquad K_{sp}=[Ag^+][Cl^-]$$
![Silver chloride precipitate](../assets/silver_chloride_precipitate.jpg =380x)

<!-- slide step -->
## Worked example — solubility → Ksp
Ca(OH)₂ solubility = 0.511 g/L (M = 74.1 g/mol)
- Molar solubility = 6.90×10⁻³ M{{attrs[.fragment]}}
- **K_sp = (6.90e-3)(2×6.90e-3)² = 1.31×10⁻⁶** (don't forget to double [OH⁻]!){{attrs[.fragment]}}

<!-- slide step -->
## Worked example — Ksp → solubility
CaCO₃, K_sp = 8.7×10⁻⁹ (1:1 salt)
- $[Ca^{2+}]=[CO_3^{2-}]=\sqrt{K_{sp}}=9.3\times10^{-5}$ M{{attrs[.fragment]}}
- **solubility = 9.3×10⁻³ g/L**{{attrs[.fragment]}}

<!-- slide step -->
## Worked example — will it precipitate?
Mix equal volumes of 2.0×10⁻⁴ M AgNO₃ and 2.0×10⁻⁴ M NaCl. K_sp(AgCl)=1.6×10⁻¹⁰
- After mixing: [Ag⁺]=[Cl⁻]=1.0×10⁻⁴ M{{attrs[.fragment]}}
- Q = 1.0×10⁻⁸ > K_sp{{attrs[.fragment]}}
- **Yes, AgCl precipitates**{{attrs[.fragment]}}

<!-- slide main-side -->
## The common ion effect, quantified
<!-- @main -->
![Molar solubility of AgCl falling by four orders of magnitude as chloride is added](../assets/common_ion_effect.svg =700x)
<!-- @side -->
Adding Cl⁻ is adding a **product** — the dissolution shifts left.

In 0.001 M Cl⁻: **79× less soluble**.

In 0.10 M Cl⁻: **7,900× less soluble**.

At a given temperature, $K_\mathrm{sp}$ itself never moves. Only the split between the two ions does.

<!-- slide step -->
## Worked example — common ion effect
Mn(OH)₂, K_sp=2×10⁻¹³. What pH limits [Mn²⁺] to 1.8×10⁻⁶ M?
- $[OH^-]=\sqrt{K_{sp}/[Mn^{2+}]}=3.3\times10^{-4}$ M{{attrs[.fragment]}}
- **pH = 10.5**{{attrs[.fragment]}}

<!-- slide template=section -->
# 4. Complex Equilibria

<!-- slide -->
## Complex ions and Kf
![Complex ion formation](../assets/complex_ion_formation.svg =600x)
Larger K_f → more stable complex

<!-- slide -->
## Amphoteric behavior, revisited
$$\ce{Al(OH)3(s) + 3H+ -> Al^3+ + 3H2O} \qquad \ce{Al(OH)3(s) + OH- <=> Al(OH)4-}$$
Same Al(OH)₃, acting as base (left) or acting as a (Lewis) acid by forming a complex (right)

<!-- slide template=closing -->
# One toolkit, four applications
Every calculation in this chapter — buffers, titrations, Ksp, or Kf — reuses Chapter 14's K/Q/ICE-table framework and Chapter 15's Ka/Kb toolkit. No new method, only new contexts.
