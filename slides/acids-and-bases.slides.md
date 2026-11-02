{{nyml
kind: document
carrier: slides
uid: doc-vj5sqjpxidfbe5bf
title: Chapter 15: Acids and Bases
ratio: 16:9
theme: paper
}}

<!-- slide template=title -->
# Acids and Bases
## The chemistry of H⁺
**General Chemistry, Chapter 15**

<!-- slide 2col -->
## Chapter Learning Objectives
<!-- @left -->
- **Objective 15.1a** — Identify conjugate acid-base pairs and diprotic acid ionization steps
- **Objective 15.1b** — Calculate pH/pOH and recognize strong/weak acids and bases
- **Objective 15.2a** — Explain hydrohalic acid and oxoacid strength trends
- **Objective 15.2b** — Predict salt solution acidity and classify oxides
- **Objective 15.3a** — Identify Lewis acids and bases
<!-- @right -->
- **Objective 15.4a** — Calculate pH for strong acid/base solutions
- **Objective 15.4b** — Calculate pH for weak acid/base solutions and percent ionization
- **Objective 15.4c** — Calculate equilibrium concentrations for a diprotic/polyprotic acid
- **Objective 15.4d** — Calculate the pH of a salt solution using hydrolysis

<!-- slide template=outline -->
## Roadmap
1. General concepts
2. Structure and property correlation
3. Lewis acids and bases
4. pH related calculations

<!-- slide -->
## Chapter Logic
{{mermaid
graph TD
  A["Conjugate acid-base pairs<br/>Water autoionization: Kw"] --> B["Strong vs. weak<br/>acids/bases"]
  B --> C["WHY acids differ:<br/>structure-property trends"]
  A --> D["Lewis acid-base theory<br/>(generalizes Bronsted)"]
  B --> E["pH calculations:<br/>strong, weak, polyprotic, salts"]
  C --> E
}}
**Visual description:** conjugate pairs and Kw establish vocabulary; strong/weak classification and structure-property trends build toward pH calculations, while Lewis theory branches off as a generalization of Brønsted theory.

<!-- slide template=section -->
# 1. General Concepts

<!-- slide -->
## Conjugate acid-base pairs
- Brønsted acid = proton donor; base = proton acceptor
- Acid loses H⁺ → conjugate base. Base gains H⁺ → conjugate acid
- Every Brønsted acid–base reaction has exactly TWO conjugate pairs

<!-- slide step -->
## Worked example — identify the pairs
CH₃COOH + H₂O ⇌ CH₃COO⁻ + H₃O⁺
- CH₃COOH (acid) / CH₃COO⁻ (its conjugate base){{attrs[.fragment]}}
- H₂O (base) / H₃O⁺ (its conjugate acid){{attrs[.fragment]}}

<!-- slide -->
## Diprotic acids: stepwise ionization
H₂CO₃ + H₂O ⇌ H₃O⁺ + HCO₃⁻ (K_a1), then HCO₃⁻ + H₂O ⇌ H₃O⁺ + CO₃²⁻ (K_a2)
- Each step has its OWN equilibrium constant

<!-- slide -->
## Acid-base indicators
![Litmus paper](../assets/litmus_paper_test.jpg =560x)

<!-- slide -->
## Water's autoionization
$$K_w=[H^+][OH^-]=1.0\times10^{-14}\ (25°C)$$
$$pH=-\log[H^+] \quad pOH=-\log[OH^-] \quad pH+pOH=14\ (25°C)$$

<!-- slide step -->
## Worked example — pH from [OH⁻]
[OH⁻] = 2.5×10⁻³ M
- $[H^+]=K_w/[OH^-]=4.0\times10^{-12}$ M{{attrs[.fragment]}}
- **pH = 11.40, pOH = 2.60**{{attrs[.fragment]}}

<!-- slide -->
## Strong vs. weak — memorize the short list
:::warning
Strong acids: HClO₄, HI, HBr, HCl, H₂SO₄, HNO₃. Everything else common (HF, HNO₂, CH₃COOH, HCN...) is weak. Weak bases are mainly amines (NH₃ and relatives).
:::

<!-- slide main-side -->
## “Strong” is not “concentrated”
<!-- @main -->
![Two beakers of equally concentrated acid: the strong acid fully ionized, the weak acid almost entirely intact](../assets/strong_vs_weak_ionization.svg =720x)
<!-- @side -->
**Strong** = how *completely* it ionizes.

**Concentrated** = how *much* is there.

They are independent — 0.001 M HCl is a dilute strong acid; 15 M acetic acid is a concentrated weak one.

<!-- slide main-side -->
## Conjugates, and water's limits
<!-- @main -->
![A ladder of acids paired with conjugate bases, with H3O+ and OH- marked as water's limits](../assets/conjugate_strength_ladder.svg =760x)
<!-- @side -->
Read a row across: **stronger acid → weaker conjugate base**.

The two purple rows are water's own two conjugate pairs (H₃O⁺/H₂O and H₂O/OH⁻).

No acid stronger than H₃O⁺ and no base stronger than OH⁻ survives in water — the **leveling effect**.

<!-- slide template=section -->
# 2. Structure and Property Correlation

<!-- slide -->
## Hydrohalic acids: weaker bond → stronger acid
![Hydrohalic acids](../assets/hydrohalic_acids_grid.svg =620x)
HF ≪ HCl < HBr < HI

<!-- slide -->
## Oxoacids: two distinct trends
- Same oxidation number, different central atom → more electronegative atom = stronger acid (HClO₃ > HBrO₃)
- Same central atom, more oxygens → stronger acid (HClO₄ > HClO₃ > HClO₂ > HClO)

<!-- slide -->
## Oxoacid strength vs. oxygen count
![Oxoacid strength trend](../assets/oxoacid_strength_trend.svg =540x)

<!-- slide -->
## Salt solutions: acidic, basic, or neutral?
| Parent acid | Parent base | Solution |
|---|---|---|
| Strong | Strong | Neutral |
| Weak | Strong | Basic |
| Strong | Weak | Acidic |
| Weak | Weak | Compare Ka, Kb |

<!-- slide step -->
## Worked example — classify three salts
NaBr, NaF, NH₄Cl
- NaBr: strong + strong → **neutral**{{attrs[.fragment]}}
- NaF: weak acid (HF) + strong base → **basic**{{attrs[.fragment]}}
- NH₄Cl: strong acid + weak base (NH₃) → **acidic**{{attrs[.fragment]}}

<!-- slide -->
## Acidic, basic, and amphoteric oxides
- Basic oxide + water → hydroxide: Na₂O + H₂O → 2NaOH
- Acidic oxide + water → acid: SO₃ + H₂O → H₂SO₄
- Amphoteric (e.g. Al₂O₃): reacts as acid OR base depending on partner

<!-- slide template=section -->
# 3. Lewis Acids and Bases

<!-- slide -->
## Beyond proton transfer
- **Lewis base** = electron-pair donor
- **Lewis acid** = electron-pair acceptor
- Generalizes Brønsted theory — no H⁺ transfer required

<!-- slide main-side -->
## One electron pair, moving
<!-- @main -->
![Three Lewis acid-base reactions drawn as an electron pair moving from a lone pair to an empty orbital](../assets/lewis_acid_base.svg =700x)
<!-- @side -->
Find the **lone pair that is donated** — that species is the base.

Find the **electron-poor atom** — that one is the acid.

None of these three reactions moves a proton, so Brønsted has nothing to say about them.

<!-- slide -->
## How the two definitions nest
- Every Brønsted base **is** a Lewis base — accepting H⁺ *is* donating a lone pair
- Not every Lewis acid is a Brønsted acid — BF₃ has no proton to give
- **Brønsted acidity is the special case where the acceptor is H⁺**

Spotting a Lewis acid: incomplete octet (BF₃, AlCl₃) · metal cation (Al³⁺, Fe³⁺) · polar multiple bond (CO₂, SO₃)

<!-- slide step -->
## Worked example — Lewis acid/base
(a) CO₂ + OH⁻ → HCO₃⁻. (b) AlCl₃ + Cl⁻ → AlCl₄⁻
- (a) OH⁻ = Lewis base; CO₂ = **Lewis acid**{{attrs[.fragment]}}
- (b) Cl⁻ = Lewis base; AlCl₃ = **Lewis acid**{{attrs[.fragment]}}
- Neither reaction transfers a proton{{attrs[.fragment]}}

<!-- slide template=section -->
# 4. pH Related Calculations

<!-- slide -->
## The pH scale
![pH scale](../assets/ph_scale.svg =820x)

<!-- slide -->
## Strong acids/bases: no ICE table needed
- [H⁺] or [OH⁻] = initial concentration directly (complete ionization; for monoprotic acids and bases with one OH⁻)
:::warning
For a base like B(OH)₂, [OH⁻] is DOUBLE the initial concentration.
:::

<!-- slide step -->
## Worked example — weak acid (HF)
0.50 M HF, K_a = 7.1×10⁻⁴
- $x^2/(0.50-x)=7.1\times10^{-4} \Rightarrow x=0.0185$ M{{attrs[.fragment]}}
- **pH = 1.73, percent ionization = 3.7%**{{attrs[.fragment]}}

<!-- slide step -->
## Worked example — weak base (NH₃)
0.40 M NH₃, K_b = 1.8×10⁻⁵
- $x^2/(0.40-x)=1.8\times10^{-5} \Rightarrow [OH^-]=0.00268$ M{{attrs[.fragment]}}
- **pOH = 2.57 → pH = 11.43**{{attrs[.fragment]}}

<!-- slide step -->
## Worked example — diprotic acid
0.10 M H₂C₂O₄, K_a1=6.5×10⁻², K_a2=6.1×10⁻⁵
- Step 1: [H⁺]=[HC₂O₄⁻]=0.054 M{{attrs[.fragment]}}
- Step 2 barely changes this: y ≈ 6.1×10⁻⁵ M{{attrs[.fragment]}}
- **[H⁺] set almost entirely by step 1**{{attrs[.fragment]}}

<!-- slide -->
## A natural pH indicator
![Red cabbage indicator](../assets/red_cabbage_indicator.jpg =620x)

<!-- slide step -->
## Worked example — salt hydrolysis
0.24 M CH₃COONa, K_b(CH₃COO⁻) = 5.6×10⁻¹⁰
- $x^2/(0.24-x)=5.6\times10^{-10} \Rightarrow [OH^-]=1.16\times10^{-5}$ M{{attrs[.fragment]}}
- **pOH = 4.94 → pH = 9.1**{{attrs[.fragment]}}

<!-- slide template=closing -->
# One toolkit, one new cast of species
Every pH calculation in this chapter — strong, weak, polyprotic, or salt — reuses Chapter 14's ICE-table method with a new K each time. This exact toolkit reappears unchanged in Chapter 16 for buffers, titrations, and solubility equilibria.
