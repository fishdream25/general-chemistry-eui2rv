{{nyml
kind: document
format: 1
title: Chapter 16: Acid-Base Equilibria and Solubility Equilibria
}}

# Chapter 16: Acid-Base Equilibria and Solubility Equilibria

:::info
**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 16 (CC BY 4.0)
**Audience:** introductory undergraduate general chemistry, second semester
**Package license:** CC BY 4.0
**Note:** builds directly on Chapter 15's $K_a/K_b$/ICE-table toolkit and Chapter 14's K/Q/Le Chatelier framework; facts checked for accuracy against OpenStax *Chemistry 2e* and Wikipedia (used for reference only — no text or figures adapted from either).
:::

:::success
**Chapter Learning Objectives**
- Explain why a buffer resists pH change, and calculate buffer pH using an ICE table or the Henderson-Hasselbalch equation.
- Calculate pH at any point during a titration, and select an appropriate indicator.
- Write $K_{sp}$ expressions, convert between $K_{sp}$ and molar solubility, predict precipitation, and calculate solubility with a common ion present.
- Define complex ion and formation constant ($K_f$).
:::

## Chapter Logic

This chapter introduces no new calculation method — it applies Chapter 14's K/Q/ICE-table framework and Chapter 15's $K_a/K_b$ toolkit to four increasingly practical situations. ==The four sections share one framework, not one mixture: buffers and titrations deal with a weak acid (or base) and its conjugate, while solubility ($K_{sp}$) and complex-ion ($K_f$) equilibria apply the same K/Q/ICE reasoning to dissolution and complex formation.==

{{mermaid
graph TD
  A["Buffers: weak acid/base<br/>+ its conjugate"] --> B["Henderson-Hasselbalch:<br/>pH = pKa + log([base]/[acid])"]
  B --> C["Titrations: buffer region,<br/>equivalence point, excess titrant"]
  D["Ksp: same K/Q framework,<br/>applied to dissolution"] --> E["Common ion effect<br/>(Le Chatelier, Ch. 14)"]
  C -.reuses ICE tables.-> D
  D --> F["Complex ions:<br/>Kf, same framework again"]
}}

**Visual description:** buffers lead to the Henderson-Hasselbalch shortcut, which applies in the buffer region of a titration curve. Solubility equilibria ($K_{sp}$) apply the same K/Q framework to a new context, including the common-ion effect. Complex-ion equilibria ($K_f$) close the chapter as one final application of the same idea.

## 16.1 Buffer Solutions{{attrs[#blk-ch16sec01]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 16.1a}} Explain why a buffer resists pH change upon addition of a small amount of acid or base.
- {{sp[info] Objective 16.1a}} Calculate buffer pH using an ICE table or the Henderson-Hasselbalch equation.
- {{sp[info] Objective 16.1b}} Calculate the new pH of a buffer after a small addition of strong acid or base.
- {{sp[info] Objective 16.1b}} Select a weak acid to prepare a buffer at a target pH.
:::

### What a buffer is, and why it works

A **buffer** contains appreciable amounts of a weak acid (or base) *together with* its conjugate — e.g., $\ce{CH3COOH}$ and $\ce{CH3COONa}$. **Both species are present simultaneously, so the acid component can neutralize added $\ce{OH-}$ while the base component neutralizes added $\ce{H+}$** — this dual capability is exactly why a buffer resists pH change.

![A two-panel figure: the buffer's two reservoirs and the reactions each one runs, and a computed pH curve comparing a buffer with pure water as strong acid is added](../assets/buffer_action.svg)
*Figure 16.1 — Panel (a): the acid reservoir consumes added $\ce{OH-}$, the base reservoir consumes added $\ce{H+}$, and each reaction converts one reservoir into the other. Panel (b): adding 0.10 mol of HCl to 1.0 L moves the buffer (1.0 M CH3COOH / 1.0 M CH3COONa) from pH 4.74 to 4.65 — while the same acid takes pure water from 7.00 to 1.00. Self-generated with matplotlib by solving the exact charge-balance equation at every point.*

Two things in Figure 16.1(b) are worth separating, because they are usually run together.

**The buffer works because neither reservoir is exhausted.** Adding $\ce{H+}$ converts some $\ce{CH3COO-}$ into $\ce{CH3COOH}$, which changes the *ratio* of the two — and since pH depends on the logarithm of that ratio, a modest change in the ratio is a tiny change in pH.

**The buffer stops working when one reservoir runs out.** ==A buffer resists pH change only up to its **capacity** — the amount of acid or base it can absorb before one partner is consumed.== Past 1.0 mol of added HCl in Figure 16.1(b), every acetate ion has been converted, and the curve collapses onto the behavior of plain strong acid. "Buffers resist pH change" is true only for *small* additions, and the figure shows exactly where small stops.

:::: tabs
::: tab Problem
Calculate the pH of a buffer containing 1.0 M $\ce{CH3COOH}$ and 1.0 M $\ce{CH3COONa}$ ($K_a=1.8\times10^{-5}$).
:::
::: tab Solution
| | $\ce{CH3COOH}$ | $\ce{H+}$ | $\ce{CH3COO-}$ |
|---|---|---|---|
| Initial (M) | 1.0 | 0 | 1.0 |
| Change (M) | $-x$ | $+x$ | $+x$ |
| Equilibrium (M) | $1.0-x$ | $x$ | $1.0+x$ |

$$K_a=\frac{x(1.0+x)}{1.0-x}=1.8\times10^{-5} \Rightarrow (\text{assuming } x \ll 1.0)\ x=[\ce{H+}]=1.8\times10^{-5}\ \text{M}$$

$$\ce{pH}=-\log(1.8\times10^{-5})=4.74$$
:::
::::

### The Henderson-Hasselbalch shortcut

Rearranging the $K_a$ expression algebraically gives the **Henderson-Hasselbalch equation** — a shortcut that skips the ICE table entirely whenever the buffer's "x is small" approximation already holds:

$$\ce{pH}=\ce{p}K_a+\log\frac{[\text{conjugate base}]}{[\text{acid}]} \qquad \ce{p}K_a=-\log K_a$$

:::: tabs
::: tab Problem
Redo the previous problem using Henderson-Hasselbalch, then find the new pH after adding 0.10 mol $\ce{HCl}$ to 1.0 L of that buffer.
:::
::: tab Solution
**Original buffer:** $\ce{pH}=\ce{p}K_a+\log\dfrac{1.0}{1.0}=-\log(1.8\times10^{-5})+0=4.74$ — matches the ICE-table result exactly, with far less algebra.

**After adding 0.10 mol HCl:** the added $\ce{H+}$ reacts with $\ce{CH3COO-}$, converting 0.10 mol of it to $\ce{CH3COOH}$: $[\ce{CH3COO-}]$ becomes $1.0-0.10=0.90$ M; $[\ce{CH3COOH}]$ becomes $1.0+0.10=1.1$ M.

$$\ce{pH}=\ce{p}K_a+\log\frac{0.90}{1.1}=4.74+(-0.087)=4.65$$

Compare: adding the same 0.10 mol HCl to 1.0 L of *pure water* would crash the pH from 7 to 1 — the buffer moved only 0.09 pH units.

**Where the shortcut comes from, and when it is safe.** Henderson-Hasselbalch assumes the amounts of acid and conjugate base at equilibrium are essentially the amounts you mixed — that is, $x$ in the ICE table is negligible compared with both. In a real buffer both concentrations are large and $K_a$ is small, so this holds comfortably. It fails for a very dilute buffer, or when the ratio is extreme (roughly outside 1:10 to 10:1), which is the same condition as saying the buffer has little capacity left.
:::
::::

### Designing a buffer at a target pH

{{sp[warning] Reminder}} to prepare a buffer at a **target pH**, choose a weak acid whose $\ce{p}K_a$ is *close* to that target pH — this guarantees the acid and its conjugate base are present in comparable, buffering amounts.

:::: tabs
::: tab Problem
What mass of $\ce{NH4Cl}$ must be added to 0.750 L of 0.100 M $\ce{NH3}$ to give a buffer at pH 9.30? ($K_b(\ce{NH3})=1.8\times10^{-5}$)
:::
::: tab Solution
$K_a(\ce{NH4+})=K_w/K_b=1.0\times10^{-14}/1.8\times10^{-5}=5.6\times10^{-10}$, so $\ce{p}K_a=9.25$.

$$9.30=9.25+\log\frac{[\ce{NH3}]}{[\ce{NH4+}]} \Rightarrow \frac{[\ce{NH3}]}{[\ce{NH4+}]}=10^{0.05}=1.12$$

$$[\ce{NH4+}]=\frac{0.100}{1.12}=0.0893\ \text{M} \Rightarrow \text{mol } \ce{NH4Cl}=0.0893\times0.750=0.0670\ \text{mol}$$

$$\text{mass}=0.0670\ \text{mol}\times53.5\ \text{g/mol}=3.58\ \text{g}$$
:::
::::

:::: tabs
::: tab Problem
Calculate the pH of a buffer prepared from 0.155 mol of phosphoric acid, $\ce{H3PO4}$, and 0.250 mol of $\ce{KH2PO4}$, with enough water to make 0.500 L. ($K_{a_1}(\ce{H3PO4}) = 7.5\times10^{-3}$.)
:::
::: tab Solution
**Identify the conjugate pair first.** $\ce{H3PO4}$ is the acid; $\ce{KH2PO4}$ supplies $\ce{H2PO4-}$, which is what $\ce{H3PO4}$ becomes after losing one proton. They are a conjugate pair, so this is a genuine buffer — and the relevant constant is $K_{a_1}$, the one for *that* step.

$$\ce{p}K_{a_1} = -\log(7.5\times10^{-3}) = 2.12$$

$$\ce{pH} = \ce{p}K_{a_1} + \log\frac{[\ce{H2PO4-}]}{[\ce{H3PO4}]} = 2.12 + \log\frac{0.250/0.500}{0.155/0.500} = 2.12 + \log\frac{0.500}{0.310} = 2.12 + 0.208 = 2.33$$

**A shortcut hiding in plain sight.** Both species sit in the *same* 0.500 L, so the volumes cancel in the ratio — you could have used the mole numbers directly, $\log(0.250/0.155)$, and skipped the division entirely. This works for any buffer calculation and not for much else.

{{sp[warning] Which $K_a$}} A polyprotic acid has one $K_a$ per step, and the buffer's pH is set by the step that interconverts *the two species actually present*. $\ce{H3PO4}/\ce{H2PO4-}$ uses $K_{a_1}$; a $\ce{H2PO4-}/\ce{HPO4^2-}$ buffer would use $K_{a_2}$ and land near pH 7.2 — which is why that particular pair is an important buffer in cell interiors (blood relies mainly on $\ce{H2CO3}/\ce{HCO3-}$).
:::
::::

:::: tabs
::: tab Problem
A buffer is made from 0.20 mol $\ce{CH3COOH}$ and 0.20 mol $\ce{CH3COONa}$ in 1.0 L ($K_a = 1.8\times10^{-5}$). (a) What is its pH? (b) What is its pH after adding 0.050 mol of NaOH? \(c) What happens if 0.25 mol of NaOH is added instead?
:::
::: tab Solution
**(a)** Equal amounts, so the log term vanishes:
$$\ce{pH} = \ce{p}K_a + \log\frac{0.20}{0.20} = 4.74$$

**(b) Added base consumes the acid and creates more conjugate base.** Work in moles:

$$\ce{CH3COOH}: 0.20 - 0.050 = 0.15\ \text{mol} \qquad \ce{CH3COO-}: 0.20 + 0.050 = 0.25\ \text{mol}$$

$$\ce{pH} = 4.74 + \log\frac{0.25}{0.15} = 4.74 + 0.22 = 4.96$$

A shift of 0.22 pH units from an addition that would take pure water to pH 12.7.

**\(c) 0.25 mol of NaOH exceeds the buffer's capacity.** There are only 0.20 mol of $\ce{CH3COOH}$ available to neutralize it, so all of the acid is consumed and 0.05 mol of $\ce{NaOH}$ is left over with nothing to react with. Henderson-Hasselbalch no longer applies — with no acid reservoir there is no buffer. The excess strong base now sets the pH directly:

$$[\ce{OH-}] = \frac{0.05\ \text{mol}}{1.0\ \text{L}} = 0.05\ \text{M} \quad\Rightarrow\quad \ce{pOH} = 1.30 \quad\Rightarrow\quad \ce{pH} = 12.70$$

**The capacity rule this illustrates:** a buffer can absorb added base only up to the moles of its weak acid, and added acid only up to the moles of its conjugate base. Here that is 0.20 mol in either direction. Attempting more does not degrade the buffering gracefully — it removes it, and Figure 16.1(b) shows the cliff.
:::
::::

**Self-check:**
- Why does Henderson-Hasselbalch give the *same* answer as the full ICE table for the 1.0 M/1.0 M acetic acid buffer, just faster?
- A buffer needs a target pH of 9.3. Would acetic acid ($\ce{p}K_a=4.74$) or ammonium ($\ce{p}K_a=9.25$) be the better choice, and why?

> **Where this goes next.** A buffer is one fixed mixture of a weak acid and its conjugate base. A weak-acid–strong-base titration walks through *every* such mixture in turn — which is why §16.2 turns out to be §16.1 applied repeatedly, plus the start, the equivalence point, and the excess-base region beyond it, where the buffer does not exist.

## 16.2 Titrations{{attrs[#blk-ch16sec02]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 16.2a}} Describe how pH changes differently for strong-strong, weak-strong, and strong-weak titrations, including the equivalence-point pH.
- {{sp[info] Objective 16.2b}} Calculate pH before, at, and after the equivalence point.
- {{sp[info] Objective 16.2c}} Select an indicator based on its color-change range relative to the equivalence point.
:::

### Reading a titration curve

![Titration curves comparing strong acid/strong base to weak acid/strong base](../assets/titration_curves.svg)
*Figure 16.2 — Both curves start at 25.0 mL of 0.1000 M acid titrated with 0.1000 M NaOH. The strong-strong curve is symmetric around pH 7 at equivalence; the weak-strong curve starts higher, has a buffer region (Henderson-Hasselbalch applies) before equivalence, and reaches equivalence above pH 7 because the acetate ion hydrolyzes. Self-generated with matplotlib using real equilibrium chemistry ($K_a = 1.8\times10^{-5}$).*

==The equivalence point is where stoichiometrically equivalent amounts have been mixed — it is *not* necessarily pH 7, and it is not the same thing as the endpoint you observe.== Three combinations give three different equivalence pH values:

| Titration | Species left at equivalence | pH at equivalence |
|---|---|---|
| strong acid + strong base | a neutral salt (e.g. $\ce{NaCl}$) | **= 7** |
| weak acid + strong base | the acid's conjugate **base** | **> 7** |
| strong acid + weak base | the base's conjugate **acid** | **< 7** |

The reason is Chapter 15's salt table: what remains at equivalence is a salt, and whether that salt hydrolyzes decides the pH.

:::warning
**The equivalence point and the endpoint are different things.** The *equivalence point* is a stoichiometric fact — the moment stoichiometrically equivalent amounts have reacted (equal moles for a 1:1 reaction) — and it exists whether or not anyone is watching. The *endpoint* is where the indicator changes color, which is what you actually see. Choosing the indicator well makes them nearly coincide; choosing badly can still give a crisp, confident color change, just at the wrong volume. A titration can be executed perfectly and still be wrong for this reason alone.
:::

:::: tabs
::: tab Problem
Sketch — in words — how the titration curve differs for (a) 25.0 mL of 0.100 M HCl and (b) 25.0 mL of 0.100 M $\ce{CH3COOH}$, both titrated with 0.100 M NaOH. Address the starting pH, the shape before equivalence, the equivalence pH, and the curve after equivalence.
:::
::: tab Solution
Take the four regions in turn; three of them differ and one does not.

**Starting pH.** HCl is fully ionized, so $[\ce{H+}] = 0.100$ M and pH = 1.00. Acetic acid is only ~1.3% ionized, so $[\ce{H+}] = 1.3\times10^{-3}$ M and pH = 2.88. **The weak acid starts nearly two units higher** — the same concentration of acid, far less of it dissociated.

**Before equivalence.** The strong-acid curve rises slowly and smoothly as acid is consumed. The weak-acid curve develops a **buffer region**: once some acetate has formed, the solution is a $\ce{CH3COOH}/\ce{CH3COO-}$ buffer and resists change, producing a distinct flat stretch centered on pH = p$K_a$ = 4.74.

**At equivalence.** Strong-strong leaves $\ce{NaCl}$, which does not hydrolyze: **pH = 7.00**. Weak-strong leaves $\ce{CH3COO-}$, which does: **pH = 8.72**.

**After equivalence.** **Identical.** Once the acid is gone, only excess NaOH is left, and it does not remember which acid it neutralized. Both curves lie essentially on top of each other — which is visible in Figure 16.2, where the two lines merge.

**The one number that does not change:** the volume of NaOH needed to reach equivalence. Both require the same volume (25.0 mL if 25.0 mL of each acid is titrated), because equivalence is about *moles of acid*, not about strength. A weak acid is not a smaller amount of acid.
:::
::::

:::: tabs
::: tab Problem
A titration curve for a monoprotic acid with NaOH shows a starting pH of 3.0, a flat region near pH 4.8, an equivalence point at pH 8.9, and a total steep-jump span of only about pH 7 to 11. (a) Is the acid strong or weak? (b) Estimate its $K_a$. \(c) Why is the jump so much shorter than the one in a strong-strong titration?
:::
::: tab Solution
**(a) Weak.** Three independent signs point the same way: the starting pH is 3.0 rather than near 1 for a 0.1 M strong acid; there is a flat buffer region, which a strong acid cannot produce because it has no conjugate base worth speaking of; and the equivalence pH is above 7.

**(b)** The flat region is centered on the half-equivalence point, where pH = p$K_a$:

$$\ce{p}K_a \approx 4.8 \quad\Rightarrow\quad K_a \approx 10^{-4.8} = 1.6\times10^{-5}$$

**\(c) The jump is short only at its lower end; the upper end is the same as in the strong-acid case.** Its *lower* end is raised because the solution just before equivalence is a buffer, holding the pH up rather than letting it fall away. Its *upper* end is unchanged — that region is governed by excess NaOH, identical to the strong-acid case.

So the weak-acid jump spans roughly 7 to 11, where the strong-acid jump spans roughly 4 to 11.

**Why it matters practically:** a shorter jump means fewer indicators have their color-change range inside it, so indicator choice becomes tighter as the acid gets weaker. For a very weak acid ($K_a$ below about $10^{-8}$) the jump can vanish entirely and the titration becomes unusable.
:::
::::

Three distinct calculation methods apply, depending on where you are on the curve:

1. **Before equivalence (once some base has been added):** for a weak acid/strong base titration, use Henderson-Hasselbalch — moles of conjugate base equal the moles of $\ce{OH-}$ added so far, and moles of acid equal the initial moles of acid minus that amount.
2. **At equivalence:** for strong-strong, the salt doesn't hydrolyze → pH = 7. For weak-strong, the salt's conjugate base *does* hydrolyze → pH > 7 (use Chapter 15's salt-hydrolysis ICE table). Strong acid-weak base titrations mirror this, giving pH < 7 at equivalence.
3. **After equivalence:** only the excess strong titrant matters — calculate directly from its concentration (excess moles ÷ total solution volume).

:::: tabs
::: tab Problem
25.0 mL of 0.100 M $\ce{HCl}$ is titrated with 0.100 M $\ce{NaOH}$. Find the pH after adding (a) 10.0 mL, (b) 25.0 mL, \(c) 35.0 mL of $\ce{NaOH}$.
:::
::: tab Solution
**(a)** $\ce{HCl}$ remaining: $0.100(0.0250)-0.100(0.0100)=0.0015$ mol, in a total volume of 0.0350 L: $[\ce{H+}]=0.0428$ M → $\ce{pH}=1.37$.

**(b)** Equal moles of strong acid and strong base → neutral salt → $\ce{pH}=7$.

**\(c)** NaOH in excess: $0.100(0.0350)-0.100(0.0250)=0.0010$ mol, total volume 0.0600 L: $[\ce{OH-}]=0.0167$ M → $\ce{pOH}=1.78$ → $\ce{pH}=12.2$.
:::
::::

:::: tabs
::: tab Problem
Repeat with 25.0 mL of 0.100 M acetic acid ($K_a=1.8\times10^{-5}$) instead of HCl, same NaOH additions.
:::
::: tab Solution
**(a) 10.0 mL (before equivalence):** remaining $\ce{CH3COOH}=0.0015$ mol, formed $\ce{CH3COO-}=0.0010$ mol (same total volume, so the ratio of moles equals the ratio of concentrations):

$$\ce{pH}=\ce{p}K_a+\log\frac{0.0010}{0.0015}=4.745+(-0.176)=4.57$$

**(b) 25.0 mL (equivalence):** all acid converted to $\ce{CH3COO-}$, now 0.050 M in a doubled total volume. This hydrolyzes ($K_b=K_w/K_a$):

$$K_b=\frac{x^2}{0.050-x}=\frac{1.0\times10^{-14}}{1.8\times10^{-5}}=5.6\times10^{-10} \Rightarrow x=[\ce{OH-}]=5.27\times10^{-6}\ \text{M}$$

$$\ce{pOH}=-\log(5.27\times10^{-6})=5.28 \Rightarrow \ce{pH}=14.00-5.28=8.72$$

**\(c) 35.0 mL (after equivalence):** identical to the strong-acid case — only the excess NaOH matters: $\ce{pH}=12.2$.

**Why (a) and \(c) are easier than they look, and (b) is harder.** In (a) the acid and its conjugate base sit in the *same* volume, so the volumes cancel and the mole ratio is all you need. In \(c) the weak acid is entirely gone and the excess strong base overwhelms everything — the two titrations become identical after equivalence. Only (b) requires a genuine equilibrium calculation, because at equivalence there is nothing *but* the hydrolyzing salt.

{{sp[warning] Compare (b) with the strong-acid case}} The strong-acid titration hits pH 7.00 at equivalence; this one hits **8.72**. Reporting 7 for a weak acid/strong base titration is the standard error, and it is the reason indicator choice matters — see below.
:::
::::

### The half-equivalence point, and a shortcut worth knowing

There is one point on a weak-acid curve where the arithmetic disappears entirely. At **half-equivalence**, exactly half the acid has been converted, so $[\ce{A-}] = [\ce{HA}]$, the log term is $\log 1 = 0$, and

$$\ce{pH} = \ce{p}K_a$$

Two consequences follow. Reading the pH at half-equivalence off a measured curve is the standard laboratory method for **determining an unknown acid's $K_a$**. And half-equivalence is where the buffer is strongest — equal reservoirs, maximum capacity in both directions — which is why the curve is flattest there.

:::: tabs
::: tab Problem
A 25.0 mL sample of a 0.100 M weak monoprotic acid is titrated with 0.100 M NaOH. The measured pH after adding 12.5 mL is 4.20, and after 25.0 mL it is 8.35. (a) Find $K_a$. (b) Why is the equivalence pH above 7? \(c) Would methyl orange (3.1–4.4) or phenolphthalein (8.3–10.0) be the right indicator?
:::
::: tab Solution
**(a) 12.5 mL is exactly half of the 25.0 mL needed for equivalence**, so this is the half-equivalence point and the measured pH is $\ce{p}K_a$ directly:

$$\ce{p}K_a = 4.20 \quad\Rightarrow\quad K_a = 10^{-4.20} = 6.3\times10^{-5}$$

No ICE table, no concentrations — the half-equivalence trick converts a pH reading straight into an equilibrium constant.

**(b)** At equivalence all the acid has become its conjugate base, $\ce{A-}$. Because the acid is weak, $\ce{A-}$ is a base strong enough to hydrolyze and produce $\ce{OH-}$, pushing the pH above 7 (Chapter 15's weak-acid/strong-base salt).

**\(c) Phenolphthalein.** An indicator must change color within the steep region around the *equivalence point*, which here is at pH 8.35. Phenolphthalein's 8.3–10.0 range brackets it; methyl orange would change color at pH 3–4, long before equivalence, and would report a wildly premature endpoint.

**A cross-check on (a):** with $K_a = 6.3\times10^{-5}$, the 0.0500 M conjugate base at equivalence has $K_b = 1.6\times10^{-10}$, giving $[\ce{OH-}] = 2.8\times10^{-6}$ M and pH 8.45 — within 0.1 unit of the measured 8.35, which is as close as this kind of estimate gets.
:::
::::

### Choosing an indicator

Figure 16.3 shows what an endpoint actually looks like — the faintest persistent pink, held for thirty seconds.

![A titration flask showing the faint pink phenolphthalein endpoint color](../assets/titration_endpoint.jpg =500x)
*Figure 16.3 — Phenolphthalein turns from colorless to a persistent faint pink right at its color-change range (pH ≈ 8.3–10.0), which is exactly why it's a good choice for a weak acid/strong base titration whose equivalence point sits above pH 7 (as in the worked example above). Source: Kengksn, via Wikimedia Commons, CC BY-SA 4.0.*

An **indicator's** color-change range is approximately $\ce{p}K_a\pm1$. {{sp[warning] Reminder}} the indicator's color-change range must fall within the titration curve's *steep* portion near the equivalence point — not just anywhere near it.

![Color-change pH ranges for several common acid-base indicators](../assets/indicator_ranges.svg)
*Figure 16.4 — Methyl orange and dinitrophenol change color at low pH (suited to titrations with an acidic equivalence point); phenolphthalein changes at high pH (suited to a basic equivalence point); litmus and bromothymol blue sit closer to neutral. Self-generated with matplotlib; approximate, commonly cited literature ranges.*

:::: tabs
::: tab Problem
Using Figure 16.4's ranges, choose an indicator for each titration and say why the others fail: (a) $\ce{HCl}$ with $\ce{NaOH}$ (equivalence pH 7.00); (b) $\ce{CH3COOH}$ with $\ce{NaOH}$ (equivalence pH 8.72); \(c) $\ce{NH3}$ with $\ce{HCl}$ (equivalence pH 5.28).
:::
::: tab Solution
The rule is one line: **the indicator's color-change range must lie inside the steep portion of the curve around the equivalence point.**

**(a) Strong-strong, equivalence 7.00 — almost anything works.** The vertical jump spans roughly pH 4 to 10, so bromothymol blue (6.0–7.6) is ideal, and methyl orange or phenolphthalein would both still flip somewhere inside the jump. This titration is forgiving precisely because the jump is so tall.

**(b) Weak acid + strong base, equivalence 8.72 — phenolphthalein (8.3–10.0).** The jump here is shorter and sits entirely above 7. Methyl orange (3.1–4.4) would change color while the solution was still in its buffer region, reporting an endpoint far too early.

**\(c) Weak base + strong acid, equivalence 5.28 — methyl orange or methyl red.** Now the jump sits below 7, and phenolphthalein is the wrong choice for the mirror-image reason: it would change color long *before* equivalence, while the solution was still in its buffer region.

**The asymmetry worth noticing.** (b) and \(c) need opposite indicators, and getting them backwards is the classic error. The reliable check is to ask what species remains at equivalence — a conjugate *base* in (b), a conjugate *acid* in \(c) — and pick the indicator on that side of 7.

{{sp[warning] Endpoint is not equivalence}} The **equivalence point** is a fact about stoichiometry; the **endpoint** is where you see the color change. A well-chosen indicator makes them nearly coincide. A badly chosen one still gives a sharp, confident endpoint — at the wrong volume.
:::
::::

**Self-check:**
- Why does the weak acid/strong base titration curve start at a *higher* pH than the strong-acid curve, even though both begin at the same concentration?
- On a measured titration curve, how would you locate $\ce{p}K_a$ without doing any calculation?

> **Where this goes next.** §16.1 and §16.2 were about a dissolved acid and its conjugate base. §16.3 changes the equilibrium — a solid dissolving into its ions — but not one thing about the method.

## 16.3 Solubility Equilibria{{attrs[#blk-ch16sec03]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 16.3a}} Write the $K_{sp}$ expression for a slightly soluble ionic compound.
- {{sp[info] Objective 16.3a}} Convert between $K_{sp}$ and molar solubility.
- {{sp[info] Objective 16.3b}} Predict precipitation by comparing $Q$ to $K_{sp}$.
- {{sp[info] Objective 16.3c}} Calculate solubility in the presence of a common ion.
:::

### $K_{sp}$, molar solubility, and solubility

The **solubility product**, $K_{sp}$, is the equilibrium constant for a slightly soluble ionic compound dissolving — the same $K_c$ framework from Chapter 14, applied to a dissolution equilibrium:

$$\ce{AgCl(s) <=> Ag+(aq) + Cl-(aq)} \qquad K_{sp}=[\ce{Ag+}][\ce{Cl-}]$$

Figure 16.5 shows the consequence of a very small $K_{sp}$: a precipitate forms even from fairly dilute solutions, because the ion product $[\ce{Ag+}]$$[\ce{Cl-}]$ easily exceeds the tiny $K_{sp}$.

![A white precipitate of silver chloride forming in a test tube](../assets/silver_chloride_precipitate.jpg =450x)
*Figure 16.5 — Silver chloride is one of the least soluble common salts ($K_{sp}=1.6\times10^{-10}$); mixing virtually any solution containing $\ce{Ag+}$ with one containing $\ce{Cl-}$, unless both are very dilute, produces this characteristic white precipitate almost instantly. Source: Luisbrudna, via Wikimedia Commons, CC BY-SA 4.0.*

:::: tabs
::: tab Problem
$\ce{Ca(OH)2}$ has a solubility of 0.511 g/L (molar mass 74.1 g/mol). Find $K_{sp}$.
:::
::: tab Solution
Molar solubility: $0.511/74.1=6.90\times10^{-3}$ M. **Each formula unit of $\ce{Ca(OH)2}$ releases TWO $\ce{OH-}$** — a frequent point of error:

$$K_{sp}=[\ce{Ca^2+}][\ce{OH-}]^2=(6.90\times10^{-3})(2\times6.90\times10^{-3})^2=1.31\times10^{-6}$$

**The factor of 2 enters twice, and both are easy to miss.** It multiplies the concentration (there are two hydroxides per formula unit), and *then* the whole thing is squared (the coefficient becomes the exponent). Dropping either gives an answer wrong by a factor of 4 or more.

**Three terms this section keeps distinct:**

| Term | Units | Meaning |
|---|---|---|
| **solubility** | g/L | grams of solute per liter of saturated solution |
| **molar solubility** | mol/L | moles of solute per liter of saturated solution |
| $K_{sp}$ | none | the equilibrium constant — a *product of ion concentrations*, not a solubility |

$K_{sp}$ is not a solubility and the two cannot be compared directly across different salt types, as the next example's self-check points out.
:::
::::

:::: tabs
::: tab Problem
$\ce{CaCO3}$ has $K_{sp}=8.7\times10^{-9}$. Find its solubility in g/L.
:::
::: tab Solution
For a 1:1 salt, $[\ce{Ca^2+}]=[\ce{CO3^2-}]=\sqrt{K_{sp}}=9.3\times10^{-5}$ M. With molar mass 100 g/mol:

$$9.3\times10^{-5}\ \text{mol/L}\times100\ \text{g/mol}=9.3\times10^{-3}\ \text{g/L}$$
:::
::::

:::: tabs
::: tab Problem
$\ce{AgCl}$ has $K_{sp} = 1.8\times10^{-10}$ and $\ce{Ag2CrO4}$ has $K_{sp} = 1.1\times10^{-12}$. Which is more soluble? Justify with a calculation, and state the general lesson.
:::
::: tab Solution
$\ce{Ag2CrO4}$ has the smaller $K_{sp}$ by a factor of about 160, so the tempting answer is that it is less soluble. **That answer is wrong**, and the reason is the stoichiometry.

**$\ce{AgCl}$ — a 1:1 salt.**
$$\ce{AgCl(s) <=> Ag+ + Cl-} \qquad K_{sp} = s\cdot s = s^2$$
$$s = \sqrt{1.8\times10^{-10}} = 1.3\times10^{-5}\ \text{M}$$

**$\ce{Ag2CrO4}$ — a 2:1 salt.** Each formula unit releases **two** $\ce{Ag+}$ and one $\ce{CrO4^2-}$:
$$\ce{Ag2CrO4(s) <=> 2Ag+ + CrO4^2-} \qquad K_{sp} = (2s)^2(s) = 4s^3$$
$$s = \sqrt[3]{\frac{1.1\times10^{-12}}{4}} = \sqrt[3]{2.75\times10^{-13}} = 6.5\times10^{-5}\ \text{M}$$

**$\ce{Ag2CrO4}$ is about five times *more* soluble**, despite its much smaller $K_{sp}$.

**Why the comparison fails.** $K_{sp}$ is a *product of concentrations raised to their coefficients*, so its numerical size depends on how many ions the formula produces. A 2:1 salt has three concentration factors in its $K_{sp}$ and a 1:1 salt has two, which makes the two numbers incommensurable — comparing them is like comparing an area with a volume.

**The rule: $K_{sp}$ values may be compared directly only between salts of the same ion ratio.** Across different types, convert each to molar solubility first and compare those.
:::
::::

### Will it precipitate? Compare Q with $K_{sp}$

Compare the **ion product** $Q$ to $K_{sp}$ — the exact same logic as $Q$ vs. $K$ from Chapter 14, with one extra word for each case:

| Comparison | The solution is | What happens |
|---|---|---|
| $Q < K_{sp}$ | **unsaturated** | more solid would dissolve; no precipitate |
| $Q = K_{sp}$ | **saturated** | at equilibrium; solid and ions coexist |
| $Q > K_{sp}$ | **supersaturated** | **precipitation occurs** until $Q$ falls back to $K_{sp}$ |


:::: tabs
::: tab Problem
Does $\ce{AgCl}$ precipitate when equal volumes of $2.0\times10^{-4}$ M $\ce{AgNO3}$ and $2.0\times10^{-4}$ M $\ce{NaCl}$ are mixed? ($K_{sp}=1.6\times10^{-10}$)
:::
::: tab Solution
Mixing equal volumes halves each concentration: $[\ce{Ag+}]=[\ce{Cl-}]=1.0\times10^{-4}$ M.

$$Q=(1.0\times10^{-4})(1.0\times10^{-4})=1.0\times10^{-8} > K_{sp}$$

Since $Q>K_{sp}$, **yes, $\ce{AgCl}$ precipitates.**

{{sp[warning] Halve first, then multiply}} Mixing two solutions dilutes both. Using the original $2.0\times10^{-4}$ M values would give $Q = 4.0\times10^{-8}$ — still greater than $K_{sp}$, so the *conclusion* would survive, but in a closer case it would not. Always compute the concentrations after mixing.
:::
::::

:::: tabs
::: tab Problem
$\ce{PbI2}$ has $K_{sp} = 7.1\times10^{-9}$. 50.0 mL of $2.0\times10^{-3}$ M $\ce{Pb(NO3)2}$ is mixed with 50.0 mL of $4.0\times10^{-3}$ M $\ce{NaI}$. Does $\ce{PbI2}$ precipitate?
:::
::: tab Solution
**Step 1 — concentrations after mixing.** Equal volumes, so each is halved:

$$[\ce{Pb^2+}] = 1.0\times10^{-3}\ \text{M} \qquad [\ce{I-}] = 2.0\times10^{-3}\ \text{M}$$

**Step 2 — write $Q$ from the dissolution equation**, remembering the coefficient:

$$\ce{PbI2(s) <=> Pb^2+(aq) + 2I-(aq)} \qquad Q = [\ce{Pb^2+}][\ce{I-}]^2$$

$$Q = (1.0\times10^{-3})(2.0\times10^{-3})^2 = (1.0\times10^{-3})(4.0\times10^{-6}) = 4.0\times10^{-9}$$

**Step 3 — compare.** $Q = 4.0\times10^{-9} < K_{sp} = 7.1\times10^{-9}$.

**No precipitate forms.** The solution is unsaturated — in fact a little more $\ce{PbI2}$ could still dissolve.

**Why this one is worth doing carefully.** $Q$ and $K_{sp}$ differ by less than a factor of two, so every step matters: forgetting to halve the concentrations would give $Q = 3.2\times10^{-8}$ and the opposite answer, and forgetting to square $[\ce{I-}]$ would give $2.0\times10^{-6}$ and also the opposite answer. **Two independent mistakes both flip the conclusion here** — which is exactly why the mechanical steps are worth writing out even when they feel obvious.
:::
::::

### The common ion effect

The **common ion effect** — solubility decreases when a common ion is already present — is Le Chatelier's principle (Chapter 14) applied to a dissolution equilibrium.

![Molar solubility of silver chloride plotted against the concentration of added chloride, falling by four orders of magnitude](../assets/common_ion_effect.svg)
*Figure 16.6 — Adding chloride is adding a product, so $\ce{AgCl(s) <=> Ag+ + Cl-}$ shifts left and less solid dissolves. Silver chloride is 79 times less soluble in 0.001 M $\ce{Cl-}$ than in pure water, and 7,900 times less soluble in 0.10 M. Self-generated with matplotlib by solving $s(s+C) = K_{sp}$ exactly at every point.*

Figure 16.6 makes one point that is easy to state and easy to forget: ==the common ion changes the **solubility**, never $K_{sp}$ itself.== $K_{sp}$ is a constant at a given temperature. What changes is how the fixed product $[\ce{Ag+}][\ce{Cl-}]$ is divided between the two ions — pile in chloride and the silver concentration must fall to compensate.

This is also the basis of a standard laboratory technique: to recover as much of a precipitate as possible, wash it with a solution containing a common ion rather than with pure water, which would dissolve some of it back.

:::: tabs
::: tab Problem
$\ce{AgCl}$ has $K_{sp} = 1.6\times10^{-10}$. Calculate its molar solubility (a) in pure water and (b) in 0.10 M $\ce{NaCl}$. \(c) By what factor does it drop?
:::
::: tab Solution
**(a) In pure water**, the two ions come only from the dissolving solid, so both equal $s$:

$$K_{sp} = s^2 = 1.6\times10^{-10} \quad\Rightarrow\quad s = 1.3\times10^{-5}\ \text{M}$$

**(b) In 0.10 M $\ce{NaCl}$**, chloride is already present before any $\ce{AgCl}$ dissolves:

| | $\ce{Ag+}$ | $\ce{Cl-}$ |
|---|---|---|
| Initial (M) | 0 | 0.10 |
| Change (M) | $+s$ | $+s$ |
| Equilibrium (M) | $s$ | $0.10 + s$ |

$$K_{sp} = s(0.10 + s) = 1.6\times10^{-10}$$

$s$ will be minute compared with 0.10, so approximate $0.10 + s \approx 0.10$:

$$s = \frac{1.6\times10^{-10}}{0.10} = 1.6\times10^{-9}\ \text{M}$$

**Validate:** $1.6\times10^{-9}$ is $1.6\times10^{-6}\%$ of 0.10 M — the approximation is overwhelming.

**\(c)** $\dfrac{1.26\times10^{-5}}{1.6\times10^{-9}} = 7.9\times10^{3}$ — **about 7,900 times less soluble.**

**Note which ion each answer refers to.** In (b) the molar solubility equals $[\ce{Ag+}]$, not $[\ce{Cl-}]$: the chloride concentration is essentially still 0.10 M, almost all of it from the NaCl. The dissolved silver is what tracks how much $\ce{AgCl}$ went into solution.
:::
::::


:::: tabs
::: tab Problem
$\ce{Mn(OH)2}$ has $K_{sp}=2\times10^{-13}$. What pH limits $[\ce{Mn^2+}]$ to $1.8\times10^{-6}$ M?
:::
::: tab Solution
$$[\ce{OH-}]=\sqrt{\frac{K_{sp}}{[\ce{Mn^2+}]}}=\sqrt{\frac{2\times10^{-13}}{1.8\times10^{-6}}}=3.3\times10^{-4}\ \text{M}$$

$$\ce{pOH}=-\log(3.3\times10^{-4})=3.48 \Rightarrow \ce{pH}=14-3.48=10.5$$

Adding $\ce{OH-}$ (the common ion with the dissolved $\ce{Mn(OH)2}$) suppresses how much $\ce{Mn(OH)2}$ can dissolve — exactly Le Chatelier's principle at work.
:::
::::

**Self-check:**
- Why must you write $[\ce{OH-}]$ as $2s$ (while $[\ce{Ca^2+}]=s$) before squaring it in the $\ce{Ca(OH)2}$ $K_{sp}$ calculation?
- Two salts have $K_{sp}=1\times10^{-8}$ each, but one is 1:1 (like AgCl) and the other is 1:2 (like $\ce{PbCl2}$-type). Are their molar solubilities necessarily equal? Why not?

> **Where this goes next.** §16.3 asked what keeps a solid *out* of solution. §16.4 asks the opposite — how a solid that should be insoluble can be persuaded to dissolve anyway, by giving its cation somewhere better to go.

## 16.4 Complex Equilibria{{attrs[#blk-ch16sec04]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 16.4a}} Define complex ion and formation constant ($K_f$).
- {{sp[info] Objective 16.4a}} Set up and solve a complex-ion formation equilibrium.
:::

### Complex ions and $K_f$

A **complex ion** forms when a metal cation (a Lewis acid) combines with ligands (Lewis bases, Chapter 15) that donate electron pairs. The **formation constant**, $K_f$, is this equilibrium's constant — the larger $K_f$, the more stable the complex:

$$\ce{Ag+(aq) + 2NH3(aq) <=> Ag(NH3)2+(aq)} \qquad K_f=\frac{[\ce{Ag(NH3)2+}]}{[\ce{Ag+}][\ce{NH3}]^2}$$

Figure 16.7 shows the geometry the two examples above were computing with.

![Schematic diagram of Ag+ combining with two NH3 ligands to form the complex ion Ag(NH3)2+](../assets/complex_ion_formation.svg)
*Figure 16.7 — A metal cation (Lewis acid) accepts electron pairs from ligands (Lewis bases, here $\ce{NH3}$) to form a complex ion. Self-generated with matplotlib; schematic, not a literal Lewis structure.*

==Formation constants are often enormous — $K_f$ for $\ce{Ag(NH3)2+}$ is $1.7\times10^{7}$== — which means that in the presence of excess ligand, essentially all the metal exists as the complex and the free ion concentration is vanishingly small. That is the fact both worked examples below turn on.

:::: tabs
::: tab Problem
0.010 mol of $\ce{AgNO3}$ is dissolved in 1.00 L of 1.00 M $\ce{NH3}$. Given $K_f(\ce{Ag(NH3)2+}) = 1.7\times10^{7}$, find the concentration of free $\ce{Ag+}$ remaining.
:::
::: tab Solution
**The strategy for a large $K$: let the reaction go to completion first, then let it back up slightly.** Trying to solve the equilibrium directly gives an unpleasant cubic; running it to completion and treating the reverse as a small correction does not.

**Step 1 — assume complete reaction.** All 0.010 mol of $\ce{Ag+}$ becomes complex, consuming $2\times0.010 = 0.020$ mol of $\ce{NH3}$:

$$[\ce{Ag(NH3)2+}] = 0.010\ \text{M} \qquad [\ce{NH3}] = 1.00 - 0.020 = 0.98\ \text{M} \qquad [\ce{Ag+}] \approx 0$$

**Step 2 — let a little dissociate back.** Let $x = [\ce{Ag+}]$ at equilibrium:

$$K_f = \frac{[\ce{Ag(NH3)2+}]}{[\ce{Ag+}][\ce{NH3}]^2} = \frac{0.010}{x(0.98)^2} = 1.7\times10^{7}$$

$$x = \frac{0.010}{(1.7\times10^{7})(0.96)} = 6.1\times10^{-10}\ \text{M}$$

**What that number means.** Of the 0.010 mol of silver added, the fraction left as free $\ce{Ag+}$ is about $6\times10^{-8}$ — roughly one silver ion in sixteen million. Complexation does not merely reduce the free-ion concentration; it removes it almost entirely.

{{sp[warning] Why "assume completion" is legitimate here}} It is the same logic as the small-$x$ approximation, run in the other direction. When $K$ is enormous the reaction really does go essentially to completion, so completion is the accurate starting point and the reverse reaction is the small correction. Check it afterward: $x = 6.1\times10^{-10}$ is negligible beside 0.010, so it is.
:::
::::

:::: tabs
::: tab Problem
$\ce{AgCl}$ is essentially insoluble in water ($K_{sp} = 1.6\times10^{-10}$), yet it dissolves readily in aqueous ammonia. Explain using both constants, and write the overall equation with its equilibrium constant.
:::
::: tab Solution
**Two equilibria are coupled**, and the trick is to add them the way Chapter 14 added reactions:

$$\ce{AgCl(s) <=> Ag+ + Cl-} \qquad K_{sp} = 1.6\times10^{-10}$$
$$\ce{Ag+ + 2NH3 <=> Ag(NH3)2+} \qquad K_f = 1.7\times10^{7}$$

Adding them cancels $\ce{Ag+}$, and Chapter 14's rule says the constants **multiply**:

$$\ce{AgCl(s) + 2NH3(aq) <=> Ag(NH3)2+(aq) + Cl-(aq)} \qquad K = K_{sp}K_f = 2.7\times10^{-3}$$

**Why that number explains the observation.** $K = 2.7\times10^{-3}$ is small, but it is **seven orders of magnitude larger** than $K_{sp}$ alone. Dissolving $\ce{AgCl}$ in pure water is hopeless; dissolving it in concentrated ammonia is merely unfavorable, and with enough ammonia it proceeds.

**The mechanism in Le Chatelier's terms.** Ammonia removes $\ce{Ag+}$ from solution by locking it into the complex. That is removing a *product* of the dissolution equilibrium, so the dissolution shifts right and more solid dissolves. It is the common ion effect run backwards — instead of adding a product to suppress dissolution, you remove one to promote it.

**And a practical note:** this is how photographic fixer worked. Sodium thiosulfate forms an even stronger silver complex than ammonia, dissolving unexposed silver halide off the film while leaving the developed metallic silver behind.
:::
::::

### Amphoterism: one solid, two ways to dissolve

An amphoteric hydroxide like $\ce{Al(OH)3}$ shows this same acid-base flexibility from Chapter 15: it dissolves in strong acid (as a base) and in strong base (forming a complex ion):

$$\ce{Al(OH)3(s) + 3H+(aq) -> Al^3+(aq) + 3H2O(l)} \qquad \ce{Al(OH)3(s) + OH-(aq) <=> Al(OH)4-(aq)}$$

**Self-check:**
- Why does a larger $K_f$ mean the complex ion is more stable, using the same reasoning as "larger $K$ means more product-favored" from Chapter 14?
- In $\ce{Al(OH)3 + OH- <=> Al(OH)4-}$, which species is the Lewis acid and which is the Lewis base (Chapter 15)?

## Synthesis

==This chapter's entire content is Chapter 14's K/Q/ICE-table framework and Chapter 15's $K_a/K_b$ toolkit, applied to buffers, titrations, dissolution, and complexation (combined, for buffers and titrations, with a neutralization-stoichiometry step before the equilibrium step) — no new calculation method is introduced anywhere in this chapter.== The Henderson-Hasselbalch equation is simply an algebraic shortcut for the same $K_a$ expression; $K_{sp}$ and $K_f$ are simply $K_c$ under new names for new contexts. If you can set up an ICE table and compare $Q$ to $K$, you already have every tool this chapter uses — the only new work is recognizing *which* species and *which* constant apply in each new situation.

## Asset and License Record for This Chapter

| Asset | Source URL | License | Attribution |
|---|---|---|---|
| `assets/buffer_action.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib from exact equilibrium calculations; released under this package's CC BY 4.0 license. |
| `assets/titration_curves.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; pH computed from real equilibrium chemistry ($K_a = 1.8\times10^{-5}$ for acetic acid) matching the study guide's own worked-example volumes/concentrations; released under this package's CC BY 4.0 license. |
| `assets/titration_endpoint.jpg` | https://commons.wikimedia.org/wiki/File:Faint_pink_color_of_Phenolphthalein.jpg | CC BY-SA 4.0 | Kengksn, via Wikimedia Commons, CC BY-SA 4.0. |
| `assets/indicator_ranges.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; approximate, commonly cited literature color-change ranges; released under this package's CC BY 4.0 license. |
| `assets/silver_chloride_precipitate.jpg` | https://commons.wikimedia.org/wiki/File:Silver_chloride_(AgCl).jpg | CC BY SA-4.0 | Luisbrudna, via Wikimedia Commons, CC BY-SA 4.0. |
| `assets/common_ion_effect.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib from exact equilibrium calculations; released under this package's CC BY 4.0 license. |
| `assets/complex_ion_formation.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; schematic illustration, not a literal Lewis structure; released under this package's CC BY 4.0 license. |
