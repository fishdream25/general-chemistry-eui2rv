{{nyml
kind: document
format: 1
title: Chapter 1: Introduction to Chemistry
}}

# Chapter 1: Introduction to Chemistry

:::info
**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 1 (CC BY 4.0)
**Audience:** introductory undergraduate general chemistry, first semester
**Package license:** CC BY 4.0
**Note:** the first chapter of the course — no prior chemistry background assumed; facts checked for accuracy against OpenStax *Chemistry 2e* and Wikipedia (used for reference only — no text or figures adapted from either).
:::

:::success
**Chapter Learning Objectives**
- Classify matter (substance vs. mixture, element vs. compound) and distinguish physical from chemical change and extensive from intensive properties.
- Use SI units and prefixes, and calculate density and temperature conversions.
- Use scientific notation and apply significant-figure rules to measurements and calculations.
- Solve unit-conversion problems using dimensional analysis.
:::

## Chapter Logic

This chapter builds no chemistry yet — it builds the *toolkit* every later chapter will assume you already have. Nothing here is difficult in isolation. ==What makes it matter is that all of it gets used, silently and constantly, from Chapter 3 onward.==

{{mermaid
graph TD
  A["Classify matter:<br/>substance, mixture, element, compound"] --> B["Measurement:<br/>SI units, mass, volume, density, temperature"]
  B --> C["Numbers:<br/>scientific notation and significant figures"]
  C --> D["Dimensional analysis:<br/>unit-factor-label method"]
}}

**Visual description:** A top-down flowchart. Classifying matter gives the vocabulary to describe what chemistry studies. Measurement introduces the physical quantities chemists report. Numbers gives the rules for expressing those quantities honestly (scientific notation, significant figures). Dimensional analysis combines units and numbers into the single problem-solving method reused in every later chapter.

## 1.1 General Concepts in Chemistry{{attrs[#blk-ch01sec01]}}

:::success
**Learning Objectives**
- Define chemistry and matter.
- {{sp[info] Objective 1.1a}} Distinguish a substance from a mixture, and a homogeneous from a heterogeneous mixture.
- {{sp[info] Objective 1.1a}} Distinguish an element from a compound.
- {{sp[info] Objective 1.1b}} Distinguish a physical change from a chemical change.
- {{sp[info] Objective 1.1b}} Distinguish an extensive property from an intensive property.
:::

**Chemistry** is the study of matter and the changes it undergoes. **Matter** is anything that occupies space and has mass — this book, the air around you, and the water in a glass are all matter.

Chemistry begins by sorting matter into categories, because the category a sample belongs to tells you what you can and cannot do with it. The whole classification reduces to **two yes/no questions**.

Figure 1.1 turns the two questions below into a single decision tree; work down it and every classification question answers itself.

### Question 1: can it be separated by physical means?

A **substance** (often called a *pure substance*) has a definite, fixed composition and its own distinct properties. Pure water is always the same stuff, with the same freezing point, wherever you find it.

A **mixture** combines two or more substances that each keep their own identity, in proportions that can vary. Salt water is a mixture: you can make it saltier or less salty, and it is still salt water.

> "Physical means" covers anything that separates components *without changing what they are* — filtering, evaporating, letting layers settle, picking pieces out with tweezers.

Mixtures come in two kinds:

- A **homogeneous** mixture has the same composition throughout, so you cannot see the separate parts (salt water, air, brass).
- A **heterogeneous** mixture does not, so you can (sand in water, oil and vinegar, trail mix).

### Question 2: can it be broken down chemically?

If a sample *is* a pure substance, the second question splits it further:

- An **element** cannot be broken down into simpler substances by chemical means — it is one kind of atom (gold, copper, oxygen gas).
- A **compound** is two or more elements chemically combined **in a fixed ratio**. Water is always 2 H : 1 O by atom count — never a variable blend of hydrogen and oxygen. That fixed ratio is exactly what separates a compound from a mixture.

![Decision tree for classifying matter into element, compound, or a homogeneous or heterogeneous mixture](../assets/matter_classification_tree.svg =700x)
*Figure 1.1 — Every "classify this substance" question is answered by working down this tree. Start at the top, answer the two questions in order, and you land on exactly one of the four categories. The examples under each box are worth memorising as anchors — when a new substance is unfamiliar, ask which of these it most resembles.*

{{sp[warning] Watch out}} The most common beginner error is calling a **homogeneous mixture** a compound, because both look uniform. Uniform appearance is not the test — **fixed ratio** is. Salt water looks as uniform as pure water, but you can dissolve more salt in it; you cannot make water "more oxygen-y." If the proportions can be changed, it is a mixture.

:::: tabs
::: tab Problem
Classify each as a pure substance or a mixture, and if a mixture, homogeneous or heterogeneous: (a) diamond; (b) milk; \(c) air; (d) Italian salad dressing (oil and vinegar, unshaken).
:::
::: tab Solution
(a) Diamond is a pure substance (element: carbon).
(b) Milk is a homogeneous mixture — it looks uniform to the eye, though it is technically a colloid.
\(c) Air is a homogeneous mixture of gases (mostly $\ce{N2}$ and $\ce{O2}$).
(d) Unshaken salad dressing is a heterogeneous mixture — the oil and vinegar layers are visibly distinct.
:::
::::

:::: tabs
::: tab Problem
Now run the tree deliberately, one question at a time, for **brass** (a solid blend of copper and zinc, uniform to the eye) and for **carbon dioxide**, $\ce{CO2}$.
:::
::: tab Solution
**Brass.** *Question 1 — separable by physical means?* Yes: brass can be made with more or less zinc, and the metals can be separated without chemical reaction. So it is a **mixture**. *Question 2 — uniform throughout?* Yes, you cannot see separate copper and zinc regions. → **homogeneous mixture**. (Uniform metal mixtures like this are called alloys.)

**Carbon dioxide.** *Question 1 — separable by physical means?* No. Cooling or filtering $\ce{CO2}$ never yields carbon and oxygen; only a chemical reaction does. So it is a **pure substance**. *Question 2 — broken down chemically?* Yes, into carbon and oxygen, and always in the same 1 C : 2 O ratio. → **compound**.

Notice that the *same two questions* handled both, even though one is a metal and one is a gas. That is the point of the tree.
:::
::::

### States of matter

Matter also comes in three familiar physical forms, shown in Figure 1.2, and the difference between them is how the particles are arranged and how freely they move rather than what the particles are.

Independently of that classification, any sample can exist in different **physical states**. The difference between them is how the particles are arranged, not what the particles are.

![Particle arrangement in solids, liquids, and gases](../assets/states_of_matter.svg =650x)
*Figure 1.2 — The three states of matter, distinguished by how tightly and regularly their particles pack: solids hold a fixed, ordered arrangement; liquids stay close together but slide past one another; gases spread far apart and move independently. Water is the same compound as ice and as steam — only the arrangement changes.*

### Changes and properties

==Whether a change is physical or chemical, and whether a property is extensive or intensive, are two separate questions students often conflate — keep them as two distinct yes/no checks.==

- A **physical change** does not alter a substance's composition or identity (melting ice, dissolving sugar, cutting paper).
- A **chemical change** produces a new substance with a different composition (rusting iron, burning wood, digesting food).
- An **extensive property** depends on how much matter is present (mass, length, volume, total energy).
- An **intensive property** does not depend on the amount present (density, temperature, color, melting point) — this is what makes intensive properties useful for *identifying* a substance, regardless of sample size.

How do you tell a chemical change actually happened? Look for **evidence that a new substance exists**: a color change that does not reverse, a gas bubbling out, a solid appearing from two clear liquids, or heat and light released. Any one of these is a signal — though none is absolute proof on its own, since some physical changes (like dissolving) also release heat.

:::: tabs
::: tab Problem
For each item, state whether the change described is physical or chemical, or whether the property described is extensive or intensive: (a) a 50 g and a 5 g sample of copper have different masses; (b) a silver spoon left in air slowly tarnishes; \(c) both samples of copper have the same density, 8.96 $\text{g}/\text{cm}^{3}$.
:::
::: tab Solution
(a) Mass is an **extensive** property — it scales with the amount of copper present; this is not a change, just a comparison of two samples.
(b) Tarnishing is a **chemical change** — silver reacts with sulfur compounds in air to form a new substance, silver sulfide, on the surface.
\(c) Density is an **intensive** property — it stays the same (8.96 $\text{g}/\text{cm}^{3}$) regardless of how much copper you have, which is exactly why it can help identify a substance.
:::
::::

:::: tabs
::: tab Problem
A contrasting pair that is easy to get backwards. Classify each as a physical or chemical change, and say what evidence supports your answer: (a) dry ice (solid $\ce{CO2}$) disappears into a cloud of fog at room temperature; (b) a strip of magnesium burns with a brilliant white flame, leaving a white powder.
:::
::: tab Solution
**(a) Physical change.** The solid sublimes into $\ce{CO2}$ gas — the *same compound* that was in the solid, now in a different state. (The gas itself is invisible; the fog is tiny droplets of liquid water formed as water vapor from the air condenses as the cold $\ce{CO2}$ chills it.) Nothing new was made; only the particle arrangement changed. The fact that a gas appears is *not* by itself proof of a chemical change, which is what makes this one a trap.

**(b) Chemical change.** The white powder is magnesium oxide, a new substance with different properties from both the magnesium and the oxygen that formed it. Evidence: light and heat released, and a product that cannot be turned back into magnesium by cooling.

The lesson: "a gas appeared" is weak evidence on its own. "A substance with new properties appeared, and the change does not simply reverse" is strong evidence.
:::
::::

> **Where this goes next.** Classification gives you the vocabulary for *what* chemistry studies. To say anything quantitative about it, you need agreed units and a way to measure — which is §1.2.

## 1.2 Measurement{{attrs[#blk-ch01sec02]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 1.2a}} Identify the SI base units and common prefixes.
- {{sp[info] Objective 1.2a}} Distinguish mass from weight.
- {{sp[info] Objective 1.2b}} Convert between volume units (mL, $\text{cm}^{3}$, L, $\text{dm}^{3}$, $\text{m}^{3}$).
- {{sp[info] Objective 1.2b}} Calculate density from mass and volume.
- {{sp[info] Objective 1.2c}} Convert temperature between Celsius, Fahrenheit, and Kelvin.
:::

### SI units and prefixes

The **International System of Units (SI)** gives chemistry a common set of base units, so that a measurement made in one lab means the same thing in another:

| Base Quantity | Name of Unit | Symbol |
|---|---|---|
| Length | meter | m |
| Mass | kilogram | kg |
| Time | second | s |
| Electrical current | ampere | A |
| Temperature | kelvin | K |
| Amount of substance | mole | mol |
| Luminous intensity | candela | cd |

Prefixes scale a unit by a power of ten — and the same prefix works on **any** unit, so learning them once covers kilometers, kilograms and kilojoules alike. The table below gives the values; Figure 1.3 shows the same information as a ladder, so the spacing between them is visible:

| Prefix | Symbol | Meaning | Example |
|---|---|---|---|
| tera- | T | $10^{12}$ | 1 Tm $=1\times10^{12}\,\text{m}$ |
| giga- | G | $10^{9}$ | 1 Gm $=1\times10^{9}\,\text{m}$ |
| mega- | M | $10^{6}$ | 1 Mm $=1\times10^{6}\,\text{m}$ |
| kilo- | k | $10^{3}$ | 1 km $=1\times10^{3}\,\text{m}$ |
| deci- | d | $10^{-1}$ | 1 dm $=1\times10^{-1}\,\text{m}$ |
| centi- | c | $10^{-2}$ | 1 cm $=1\times10^{-2}\,\text{m}$ |
| milli- | m | $10^{-3}$ | 1 mm $=1\times10^{-3}\,\text{m}$ |
| micro- | μ | $10^{-6}$ | 1 μm $=1\times10^{-6}\,\text{m}$ |
| nano- | n | $10^{-9}$ | 1 nm $=1\times10^{-9}\,\text{m}$ |
| pico- | p | $10^{-12}$ | 1 pm $=1\times10^{-12}\,\text{m}$ |

![The SI prefix ladder from pico- to tera-, plotted by power of ten](../assets/si_prefix_ladder.svg =600x)
*Figure 1.3 — The same prefixes as the table, arranged by size so the spacing is visible. Prefixes above the base (kilo-, mega-, giga-, tera-) make a unit larger; prefixes below it (centi-, milli-, micro-, nano-, pico-) make it smaller. The nanometer and picometer end of this ladder is where atoms live — a typical atom is about 100 pm across.*

:::: tabs
::: tab Problem
Convert (a) 2.5 km to millimeters, and (b) 450 nm (the wavelength of blue light) to meters.
:::
::: tab Solution
Go through the base unit every time — it turns one unfamiliar jump into two familiar ones.

**(a)** km → m → mm:
$$2.5\,\text{km}\times\frac{10^{3}\,\text{m}}{1\,\text{km}}\times\frac{1\,\text{mm}}{10^{-3}\,\text{m}}=2.5\times10^{6}\ \text{mm}$$

**(b)** nm → m, a single step:
$$450\,\text{nm}\times\frac{10^{-9}\,\text{m}}{1\,\text{nm}}=4.50\times10^{-7}\ \text{m}$$

Sanity check both: millimeters are *much* smaller than kilometers, so the number must get much bigger — it did. Meters are much bigger than nanometers, so the number must get much smaller — it did.
:::
::::

{{sp[warning] Reminder}} **Mass** (kg) measures the quantity of matter in an object and does not change with location; **weight** is the force gravity exerts on that mass, and it *does* change (an astronaut has the same mass on the Moon but weighs about one-sixth as much).

### Mass, volume, and density

:::warning
**Mass is not weight.** *Mass* is the quantity of matter in an object and does not change with location. *Weight* is the force gravity exerts on that mass, so it does change — the same sample weighs about one sixth as much on the Moon while its mass is identical. Chemistry deals in mass, and a balance measures mass, which is why a measured mass means the same thing anywhere. The two words are used interchangeably in everyday speech; in this course they are not interchangeable.
:::

**Volume** has a derived SI unit ($\text{m}^{3}$), but chemists most often use liters and milliliters:
$$1\,\text{mL} = 1\,\text{cm}^3 = 1\times10^{-6}\,\text{m}^3 \qquad 1\,\text{L} = 1\,\text{dm}^3 = 1000\,\text{mL} = 1\times10^{-3}\,\text{m}^3$$

==The one worth committing to memory is 1 mL = 1 $\text{cm}^{3}$, because it lets you move between a volume read off a graduated cylinder and a volume calculated from dimensions without any conversion at all.==

Mass is measured on a balance: Figure 1.4 shows the electronic kind you will actually use, and Figure 1.5 the older mechanical kind that makes the underlying idea visible. **Density** links mass and volume into a single intensive property:
$$d=\frac{m}{V} \qquad 1\,\text{g/cm}^3 = 1\,\text{g/mL} = 1000\,\text{kg/m}^3$$

![Electronic analytical balance with a draft shield, displaying a mass to four decimal places](../assets/electronic_balance.jpg =520x)
*Figure 1.4 — The electronic analytical balance you will actually use in lab. Note the display reading 200.0000 g: the balance reports mass to four decimal places, so every one of those digits is significant — this instrument is precise to ±0.0001 g. The glass draft shield keeps air currents from disturbing readings at that precision.*

![Two-pan mechanical analytical balance used to measure mass](../assets/lab_balance.jpg =460x)
*Figure 1.5 — The older two-pan mechanical balance makes the underlying idea visible: mass is determined by **comparing** an unknown sample against known reference masses until the beam balances. An electronic balance instead measures the force needed to support the sample and converts it to mass using a calibration against known reference masses, so it reports the same physical quantity.*

Because $d=m/V$ has three quantities, any one can be found from the other two. All three versions come up constantly, so it is worth seeing each solved rather than memorising three separate formulas — rearranging one equation is enough.

:::: tabs
::: tab Problem
The mass of a piece of gold is 45.3 g and its volume is 2.35 $\text{cm}^{3}$. What is its density?
:::
::: tab Solution
$$d=\frac{m}{V}=\frac{45.3\,\text{g}}{2.35\,\text{cm}^3}=19.3\ \text{g/cm}^3$$
This matches the accepted density of gold (19.3 $\text{g}/\text{cm}^{3}$) — a useful check that the calculation is reasonable.
:::
::::

:::: tabs
::: tab Problem
The same relationship, solved the other two ways. (a) Ethanol has a density of 0.789 g/mL. What is the mass of 25.0 mL of ethanol? (b) A piece of aluminum (density 2.70 $\text{g}/\text{cm}^{3}$) has a mass of 54.0 g. What is its volume?
:::
::: tab Solution
**(a) Solve for mass.** Rearranging $d=m/V$ gives $m=d\times V$:
$$m=0.789\,\frac{\text{g}}{\text{mL}}\times25.0\,\text{mL}=19.7\ \text{g}$$
The mL cancel, leaving grams — a check that the rearrangement was right.

**(b) Solve for volume.** Rearranging gives $V=m/d$:
$$V=\frac{54.0\,\text{g}}{2.70\,\text{g/cm}^3}=20.0\ \text{cm}^3$$

Note how the units confirm each answer independently of the arithmetic: dividing g by $\text{g}/\text{cm}^{3}$ leaves $\text{cm}^{3}$. If your rearrangement had been upside-down, the units would have come out as 1/$\text{cm}^{3}$ and told you so immediately.
:::
::::

### Temperature scales

Three temperature scales are used side by side in chemistry, and every conversion anchors to the same two fixed points — water's freezing point (0 °C = 32 °F = 273.15 K) and boiling point (100 °C = 212 °F = 373.15 K):

$$?\,^\circ\text{C} = (^\circ\text{F}-32\,^\circ\text{F})\times\frac{5\,^\circ\text{C}}{9\,^\circ\text{F}} \qquad ?\,^\circ\text{F} = \frac{9\,^\circ\text{F}}{5\,^\circ\text{C}}\times(^\circ\text{C})+32\,^\circ\text{F}$$
$$?\,\text{K}=(^\circ\text{C}+273.15\,^\circ\text{C})\frac{1\,\text{K}}{1\,^\circ\text{C}} \qquad ?\,^\circ\text{C} = (\text{K}-273.15\,\text{K})\frac{1\,^\circ\text{C}}{1\,\text{K}}$$

The **kelvin** scale deserves special attention because it is the one chemistry actually runs on. Its zero point is **absolute zero** — the coldest temperature that can exist — so a Kelvin temperature is never negative. That is why gas-law calculations from Chapter 5 onward require kelvin: those laws involve *ratios* of temperature, and ratios only behave sensibly on a scale with a true zero. Note also that kelvin takes no degree symbol: 298 K, not 298 °K.

:::: tabs
::: tab Problem
Convert (a) normal human body temperature, 37.0 °C, to Fahrenheit; (b) 74 °F to Celsius.
:::
::: tab Solution
**(a)** $\frac{9}{5}\times37.0=66.6$: 37.0 has 3 significant figures and 9/5 is exact, so the product keeps 3, to the tenths place. Then $66.6+32=98.6$; 32 is an exact reference point, so the sum keeps one decimal place: **98.6 °F** — the well-known Fahrenheit value for body temperature. (Rounding 66.6 to 67 *before* adding 32 would give 99 °F, a digit lost to premature rounding. Note too that the familiar 98.6 °F needs the reading 37.0 °C: from "37 °C", with only 2 significant figures, the answer is 99 °F.)

**(b)** $(74-32)\times\frac{5}{9}=42\times\frac{5}{9}=23.3\overline{3}$. Here 74 °F has 2 significant figures, which limits the multiplication/division result to 2 significant figures: **23 °C**.
:::
::::

:::: tabs
::: tab Problem
Now the conversion you will use most often. (a) Convert 25.0 °C (a typical "room temperature") to kelvin. (b) Liquid nitrogen boils at 77 K — what is that in °C, and why can the answer be negative when the kelvin value cannot?
:::
::: tab Solution
**(a)** $?\,\text{K}=25.0+273.15=298.15\ \text{K}$, reported as **298.2 K** to match the one decimal place in 25.0. (Many textbooks round 273.15 to 273 for convenience, giving 298 K; either is acceptable as long as you are consistent.)

**(b)** $?\,^\circ\text{C}=77-273.15=-196\ ^\circ\text{C}$.

The Celsius answer is negative because the Celsius zero is an arbitrary reference — the freezing point of water — and plenty of things are colder than that. The kelvin zero is not arbitrary: it is the true floor of temperature, so nothing can lie below it. Converting between the two is only ever a shift of 273.15, never a stretch, which is why a *change* of 1 °C and a *change* of 1 K are the same size.
:::
::::

> **Where this goes next.** You can now measure quantities and state their units. But a measurement is not just a number — it carries a claim about how precisely it is known, and §1.3 is the set of rules for making that claim honestly.

## 1.3 Numbers{{attrs[#blk-ch01sec03]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 1.3a}} Convert numbers to and from scientific notation, and add, subtract, multiply, and divide numbers written that way.
- {{sp[info] Objective 1.3b}} {{sp[info] Objective 1.3c}} Apply the significant-figure rules to a measured value, including in addition/subtraction and multiplication/division.
- {{sp[info] Objective 1.3c}} Distinguish accuracy from precision.
- {{sp[info] Objective 1.3b}} Read a measuring instrument to the correct number of significant figures, including one estimated digit.
:::

### Scientific notation

**Scientific notation** writes any number as $N\times10^n$, where $N$ is at least 1 but less than 10 ($1 \le N < 10$):
$$568.762 = 5.68762\times10^2 \qquad 0.00000772 = 7.72\times10^{-6}$$

The exponent counts how far the decimal point moved: **left** gives a positive exponent, **right** gives a negative one. Chemistry reaches for this constantly because its numbers run to extremes — a mole is $6.022\times10^{23}$ particles, and an atom is about $1\times10^{-10}$ m across. Both are awkward and error-prone to write out in full.

- **Addition/subtraction:** first rewrite every term with the *same* exponent, then add: $4.31\times10^4+3.9\times10^3=4.31\times10^4+0.39\times10^4=4.70\times10^4$.
- **Multiplication/division:** multiply or divide the $N$ values, then add or subtract the exponents:
$$(8.0\times10^4)\times(5.0\times10^2)=(8.0\times5.0)(10^{4+2})=40\times10^6=4.0\times10^7$$
$$\frac{8.5\times10^4}{5.0\times10^9}=\frac{8.5}{5.0}\times10^{4-9}=1.7\times10^{-5}$$

{{sp[warning] Watch out}} The two rules are genuinely different, and mixing them up is the most common error here. Addition needs matching exponents *first*; multiplication needs no such thing. If you find yourself adding exponents during an addition problem, you have applied the wrong rule.

:::: tabs
::: tab Problem
(a) Write 0.000418 in scientific notation, and $6.7\times10^{5}$ as an ordinary number. (b) Evaluate $(3.0\times10^{-3})\times(4.0\times10^{6})$.
:::
::: tab Solution
**(a)** For 0.000418 the decimal moves 4 places to the **right** to sit after the first nonzero digit, so the exponent is $-4$: $4.18\times10^{-4}$. For $6.7\times10^{5}$ the positive exponent means move the decimal 5 places right: $670{,}000$.

**(b)** Multiply the $N$ values and add the exponents:
$$(3.0\times4.0)\times10^{-3+6}=12\times10^{3}=1.2\times10^{4}$$
Note the last step: $12\times10^3$ is a correct value but not proper scientific notation, because 12 is not between 1 and 10. Shifting one place gives $1.2\times10^4$.
:::
::::

### Significant figures: counting them

==Significant figures record how precisely a quantity is actually known — every digit that survives a calculation should reflect real measurement precision, not calculator display precision.==

**Counting rules:**
1. Any nonzero digit is significant.
2. Zeros *between* nonzero digits are significant.
3. Zeros to the left of the first nonzero digit are never significant.
4. For a number greater than 1, all zeros written to the right of the decimal point count as significant.
5. For numbers with no decimal point, trailing zeros may or may not be significant — different textbooks differ, so use scientific notation to remove the ambiguity.

:::: tabs
::: tab Problem
How many significant figures are in each: (a) 358 m; (b) 35.1 g; \(c) 0.932 kg; (d) 0.0068 m; (e) $9.320\times10^{23}$ molecules; (f) 3400 mL?
:::
::: tab Solution
(a) 3 (all nonzero digits). (b) 3. \(c) 3 (the leading zero doesn't count). (d) 2 (leading zeros don't count; 6 and 8 do). (e) 4 (all digits before ×$10^{n}$ count, including the trailing zero after a decimal). (f) Ambiguous — 2, 3, or 4, depending on which trailing zeros were measured; write $3.400\times10^3$ mL to state 4 sig figs unambiguously, or $3.4\times10^3$ mL for 2.
:::
::::


### Significant figures in calculations

Counting them is the easy half. The harder half is knowing how many survive an arithmetic operation — and the rule is different for the two kinds of operation.

1. In **addition and subtraction**, the answer cannot have more digits to the right of the decimal point than either original number. *Decimal places* are what carry over.
2. In **multiplication and division**, the number of significant figures in the result is set by the original value with the *fewest* significant figures. *Significant figures* are what carry over.
3. **Exact numbers** — from definitions or from counting objects — have an infinite number of significant figures and never limit a calculation.

{{sp[warning] Watch out}} Rule 1 counts decimal places, rule 2 counts significant figures. They are different quantities, and the same measured value can limit an answer by either route.

:::: tabs
::: tab Problem
Give each result with the correct number of significant figures: (a) $3245+1.649$; (b) $54.3-3.32$; \(c) $3.14\times2.5$; (d) $0.0029\div92.1$; (e) $6.02\times10^{-4}-1.1\times10^{-5}$.
:::
::: tab Solution
Decide **which rule applies** before you round — that is the whole skill.

(a) Addition → decimal places. $3245+1.649=3246.649$; 3245 has 0 decimal places, so round to **3247**.
(b) Subtraction → decimal places. $54.3-3.32=50.98$; 54.3 has 1 decimal place, so round to **51.0**. (Keep the trailing zero — it states that the tenths place is known.)
\(c) Multiplication → significant figures. $3.14\times2.5=7.85$; 2.5 has only 2 sig figs, so round to **7.9**. (An exact half rounds *up* — the convention used throughout this course, and the same one that takes 2.45 to 2.5 in the next problem.)
(d) Division → significant figures. $0.0029\div92.1=0.00003148\ldots$; 0.0029 has 2 sig figs, so **0.000031**, i.e. $3.1\times10^{-5}$.
(e) Subtraction in scientific notation → match exponents first, then use decimal places:
$$6.02\times10^{-4}-0.11\times10^{-4}=5.91\times10^{-4}$$
Both terms now carry 2 decimal places in their $N$ values, so the answer keeps 2: **$5.91\times10^{-4}$**.
:::
::::

:::: tabs
::: tab Problem
A two-step calculation, where the rule changes partway through. A student measures a rectangular metal sheet as 12.5 cm by 3.2 cm, then cuts off a strip 0.75 cm wide along the long side, narrowing the 3.2 cm width. Report (a) the original area and (b) the remaining width after the cut, each to the correct precision.
:::
::: tab Solution
**(a) Area — multiplication, so significant figures.** $12.5\times3.2=40.0\ \text{cm}^{2}$. The value 3.2 has only 2 significant figures, so the answer must too: **40. $\text{cm}^{2}$**, better written $4.0\times10^1\ \text{cm}^{2}$ to make the 2 sig figs unambiguous.

**(b) Remaining width — subtraction, so decimal places.** $3.2-0.75=2.45$ cm. The value 3.2 has only 1 decimal place, so round to **2.5 cm**.

The same measurement, 3.2 cm, limited the answer *both* times — but by a different mechanism each time (2 sig figs in the multiplication, 1 decimal place in the subtraction). Identify the operation first; the rule follows from it.
:::
::::


### Accuracy and precision

**Accuracy** is how close a measurement is to the true value; **precision** is how closely repeated measurements agree with *each other*. Figure 1.6 shows why both words are needed: the two qualities are independent, so all four combinations occur.

![Four dartboards contrasting accuracy and precision as independent qualities](../assets/accuracy_vs_precision.svg =700x)
*Figure 1.6 — The two ideas are independent, which is why all four combinations exist. The case worth dwelling on is the second: tightly clustered results that are consistently wrong. Precision is easy to see (the readings agree), accuracy is not (nothing in the data itself reveals the offset) — so precise-but-inaccurate results are the most dangerous kind, and only calibration against a known standard exposes them.*

:::: tabs
::: tab Problem
A sample's true mass is 10.00 g. Three students each weigh it four times and report: **A** — 10.01, 9.99, 10.00, 10.00 g; **B** — 9.21, 9.22, 9.20, 9.21 g; **C** — 9.71, 10.30, 9.95, 10.04 g. Describe each student's results as accurate, precise, both, or neither, and say which set is the most dangerous to trust.
:::
::: tab Solution
**Student A** — the four readings agree closely with one another (precise) and cluster on 10.00 g (accurate). **Both.**

**Student B** — the readings agree with one another to within 0.02 g (very precise) but are all about 0.8 g low. **Precise but not accurate.**

**Student C** — the readings average close to 10.00 g (roughly accurate) but scatter over half a gram. **Accurate but not precise.**

**Student B's set is the most dangerous.** Poor precision announces itself: student C can see the scatter and knows not to trust any single reading. Student B's data looks excellent — tight, repeatable, professional — and is wrong every time, probably from a systematic error such as a balance that was never zeroed. **Nothing inside a precise dataset reveals that it is inaccurate; only comparison with a known standard can.**
:::
::::

### Reading an instrument

The numbers of measured quantities, unlike defined or counted quantities, are never exact. When you read a liquid volume, the bottom of the meniscus in Figure 1.7 clearly lies between the 21 and 22 mL marks — so the volume is certainly more than 21 mL and less than 22. It sits a little nearer the 22 mark, so a reasonable estimate is 21.6 mL. In "21.6", the digits 2 and 1 are **certain** and the 6 is **estimated**. Another reader might judge 21.5 or 21.7; that disagreement in the last place is expected and acceptable. What would be pointless is estimating a hundredths digit, when the tenths digit is already uncertain.

As a general rule, a scale like this can be read to one-tenth of its smallest division — so 1-mL divisions support a reading to the nearest 0.1 mL, and the last digit you write is always the estimated one.

![Reading a graduated cylinder at the bottom of the meniscus, with an estimated digit](../assets/graduated_cylinder_meniscus.svg =420x)
*Figure 1.7 — Liquid in a glass cylinder curves upward at the walls, forming a concave **meniscus**; the volume is always read at the **bottom** of that curve, with your eye level with it. Reading from above or below introduces a parallax error that no amount of care with significant figures can undo.*

> **Where this goes next.** You can now record a measurement honestly. The last tool, in §1.4, is the method for *converting* one into different units without losing that honesty — and it is the single technique you will use most in this course.

:::: tabs
::: tab Problem
A burette is marked every 0.1 mL. The liquid level sits just past the 15.2 mL mark, roughly a third of the way to 15.3. How should the volume be recorded, and how many significant figures does it have?
:::
::: tab Solution
The certain digits are the ones the markings give you directly: **15.2**. One further digit is estimated by eye between the marks — about a third of the way, so **15.23 mL**.

That is **4 significant figures**: three certain, one estimated.

Two errors are common here. Recording 15.2 mL throws away real information you could see. Recording 15.234 mL claims a thousandths digit you never had, since the tenths place was already the last marked one. Always report every certain digit plus exactly one estimated digit — no more, no fewer.
:::
::::

§1.3 gave every measurement a unit and a defensible number of digits. What it did not give you is a way to *move* between units — and almost every calculation in this course starts in units you were handed and has to end in units you actually want. §1.4 supplies that missing step, and it turns out the units themselves will tell you whether your setup is right.

## 1.4 Dimensional Analysis{{attrs[#blk-ch01sec04]}}

:::success
**Learning Objectives**
- {{sp[info] Objective 1.4a}} Identify the unit-conversion factor(s) needed to solve a problem.
- {{sp[info] Objective 1.4a}} Set up a calculation so that units cancel to leave only the desired unit.
- {{sp[info] Objective 1.4a}} Verify a calculated answer by checking that all units canceled correctly.
:::

### The unit-factor method

**Dimensional analysis** (the unit-factor-label method) treats a conversion factor as a fraction equal to 1, chosen so unwanted units cancel:
$$\text{given unit}\times\frac{\text{desired unit}}{\text{given unit}}=\text{desired unit}$$

Figure 1.8 shows why the method is self-checking. The procedure is always the same three steps: **(1)** decide which conversion factor(s) you need; **(2)** carry the units through the calculation alongside the numbers; **(3)** check that everything cancels except the unit you wanted. If it does, the factors were set up (oriented) correctly, though you still need to confirm each factor's numerical value.

![Unit-cancellation diagram for a single-factor dimensional-analysis conversion](../assets/dimensional_analysis_cancel.svg =620x)
*Figure 1.8 — Why the method is self-checking. Because 1 oz and 28.349 g are the same mass, the factor equals 1 — multiplying by it changes the units without changing the amount. Writing grams on the bottom makes the given grams cancel, leaving ounces. This is the useful part: the units tell you whether the setup is right **before** you do any arithmetic.*

==This is the single most-reused problem-solving method in the course — it reappears explicitly in mole/mass conversions (Ch. 3), gas-law unit conversions (Ch. 5), and concentration-unit conversions (Ch. 12).== Time spent here is repaid many times over.

:::: tabs
::: tab Problem
A competition frisbee has a mass of 125 g. Convert its mass to ounces, given 1 oz = 28.349 g.
:::
::: tab Solution
$$x\,\text{oz}=125\,\text{g}\times\frac{1\,\text{oz}}{28.349\,\text{g}}=4.41\ \text{oz}$$
The conversion factor is written with grams in the denominator specifically so the given "g" cancels, leaving only "oz."
:::
::::

### Chaining several conversions

Most real problems need more than one factor. They are chained into a single line, and the cancellation check works exactly the same way.

:::: tabs
::: tab Problem
The same idea, chained. A car is traveling at 65 miles per hour. What is its speed in meters per second, given 1 mile = 1609 m?
:::
::: tab Solution
Two separate conversions are needed — miles → meters on the top, hours → seconds on the bottom — and they can be strung into one line:
$$65\,\frac{\text{mi}}{\text{h}}\times\frac{1609\,\text{m}}{1\,\text{mi}}\times\frac{1\,\text{h}}{60\,\text{min}}\times\frac{1\,\text{min}}{60\,\text{s}}=29\ \frac{\text{m}}{\text{s}}$$
Track the cancellation: mi cancels against mi, h against h, min against min — leaving m on top and s on the bottom, exactly the unit asked for.

Two sig figs, because 65 has two (the time conversions are exact definitions and 1609 m has four sig figs, so none of the conversion factors limits the answer). And a plausibility check: 29 m/s is roughly 100 km/h, which is about right for 65 mph.
:::
::::

:::: tabs
::: tab Problem
A 4.00 qt sample of antifreeze weighs 9.26 lb. Find its density in g/mL, given 1 lb = 453.59 g and 1 L = 1.0567 qt.
:::
::: tab Solution
This needs conversions on *both* the top and the bottom of a ratio — mass (lb → g) and volume (qt → L → mL). Doing each piece separately is often clearer than one long chain:
$$9.26\,\text{lb}\times\frac{453.59\,\text{g}}{1\,\text{lb}}=4.20\times10^{3}\,\text{g} \qquad 4.00\,\text{qt}\times\frac{1\,\text{L}}{1.0567\,\text{qt}}\times\frac{1000\,\text{mL}}{1\,\text{L}}=3785\,\text{mL}$$
$$d=\frac{4.20\times10^{3}\,\text{g}}{3785\,\text{mL}}=1.11\ \text{g/mL}$$
A check on the answer: antifreeze should be a little denser than water (1.00 g/mL), and 1.11 g/mL is exactly that sort of value.
:::
::::

## Synthesis

==This chapter builds no chemical reactions, but it builds the toolkit every later chapter assumes: matter classification gives the vocabulary, measurement gives the quantities, significant figures give the honesty about precision, and dimensional analysis gives the method for converting between them.== A student who leaves Chapter 1 fluent in unit conversion and significant-figure reporting will find the *arithmetic* of every later chapter (molar mass in Ch. 3, gas laws in Ch. 5, concentration units in Ch. 12) far less of an obstacle than the underlying chemistry itself.

If you take only one habit from this chapter, make it the unit check: **carry units through every calculation and confirm they cancel to what you wanted.** It catches more errors, more cheaply, than any other single practice in chemistry.

## Asset and License Record for This Chapter

| Asset | Source URL | License | Attribution |
|---|---|---|---|
| `assets/matter_classification_tree.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
| `assets/states_of_matter.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
| `assets/si_prefix_ladder.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
| `assets/electronic_balance.jpg` | https://commons.wikimedia.org/wiki/File:Analytical_Weighing_Balance_UP_Scales.jpg | CC BY-SA 4.0 | Manishbookmyuniversity, via Wikimedia Commons. |
| `assets/lab_balance.jpg` | https://commons.wikimedia.org/wiki/File:Analytical_balance_scales.jpg | CC BY-SA 4.0 | Drugs Rehab Center Parus - Moscow, via Wikimedia Commons. |
| `assets/accuracy_vs_precision.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
| `assets/graduated_cylinder_meniscus.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
| `assets/dimensional_analysis_cancel.svg` | — (self-generated, matplotlib) | CC BY 4.0 | Self-generated; released under this package's CC BY 4.0 license. |
