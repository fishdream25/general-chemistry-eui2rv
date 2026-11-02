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
## The chemistry of $\ce{H+}$
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
**Visual description:** conjugate pairs and $K_w$ establish vocabulary; strong/weak classification and structure-property trends build toward pH calculations, while Lewis theory branches off as a generalization of Brønsted theory.

<!-- slide template=section -->
# 1. General Concepts

<!-- slide -->
## Conjugate acid-base pairs
- Brønsted acid = proton donor; base = proton acceptor
- Acid loses $\ce{H+}$ → conjugate base. Base gains $\ce{H+}$ → conjugate acid
- Every Brønsted acid–base reaction has exactly TWO conjugate pairs

<!-- slide step -->
## Worked example — identify the pairs
$\ce{CH3COOH + H2O <=> CH3COO- + H3O+}$
- $\ce{CH3COOH}$ (acid) / $\ce{CH3COO-}$ (its conjugate base){{attrs[.fragment]}}
- $\ce{H2O}$ (base) / $\ce{H3O+}$ (its conjugate acid){{attrs[.fragment]}}

<!-- slide -->
## Diprotic acids: stepwise ionization
$\ce{H2CO3 + H2O <=> H3O+ + HCO3-}$ ($K_{a1}$), then $\ce{HCO3- + H2O <=> H3O+ + CO3^2-}$ ($K_{a2}$)
- Each step has its OWN equilibrium constant

<!-- slide -->
## Acid-base indicators
![Litmus paper](../assets/litmus_paper_test.jpg =560x)

<!-- slide -->
## Water's autoionization
$$K_w=[H^+][OH^-]=1.0\times10^{-14}\ (25°C)$$
$$pH=-\log[H^+] \quad pOH=-\log[OH^-] \quad pH+pOH=14\ (25°C)$$

<!-- slide step -->
## Worked example — pH from $[\ce{OH-}]$
$[\ce{OH-}] = 2.5\times10^{-3}$ M
- $[H^+]=K_w/[OH^-]=4.0\times10^{-12}$ M{{attrs[.fragment]}}
- **pH = 11.40, pOH = 2.60**{{attrs[.fragment]}}

<!-- slide -->
## Strong vs. weak — memorize the short list
:::warning
Strong acids: $\ce{HClO4}$, $\ce{HI}$, $\ce{HBr}$, $\ce{HCl}$, $\ce{H2SO4}$, $\ce{HNO3}$. Everything else common ($\ce{HF}$, $\ce{HNO2}$, $\ce{CH3COOH}$, $\ce{HCN}$...) is weak. Weak bases are mainly amines ($\ce{NH3}$ and relatives).
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

The two purple rows are water's own two conjugate pairs ($\ce{H3O+}/\ce{H2O}$ and $\ce{H2O}/\ce{OH-}$).

No acid stronger than $\ce{H3O+}$ and no base stronger than $\ce{OH-}$ survives in water — the **leveling effect**.

<!-- slide template=section -->
# 2. Structure and Property Correlation

<!-- slide -->
## Hydrohalic acids: weaker bond → stronger acid
![Hydrohalic acids](../assets/hydrohalic_acids_grid.svg =620x)
HF ≪ HCl < HBr < HI

<!-- slide -->
## Oxoacids: two distinct trends
- Same oxidation number, different central atom → more electronegative atom = stronger acid ($\ce{HClO3} > \ce{HBrO3}$)
- Same central atom, more oxygens → stronger acid ($\ce{HClO4} > \ce{HClO3} > \ce{HClO2} > \ce{HClO}$)

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
| Weak | Weak | Compare $K_a$, $K_b$ |

<!-- slide step -->
## Worked example — classify three salts
$\ce{NaBr}$, $\ce{NaF}$, $\ce{NH4Cl}$
- $\ce{NaBr}$: strong + strong → **neutral**{{attrs[.fragment]}}
- NaF: weak acid (HF) + strong base → **basic**{{attrs[.fragment]}}
- $\ce{NH4Cl}$: strong acid + weak base ($\ce{NH3}$) → **acidic**{{attrs[.fragment]}}

<!-- slide -->
## Acidic, basic, and amphoteric oxides
- Basic oxide + water → hydroxide: $\ce{Na2O + H2O -> 2NaOH}$
- Acidic oxide + water → acid: $\ce{SO3 + H2O -> H2SO4}$
- Amphoteric (e.g. $\ce{Al2O3}$): reacts as acid OR base depending on partner

<!-- slide template=section -->
# 3. Lewis Acids and Bases

<!-- slide -->
## Beyond proton transfer
- **Lewis base** = electron-pair donor
- **Lewis acid** = electron-pair acceptor
- Generalizes Brønsted theory — no $\ce{H+}$ transfer required

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
- Every Brønsted base **is** a Lewis base — accepting $\ce{H+}$ *is* donating a lone pair
- Not every Lewis acid is a Brønsted acid — $\ce{BF3}$ has no proton to give
- **Brønsted acidity is the special case where the electron-pair acceptor is $\ce{H+}$**

Spotting a Lewis acid: incomplete octet ($\ce{BF3}$, $\ce{AlCl3}$) · metal cation ($\ce{Al3+}$, $\ce{Fe3+}$) · polar multiple bond ($\ce{CO2}$, $\ce{SO3}$)

<!-- slide step -->
## Worked example — Lewis acid/base
(a) $\ce{CO2 + OH- -> HCO3-}$. (b) $\ce{AlCl3 + Cl- -> AlCl4-}$
- (a) $\ce{OH-}$ = Lewis base; $\ce{CO2}$ = **Lewis acid**{{attrs[.fragment]}}
- (b) $\ce{Cl-}$ = Lewis base; $\ce{AlCl3}$ = **Lewis acid**{{attrs[.fragment]}}
- Neither reaction transfers a proton{{attrs[.fragment]}}

<!-- slide template=section -->
# 4. pH Related Calculations

<!-- slide -->
## The pH scale
![pH scale](../assets/ph_scale.svg =820x)

<!-- slide -->
## Strong acids/bases: no ICE table needed
- $[\ce{H+}]$ or $[\ce{OH-}]$ = initial concentration directly (complete ionization; for monoprotic acids and bases with one $\ce{OH-}$)
:::warning
For a base like $\ce{B(OH)2}$, $[\ce{OH-}]$ is DOUBLE the initial concentration.
:::

<!-- slide step -->
## Worked example — weak acid (HF)
0.50 M HF, $K_a = 7.1\times10^{-4}$
- $x^2/(0.50-x)=7.1\times10^{-4} \Rightarrow x=0.0185$ M{{attrs[.fragment]}}
- **pH = 1.73, percent ionization = 3.7%**{{attrs[.fragment]}}

<!-- slide step -->
## Worked example — weak base ($\ce{NH3}$)
0.40 M $\ce{NH3}$, $K_b = 1.8\times10^{-5}$
- $x^2/(0.40-x)=1.8\times10^{-5} \Rightarrow [OH^-]=0.00268$ M{{attrs[.fragment]}}
- **pOH = 2.57 → pH = 11.43**{{attrs[.fragment]}}

<!-- slide step -->
## Worked example — diprotic acid
0.10 M $\ce{H2C2O4}$, $K_{a1} = 6.5\times10^{-2}$, $K_{a2} = 6.1\times10^{-5}$
- Step 1: $[\ce{H+}] = [\ce{HC2O4-}] = 0.054$ M{{attrs[.fragment]}}
- Step 2 barely changes this: y ≈ $6.1\times10^{-5}$ M{{attrs[.fragment]}}
- **$[\ce{H+}]$ set almost entirely by step 1**{{attrs[.fragment]}}

<!-- slide -->
## A natural pH indicator
![Red cabbage indicator](../assets/red_cabbage_indicator.jpg =620x)

<!-- slide step -->
## Worked example — salt hydrolysis
0.24 M $\ce{CH3COONa}$, $K_b(\ce{CH3COO-}) = 5.6\times10^{-10}$
- $x^2/(0.24-x)=5.6\times10^{-10} \Rightarrow [OH^-]=1.16\times10^{-5}$ M{{attrs[.fragment]}}
- **pOH = 4.94 → pH = 9.1**{{attrs[.fragment]}}

<!-- slide template=closing -->
# One toolkit, one new cast of species
Every pH calculation in this chapter — strong, weak, polyprotic, or salt — reuses Chapter 14's ICE-table method with a new K each time. This exact toolkit reappears unchanged in Chapter 16 for buffers, titrations, and solubility equilibria.
