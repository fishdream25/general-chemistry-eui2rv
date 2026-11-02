{{nyml
kind: document
format: 1
title: Chapter 5 Assessment Guide: Gases
}}

# Chapter 5 Assessment Guide: Gases

## Source and Format

**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 5 (CC BY 4.0). **Audience:** introductory undergraduate general chemistry, first semester. **Note:** this is design guidance for building assessments — question *guides* an instructor or generator can instantiate into many concrete questions — not a finished question bank or answer key.

## General Assessment Priorities

- Require temperature to be converted to kelvin as an explicit first step in every ideal-gas-equation problem — this is the single most common source of numeric errors in the chapter.
- Test the ideal gas equation in all four "solve for X" directions (P, V, n, T) across the assessment set, not just "solve for P."
- Pair every partial-pressure problem with an explicit mole-fraction or Dalton's-law justification, not just a bare final number.
- Require kinetic-molecular-theory explanations to name the *specific* assumption(s) responsible for a given gas-law behavior, not just restate the law itself.

## Objective 5.1a: Convert between pressure units

### Target understanding

A student can convert a pressure value among Pa, atm, mmHg, and torr using the fixed conversion factors.

### Question guides

**1. Forward — convert mmHg to Pa**
- Variables & ranges: any pressure in mmHg.
- Constraint: correct use of $1\,\text{atm}=760\,\text{mmHg}=101325\,\text{Pa}$.
- Contexts: any measured gas pressure.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (489 mmHg → Pa).

**2. Inverse — convert Pa or atm to torr**
- Variables & ranges: any pressure in Pa or atm.
- Constraint: recognize $1\,\text{torr}=1\,\text{mmHg}$.
- Contexts: any measured gas pressure.
- Formats: workout.
- Worked instantiation: "Convert 2.00 atm to torr." → $2.00\times760=1520$ torr.

**3. Conceptual — why so many pressure units exist**
- Variables & ranges: qualitative.
- Constraint: must reference historical/instrumental origins (mercury barometers vs. SI-derived units).
- Contexts: any pressure-measuring instrument.
- Formats: short-answer.
- Worked instantiation: "Why do both mmHg and Pa remain in common use for gas pressure?" → mmHg (and torr) originate from mercury-barometer measurement and remain common in lab and medical contexts; Pa is the SI-derived unit used in more formal physical-chemistry contexts — both describe the same physical quantity.

**4. Error analysis**
- Variables & ranges: a student uses $1\,\text{atm}=760\,\text{Pa}$ (confusing mmHg and Pa conversion factors).
- Constraint: correction must state the correct atm-to-Pa factor.
- Contexts: any pressure conversion.
- Formats: short-answer.
- Worked instantiation: "A student converts atm to Pa using the factor 760. What's wrong?" → 760 is the mmHg-per-atm factor, not the Pa-per-atm factor; 1 atm equals 101325 Pa, not 760 Pa.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 pressure-unit conversions across different unit pairs. |
| Group discussion | Understand | Discuss why medicine (blood pressure) still uses mmHg. |
| Quiz | Apply | One pressure conversion. |
| Exam | Apply | Combine with Objective 5.2a (convert given pressure units before using $PV=nRT$). |
| Project/activity | Understand | Students find 3 real-world pressure readings (weather report, tire gauge, etc.) and convert each to atm. |

## Objective 5.2a: Apply the ideal gas equation

### Target understanding

A student can solve $PV=nRT$ for any one variable given the other three, including combined-gas-law scenarios where $n$ is held constant across two states.

### Question guides

**1. Forward — solve for pressure**
- Variables & ranges: given $n$, $V$, $T$ (°C, must convert to K).
- Constraint: temperature converted to kelvin before substitution.
- Contexts: any ideal-gas scenario.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (1.92 mol, 4.50 L, 25.6 °C → 10.5 atm).

**2. Inverse — combined gas law (two-state problem)**
- Variables & ranges: initial and final $P$, $V$, $T$ with $n$ constant.
- Constraint: student must recognize $n$ is constant and set up $P_iV_i/T_i=P_fV_f/T_f$.
- Contexts: a gas sample changing conditions (e.g., rising through a fluid, heated in a sealed container).
- Formats: workout.
- Worked instantiation: see the study guide's worked example (lake air bubble).

**3. Conceptual — why n must be explicitly tracked**
- Variables & ranges: qualitative.
- Constraint: must reference that a combined-gas-law shortcut is only valid when moles don't change.
- Contexts: any two-state gas problem, contrasted with one where gas is added/removed.
- Formats: short-answer.
- Worked instantiation: "Why can't you use $P_iV_i/T_i=P_fV_f/T_f$ if gas is added to the container partway through?" → That shortcut comes from canceling $n$ and $R$ between the initial and final $PV=nRT$ equations, which is only valid when $n$ is the same in both states; if gas is added, $n$ changes and the full ideal gas equation must be used at each state separately.

**4. Error analysis**
- Variables & ranges: a student uses Celsius directly in $PV=nRT$.
- Constraint: correction must show the required kelvin conversion.
- Contexts: any ideal-gas-equation problem stated in °C.
- Formats: short-answer.
- Worked instantiation: "A student computes $P=nRT/V$ using $T=25.6$ (in °C) directly. What's wrong?" → The ideal gas equation requires temperature in kelvin; $T$ must first be converted to $25.6+273.2=298.8$ K before substituting.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 4–6 ideal-gas-equation problems, solving for each of P, V, n, T at least once. |
| Group discussion | Understand | Discuss why STP conditions (0 °C, 1 atm) are a useful reference point. |
| Quiz | Apply | One ideal-gas-equation problem. |
| Exam | Analyze | Combine with a stoichiometric setup (Objective 5.2b or a Chapter 3 mole conversion) requiring the ideal gas law as a final step. |
| Project/activity | Apply | Students calculate the volume of gas produced by a real reaction (e.g., an airbag inflator, a fire extinguisher) at given conditions. |

## Objective 5.2b: Calculate gas density and molar mass

### Target understanding

A student can rearrange the ideal gas equation to find a gas's molar mass from its density (or vice versa), using $\mathcal{M}=dRT/P$.

### Question guides

**1. Forward — molar mass from density**
- Variables & ranges: given density, temperature, pressure.
- Constraint: correct rearrangement of $PV=nRT$ via $n=m/\mathcal{M}$ and $d=m/V$.
- Contexts: any pure gas sample.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (7.71 g/L, 36.0 °C, 2.88 atm → 68.0 g/mol).

**2. Inverse — density from molar mass**
- Variables & ranges: given molar mass, temperature, pressure.
- Constraint: correct rearrangement in the reverse direction.
- Contexts: any known gas at specified conditions.
- Formats: workout.
- Worked instantiation: "Find the density of $\ce{CO2}$ (molar mass 44.01 g/mol) at 25 °C and 1.00 atm." → $d=\mathcal{M}P/(RT)=44.01\times1.00/(0.0821\times298.15)=1.80$ g/L.

**3. Conceptual — why gas density depends on both T and P**
- Variables & ranges: qualitative, contrasting gas density with liquid/solid density.
- Constraint: must reference gas compressibility (unlike liquids/solids).
- Contexts: any gas sample at changing conditions.
- Formats: short-answer.
- Worked instantiation: "Why does a gas's density change significantly with temperature and pressure, while a liquid's density barely does?" → Gases are highly compressible — changing $T$ or $P$ changes the volume a fixed mass occupies substantially, directly changing density; liquids and solids are nearly incompressible, so their volume (and density) barely changes.

**4. Error analysis**
- Variables & ranges: a student forgets to convert density units consistently with the other variables (e.g., mixing g/mL with L·atm/(K·mol) R value).
- Constraint: correction must show the unit mismatch.
- Contexts: any density/molar-mass calculation.
- Formats: short-answer.
- Worked instantiation: "A student uses a density in g/mL directly with $R=0.0821$ L·atm/(K·mol). What's the risk?" → $R=0.0821$ L·atm/(K·mol) requires density in g/L to stay dimensionally consistent; a density given in g/mL must first be converted to g/L (×1000) or a different value of $R$ must be used.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 density/molar-mass problems, both directions. |
| Group discussion | Understand | Discuss how gas density measurements can help identify an unknown gas. |
| Quiz | Apply | One density-to-molar-mass problem. |
| Exam | Analyze | Combine with Objective 5.1a (unit conversion required before substitution). |
| Project/activity | Apply | Students identify an unknown gas from its measured density at known T and P. |

## Objective 5.3a: Apply Dalton's law of partial pressures and mole fraction

### Target understanding

A student can calculate a component gas's partial pressure from its mole fraction and the total pressure, and can verify that partial pressures sum to the total.

### Question guides

**1. Forward — partial pressure from mole data**
- Variables & ranges: moles of 2–3 gases and a total pressure.
- Constraint: correct mole-fraction calculation before multiplying by total pressure.
- Contexts: any gas mixture.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (gases A, B, C; 3.46 atm total).

**2. Inverse — total pressure from partial pressures**
- Variables & ranges: 2–3 given partial pressures.
- Constraint: simple addition, correctly applied.
- Contexts: any gas mixture.
- Formats: workout.
- Worked instantiation: "Two gases have partial pressures 0.911 atm and 0.975 atm in a mixture. If these are the only two gases present, what is the total pressure?" → $0.911+0.975=1.886$ atm.

**3. Conceptual — why mole fraction, not mass fraction, determines partial pressure**
- Variables & ranges: qualitative.
- Constraint: must reference that pressure arises from the number of colliding particles, not their mass.
- Contexts: a mixture of gases with different molar masses.
- Formats: short-answer.
- Worked instantiation: "Why does partial pressure depend on mole fraction rather than mass fraction?" → Pressure arises from the frequency and force of molecular collisions with the container walls, which depends on the *number* of molecules (moles) present, not their mass.

**4. Error analysis**
- Variables & ranges: a student computes mole fraction using mass instead of moles.
- Constraint: correction must show the required mass-to-mole conversion first.
- Contexts: any gas mixture given in mass units.
- Formats: short-answer.
- Worked instantiation: "A student computes mole fraction directly from grams of each gas, without converting to moles first. What's wrong?" → Mole fraction is defined in terms of moles, not mass; each gas's mass must first be divided by its own molar mass to get moles before computing the fraction.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 partial-pressure/mole-fraction problems. |
| Group discussion | Understand | Discuss how Dalton's law applies to Earth's atmosphere (N₂, O₂, Ar partial pressures). |
| Quiz | Apply | One partial-pressure calculation. |
| Exam | Analyze | Combine with Objective 5.3b (subtract water vapor pressure, then apply Dalton's law reasoning). |
| Project/activity | Apply | Students calculate the partial pressures of the major components of dry air at 1.00 atm. |

## Objective 5.3b: Correct for water vapor pressure when a gas is collected over water

### Target understanding

A student can subtract water's vapor pressure from a measured total pressure to find a collected gas's true partial pressure, then use it in further calculations.

### Question guides

**1. Forward — find moles of gas collected over water**
- Variables & ranges: total pressure, water vapor pressure at the given temperature, volume, temperature.
- Constraint: subtraction must happen before applying $PV=nRT$.
- Contexts: any gas generated and collected over water (a classic lab technique).
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{H2}$ collected over water, 153 mL).

**2. Inverse — find the total measured pressure given a known dry-gas amount**
- Variables & ranges: known moles of dry gas, volume, temperature, and water's vapor pressure.
- Constraint: student must add water's vapor pressure back to the calculated dry-gas partial pressure.
- Contexts: the reverse of the forward guide.
- Formats: workout.
- Worked instantiation: "If $6.08\times10^{-3}$ mol of dry $\ce{H2}$ occupies 153 mL at 23.7 °C, and water's vapor pressure at that temperature is 22.4 mmHg, what total pressure would a manometer read?" → Solve for $P_{H_2}$ from $PV=nRT$ (≈736 mmHg), then add 22.4 mmHg → ≈758 mmHg total.

**3. Conceptual — why water vapor pressure depends only on temperature**
- Variables & ranges: qualitative.
- Constraint: must reference vapor-liquid equilibrium (forward link to Ch. 11/17).
- Contexts: any gas-over-water collection at a stated temperature.
- Formats: short-answer.
- Worked instantiation: "Why can you look up a single 'water vapor pressure' value for a given temperature, regardless of how much gas is being collected?" → At a given temperature, water's vapor pressure is a fixed equilibrium property of water itself (how much water vapor the air above liquid water can hold before condensation balances evaporation) — it doesn't depend on what other gas is present or how much of it there is.

**4. Error analysis**
- Variables & ranges: a student uses the *total* measured pressure directly in $PV=nRT$ without subtracting water's vapor pressure.
- Constraint: correction must show the resulting overestimate of moles of collected gas.
- Contexts: any gas-over-water collection.
- Formats: short-answer.
- Worked instantiation: "A student computes moles of $\ce{H2}$ using the full 758 mmHg instead of the corrected 736 mmHg. What's the error's effect?" → Using the higher, uncorrected pressure overstates the partial pressure attributable to $\ce{H2}$ alone, which would overestimate the calculated moles of $\ce{H2}$ actually collected.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 gas-collected-over-water problems. |
| Group discussion | Understand | Discuss why this technique is common for collecting gases that don't react with or dissolve in water. |
| Quiz | Apply | One water-vapor-correction problem. |
| Exam | Analyze | Combine with Objective 5.2a (the corrected pressure feeds into a standard ideal-gas-equation calculation). |
| Project/activity | Evaluate | Students look up water's vapor pressure at 3 different temperatures and discuss the trend. |

## Objective 5.4a: State the kinetic molecular theory and use it to explain gas-law behavior

### Target understanding

A student can state the four assumptions of kinetic molecular theory and explain each gas law (Boyle's, Charles's, Avogadro's, Dalton's) in terms of those specific assumptions.

### Question guides

**1. Forward — explain a gas law via KMT**
- Variables & ranges: one of Boyle's, Charles's, Avogadro's, or Dalton's laws.
- Constraint: explanation must cite the specific relevant KMT assumption(s).
- Contexts: any of the four gas laws.
- Formats: short-answer.
- Worked instantiation: see the study guide's explanation of each law from KMT.

**2. Inverse — identify which KMT assumption a scenario tests**
- Variables & ranges: a described scenario (e.g., two different gases at the same temperature).
- Constraint: student must name the specific assumption (not just "kinetic theory" vaguely).
- Contexts: any KMT-related scenario.
- Formats: short-answer.
- Worked instantiation: "Two different ideal gases are at the same temperature. What does KMT say must be true about them?" → They must have the same average kinetic energy (assumption 4), even though they may have very different average speeds if their molar masses differ.

**3. Conceptual — why real gases only approximately follow KMT**
- Variables & ranges: qualitative, forward link to Objective 5.5a.
- Constraint: must connect specific KMT assumptions to where they fail for real gases.
- Contexts: real-gas behavior at high pressure or low temperature.
- Formats: short-answer.
- Worked instantiation: "Which KMT assumption(s) fail most clearly for a real gas at high pressure?" → The assumption that molecules have negligible volume — at high pressure, molecules are packed close enough that their actual volume becomes a significant fraction of the container's volume.

**4. Error analysis**
- Variables & ranges: a student claims two gases at the same temperature have the same average speed.
- Constraint: correction must distinguish kinetic energy (same) from speed (different, depends on mass).
- Contexts: two gases of different molar mass at the same temperature.
- Formats: short-answer.
- Worked instantiation: "A student says $\ce{H2}$ and $\ce{O2}$ at the same temperature must have the same average speed, since KMT says they have the same average kinetic energy. What's wrong?" → Equal kinetic energy ($\frac12m\overline{u^2}$) with very different masses means very different speeds — the lighter $\ce{H2}$ molecules move much faster than the heavier $\ce{O2}$ molecules, even though $\overline{KE}$ is the same for both.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | 3–4 "explain this gas law using KMT" items. |
| Group discussion | Analyze | Debate which single KMT assumption is most important for explaining Boyle's Law specifically. |
| Quiz | Understand | One KMT-explanation item. |
| Exam | Analyze | Combine with Objective 5.5a (identify which assumptions real gases violate). |
| Project/activity | Understand | Students create a one-page diagram connecting each KMT assumption to the gas law(s) it explains. |

## Objective 5.4b: Apply Graham's law of effusion and diffusion

### Target understanding

A student can use Graham's law to relate the effusion/diffusion rates (or times) of two gases to their molar masses.

### Question guides

**1. Forward — compare effusion rates**
- Variables & ranges: two gases with known molar masses.
- Constraint: correct square-root relationship, not a direct ratio.
- Contexts: any two-gas comparison.
- Formats: workout.
- Worked instantiation: see the study guide's Figure 5.3 (H₂ vs. CO₂ effusion rate ratio).

**2. Inverse — find an unknown molar mass from a time ratio**
- Variables & ranges: a known gas's molar mass and time, plus an unknown gas's time.
- Constraint: correct algebraic rearrangement of Graham's law.
- Contexts: any effusion-time comparison experiment.
- Formats: workout.
- Worked instantiation: "Gas X takes 3.0 times as long to effuse as $\ce{H2}$ (2.02 g/mol) under the same conditions. What is X's molar mass?" → $t_X/t_{H_2}=\sqrt{\mathcal{M}_X/\mathcal{M}_{H_2}} \Rightarrow \mathcal{M}_X=\mathcal{M}_{H_2}\times(t_X/t_{H_2})^2=2.02\times9=18.2$ g/mol.

**3. Conceptual — why the relationship is a square root, not linear**
- Variables & ranges: qualitative, connecting to $u_{rms}=\sqrt{3RT/\mathcal{M}}$.
- Constraint: must reference that speed depends on the square root of $1/\mathcal{M}$, not $1/\mathcal{M}$ directly.
- Contexts: the $u_{rms}$ formula.
- Formats: short-answer.
- Worked instantiation: "Why does doubling a gas's molar mass not simply halve its effusion rate?" → Effusion rate is proportional to average speed, which scales as $\sqrt{1/\mathcal{M}}$ (from $u_{rms}=\sqrt{3RT/\mathcal{M}}$) — a square-root relationship, not a direct inverse proportionality, so doubling molar mass only reduces speed by a factor of $\sqrt{2}$, not 2.

**4. Error analysis**
- Variables & ranges: a student uses molar mass ratios directly (without the square root) in Graham's law.
- Constraint: correction must reinsert the square root.
- Contexts: any Graham's-law problem.
- Formats: short-answer.
- Worked instantiation: "A student computes $r_1/r_2=\mathcal{M}_2/\mathcal{M}_1$ (no square root). What's wrong?" → Graham's law requires the square root of the molar-mass ratio, not the ratio itself; omitting the square root overstates the actual rate difference.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 Graham's-law problems, both directions. |
| Group discussion | Understand | Discuss why helium balloons deflate faster than air-filled ones (effusion through microscopic pores). |
| Quiz | Apply | One Graham's-law problem. |
| Exam | Apply | Combine with Objective 5.4a (connect the square-root relationship back to KMT's speed-mass relationship). |
| Project/activity | Evaluate | Students design an experiment (real or thought experiment) to measure the molar mass of an unknown gas via effusion timing. |

## Objective 5.5a: Explain why and when real gases deviate from ideal behavior

### Target understanding

A student can explain that real gases deviate from ideal behavior most significantly at high pressure and low temperature, identify the two physical causes (molecular volume, intermolecular attraction), and recognize the van der Waals equation as the correction.

### Question guides

**1. Forward — predict the direction of deviation**
- Variables & ranges: a gas at high pressure vs. low pressure, or low temperature vs. high temperature.
- Constraint: must state whether deviation increases or decreases, and why.
- Contexts: any real gas under varying conditions.
- Formats: short-answer.
- Worked instantiation: "Would you expect $\ce{CO2}$ to behave more or less ideally at 500 atm compared to 1 atm?" → Less ideally — at very high pressure, the gas's own molecular volume becomes a significant fraction of the total volume, and this deviation grows with increasing pressure.

**2. Inverse — identify which correction term addresses which effect**
- Variables & ranges: the van der Waals equation's $a$ and $b$ terms.
- Constraint: student must match each term to its physical meaning.
- Contexts: the van der Waals equation.
- Formats: short-answer.
- Worked instantiation: "In the van der Waals equation, which term corrects for intermolecular attraction, and which corrects for molecular volume?" → The $an^2/V^2$ term (added to pressure) corrects for attraction; the $nb$ term (subtracted from volume) corrects for molecular volume.

**3. Conceptual — why low temperature (not just high pressure) causes deviation**
- Variables & ranges: qualitative.
- Constraint: must reference that slow-moving molecules spend more time near each other, allowing attraction to matter more.
- Contexts: any real gas near its condensation point.
- Formats: short-answer.
- Worked instantiation: "Why does low temperature increase deviation from ideal behavior, even at moderate pressure?" → At low temperature, molecules move more slowly, giving intermolecular attractive forces more time to act — an effect the ideal gas model assumes away entirely.

**4. Error analysis**
- Variables & ranges: a student assumes all real gases deviate from ideal behavior in the same way (always $Z<1$).
- Constraint: correction must note that weakly-attracting gases (H₂, He) can show $Z>1$ instead.
- Contexts: Figure 5.4 (compressibility factor chart).
- Formats: short-answer.
- Worked instantiation: "A student assumes the compressibility factor $Z$ is always less than 1 for real gases. What's the exception?" → Gases with very weak intermolecular attraction (like H₂ and He) can show $Z>1$ across most pressures, since their molecular-volume effect dominates over their (very weak) attractive effect.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | 3–4 real-gas-deviation prediction/explanation items. |
| Group discussion | Analyze | Debate why H₂ and He behave differently from N₂ or CO₂ in Figure 5.4. |
| Quiz | Understand | One real-gas-deviation explanation item. |
| Exam | Analyze | Combine with Objective 5.4a (connect back to which specific KMT assumptions fail). |
| Project/activity | Understand | Students look up van der Waals $a$ and $b$ constants for 3 gases and relate the values to molecular size/polarity. |

## Rubric Themes for Chapter 5

- **Kelvin conversion is mandatory, not optional.** Any ideal-gas-equation answer using an uncoverted Celsius temperature is treated as incorrect, even if the rest of the setup is right.
- **Show the mole-fraction/partial-pressure reasoning explicitly.** A bare final partial-pressure number without the mole-fraction calculation shown does not receive full credit.
- **KMT explanations must name the specific assumption invoked**, not just restate the gas law in different words.
- **Graham's law answers must include the square root.** Omitting it (using a direct mass ratio) is treated as a conceptual error, not a rounding issue.
