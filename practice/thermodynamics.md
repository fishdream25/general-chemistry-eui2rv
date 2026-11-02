{{nyml
kind: document
format: 1
title: Chapter 17 Practice: Entropy, Free Energy, and Equilibrium
}}

# Chapter 17 Practice: Entropy, Free Energy, and Equilibrium

*Auto-generated from the assessment guide (`assessment-support/thermodynamics.md`), grouped by objective. 27 questions spanning multiple-choice, short-answer, and workout formats.*

:::: tabs
::: tab Q 1
{{sp[info] Objective 17.1a}} · *short answer* Predict the sign of $\Delta S$ for $\ce{Br2(l) -> Br2(g)}$, and explain why.
:::
::: tab Answer
**Positive.** Going from liquid to gas dramatically increases the number of accessible microstates (gas molecules can occupy far more positions and momenta than a liquid's), so entropy increases.
:::
::::

:::: tabs
::: tab Q 2
{{sp[info] Objective 17.1a}} · *short answer* Arrange $\ce{Al(s)}$, $\ce{H2O(l)}$, and $\ce{HF(g)}$ in order of increasing standard molar entropy at 25 °C.
:::
::: tab Answer
$$\ce{Al(s)} < \ce{H2O(l)} < \ce{HF(g)}$$

This follows the general trend gas ≫ liquid > solid.
:::
::::

:::: tabs
::: tab Q 3
{{sp[info] Objective 17.1a}} · *multiple-choice* Which of these correctly balanced combustion reactions would you expect to have $\Delta S^\circ$ closest to zero?

A. $\ce{CH4(g) + 2O2(g) -> CO2(g) + 2H2O(g)}$\
B. $\ce{C3H8(g) + 5O2(g) -> 3CO2(g) + 4H2O(g)}$\
C. $\ce{2C2H2(g) + 5O2(g) -> 4CO2(g) + 2H2O(g)}$
:::
::: tab Answer
**A.** Reactant and product gas moles are equal (3 mol gas on each side, $\Delta n = 0$), so $\Delta S^\circ$ should be small in magnitude. (B has $\Delta n$ = +1: 6 mol gas → 7 mol gas, a modest positive $\Delta S^\circ$. C has $\Delta n = -1$: 7 mol gas → 6 mol gas, a modest negative $\Delta S^\circ$. Both B and C involve a net change in gas moles, so their $|\Delta S^\circ|$ should exceed A's.)
:::
::::

:::: tabs
::: tab Q 4
{{sp[info] Objective 17.1b}} · *workout* Calculate $\Delta S^\circ_\text{rxn}$ for $\ce{S(s) + O2(g) -> SO2(g)}$. ($S^\circ$: $\ce{S(s)}=31.88$, $\ce{O2(g)}=205.0$, $\ce{SO2(g)}=248.5$ J/K·mol)
:::
::: tab Answer
$$\Delta S^\circ_\text{rxn}=248.5-(31.88+205.0)=248.5-236.88=11.6\ \text{J/K·mol}$$

Small in magnitude, as expected — there is no net change in gas moles (1 mol gas in, 1 mol gas out).
:::
::::

:::: tabs
::: tab Q 5
{{sp[info] Objective 17.1b}} · *workout* Calculate $\Delta S^\circ_\text{rxn}$ for $\ce{N2(g) + 3H2(g) -> 2NH3(g)}$. ($S^\circ$: $\ce{N2}=191.6$, $\ce{H2}=130.7$, $\ce{NH3}=192.8$ J/K·mol)
:::
::: tab Answer
$$\Delta S^\circ_\text{rxn}=2(192.8)-[191.6+3(130.7)]=385.6-(191.6+392.1)=-198.1\ \text{J/K·mol}$$

Strongly negative, as expected: 4 mol of gas become 2 mol of gas.
:::
::::

:::: tabs
::: tab Q 6
{{sp[info] Objective 17.1b}} · *workout* Calculate $\Delta S^\circ_\text{rxn}$ for $\ce{N2(g) + 3H2(g) -> 2NH3(g)}$. ($S^\circ$: $\ce{N2} = 191.6$, $\ce{H2} = 130.7$, $\ce{NH3} = 192.8\ \text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$.) Predict the sign first.
:::
::: tab Answer
**Predict first.** Four moles of gas become two, so gas particles are lost and $\Delta S^\circ$ should be **negative and substantial**.

**Now compute**, remembering that the coefficients multiply each $S^\circ$:

$$\Delta S^\circ_\text{rxn} = 2S^\circ(\ce{NH3}) - [S^\circ(\ce{N2}) + 3S^\circ(\ce{H2})]$$
$$= 2(192.8) - [191.6 + 3(130.7)] = 385.6 - [191.6 + 392.1] = 385.6 - 583.7 = -198.1\ \text{J K}^{-1}\text{mol}^{-1}$$

**Negative and substantial, as predicted** ✓

{{sp[warning] Elements are not zero here}} $\ce{N2}$ contributes 191.6 and $\ce{H2}$ contributes 130.7, even though both are elements in their standard states. That convention belongs to $\Delta H^\circ_f$ and $\Delta G^\circ_f$, never to $S^\circ$ — absolute entropies are measured from the third-law zero, and only a perfect crystal at 0 K sits there.

**Looking ahead:** this reaction has $\Delta H^\circ = -92.2$ kJ/mol as well, so both quantities are negative — Figure 17.1's bottom-left cell, spontaneous under standard conditions only below $T = 92{,}200/198.1 = 465$ K. The Haber process runs near 700 K for kinetic reasons, well above that ceiling, which is exactly why its single-pass yield is poor.
:::
::::

:::: tabs
::: tab Q 7
{{sp[info] Objective 17.2a}} · *short answer* Water freezing at −5 °C is spontaneous, yet the system's entropy decreases (liquid → solid). Is this consistent with the second law? Explain.
:::
::: tab Answer
**Yes.** The second law requires only that the *total* (universe) entropy increases, not the system's entropy alone. Freezing releases heat to the surroundings, increasing the surroundings' entropy by more than the system's entropy decreases — the net change for the universe is still positive.
:::
::::

:::: tabs
::: tab Q 8
{{sp[info] Objective 17.2a}} · *multiple-choice* Which statement correctly expresses the second law of thermodynamics?

(A) Energy cannot be created or destroyed\
(B) The entropy of any system always increases\
\(C) The total entropy of a system plus its surroundings increases in any spontaneous process\
(D) The entropy of a perfect crystal at 0 K is zero
:::
::: tab Answer
**\(C).** The second law constrains the **universe** — system plus surroundings taken together — not any chosen part of it.

**Why the others fail:**
- **(A)** is the **first** law, conservation of energy. It says nothing about direction, which is precisely the gap the second law fills: energy is conserved whether a bouncing ball comes to rest or a resting ball starts bouncing on its own, so conservation alone cannot explain why one happens and the other does not.
- **(B)** is the common misstatement, and it is false. A system's entropy decreases every time water freezes, a crystal grows, or an organism builds tissue. Each is spontaneous because the surroundings gain more than the system loses.
- **(D)** is the **third** law, which supplies the absolute zero of entropy and lets $S^\circ$ be tabulated.

**The distinction that matters most in practice:** because the second law refers to the universe, applying it directly means tracking the surroundings. Gibbs free energy exists to avoid that — at constant temperature and pressure, $\Delta G < 0$ is the second law rewritten in terms of the system alone.
:::
::::

:::: tabs
::: tab Q 9
{{sp[info] Objective 17.2a}} · *short answer* A refrigerator makes its interior colder, decreasing the entropy of the food inside. Explain why this does not violate the second law, and identify where the compensating entropy increase occurs.
:::
::: tab Answer
**The refrigerator's interior is not an isolated system**, and the second law constrains only the total.

**What the machine actually does.** It moves heat from a cold interior to a warm room — the opposite of the direction heat flows on its own. That transfer alone *would* decrease the universe's entropy, because removing heat $q$ from a cold reservoir costs $q/T_\text{cold}$ while delivering it to a warm one buys only $q/T_\text{warm}$, and $T_\text{cold} < T_\text{warm}$ makes the loss larger than the gain.

**Which is exactly why the machine needs a power supply.** The compressor does work on the refrigerant, and essentially all of that electrical energy is ultimately dumped into the room as additional heat — through the coils on the back. So the room receives not just the heat removed from the food but the compressor's work as well:

$$\Delta S_\text{univ} = \underbrace{-\frac{q}{T_\text{cold}}}_{\text{food}} + \underbrace{\frac{q + w}{T_\text{warm}}}_{\text{room}} > 0$$

The extra $w$, which must be at least $q(T_\text{warm}/T_\text{cold} - 1)$, is what makes the sum positive. **A refrigerator does not defeat the second law; it pays it, in electricity.**

**The observable proof:** a refrigerator with its door open warms a sealed kitchen rather than cooling it, because everything it removes from the interior plus everything the compressor consumes ends up in the same room.

**The general pattern, again:** local order is always purchased with a larger disorder elsewhere. Same structure as water freezing, and as the objection about life.
:::
::::

:::: tabs
::: tab Q 10
{{sp[info] Objective 17.2b}} · *short answer* Diamond has $S^\circ=2.4$ J/K·mol at 25 °C, much smaller than $\ce{O2(g)}$'s $S^\circ=205.2$ J/K·mol. Explain why, and explain how the third law makes this an *absolute* value.
:::
::: tab Answer
Diamond's carbon atoms are locked into a rigid, highly ordered crystal lattice with very few accessible microstates, while $\ce{O2}$ molecules (gas) can occupy vastly more positions and momenta — far more microstates, far higher entropy. The third law (a perfect crystal at 0 K has exactly zero entropy) provides the zero-point reference that lets $S^\circ$ be tabulated as an absolute value, unlike enthalpy, which is only ever reported as a *change*.
:::
::::

:::: tabs
::: tab Q 11
{{sp[info] Objective 17.2b}} · *short answer* Explain why standard entropies $S^\circ$ are always positive for substances at 298 K, while standard enthalpies of formation $\Delta H^\circ_f$ can be positive, negative, or zero.
:::
::: tab Answer
**The difference is that entropy has an absolute zero and enthalpy does not.**

**Entropy: measured from a real baseline.** The third law fixes $S = 0$ for a perfect crystal at 0 K, where there is exactly one arrangement and $S = k\ln 1 = 0$. Warming anything above 0 K adds accessible microstates, so $S$ rises and can only rise. Every $S^\circ$ at 298 K is therefore a genuinely positive number measured up from a physical zero — including for elements, which is why $S^\circ(\ce{O2}) = 205.2$ J/(mol·K) rather than 0.

**Enthalpy: measured from an arbitrary baseline.** No experiment returns an absolute enthalpy; only *changes* are measurable. Chemistry therefore adopts a convention — elements in their standard states are assigned $\Delta H^\circ_f = 0$ — and every tabulated value is a difference relative to that choice. A compound more stable than its elements gets a negative value, a less stable one a positive value, and the elements themselves get zero **by definition, not by measurement**.

**The consequence for calculations:** in $\Delta H^\circ_\text{rxn}$ the element terms drop out; in $\Delta S^\circ_\text{rxn}$ they must be included. Forgetting this is one of the two commonest errors in the chapter — the other being the J/kJ mismatch between $S^\circ$ and $\Delta H^\circ$.
:::
::::

:::: tabs
::: tab Q 12
{{sp[info] Objective 17.2b}} · *multiple-choice* Which substance would you expect to have a non-zero entropy at 0 K?

(A) A perfect crystal of copper\
(B) A perfect crystal of sodium chloride\
\(C) A glass (amorphous silica)\
(D) Solid neon, perfectly crystallized
:::
::: tab Answer
**\(C) A glass.**

The third law states that a **perfect crystalline** substance has $S = 0$ at 0 K, because there is exactly one way to arrange it and $S = k\ln 1 = 0$. The qualifier "perfect crystalline" is doing real work.

**Why glass is the exception.** Amorphous silica is a liquid structure frozen in place. As it cools it becomes too viscous to find the single lowest-energy arrangement, so it locks into one of an enormous number of nearly equivalent disordered configurations. With $W \gg 1$ even at 0 K, $S = k\ln W > 0$. This leftover is called **residual entropy**.

**Why (A), (B) and (D) all give zero:** each is specified as a perfect crystal, so each has a single arrangement at 0 K regardless of what it is made of. The third law makes no distinction between elements and compounds, or between metals and ionic solids — only between ordered and disordered.

**A near-miss worth knowing.** Carbon monoxide *does* crystallize, yet retains about 4.6 $\text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$ at 0 K, because its two ends are nearly indistinguishable and molecules freeze in pointing either way. It is a *crystal* but not a *perfect* one — which is why the third law's wording is so careful.
:::
::::

:::: tabs
::: tab Q 13
{{sp[info] Objective 17.3a}} · *multiple-choice* For a reaction, $\Delta H^\circ=-20.2$ kJ/mol and $\Delta S^\circ=4.3$ J/K·mol. Which statement is true?

A. The reaction is only spontaneous at low temperature.\
B. The reaction is spontaneous only at high temperature.\
C. The reaction is spontaneous at all temperatures.\
D. $\Delta G^\circ$ becomes larger (more positive) as temperature increases.
:::
::: tab Answer
**C.** $\Delta G^\circ=\Delta H^\circ-T\Delta S^\circ=(-20.2\ \text{kJ/mol})-T(0.0043\ \text{kJ/K·mol})$. Since $\Delta H^\circ<0$ and $\Delta S^\circ>0$, every term is negative for any positive $T$ — $\Delta G^\circ<0$ at all temperatures. (D is also false: increasing $T$ makes $\Delta G^\circ$ *more* negative here, not larger.)
:::
::::

:::: tabs
::: tab Q 14
{{sp[info] Objective 17.3a}} · *short answer* A reaction has $\Delta H^\circ>0$ and $\Delta S^\circ<0$. Is it ever spontaneous? Explain.
:::
::: tab Answer
**Never**, at any temperature. $\Delta G^\circ=\Delta H^\circ-T\Delta S^\circ$: since $\Delta H^\circ>0$ and $-T\Delta S^\circ>0$ (because $\Delta S^\circ<0$), both terms are positive for every positive $T$, so $\Delta G^\circ>0$ always — this reaction is nonspontaneous in the forward direction under standard conditions at all temperatures.
:::
::::

:::: tabs
::: tab Q 15
{{sp[info] Objective 17.3a}} · *workout* For the vaporization of ethanol, $\Delta H^\circ_\text{vap} = 38.6$ kJ/mol and $\Delta S^\circ_\text{vap} = 110.0\ \text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$. (a) Calculate $\Delta G$ at 298 K and at 373 K. (b) Interpret each. \(c) What is ethanol's normal boiling point according to these numbers?
:::
::: tab Answer
**(a)** Convert $\Delta S^\circ$ to $\text{kJ}\,\text{K}^{-1}\,\text{mol}^{-1}$ (0.1100):

$$T = 298: \quad \Delta G = 38.6 - (298)(0.1100) = 38.6 - 32.8 = +5.8\ \text{kJ/mol}$$
$$T = 373: \quad \Delta G = 38.6 - (373)(0.1100) = 38.6 - 41.0 = -2.4\ \text{kJ/mol}$$

**(b)** At 298 K, $\Delta G > 0$: ethanol does **not** spontaneously become vapor at 1 atm — it does not boil (though it still evaporates into open air, where its vapor pressure is below 1 atm), which matches ordinary experience. At 373 K, $\Delta G < 0$: vaporization is now spontaneous at 1 atm, so ethanol would boil away.

**\(c)** Set $\Delta G = 0$:

$$T_b = \frac{\Delta H^\circ_\text{vap}}{\Delta S^\circ_\text{vap}} = \frac{38{,}600}{110.0} = 351\ \text{K} = 78\ \text{°C}$$

**The accepted boiling point of ethanol is 78.4 °C** — an excellent match from two tabulated numbers and no experiment.

**Note the pattern this belongs to.** Vaporization always has $\Delta H > 0$ and $\Delta S > 0$, which is Figure 17.1's top-right cell: nonspontaneous cold, spontaneous hot, with the crossover at $\Delta H/\Delta S$. **For a phase transition that crossover has a name — it is the transition temperature itself.**
:::
::::

:::: tabs
::: tab Q 16
{{sp[info] Objective 17.3b}} · *workout* Given $\ce{ZnS(s)->Zn(s)+S(s)}$, $\Delta G^\circ_1=201.3$ kJ/mol, and $\ce{S(s)+H2(g)->H2S(g)}$, $\Delta G^\circ_2=-33.4$ kJ/mol, find $\Delta G^\circ_3$ for $\ce{ZnS(s)+H2(g)->Zn(s)+H2S(g)}$.
:::
::: tab Answer
Reaction 3 = reaction 1 + reaction 2 (S(s) cancels):

$$\Delta G^\circ_3=201.3+(-33.4)=167.9\ \text{kJ/mol}$$
:::
::::

:::: tabs
::: tab Q 17
{{sp[info] Objective 17.3b}} · *workout* Calculate $\Delta G^\circ_\text{rxn}$ at 298 K for $\ce{CH4(g) + 2O2(g) -> CO2(g) + 2H2O(l)}$. ($\Delta G^\circ_f$ in kJ/mol: $\ce{CH4} = -50.5$, $\ce{O2} = 0$, $\ce{CO2} = -394.4$, $\ce{H2O(l)} = -237.1$.)
:::
::: tab Answer
Products minus reactants, each multiplied by its coefficient:

$$\Delta G^\circ_\text{rxn} = [\Delta G^\circ_f(\ce{CO2}) + 2\Delta G^\circ_f(\ce{H2O})] - [\Delta G^\circ_f(\ce{CH4}) + 2\Delta G^\circ_f(\ce{O2})]$$

$$= [-394.4 + 2(-237.1)] - [-50.5 + 2(0)]$$
$$= [-394.4 - 474.2] - [-50.5] = -868.6 + 50.5 = -818.1\ \text{kJ/mol}$$

**Strongly negative — methane combustion is overwhelmingly spontaneous**, as it should be.

**Two checks worth making.** $\ce{O2}$ is an element in its standard state, so its $\Delta G^\circ_f$ is zero by definition and contributes nothing — unlike in an entropy calculation. And the *sign* of the $\ce{CH4}$ term flips when it moves to the reactant side: subtracting $-50.5$ adds 50.5.

**What this does and does not tell you.** $\Delta G^\circ = -818$ kJ/mol corresponds to $K = e^{818{,}000/2478} \approx 10^{143}$ — for all practical purposes the reaction goes to completion. And yet methane sits indefinitely in a pipeline in contact with air. **Thermodynamics sets the destination; the activation barrier of Chapter 13 sets whether you ever arrive.**
:::
::::

:::: tabs
::: tab Q 18
{{sp[info] Objective 17.3b}} · *workout* Calculate $\Delta G^\circ_\text{rxn}$ at 298 K for $\ce{2NO(g) + O2(g) -> 2NO2(g)}$ two different ways: (a) from $\Delta G^\circ_f$ values ($\ce{NO} = 86.6$, $\ce{O2} = 0$, $\ce{NO2} = 51.3$ kJ/mol); (b) from $\Delta H^\circ = -114.1$ kJ/mol and $\Delta S^\circ = -146.5\ \text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$. Do they agree?
:::
::: tab Answer
**(a) From free energies of formation:**

$$\Delta G^\circ_\text{rxn} = 2(51.3) - [2(86.6) + 0] = 102.6 - 173.2 = -70.6\ \text{kJ/mol}$$

**(b) From enthalpy and entropy**, converting $\Delta S^\circ$ to $\text{kJ}\,\text{K}^{-1}\,\text{mol}^{-1}$:

$$\Delta G^\circ = \Delta H^\circ - T\Delta S^\circ = -114.1 - (298)(-0.1465) = -114.1 + 43.7 = -70.4\ \text{kJ/mol}$$

**They agree to within 0.2 kJ/mol** — the difference is rounding in the tabulated inputs, not a real discrepancy.

**Why they must agree.** $G$ is defined as $H - TS$, so $\Delta G^\circ_f$ values are themselves derived from $\Delta H^\circ_f$ and $S^\circ$ data. The two routes are the same calculation performed in a different order, and agreement is a consistency check on your arithmetic rather than new information.

**When to prefer each.** Route (a) is faster and is the only option when you have only a $\Delta G^\circ_f$ table. Route (b) is essential whenever the temperature is **not** 298 K, because tabulated $\Delta G^\circ_f$ values are quoted only at 298 K while $\Delta H^\circ$ and $\Delta S^\circ$ can be treated as roughly constant and used at any temperature.

**Reading the result:** exothermic and entropy-decreasing — Figure 17.1's bottom-left cell, spontaneous below $T = 114{,}100/146.5 = 779$ K.
:::
::::

:::: tabs
::: tab Q 19
{{sp[info] Objective 17.3c}} · *workout* Benzene melts at 5.5 °C with $\Delta H^\circ_\text{fus}=10.9$ kJ/mol. Calculate its molar entropy of fusion.
:::
::: tab Answer
At the melting point, solid and liquid are in equilibrium ($\Delta G=0$), so $\Delta S=\Delta H/T$:

$$T=5.5+273.15=278.65\ \text{K}$$

$$\Delta S^\circ_\text{fus}=\frac{10{,}900\ \text{J/mol}}{278.65\ \text{K}}=39.1\ \text{J/K·mol}$$
:::
::::

:::: tabs
::: tab Q 20
{{sp[info] Objective 17.3c}} · *workout* Using $\Delta H^\circ_\text{vap}=28.8$ kJ/mol and $\Delta S^\circ_\text{vap}=92.4$ J/K·mol for $\ce{CH2Cl2}$, calculate its normal boiling point.
:::
::: tab Answer
At the boiling point, liquid and gas are in equilibrium: $\Delta G^\circ_\text{vap}=\Delta H^\circ_\text{vap}-T\Delta S^\circ_\text{vap}=0$

$$T=\frac{\Delta H^\circ_\text{vap}}{\Delta S^\circ_\text{vap}}=\frac{28{,}800\ \text{J/mol}}{92.4\ \text{J/K·mol}}=312\ \text{K}=39\ °\text{C}$$
:::
::::

:::: tabs
::: tab Q 21
{{sp[info] Objective 17.3c}} · *workout* Mercury(II) oxide decomposes: $\ce{2HgO(s) -> 2Hg(l) + O2(g)}$, with $\Delta H^\circ = +181.6$ kJ/mol and $\Delta S^\circ = +216.6\ \text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$. (a) Is it spontaneous at 298 K? (b) Above what temperature does it become spontaneous? \(c) Which quadrant of Figure 17.1 is this?
:::
::: tab Answer
**(a)** Compute $\Delta G^\circ$ at 298 K, converting $\Delta S^\circ$ to kJ:

$$\Delta G^\circ = 181.6 - (298)(0.2166) = 181.6 - 64.5 = +117.1\ \text{kJ/mol}$$

**Positive — not spontaneous at room temperature.** Mercury(II) oxide is a stable red solid on the shelf.

**(b)** Set $\Delta G^\circ = 0$:

$$T = \frac{\Delta H^\circ}{\Delta S^\circ} = \frac{181{,}600}{216.6} = 838\ \text{K} = 565\ \text{°C}$$

Above about 565 °C the decomposition becomes spontaneous.

**\(c) Top-right: $\Delta H > 0$, $\Delta S > 0$** — the two terms disagree, and heating settles the argument in favor of entropy.

**Why the entropy term is large here:** a solid produces a liquid *and* a gas. Generating a mole of gas from a condensed phase is worth roughly 150–200 $\text{J}\,\text{K}^{-1}\,\text{mol}^{-1}$ on its own, which is most of the 216.6.

**A historical footnote.** This is the reaction Priestley and Lavoisier used to isolate oxygen in the 1770s, by heating mercury(II) oxide in a sealed vessel. The calculation above says why heat was required — and roughly how much.
:::
::::

:::: tabs
::: tab Q 22
{{sp[info] Objective 17.3d}} · *workout* For $\ce{PCl5(g) <=> PCl3(g) + Cl2(g)}$ at 25 °C, $\Delta G^\circ_f$: $\ce{Cl2}=0$, $\ce{PCl3}=-286$, $\ce{PCl5}=-325$ kJ/mol. Calculate $\Delta G^\circ_\text{rxn}$ and $K_p$.
:::
::: tab Answer
$$\Delta G^\circ_\text{rxn}=(-286+0)-(-325)=39\ \text{kJ/mol}$$

Since $\Delta G^\circ>0$, predict $K_p<1$ before calculating:

$$K_p=e^{-39{,}000/(8.314\times298)}=1.47\times10^{-7}$$

Confirmed: $K_p\ll1$, consistent with the positive $\Delta G^\circ$.
:::
::::

:::: tabs
::: tab Q 23
{{sp[info] Objective 17.3d}} · *workout* For $\ce{H2(g) + I2(g) <=> 2HI(g)}$, $K_p = 54$ at 700 K. (a) Calculate $\Delta G^\circ$ at 700 K. (b) Would you expect $\Delta G^\circ$ to be large or small in magnitude, before calculating?
:::
::: tab Answer
**(b) first, since the prediction is the point.** $K = 54$ is greater than 1 but not enormously so — products are favored, yet a measurable amount of reactant remains at equilibrium. $\Delta G^\circ$ should therefore be **negative but modest**, a few tens of kJ/mol at most.

**(a)** Apply $\Delta G^\circ = -RT\ln K$, with $T = 700$ K:

$$\Delta G^\circ = -(8.314)(700)\ln(54) = -(5820)(3.989) = -2.32\times10^{4}\ \text{J/mol} = -23.2\ \text{kJ/mol}$$

**Negative and modest, as predicted** ✓

**Calibrating your intuition for this relationship.** At 700 K, $RT = 5.82$ kJ/mol, so each factor of ten in $K$ corresponds to $RT\ln 10 = 13.4$ kJ/mol. Chemical $\Delta G^\circ$ values of $\pm 100$ kJ/mol are ordinary, and they correspond to $K$ values around $10^{\pm 7}$ — which is why so many reactions appear to go to completion or not to go at all. **A $K$ near 1 requires $\Delta G^\circ$ to be near zero, and that is the unusual case, not the typical one.**

{{sp[warning] Use the right T}} $\Delta G^\circ = -RT\ln K$ needs the temperature at which $K$ was measured. Using 298 K here would give $-9.9$ kJ/mol, which is the standard free energy of a reaction that was never performed at 298 K.
:::
::::

:::: tabs
::: tab Q 24
{{sp[info] Objective 17.3d}} · *short answer* Reaction A has $\Delta G^\circ = -5.0$ kJ/mol and reaction B has $\Delta G^\circ = -50.0$ kJ/mol, both at 298 K. Calculate $K$ for each and comment on what the tenfold difference in $\Delta G^\circ$ does to $K$.
:::
::: tab Answer
Apply $K = e^{-\Delta G^\circ/RT}$ with $RT = (8.314)(298) = 2478$ J/mol:

**Reaction A:**
$$K = e^{5000/2478} = e^{2.018} = 7.5$$

**Reaction B:**
$$K = e^{50{,}000/2478} = e^{20.18} = 5.8\times10^{8}$$

**A tenfold change in $\Delta G^\circ$ produced a change of nearly eight orders of magnitude in $K$** — because $\Delta G^\circ$ sits in an **exponent**. Linear intuition fails badly here, and this is the single most important thing to internalize about the relationship.

**A useful conversion factor.** At 298 K, $RT\ln 10 = 5.7$ kJ/mol, so **every 5.7 kJ/mol of $\Delta G^\circ$ multiplies or divides $K$ by ten.** Reaction A's $-5.0$ kJ/mol is not quite one factor of ten; reaction B's $-50.0$ is nearly nine of them.

**What each means chemically.** $K = 7.5$ is a genuinely reversible reaction — appreciable amounts of both reactant and product at equilibrium, and Le Chatelier's levers (Chapter 14) can shift it usefully. $K = 5.8\times10^{8}$ is effectively complete; no practical stress will pull it back.

**And the same leverage in reverse:** a modest *positive* $\Delta G^\circ$ of $+50$ kJ/mol gives $K = 1.7\times10^{-9}$, which is why so many reactions appear simply not to happen.
:::
::::

:::: tabs
::: tab Q 25
{{sp[info] Objective 17.3e}} · *workout* For the reaction $\ce{PCl5(g) <=> PCl3(g) + Cl2(g)}$ at 298 K ($\Delta G^\circ = +39.0$ kJ/mol, $K_p = 1.47\times10^{-7}$), the pressures are $P_{\ce{Cl2}}=0.363$, $P_{\ce{PCl3}}=0.215$, $P_{\ce{PCl5}}=0.00300$ atm. Calculate $Q$ and $\Delta G$, and predict the reaction direction.
:::
::: tab Answer
$$Q=\frac{P_{\ce{PCl3}}P_{\ce{Cl2}}}{P_{\ce{PCl5}}}=\frac{(0.215)(0.363)}{0.00300}=26.0$$

$$\Delta G=\Delta G^\circ+RT\ln Q=39{,}000+(8.314)(298)\ln(26.0)=39{,}000+8{,}070=47{,}000\ \text{J/mol}=47\ \text{kJ/mol}$$

Since $\Delta G>0$, the reaction proceeds in **reverse** (toward $\ce{PCl5}$) — consistent with $Q=26.0 \gg K_p=1.47\times10^{-7}$.
:::
::::

:::: tabs
::: tab Q 26
{{sp[info] Objective 17.3e}} · *short answer* A calculated $\Delta G$ for a reaction under specific conditions is +18 kJ/mol. Which direction does the reaction proceed, and is this the same as saying $Q<K$ or $Q>K$?
:::
::: tab Answer
**Reverse** (right to left) — a positive $\Delta G$ under the given conditions means the forward reaction is nonspontaneous and the reverse direction is spontaneous. This corresponds to $Q>K$ (too much product relative to equilibrium), exactly mirroring Chapter 14's Q-vs-K rule.
:::
::::

:::: tabs
::: tab Q 27
{{sp[info] Objective 17.3e}} · *short answer* A reaction has $\Delta G^\circ = -15.0$ kJ/mol at 298 K. Under a particular set of non-standard conditions $Q = 8.0\times10^{4}$. (a) Calculate $\Delta G$. (b) Which direction does the reaction run? \(c) Reconcile the two signs.
:::
::: tab Answer
**(a)**

$$\Delta G = \Delta G^\circ + RT\ln Q = -15{,}000 + (2478)\ln(8.0\times10^{4})$$
$$= -15{,}000 + (2478)(11.29) = -15{,}000 + 27{,}980 = +13{,}000\ \text{J/mol} = +13.0\ \text{kJ/mol}$$

**(b) $\Delta G > 0$, so the forward reaction is nonspontaneous** — the reaction runs **in reverse** under these conditions.

**\(c) The two signs describe different questions, and both are correct.**

$\Delta G^\circ = -15.0$ kJ/mol says that *starting from standard conditions* — everything at 1 M or 1 atm, so $Q = 1$ — the reaction would run forward. It also fixes $K$:

$$K = e^{15{,}000/2478} = e^{6.05} = 4.3\times10^{2}$$

$\Delta G = +13.0$ kJ/mol says that *from this particular mixture* it runs backward. And the reason is visible in the comparison: $Q = 8.0\times10^{4}$ against $K = 4.3\times10^{2}$, so $Q$ is nearly 200 times larger than $K$. The vessel is far too rich in product, and the system must consume product to bring $Q$ down to $K$.

**The general statement.** $\Delta G^\circ$ is a property of the *reaction*; $\Delta G$ is a property of the *mixture*. A favorable $\Delta G^\circ$ guarantees nothing about a mixture that has already overshot equilibrium — which is Chapter 14's $Q$-versus-$K$ rule, restated in energy.
:::
::::
