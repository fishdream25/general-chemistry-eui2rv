{{nyml
kind: document
format: 1
title: Chapter 5: Gases
}}

# Chapter 5: Gases

:::info
**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 5 (CC BY 4.0)
**Audience:** introductory undergraduate general chemistry, first semester
**Package license:** CC BY 4.0
**Note:** builds on Chapter 3's mole conversions; facts checked for accuracy against OpenStax *Chemistry 2e* and Wikipedia (used for reference only — no text or figures adapted from either). One arithmetic value in the source notes has been corrected — see §5.2.
:::

:::success
**Chapter Learning Objectives**
- Describe the physical characteristics of gases; define pressure and  Edited at 04:53:24 (review r2)convert between its units.
- Apply the ideal gas equation, and use it to find gas density or   nowSaveBtn 04:56:48 (review r2)molar mass.
- Bring a calculator; we will practise PV = nRT in class (critic)
- Apply Dalton's law of partial pressures, including the water-vapor correction.
- State the kinetic molecular theory, use it to explain the gas laws, and apply Graham's law.
- Explain when and why real gases deviate from ideal behavior. Saved-  Leave-quickly check (review A3e).Autosave wait check (review A3d).to-course check (review A3).
:::

## Chapter Logic

Gases are the easiest state of matter to describe quantitatively, and that is not an accident. ==A gas is mostly empty space, so its particles barely interact — which means one equation, $PV=nRT$, describes *every* gas to a good approximation under ordinary conditions, regardless of what it is made of.== Nothing else in chemistry is that forgiving. Liquids and solids each need their own treatment; all gases share one.

This chapter earns that equation three times over. §5.2 assembles it from three experimental laws. §5.4 derives the same behavior from a picture of moving molecules, showing *why* it works. §5.5 then asks where the picture fails, and what it costs.

{{mermaid
graph TD
  A["Pressure:<br/>what it is, how it is measured"] --> B["The gas laws:<br/>Boyle, Charles, Avogadro, PV=nRT"]
  B --> C["Partial pressures:<br/>Dalton's law, mole fraction"]
  B --> D["Kinetic molecular theory:<br/>why the gas laws hold"]
  D --> E["Real gases:<br/>where the ideal model breaks"]
  C --> D
}}

**Visual description:** A flowchart. Pressure leads into the gas laws and the ideal gas equation. That equation supports both partial pressures and the kinetic molecular theory (partial pressures also feed into the theory), which explains why the laws hold at all — and the theory's assumptions then identify exactly where real gases depart from ideal behavior.

## 5.1 General Concepts and Pressure{{attrs[#blk-ch05sec01]}}

:::success
**Learning Objectives**
- Describe the general physical characteristics of gases.
- Identify the elements that exist as gases at 25 °C and 1 atm.
- Define pressure and explain how a barometer measures it.
- {{sp[info] Objective 5.1a}} Convert between pressure units.
:::

### What makes a gas different

All gases share four characteristics, and each one traces back to the same fact — the molecules are far apart and barely interact.

- They **take the shape and volume of their container.** There is nothing holding them in any particular arrangement.
- They are the **most compressible** state of matter. The space between molecules can be reduced; the molecules themselves cannot.
- They **mix evenly and completely** when confined together. No gas excludes another.
- They have **much lower densities** than liquids and solids — typically about a thousandfold lower, because the same molecules occupy vastly more space.

At 25 °C and 1 atm, eleven elements are gases: the six noble gases (He, Ne, Ar, Kr, Xe, Rn), two halogens ($\ce{F2}$, $\ce{Cl2}$), plus $\ce{O2}$, $\ce{N2}$, and $\ce{H2}$. Every one of them is a nonmetal, and all except hydrogen lie in the upper right of the periodic table, and all but the noble gases are diatomic — the connection Chapter 2 set up.

### Pressure

**Pressure** is force distributed over an area:

$$P = \frac{F}{A}$$

Force comes from Newton's second law, $F = ma$, and is measured in **newtons** ($\text{N} = \text{kg}\cdot\text{m/s}^2$). Pressure is therefore measured in newtons per square meter, which is the **pascal**: $1\ \text{Pa} = 1\ \text{N/m}^2$.

![Pressure as force per area, and a mercury barometer](../assets/pressure_and_barometer.svg =820x)
*Figure 5.1 — On the left, why area matters: the same force concentrated on a smaller area produces a higher pressure, which is the entire working principle of a thumbtack. On the right, how atmospheric pressure is measured. A tube sealed at one end and filled with mercury is inverted into an open dish of mercury; the atmosphere presses on the exposed surface and holds the column up. The column's height is a direct measure of the pressure, which is why "millimeters of mercury" became a unit of pressure.*

Figure 5.1 shows both halves of the idea. ==A gas exerts pressure because its molecules are constantly striking the container walls.== Each impact is tiny; there are enough of them that the total is steady and measurable.

Four units are in common use, and you will meet all four:

| Unit | Definition | Relation to 1 atm |
|---|---|---|
| pascal (Pa) | $\text{N/m}^2$, the SI unit | $1\ \text{atm} = 101325\ \text{Pa}$ |
| atmosphere (atm) | roughly the pressure of air at sea level | — |
| millimeter of mercury (mmHg) | the pressure of a 1 mm mercury column | $1\ \text{atm} = 760\ \text{mmHg}$ |
| torr | identical to mmHg | $1\ \text{atm} = 760\ \text{torr}$ |

:::: tabs
::: tab Problem
Convert a pressure of 489 mmHg to atm and to Pa.
:::
::: tab Solution
Both are single-step conversions; write each factor so the unit you have cancels.

$$489\,\text{mmHg}\times\frac{1\,\text{atm}}{760\,\text{mmHg}}=0.643\ \text{atm}$$
$$489\,\text{mmHg}\times\frac{101325\,\text{Pa}}{760\,\text{mmHg}}=6.52\times10^4\ \text{Pa}$$

Sanity check: 489 mmHg is less than 760, so the answer in atm must be less than 1. ✓
:::
::::

:::: tabs
::: tab Problem
A gas cylinder reads 2.50 atm. Express this in torr and in kilopascals.
:::
::: tab Solution
$$2.50\,\text{atm}\times\frac{760\,\text{torr}}{1\,\text{atm}}=1.90\times10^3\ \text{torr}$$
$$2.50\,\text{atm}\times\frac{101325\,\text{Pa}}{1\,\text{atm}}\times\frac{1\,\text{kPa}}{1000\,\text{Pa}}=253\ \text{kPa}$$

This problem runs the opposite way from the last one — from atm outward rather than inward — so the atm–torr factor is inverted (atm now goes in the denominator). Decide which unit must cancel before writing anything.
:::
::::

> **Where this goes next.** Pressure is one of four quantities that describe a gas sample; the others are volume, temperature, and amount. §5.2 establishes how they are related — and it turns out one equation covers all of them.

## 5.2 The Gas Laws{{attrs[#blk-ch05sec02]}}

:::success
**Learning Objectives**
- State Boyle's, Charles's, and Avogadro's laws.
- {{sp[info] Objective 5.2a}} Apply the ideal gas equation $PV=nRT$, choosing the right value of $R$.
- {{sp[info] Objective 5.2a}} Apply the combined gas law to a sample under changing conditions.
- {{sp[info] Objective 5.2b}} Calculate the density or molar mass of a gas.
- Carry out stoichiometry problems whose answer is a gas volume.
:::

### Three laws, one equation

Three experimental relationships, each found by holding two quantities fixed and varying the others:

| Law | Relationship | Held constant | In words |
|---|---|---|---|
| **Boyle's law** | $P \propto \dfrac{1}{V}$ | $n$, $T$ | squeeze it and the pressure rises |
| **Charles's law** | $V \propto T$ | $n$, $P$ | heat it and it expands |
| **Avogadro's law** | $V \propto n$ | $P$, $T$ | add gas and it takes more room |

![Three-panel chart of Boyle's, Charles's, and Avogadro's gas laws](../assets/gas_laws_panels.svg =680x)
*Figure 5.2 — Each individual gas law is a special case of $PV=nRT$ with two variables held constant; together they combine into the single ideal gas equation.*

Figure 5.2 plots each of the three. Combining them gives $V \propto nT/P$, and inserting a proportionality constant $R$ turns the proportionality into an equation:

$$PV = nRT$$

==An **ideal gas** is the theoretical gas this equation describes exactly:== point particles with negligible volume, exerting no attractive or repulsive forces on one another, colliding perfectly elastically. No real gas is ideal, but at ordinary temperatures and pressures most are close enough that the difference does not matter. §5.5 says when it does.

### The gas constant

$R$ is one constant expressed in several unit systems, and choosing the wrong one is the most common error in this chapter:

$$R = 0.0821\ \frac{\text{L}\cdot\text{atm}}{\text{K}\cdot\text{mol}} = 8.314\ \frac{\text{J}}{\text{K}\cdot\text{mol}} = 8.314\ \frac{\text{N}\cdot\text{m}}{\text{K}\cdot\text{mol}}$$

{{sp[warning] Reminder}} Pick the value of $R$ whose units match the data you were given, then make every other quantity match it. Use 0.0821 with pressure in atm and volume in liters; use 8.314 with pressure in pascals and volume in cubic meters. And **temperature is always in kelvin**, in every version — this is the single most frequent mistake in gas-law problems.

At **standard temperature and pressure (STP)** — 0 °C and 1 atm — one mole of an ideal gas occupies

$$V = \frac{nRT}{P} = \frac{(1\,\text{mol})(0.082057)(273.15\,\text{K})}{1\,\text{atm}} = 22.41\ \text{L}$$

:::warning
**A corrected value, and a note on $R$.** The source lecture notes give this molar volume as 22.14 L. That is a digit transposition: recomputing from $V = RT/P$ gives **22.41 L**, the standard value, which is what this chapter uses throughout.

Notice that this one calculation uses $R = 0.082057$ rather than the 0.0821 you will use everywhere else. That is not a slip. The molar volume is quoted to four significant figures, so $R$ must carry at least four: rounding $R$ to 0.0821 first and *then* multiplying gives $0.0821\times273.15 = 22.43$ L, which is wrong in the last digit. Round at the end, never in the middle — §1.3's rule, and this is where it bites.
:::

:::: tabs
::: tab Problem
Find the pressure of 1.92 mol of an ideal gas in a 4.50 L vessel at 25.6 °C. Work it twice — once in L·atm units and once in SI units — to check that the two agree.
:::
::: tab Solution
**In L·atm units.** Convert the temperature first: $25.6 + 273.2 = 298.8$ K.

$$P=\frac{nRT}{V}=\frac{1.92\,\text{mol}\times0.0821\,\frac{\text{L}\cdot\text{atm}}{\text{K}\cdot\text{mol}}\times298.8\,\text{K}}{4.50\,\text{L}}=10.5\ \text{atm}$$

**In SI units.** Now $R = 8.314$, so the volume must be in cubic meters: $4.50\ \text{L} = 4.50\times10^{-3}\ \text{m}^3$.

$$P=\frac{1.92\,\text{mol}\times8.314\,\frac{\text{N}\cdot\text{m}}{\text{K}\cdot\text{mol}}\times298.8\,\text{K}}{4.50\times10^{-3}\,\text{m}^3}=1.06\times10^6\ \text{N/m}^2=1.06\times10^6\ \text{Pa}$$

**They agree:** $1.06\times10^6\ \text{Pa} \div 101325 = 10.5$ atm. ✓

The two versions are the same physics in different clothing. What matters is that $R$, $P$, and $V$ all speak the same unit system.
:::
::::

### The combined gas law

Many problems describe *one sample of gas under two sets of conditions*. Since the amount of gas does not change, $n$ and $R$ are the same before and after, so $PV/T$ must be too:

$$\frac{P_iV_i}{T_i} = \frac{P_fV_f}{T_f}$$

This is not a new law. It is $PV = nRT$ written twice and divided, and it saves you from ever needing to know $n$.

:::: tabs
::: tab Problem
An air bubble of volume 2.54 mL rises from the bottom of a lake, where the temperature is 6.42 °C and the pressure 4.56 atm, to the surface at 24.8 °C and 1.00 atm. Find its final volume.
:::
::: tab Solution
The amount of gas in the bubble does not change as it rises, so use the combined form. Convert both temperatures to kelvin: $279.57$ K and $297.95$ K.

$$V_f=\frac{P_iV_i}{T_i}\times\frac{T_f}{P_f}=\frac{4.56\,\text{atm}\times2.54\,\text{mL}}{279.57\,\text{K}}\times\frac{297.95\,\text{K}}{1.00\,\text{atm}}=12.3\ \text{mL}$$

The bubble grew almost fivefold. Both changes push the same way — the pressure dropped by a factor of 4.56 (a large effect) and the temperature rose slightly (a small one) — which is why bubbles visibly expand as they rise.

Notice that the volume stayed in milliliters throughout. Because $V$ appears on both sides as a ratio, any consistent unit works.
:::
::::

:::: tabs
::: tab Problem
A sealed 2.00 L flask of gas at 20.0 °C and 1.00 atm is heated to 150.0 °C. What is the new pressure?
:::
::: tab Solution
The flask is sealed and rigid, so both $n$ and $V$ are fixed and the combined law reduces to $P_i/T_i = P_f/T_f$.

$$P_f = P_i\times\frac{T_f}{T_i} = 1.00\,\text{atm}\times\frac{423.15\,\text{K}}{293.15\,\text{K}} = 1.44\ \text{atm}$$

{{sp[warning] Watch out}} Using Celsius here would give $1.00 \times 150.0/20.0 = 7.5$ atm — off by a factor of five. The ratio $T_f/T_i$ is only meaningful on an absolute scale, which is why kelvin is not optional.
:::
::::

### Density and molar mass of a gas

Since $n = m/\mathcal{M}$ (mass over molar mass), substituting into $PV = nRT$ gives

$$PV = \frac{m}{\mathcal{M}}RT \quad\Longrightarrow\quad \frac{m}{V} = \frac{P\mathcal{M}}{RT}$$

and since density is $d = m/V$:

$$d = \frac{P\mathcal{M}}{RT} \qquad\text{or}\qquad \mathcal{M} = \frac{dRT}{P}$$

This is genuinely useful: it means an unknown gas can be identified by weighing a known volume of it at a known temperature and pressure — and, as Figure 5.3 shows, it also explains how a balloon flies.

![View from inside an inflating hot air balloon](../assets/hot_air_balloon.jpg =480x)
*Figure 5.3 — $d = P\mathcal{M}/RT$ explains a hot air balloon. Heating the air inside lowers its density while the air outside stays cool and dense, and the difference lifts the balloon. Charles's law describes the expansion; the density relation explains why the expansion is useful.*

:::: tabs
::: tab Problem
A gas has a density of 7.71 g/L at 36.0 °C and 2.88 atm. What is its molar mass?
:::
::: tab Solution
$$\mathcal{M}=\frac{dRT}{P}=\frac{7.71\,\text{g/L}\times0.0821\,\frac{\text{L}\cdot\text{atm}}{\text{K}\cdot\text{mol}}\times309.2\,\text{K}}{2.88\,\text{atm}}=68.0\ \text{g/mol}$$

Check the units: $\frac{(\text{g/L})(\text{L}\cdot\text{atm}/\text{K}\cdot\text{mol})(\text{K})}{\text{atm}} = \text{g/mol}$. ✓
:::
::::

:::: tabs
::: tab Problem
What is the density of $\ce{CO2}$ (44.01 g/mol) at STP? Compare it with $\ce{N2}$ (28.02 g/mol), and say what that implies.
:::
::: tab Solution
Use the equation in its density form, with STP meaning 273.15 K and 1 atm.

$$d_{\ce{CO2}}=\frac{P\mathcal{M}}{RT}=\frac{1.00\,\text{atm}\times44.01\,\text{g/mol}}{0.0821\times273.15\,\text{K}}=1.96\ \text{g/L}$$
$$d_{\ce{N2}}=\frac{1.00\times28.02}{0.0821\times273.15}=1.25\ \text{g/L}$$

At the same temperature and pressure, density is directly proportional to molar mass — everything else in the expression is identical. $\ce{CO2}$ is $44.01/28.02 = 1.57$ times denser than nitrogen, which is why it pools in low-lying spaces and why a $\ce{CO2}$ fire extinguisher blankets a fire rather than dispersing.

A shortcut worth noticing: at STP you could also divide the molar mass by 22.41 L/mol. $44.01/22.41 = 1.96$ g/L. ✓
:::
::::

### Gas stoichiometry

Chapter 3's road map ended at a mass because a balance is what you had. For a gas, a volume is what you can measure — and the ideal gas equation converts moles into exactly that, as Figure 5.4 sets out.

![Gas stoichiometry road map, from mass of a reactant to volume of a gaseous product](../assets/gas_stoichiometry_road_map.svg =840x)
*Figure 5.4 — Nothing about the first two steps changes. The given mass still becomes moles by molar mass, and moles of one substance still cross to moles of another through the coefficients of the balanced equation. All the ideal gas equation adds is a final step, V = nRT/P at the gas's temperature and pressure, that expresses the answer as a volume.*

:::: tabs
::: tab Problem
In the airbag reaction $\ce{2NaN3(s) -> 2Na(s) + 3N2(g)}$, what volume of $\ce{N2}$ is generated by 38.2 g of $\ce{NaN3}$ (65.02 g/mol) at 20.5 °C and 0.982 atm?
:::
::: tab Solution
**Steps 1 and 2 — Chapter 3, unchanged.** Get to moles of the gas you want:

$$38.2\,\text{g}\,\ce{NaN3}\times\frac{1\,\text{mol}\,\ce{NaN3}}{65.02\,\text{g}}\times\frac{3\,\text{mol}\,\ce{N2}}{2\,\text{mol}\,\ce{NaN3}}=0.881\ \text{mol}\,\ce{N2}$$

**Step 3 — the new one.** Convert moles to a volume at the stated conditions ($T = 293.7$ K):

$$V=\frac{nRT}{P}=\frac{0.881\,\text{mol}\times0.0821\,\tfrac{\text{L·atm}}{\text{mol·K}}\times293.7\,\text{K}}{0.982\,\text{atm}}=21.6\ \text{L}$$

Twenty-one liters from thirty-eight grams of solid, in milliseconds — which is exactly why sodium azide was used to inflate airbags.

{{sp[warning] Reminder}} The conditions given in the problem (20.5 °C, 0.982 atm) are *not* STP, so the 22.41 L/mol shortcut does not apply here. Use it only when the problem actually says STP.
:::
::::

> **Where this goes next.** Everything so far assumed one pure gas. Air is not one gas, and neither is anything you collect in a lab. §5.3 extends the same equation to mixtures.

## 5.3 Partial Pressures{{attrs[#blk-ch05sec03]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 5.3a}} State Dalton's law of partial pressures.
- {{sp[info] Objective 5.3a}} Calculate a mole fraction and use it to find a partial pressure.
- {{sp[info] Objective 5.3b}} Correct for water vapor pressure when a gas is collected over water.
:::

### Dalton's law

In a mixture, each gas behaves as if the others were not there. That is the content of §5.4's assumption that molecules do not interact, and it has an immediate consequence.

The **partial pressure** of a component is the pressure it would exert alone in the same container at the same temperature:

$$P_1 = \frac{n_1RT}{V}, \qquad P_2 = \frac{n_2RT}{V}, \qquad \dots$$

Since $n = n_1 + n_2 + \dots$ and $R$, $T$, $V$ are shared, adding the partial pressures gives the total. This is **Dalton's law of partial pressures**:

$$P_{\text{total}} = P_1 + P_2 + \dots$$

### Mole fraction

The **mole fraction** of a component is its share of the total moles:

$$X_i = \frac{n_i}{n_{\text{total}}}$$

Mole fractions have no units and always sum to 1. Combining the two ideas gives the relation you will use most:

$$P_i = X_i P_{\text{total}}$$

==A gas's share of the pressure equals its share of the molecules.== It makes no difference which gas it is — 20% of the molecules produce 20% of the pressure whether they are helium or radon.

:::: tabs
::: tab Problem
A mixture of gases A, B, and C has a total pressure of 3.46 atm and contains 1.53 mol A, 1.64 mol B, and 2.64 mol C. Find all three partial pressures.
:::
::: tab Solution
Total moles: $1.53 + 1.64 + 2.64 = 5.81$ mol.

$$P_\ce{A}=3.46\,\text{atm}\times\frac{1.53}{5.81}=0.911\ \text{atm}$$
$$P_\ce{B}=3.46\,\text{atm}\times\frac{1.64}{5.81}=0.977\ \text{atm}$$
$$P_\ce{C}=3.46\,\text{atm}\times\frac{2.64}{5.81}=1.57\ \text{atm}$$

**Check:** $0.911 + 0.977 + 1.57 = 3.46$ atm. ✓ The partial pressures must add to the total, and that check costs nothing.
:::
::::

:::: tabs
::: tab Problem
Dry air is 78.1% $\ce{N2}$, 20.9% $\ce{O2}$, and 0.9% Ar by moles. What is the partial pressure of oxygen when the atmospheric pressure is 1.00 atm? What if you climb to an altitude where the pressure is 0.50 atm?
:::
::: tab Solution
Percent by moles *is* the mole fraction (times 100), so $X_{\ce{O2}} = 0.209$.

**At sea level:** $P_{\ce{O2}} = 0.209\times1.00\ \text{atm} = 0.209\ \text{atm}$.

**At altitude:** $P_{\ce{O2}} = 0.209\times0.50\ \text{atm} = 0.105\ \text{atm}$.

The *composition* of air does not change with altitude — it is still 20.9% oxygen. What changes is the total pressure, and therefore the partial pressure of oxygen. Your body responds to $P_{\ce{O2}}$, not to the percentage, which is why altitude sickness is possible in air that is chemically identical to air at sea level.
:::
::::

### Collecting a gas over water

A gas produced in a reaction is often collected by bubbling it into an inverted tube filled with water (Figure 5.5). It is a convenient method with one complication: water evaporates into the collected gas.

![Collecting a gas over water, and the water-vapor correction](../assets/gas_collected_over_water.svg =800x)
*Figure 5.5 — The tube never contains only the gas you made. Water evaporates into it until the water vapor reaches its equilibrium pressure at that temperature, so the total pressure — which is what a gauge reports, or the barometer when the water levels inside and outside the tube are equal — is the sum of two partial pressures. Dalton's law makes the correction straightforward: subtract the tabulated water vapor pressure.*

{{sp[warning] Reminder}} The vapor pressure of water depends only on the temperature, and is looked up in a table — it does not depend on how much gas you collected or how large the tube is.

:::: tabs
::: tab Problem
153 mL of $\ce{H2}$ is collected over water at 23.7 °C. The atmospheric pressure is 758 mmHg and the vapor pressure of water at 23.7 °C is 22.0 mmHg. How many moles of $\ce{H2}$ were collected?
:::
::: tab Solution
**Step 1 — correct the pressure.** The 758 mmHg is the total; the hydrogen accounts for the rest after water vapor:

$$P_{\ce{H2}}=758-22.0=736\ \text{mmHg}=736\times\frac{1\,\text{atm}}{760\,\text{mmHg}}=0.968\ \text{atm}$$

**Step 2 — apply the ideal gas equation** with the *corrected* pressure:

$$n=\frac{PV}{RT}=\frac{0.968\,\text{atm}\times0.153\,\text{L}}{0.0821\times296.9\,\text{K}}=6.08\times10^{-3}\ \text{mol}$$

Skipping step 1 would give $6.26\times10^{-3}$ mol — about 3% too high. The correction is small but systematic, and it is always in the same direction: forgetting it always overstates your yield.
:::
::::

> **Where this goes next.** You can now calculate with gases confidently. §5.4 asks the harder question: *why* does one equation work so well for every gas at ordinary conditions? The answer is a picture of what molecules are doing.

## 5.4 The Kinetic Molecular Theory of Gases{{attrs[#blk-ch05sec04]}}

:::success
**Learning Objectives**
- Define energy, work, and kinetic energy.
- {{sp[info] Objective 5.4a}} State the four assumptions of the kinetic molecular theory.
- {{sp[info] Objective 5.4a}} Use the theory to explain each gas law.
- {{sp[info] Objective 5.4a}} Describe the distribution of molecular speeds and calculate $u_\text{rms}$.
- {{sp[info] Objective 5.4b}} Distinguish diffusion from effusion and apply Graham's law.
:::

### Energy, work, and kinetic energy

The theory is built on molecular motion, so three mechanical terms are needed first — and Chapter 6 will assume all three.

**Energy** is the capacity to do work or produce change. **Work**, in mechanics, is force times distance. Since energy can be measured as work done:

$$\text{energy} = \text{work} = \text{force}\times\text{distance}$$

The SI unit is the **joule**:

$$1\ \text{J} = 1\ \text{kg}\cdot\text{m}^2/\text{s}^2 = 1\ \text{N}\cdot\text{m}$$

**Kinetic energy** is the energy of motion, $KE = \frac{1}{2}mu^2$ for a particle of mass $m$ moving at speed $u$.

### The four assumptions

1. A gas consists of molecules separated by distances **far greater than their own size**. They have mass but effectively no volume.
2. Molecules are in **constant random motion** and collide frequently. All collisions are **perfectly elastic** — an elastic collision is one in which the total kinetic energy afterwards equals the total before, so no energy is lost to the collision itself.
3. Molecules exert **neither attractive nor repulsive forces** on one another.
4. The **average kinetic energy is proportional to the absolute temperature**:
$$\overline{KE}=\tfrac{1}{2}m\overline{u^2}\ \propto\ T$$

Assumption 4 carries a consequence worth stating on its own: **any two gases at the same temperature have the same average kinetic energy**. Not the same speed — the same energy. Since $KE$ depends on both mass and speed, heavier molecules must, on average, be moving more slowly to have the same average energy as lighter ones. That single fact drives the rest of this section.

### Why each gas law holds

![Molecular pictures explaining the gas laws](../assets/kmt_explains_gas_laws.svg =820x)
*Figure 5.6 — Pressure is molecules striking the walls, so any change to the rate or force of those impacts changes the pressure. Compressing the gas packs the same molecules into less space, so they hit the walls more often (Boyle). Heating them makes each impact faster and harder, so the gas expands until the pressure balances again (Charles).*

Figure 5.6 draws the two that are hardest to see in words.

- **Compressibility.** Assumption 1: the molecules are mostly far apart, so there is empty space to remove.
- **Boyle's law.** Pressure comes from the rate of wall collisions, which is proportional to the number of molecules per unit volume. At constant temperature and a fixed amount of gas (so each collision delivers the same average force), halve the volume and you double the number density, so you double the collision rate — and therefore the pressure. Hence $P \propto 1/V$.
- **Charles's law.** Assumption 4 says raising the temperature raises the average kinetic energy, so molecules strike the walls both more often and harder. At fixed external pressure the gas must expand until the reduced number density brings the pressure back into balance. Hence $V \propto T$ (with $T$ in kelvins).
- **Avogadro's law.** If two gases are at the same $P$, $V$, and $T$, then by $PV=nRT$ they must contain the same $n$ — equal volumes hold equal numbers of molecules, whatever they are.
- **Dalton's law.** Assumption 3: molecules ignore one another, so the presence of a second gas does not change how the first one strikes the walls. The pressures therefore simply add.

:::: tabs
::: tab Problem
A sealed rigid container of gas is heated. Using the kinetic molecular theory rather than the gas laws, explain why the pressure rises — and identify which assumption does the work.
:::
::: tab Solution
Start from what pressure *is*: molecules striking the walls. The pressure depends on how often they strike and how hard.

**Assumption 4** is the one that matters: average kinetic energy is proportional to absolute temperature. Heating the gas therefore raises the average kinetic energy, so the molecules move faster.

Two consequences follow, and both push the pressure the same way:
1. Faster molecules cross the container more often, so the **collision rate rises**.
2. Each collision carries more momentum, so **each impact is harder**.

The container is rigid, so the gas cannot relieve either effect by expanding. The pressure must rise.

Note the contrast with Charles's law, where the *pressure* is held fixed instead and the gas expands until the falling number density cancels the faster impacts. Same mechanism, different constraint — and the constraint is what decides which quantity changes.
:::
::::

### Molecular speeds

Molecules do not all move at the same speed; there is a distribution, and it has a characteristic shape. A convenient single number to summarize it is the **root-mean-square speed**:

$$u_\text{rms}=\sqrt{\frac{3RT}{\mathcal{M}}}$$

with $R = 8.314$ J/(K·mol) and $\mathcal{M}$ the molar mass **in kg/mol**.

![Maxwell-Boltzmann speed distributions by molar mass and by temperature](../assets/molecular_speed_distribution.svg =840x)
*Figure 5.7 — The spread of molecular speeds. **Left:** three gases at the same temperature. All three have the same average kinetic energy, so the heaviest moves slowest — $\ce{CO2}$ peaks far below helium. **Right:** one gas at three temperatures. Heating shifts the whole distribution to higher speeds and spreads it out. Dashed lines mark $u_\text{rms}$ in each case.*

Figure 5.7 shows what those distributions look like. The square root is worth dwelling on, because it makes mass matter much less than students expect. ==At the same temperature, a molecule 100 times heavier moves not 100 times slower, but $\sqrt{100} = 10$ times slower.==

:::: tabs
::: tab Problem
Calculate $u_\text{rms}$ for $\ce{N2}$ (28.02 g/mol) and for He (4.003 g/mol) at 25 °C.
:::
::: tab Solution
Convert molar masses to kg/mol — this is the step people miss — and the temperature to kelvin (298 K).

$$u_\text{rms}(\ce{N2})=\sqrt{\frac{3\times8.314\times298}{0.02802}}=515\ \text{m/s}$$
$$u_\text{rms}(\ce{He})=\sqrt{\frac{3\times8.314\times298}{0.004003}}=1363\ \text{m/s}$$

Helium is about 2.6 times faster. Check that against the square-root rule: $\sqrt{28.02/4.003}=\sqrt{7.00}=2.65$. ✓

Both figures are startlingly large — 515 m/s is faster than the speed of sound in air. Molecules do not travel far at that speed before colliding, which is why gases mix in seconds rather than instantly.
:::
::::

### Diffusion and effusion

**Diffusion** is the gradual mixing of one gas through another by molecular motion. **Effusion** is the escape of a gas through a small opening into a vacuum. They are different processes, but both are governed by molecular speed, so both obey the same relation (exactly for effusion, approximately for diffusion) — **Graham's law**:

$$\frac{r_1}{r_2}=\frac{t_2}{t_1}=\sqrt{\frac{\mathcal{M}_2}{\mathcal{M}_1}}$$

where $r$ is a rate and $t$ is the time taken for the same amount of gas to effuse or diffuse. Note the inversion: the *lighter* gas has the *larger* rate, so each gas's molar mass appears on the opposite side from its rate (gas 1's molar mass is in the *denominator* on the right). Figure 5.8 puts numbers to it.

![Bar chart of relative effusion rates for 5 gases](../assets/grahams_law_effusion.svg =520x)
*Figure 5.8 — Lighter molecules move faster at the same temperature, so they effuse faster: $\ce{H2}$ effuses roughly 4.7× faster than $\ce{CO2}$, matching $\sqrt{44.01/2.02}\approx4.67$.*

:::: tabs
::: tab Problem
How much faster does helium (4.003 g/mol) effuse than argon (39.95 g/mol)?
:::
::: tab Solution
Put the gas whose rate you want in position 1:

$$\frac{r_{\ce{He}}}{r_{\ce{Ar}}}=\sqrt{\frac{\mathcal{M}_{\ce{Ar}}}{\mathcal{M}_{\ce{He}}}}=\sqrt{\frac{39.95}{4.003}}=\sqrt{9.98}=3.16$$

Helium effuses **3.16 times faster**.

Sanity check the direction: helium is lighter, so it should be faster, and 3.16 > 1. ✓ If your answer comes out less than 1 for the lighter gas, you have the ratio upside down.
:::
::::

:::: tabs
::: tab Problem
An unknown gas effuses 0.355 times as fast as helium (4.003 g/mol) under the same conditions. What is its molar mass?
:::
::: tab Solution
This runs Graham's law backwards — you have the rate ratio and want a molar mass.

$$\frac{r_{\text{unk}}}{r_{\ce{He}}}=\sqrt{\frac{\mathcal{M}_{\ce{He}}}{\mathcal{M}_{\text{unk}}}} \;\Longrightarrow\; 0.355=\sqrt{\frac{4.003}{\mathcal{M}_{\text{unk}}}}$$

Square both sides and solve:

$$0.126=\frac{4.003}{\mathcal{M}_{\text{unk}}} \;\Longrightarrow\; \mathcal{M}_{\text{unk}}=\frac{4.003}{0.126}=31.8\ \text{g/mol}$$

About 32 g/mol — consistent with $\ce{O2}$. Sanity check: the gas is slower than helium, so it must be heavier, and 31.8 > 4.003. ✓

This is how effusion measurements identify unknown gases, and — at industrial scale — how uranium isotopes have been separated (as gaseous UF6).
:::
::::

> **Where this goes next.** Two key assumptions in §5.4 were idealizations: molecules with no volume, exerting no forces. §5.5 asks what happens when those assumptions stop being safe.

## 5.5 Deviations from Ideal Behavior{{attrs[#blk-ch05sec05]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 5.5a}} Explain why real gases deviate from ideal behavior.
- {{sp[info] Objective 5.5a}} Predict the conditions under which deviations become significant.
- {{sp[info] Objective 5.5a}} Interpret the compressibility factor.
- {{sp[info] Objective 5.5a}} Recognize the van der Waals equation and what each correction term does.
:::

### Where the model fails

Two of the kinetic-theory assumptions are simply false for real molecules:

- **Molecules do occupy volume.** Assumption 1 treated them as points. The volume available for a molecule to move in is the container's volume *minus* the space the other molecules take up — so the free volume is always less than $V$.
- **Molecules do attract one another.** Assumption 3 denied it. A molecule approaching the wall is pulled back slightly by its neighbors, so it strikes with less force than it otherwise would — meaning the observed pressure is *lower* than the ideal equation predicts.

Both effects exist always. What matters is when they become large enough to notice, and the answer follows from the two bullets:

- At **high pressure**, molecules are crowded, so the space they occupy is a significant fraction of the container.
- At **low temperature**, molecules move slowly, so attractive forces have time to act and are no longer negligible compared with the kinetic energy.

==Deviations are largest at high pressure and low temperature — precisely the conditions under which a gas is on the verge of condensing into a liquid.== A model that ignores intermolecular forces is bound to fail exactly where those forces are about to win.

![Schematic compressibility-factor chart](../assets/real_gas_deviation.svg =520x)
*Figure 5.9 — The compressibility factor $Z=PV/nRT$ equals exactly 1 for an ideal gas at every pressure. Real gases with weak attractions ($\ce{H2}$, He) drift above 1 almost immediately; most real gases first dip below 1 (attraction dominates) before rising above 1 at very high pressure (molecular volume dominates).*

The compressibility factor $Z = PV/nRT$ is a convenient way to measure the failure, because it is exactly 1 for an ideal gas at all conditions. Reading a real gas's curve tells you which effect is winning: $Z < 1$ means attractions dominate (the gas is more compressible than ideal), and $Z > 1$ means molecular volume dominates (less compressible than ideal).

:::: tabs
::: tab Problem
A gas is compressed at constant temperature and its measured $Z = PV/nRT$ falls to 0.85. Which effect is dominating, and what does it say about the gas's molar volume compared with the ideal prediction?
:::
::: tab Solution
$Z < 1$ means $PV < nRT$, so the actual volume is *smaller* than the ideal gas equation predicts at that pressure.

That is the signature of **attraction dominating**: the molecules are pulling on one another, which effectively helps the compression along, so the gas takes up less room than an ideal gas would.

Had the answer been $Z > 1$, the opposite would apply — the molecules' own finite volume would be resisting further compression, and the gas would occupy more room than ideal. The crossover from one regime to the other is what produces the dip-then-rise shape of the curves in Figure 5.9.
:::
::::

### The van der Waals equation

The van der Waals equation repairs the ideal gas equation by correcting each failure directly:

$$\left(P+\frac{an^2}{V^2}\right)(V-nb)=nRT$$

- The **$an^2/V^2$ term is added to $P$**, compensating for the pressure lost to intermolecular attraction. Larger $a$ means stronger attractions.
- The **$nb$ term is subtracted from $V$**, removing the space the molecules themselves occupy. Larger $b$ means bigger molecules.

Both $a$ and $b$ are measured experimentally and are specific to each gas. Set them both to zero and the equation collapses back to $PV = nRT$ — the ideal gas equation is the special case in which molecules have no size and no attractions.

:::: tabs
::: tab Problem
Which gas would you expect to behave more ideally at room temperature and 1 atm: helium or water vapor? Which has the larger van der Waals $a$?
:::
::: tab Solution
**Helium behaves more ideally.** It is a small, nonpolar atom with only very weak attractions between atoms, so both corrections are tiny.

Water molecules are polar and hydrogen-bond strongly to one another (Chapter 11), so their attractions are large — which is why water is a *liquid* at room temperature while helium remains a gas down to nearly absolute zero.

**Water has the much larger $a$**, since $a$ measures the strength of intermolecular attraction. The two facts are the same fact: strong attractions cause both large deviations from ideality and high boiling points.
:::
::::


## Synthesis

==This chapter builds one equation, $PV=nRT$, three ways over: assembled from three experimental laws in §5.2, explained from molecular motion in §5.4, and then bounded in §5.5 by identifying exactly where its assumptions fail.== That progression — empirical law, then mechanism, then limits — is the shape of most of what follows in this course.

Backwards, the chapter rests entirely on Chapter 3: every gas-stoichiometry problem is the mole road map with one extra step. Forwards, the kinetic picture developed in §5.4 is reused immediately. Chapter 6 defines pressure–volume work as that done by a gas expanding against an external pressure. Chapter 11 takes the intermolecular attractions that §5.5 treats as a nuisance and makes them the entire subject, explaining why substances condense at all. Chapter 13 uses molecular speeds and collision frequencies to explain reaction rates. And the ideal gas equation itself reappears whenever a gas is a reactant or a product, from equilibrium constants in Chapter 14 to electrochemical cells in Chapter 18.

## Asset and License Record for This Chapter

| Asset | Source URL | License | Attribution |
|---|---|---|---|
| `assets/pressure_and_barometer.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; released under this package's CC BY 4.0 license. |
| `assets/gas_laws_panels.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; released under this package's CC BY 4.0 license. |
| `assets/hot_air_balloon.jpg` | https://commons.wikimedia.org/wiki/File:Inside_an_inflating_hot_air_balloon.jpg | CC BY 2.0 | Ville Miettinen, via Wikimedia Commons (originally Flickr), CC BY 2.0. Resized from the original for web use. |
| `assets/gas_stoichiometry_road_map.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; released under this package's CC BY 4.0 license. |
| `assets/gas_collected_over_water.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; released under this package's CC BY 4.0 license. |
| `assets/kmt_explains_gas_laws.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; released under this package's CC BY 4.0 license. |
| `assets/molecular_speed_distribution.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib; released under this package's CC BY 4.0 license. |
| `assets/grahams_law_effusion.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib using real molar masses; released under this package's CC BY 4.0 license. |
| `assets/real_gas_deviation.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated with matplotlib, schematic; released under this package's CC BY 4.0 license. |
