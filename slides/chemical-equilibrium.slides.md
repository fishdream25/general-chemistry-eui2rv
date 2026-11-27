{{nyml
kind: document
carrier: slides
uid: doc-bq37i1j3e946jwhx
title: Chapter 14: Chemical Equilibrium
ratio: 16:9
theme: paper
}}

<!-- slide template=title -->
# Chemical Equilibrium
## How far — and where does it stop?
**General Chemistry, Chapter 14**

<!-- slide 2col -->
## Chapter Learning Objectives
<!-- @left -->
- **Objective 14.1a** — Derive and apply $K = k_f/k_r$, including the effect of reversing a reaction
- **Objective 14.1b** — Interpret the magnitude of K
- **Objective 14.2a** — Write and convert $K_c/K_p$ for homogeneous gas-phase equilibria
- **Objective 14.2b** — Write equilibrium expressions for liquid-phase and heterogeneous equilibria
- **Objective 14.2c** — Combine equilibrium constants for multi-step reactions
<!-- @right -->
- **Objective 14.3a** — Calculate Q and compare to K to predict reaction direction
- **Objective 14.4a** — Set up and solve an ICE table for equilibrium concentrations
- **Objective 14.4b** — Apply and validate the small-x approximation
- **Objective 14.5a** — Apply Le Chatelier's principle across all stress types

<!-- slide template=outline -->
## Roadmap
1. Chemical equilibrium
2. Equilibrium constants
3. Reaction quotient
4. Equilibrium concentrations
5. Le Chatelier's principle

<!-- slide -->
## Chapter Logic
{{mermaid
graph TD
  A["Forward rate = reverse rate<br/>K = k_f/k_r (elementary step)"] --> B["K_c, K_p expressions<br/>(homogeneous & heterogeneous)"]
  B --> C["Reaction quotient Q<br/>compare Q to K"]
  C --> D["ICE tables:<br/>solve for equilibrium concentrations"]
  D --> E["Le Chatelier's principle:<br/>predict shifts under stress"]
}}
**Visual description:** forward-rate-equals-reverse-rate defines K; K's expression is built for homogeneous/heterogeneous cases; Q reuses that expression to diagnose direction; ICE tables solve for unknowns; Le Chatelier predicts qualitative shifts.

<!-- slide template=section -->
# 1. Chemical Equilibrium

<!-- slide -->
## Dynamic equilibrium: rate_f = rate_r
- Concentrations stop changing — but BOTH reactions still occur, at equal rates
- For an elementary (single-step) reaction: $k_f[A]^a[B]^b = k_r[C]^c[D]^d \Rightarrow K = \dfrac{[C]^c[D]^d}{[A]^a[B]^b} = \dfrac{k_f}{k_r}$
- Reversing the reaction inverts K
- K ≫ 1 → favors products; K ≪ 1 → favors reactants

<!-- slide -->
## What K's magnitude means
![K magnitude schematic](../assets/k_magnitude_schematic.svg =620x)

<!-- slide step -->
## Worked example — K from rate constants
A ⇌ B, $k_f = 0.20\ \text{s}^{-1}$, $k_r = 0.05\ \text{s}^{-1}$
- (a) $K=k_f/k_r=4.0$ → favors B{{attrs[.fragment]}}
- (b) Reverse reaction: $K=1/4.0=0.25${{attrs[.fragment]}}

<!-- slide -->
## Reaching dynamic equilibrium
![Approach to equilibrium](../assets/approach_to_equilibrium.svg =520x)

<!-- slide template=section -->
# 2. Equilibrium Constants

<!-- slide -->
## Homogeneous equilibria (gas phase)
$$K_p=K_c(RT)^{\Delta n}, \quad \Delta n=(c+d)-(a+b)$$
- Same phase throughout; $K_c$ (concentrations) or $K_p$ (partial pressures)
- Convert between them via the ideal gas law (Ch. 5)

<!-- slide step -->
## Worked example — $K_p$ ↔ $K_c$
$\ce{2NH3 <=> N2 + 3H2}$, $K_p = 15.6$ at 217°C (490 K)
- $\Delta n = (1+3)-2=2${{attrs[.fragment]}}
- $K_c=K_p(RT)^{-\Delta n}=15.6\times(0.0821\times490)^{-2}${{attrs[.fragment]}}
- **$K_c = 0.00964$**{{attrs[.fragment]}}

<!-- slide -->
## Liquid-phase & heterogeneous equilibria
- Liquid phase: only $K_c$; excess solvent absorbed into the constant
- **Heterogeneous:** pure solids/liquids OMITTED — their "concentration" never changes

<!-- slide step -->
## Worked example — pure solid omitted
$\ce{CaCO3(s) <=> CaO(s) + CO2(g)}$, equilibrium $\ce{P(CO2)} = 0.220$ atm
- $K_p = P_{\text{CO}_2} = 0.220$ ($\ce{CaCO3}$, $\ce{CaO}$ don't appear){{attrs[.fragment]}}
- **Adding more $\ce{CaCO3(s)}$ does NOT change this pressure**{{attrs[.fragment]}}

<!-- slide step -->
## Worked example — multi-step reactions
$K_3$ for reaction 3, where reaction 3 = reaction 1 + reaction 2
- $K_{c1} = 490$, $K_{c2} = 0.0149${{attrs[.fragment]}}
- **$K_{c3} = K_{c1} \times K_{c2} = 7.30$** (equilibrium's Hess's law){{attrs[.fragment]}}

<!-- slide template=section -->
# 3. Reaction Quotient

<!-- slide -->
## Q uses the SAME expression as K
- Q: whatever concentrations you're given (often NOT at equilibrium)
- K: equilibrium concentrations only

| Comparison | Direction |
|---|---|
| Q > K | Reverse (right→left) |
| Q = K | At equilibrium |
| Q < K | Forward (left→right) |

<!-- slide -->
## Q and K live on the same axis
![A number line with K marked and the shift direction shown for Q below and above it](../assets/q_versus_k.svg =1000x)
The system always moves so that $Q$ travels toward $K$. That single sentence replaces memorizing three cases.

<!-- slide step -->
## Worked example — Q vs K
$\ce{2SO2 + O2 <=> 2SO3}$, $K_c = 4.3$ (from equilibrium data)
- New mixture: $[\ce{SO2}] = 1.9$, $[\ce{O2}] = 0.17$, $[\ce{SO3}] = 0.61${{attrs[.fragment]}}
- $Q_c = 0.61^2/(1.9^2\times0.17) = 0.61${{attrs[.fragment]}}
- **$Q_c < K_c$ → proceeds forward**{{attrs[.fragment]}}

<!-- slide step -->
## Worked example — the OTHER direction
Same reaction, $K_c = 4.3$. Mixture: $[\ce{SO2}] = 0.40$, $[\ce{O2}] = 0.20$, $[\ce{SO3}] = 2.5$
- $Q_c = 2.5^2/(0.40^2\times0.20) = 195${{attrs[.fragment]}}
- **$Q_c \gg K_c$ → proceeds in REVERSE**{{attrs[.fragment]}}

<!-- slide template=section -->
# 4. Equilibrium Concentrations

<!-- slide -->
## The ICE table
| | A | B | C | D |
|---|---|---|---|---|
| Initial | $[\text{A}]_0$ | $[\text{B}]_0$ | 0 | 0 |
| Change | −ax | −bx | +cx | +dx |
| Equilibrium | $[\text{A}]_0 - ax$ | $[\text{B}]_0 - bx$ | $cx$ | $dx$ |
- Substitute Equilibrium row into K, solve for x

<!-- slide step -->
## Worked example — perfect-square case
$\ce{CH3COOH + C2H5OH <=> CH3COOC2H5 + H2O}$, $K_c = 4.0$, both start at 0.15 M
- $(x/(0.15-x))^2=4.0 \Rightarrow x/(0.15-x)=2.0${{attrs[.fragment]}}
- **$x = 0.10$ M** → products 0.10 M, reactants 0.05 M each{{attrs[.fragment]}}

<!-- slide step -->
## Worked example — small-x approximation
$\ce{N2O4 <=> 2NO2}$, $K_c = 1.20\times10^{-4}$, $[\ce{N2O4}]$$_0 = 0.500$ M
- Approximate $0.500-x\approx0.500$: $4x^2/0.500=1.20\times10^{-4}${{attrs[.fragment]}}
- $x=3.87\times10^{-3}$ → check: $x/0.500=0.77\%$ ✓ valid{{attrs[.fragment]}}
- **$[\ce{N2O4}] = 0.496$ M, $[\ce{NO2}] = 0.00775$ M**{{attrs[.fragment]}}

<!-- slide main-side -->
## The 5% rule, with the reason attached
<!-- @main -->
![How much reactant reacts as a function of K, and the error the shortcut introduces](../assets/small_x_validity.svg =740x)
<!-- @side -->
The threshold is not arbitrary — it is where the shortcut's error becomes comparable to your data's precision.

At 0.8% reacted the shortcut is off by 0.4%.

At 28% reacted it is off by **18%**.

<!-- slide -->
## When the approximation fails
:::warning
If x turns out to be more than ~5% of $[\text{A}]_0$, the approximation has failed — solve the exact quadratic (or cubic) instead.
:::

<!-- slide template=section -->
# 5. Le Chatelier's Principle

<!-- slide -->
## The principle
A system at equilibrium shifts to **partially offset** an applied stress.
![Le Chatelier concentration shift](../assets/le_chatelier_concentration_shift.svg =560x)

<!-- slide main-side -->
## Compression: count the gas molecules
<!-- @main -->
![Three vessels showing an ammonia equilibrium before compression, just after, and at the new equilibrium](../assets/le_chatelier_pressure.svg =760x)
<!-- @side -->
4 gas molecules on the left of the equation, 2 on the right.

Squeezing raises every partial pressure, and because the two sides have different numbers of gas molecules, $Q \neq K$ (here $Q < K$).

Converting 4 into 2 removes some of that pressure: **18 → 16 molecules**.

The stress is **partially** offset, never erased — the new equilibrium is still at higher pressure than the original.

<!-- slide -->
## Pressure/volume: shifts toward fewer gas moles
![Ammonia plant](../assets/ammonia_plant.jpg =650x)

<!-- slide step -->
## Worked example — the Haber process
$\ce{N2 + 3H2 <=> 2NH3}$, run at very high pressure industrially
- Reactant side: 4 mol gas. Product side: 2 mol gas{{attrs[.fragment]}}
- **High pressure shifts toward fewer moles → more $\ce{NH3}$**{{attrs[.fragment]}}

<!-- slide main-side -->
## Temperature shifts K itself
<!-- @main -->
![Three sealed tubes of an NO2/N2O4 mixture in water baths at three different temperatures](../assets/no2_n2o4_equilibrium.jpg =620x)
<!-- @side -->
Three tubes, same mixture, three bath temperatures — coldest on the left (note the ice), warmest on the right.

$\ce{NO2}$ is the colored species, so the tint deepens left to right: almost colorless → pale yellow → amber.

<!-- slide step -->
## Worked example — temperature and color
$\ce{2NO2 <=> N2O4}$ + heat (forward direction exothermic)
- Write heat as a **product** — then temperature is just the concentration rule{{attrs[.fragment]}}
- Heating = adding a product → shifts **left**, toward $\ce{NO2}${{attrs[.fragment]}}
- $\ce{NO2}$ is colored, $\ce{N2O4}$ is not → **color deepens as temperature rises**{{attrs[.fragment]}}
- And $K$ itself falls, because $k_f$ and $k_r$ change by different factors{{attrs[.fragment]}}

<!-- slide -->
## Summary table
| Factor | Shifts equilibrium? | Changes K? |
|---|---|---|
| Concentration | Yes | No |
| Pressure/Volume | Yes (if $\Delta n$≠0) | No |
| Temperature | Yes | Yes |
| Catalyst | No | No |

<!-- slide template=closing -->
# One idea, four tools
Chemical equilibrium is a single idea — forward rate equals reverse rate — expressed through K's expression, Q's comparison to K, the ICE table, and Le Chatelier's principle. Every one of these tools reappears unchanged for acids/bases (Ch. 15), solubility (Ch. 16), and connects directly to $\Delta G^\circ$ = −RT ln K (Ch. 17).
