{{nyml
kind: document
format: 1
title: Chapter 18 Assessment Guide: Redox Reactions and Electrochemistry
}}

# Chapter 18 Assessment Guide: Redox Reactions and Electrochemistry

## Source and Format

**Reference:** Yu Wang's General Chemistry Lecture Notes, Chapter 18 (CC BY 4.0). **Audience:** introductory undergraduate general chemistry, second semester. **Note:** this is design guidance for building assessments — question *guides* an instructor or generator can instantiate into many concrete questions — not a finished question bank or answer key.

## General Assessment Priorities

- Anchor the **cathode/anode selection rule** to one fixed criterion — the half-reaction with the *higher* E° is always the cathode — computed by comparison every time, never by intuition about "which metal is more reactive."
- Require students to **explicitly rewrite the anode half-reaction as an oxidation** (reversed from its tabulated reduction form, with the sign of E° left unchanged) as a separate, visible step before combining half-reactions.
- Require **equalizing electron counts (n)** between half-reactions as an explicit, checkable step, and confirm the same n is reused consistently in ΔG°, K, and Nernst-equation calculations.
- Test the **E° vs. Nernst-equation** distinction directly: ask whether given conditions are standard (1 M, 1 atm) before choosing which formula applies.

## Objective 18.1a: Assign oxidation numbers

### Target understanding

A student can assign oxidation numbers to atoms in a compound or ion using the standard rule set, including the common exceptions (hydrides, peroxides), and verify the result sums correctly to the overall charge.

### Question guides

**1. Forward — simple compound**
- Variables & ranges: a compound with unambiguous oxidation states from the standard rules.
- Constraint: correct application of the H=+1, O=−2 default rules.
- Contexts: common oxoanions, oxides, or acids.
- Formats: workout.
- Worked instantiation: assign oxidation numbers to Mn in $\ce{MnO4-}$ (O is −2 ×4 = −8; charge is −1; Mn = −1−(−8) = +7).

**2. Forward — an exception case**
- Variables & ranges: a hydride ($\ce{LiH}$-type) or peroxide ($\ce{H2O2}$-type) compound.
- Constraint: correct recognition that the default H/O rule doesn't apply here.
- Contexts: active-metal hydrides, peroxides.
- Formats: workout.
- Worked instantiation: assign oxidation numbers to both atoms in $\ce{CaH2}$ (H is −1 here, since Ca is an active metal forming a hydride; Ca is +2).

**3. Conceptual — verifying via charge sum**
- Variables & ranges: any assigned set of oxidation numbers for a polyatomic ion.
- Constraint: explanation must reference the sum-equals-charge rule as a check.
- Contexts: any oxoanion.
- Formats: short-answer.
- Worked instantiation: "After assigning oxidation numbers in $\ce{SO4^2-}$, how can you check your work?" → Sum all oxidation numbers (S plus 4× O) and confirm the total equals the ion's overall charge (−2); if it doesn't, an assignment was made incorrectly.

**4. Error analysis**
- Variables & ranges: a student who applies the default O=−2 rule to a peroxide.
- Constraint: correction must identify the exception and its correct value.
- Contexts: $\ce{H2O2}$ or a similar peroxide.
- Formats: short-answer.
- Worked instantiation: "A student assigns O as −2 in $\ce{H2O2}$, then can't make the oxidation numbers sum to zero. What's the fix?" → $\ce{H2O2}$ is a peroxide, where O is an exception at −1 (not the default −2); using −1 for both oxygens (with H at +1) correctly sums to zero.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 3–4 oxidation-number assignments, including at least one exception case. |
| Group discussion | Understand | Debate why oxidation number is a "hypothetical" ionic-bonding assumption, not a real physical charge. |
| Quiz | Apply | One standard-case, one exception-case assignment. |
| Exam | Analyze | Require the charge-sum check explicitly as part of the answer. |
| Project/activity | Evaluate | Assign oxidation numbers throughout a multi-step industrial redox process (e.g., steelmaking). |

## Objective 18.1b: Balance redox equations using the half-reaction method

### Target understanding

A student can balance a redox equation in acidic solution using the systematic half-reaction method, and adapt the result for basic solution by neutralizing H⁺ with OH⁻.

### Question guides

**1. Forward — balance in acidic solution**
- Variables & ranges: two half-reactions (unbalanced), acidic conditions.
- Constraint: correct sequential application of all steps (atoms, O/H, charge, electron equalization).
- Contexts: any redox pair, including polyatomic oxidizing/reducing agents.
- Formats: workout.
- Worked instantiation: see the study guide's worked example ($\ce{H2O2+Sn^2+->H2O+Sn^4+}$, acidic).

**2. Forward — adapt to basic solution**
- Variables & ranges: the same reaction, now in basic solution.
- Constraint: correct addition of OH⁻ to both sides and combination into water.
- Contexts: the same or a different redox pair.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (same reaction, basic solution version).

**3. Conceptual — why equalize electrons before adding**
- Variables & ranges: any two half-reactions with different numbers of transferred electrons.
- Constraint: explanation must reference charge balance in the final combined equation.
- Contexts: any half-reaction pair with unequal electron counts.
- Formats: short-answer.
- Worked instantiation: "Why must the electrons in the two half-reactions be equal before adding them together?" → Electrons don't appear as a species in the overall reaction — they must cancel out exactly when the half-reactions are added; if the electron counts differ, extra electrons would remain in the "balanced" equation, which is not physically meaningful.

**4. Error analysis**
- Variables & ranges: a student who balances O and H but forgets to check the final charge balance.
- Constraint: correction must require an explicit charge-balance check as the final step.
- Contexts: any redox-balancing problem.
- Formats: short-answer.
- Worked instantiation: "A student balances atoms and thinks they're done, without checking that charge is balanced on both sides. What could still be wrong?" → Atom balance alone doesn't guarantee charge balance — the number of electrons added to balance charge in each half-reaction must be checked, and the final combined equation should have identical net charge on both sides as a last verification step.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 full redox-balancing problems, at least one requiring the basic-solution adaptation. |
| Group discussion | Analyze | Walk through each step of the method as a group, catching errors at each stage. |
| Quiz | Apply | One acidic-solution balancing problem. |
| Exam | Analyze | Require both acidic and basic versions of the same reaction. |
| Project/activity | Evaluate | Balance a real multi-electron industrial or biological redox reaction (e.g., a metallurgical extraction). |

## Objective 18.2a: Define galvanic cells and write cell diagrams

### Target understanding

A student can define galvanic cell, electrode, anode, and cathode, and can write the standard cell-diagram notation for a given set of half-reactions or overall reaction.

### Question guides

**1. Forward — write a cell diagram from half-reactions**
- Variables & ranges: two given half-reactions (with an inert electrode where needed).
- Constraint: correct anode-first ordering, correct phase-boundary (`|`) and salt-bridge (`||`) notation.
- Contexts: any pair of half-reactions, including one requiring an inert electrode.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (Mg/Fe³⁺/Fe²⁺ cell with Pt cathode).

**2. Inverse — extract half-reactions from a cell diagram**
- Variables & ranges: a given cell diagram, extract the anode/cathode half-reactions.
- Constraint: correct identification of oxidation (anode side) vs. reduction (cathode side) from diagram position.
- Contexts: any properly formatted cell diagram.
- Formats: short-answer.
- Worked instantiation: given $\ce{Zn(s)|Zn^2+}(1M)||\ce{Cu^2+}(1M)|\ce{Cu(s)}$, write both half-reactions.

**3. Conceptual — why a salt bridge is needed**
- Variables & ranges: any two-half-cell setup.
- Constraint: explanation must reference maintaining electrical neutrality in each half-cell.
- Contexts: any galvanic cell.
- Formats: short-answer.
- Worked instantiation: "Why does a galvanic cell need a salt bridge (or porous barrier) between its two half-cells?" → As the reaction proceeds, one half-cell accumulates excess positive charge (cations forming) and the other accumulates excess negative charge (cations being consumed); the salt bridge allows ion flow to maintain electrical neutrality in both half-cells, without which the reaction would quickly stop.

**4. Error analysis**
- Variables & ranges: a student who writes the cell diagram cathode-first.
- Constraint: correction must restate the anode-first convention.
- Contexts: any cell-diagram-writing task.
- Formats: short-answer.
- Worked instantiation: "A student writes $\ce{Cu(s)|Cu^2+}||\ce{Zn^2+}|\ce{Zn(s)}$ for a Zn/Cu cell where Zn is the anode. What's wrong?" → The cell diagram convention always starts with the anode and ends with the cathode; since Zn is the anode here, the correct diagram is $\ce{Zn(s)|Zn^2+}||\ce{Cu^2+}|\ce{Cu(s)}$ — the student's version has the electrodes reversed.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 cell-diagram-writing problems, including one requiring an inert electrode. |
| Group discussion | Understand | Discuss the physical role of the salt bridge with a concrete analogy. |
| Quiz | Apply | One cell-diagram item, either direction (write it, or extract half-reactions from it). |
| Exam | Analyze | Require identifying which species is oxidized/reduced directly from a given cell diagram. |
| Project/activity | Evaluate | Research a real historical galvanic cell design (e.g., the Daniell cell) and diagram it. |

## Objective 18.3a: Define standard reduction potential and the SHE

### Target understanding

A student can define standard reduction potential (E°), explain the standard hydrogen electrode's role as the zero reference, and state that E° does not change with stoichiometric scaling.

### Question guides

**1. Conceptual — why a reference electrode is needed**
- Variables & ranges: any discussion of measuring electrode potentials.
- Constraint: explanation must state that only *cell* (relative) potentials are directly measurable, not single-electrode potentials in isolation.
- Contexts: general electrochemistry.
- Formats: short-answer.
- Worked instantiation: "Why can't we measure a single electrode's potential directly, without reference to another electrode?" → A voltmeter measures a potential *difference* between two points; a single electrode's potential has no meaning on its own, so all standard reduction potentials are defined relative to the standard hydrogen electrode (arbitrarily set to 0 V), which provides a universal reference point.

**2. Forward — scaling invariance**
- Variables & ranges: a half-reaction with its coefficients doubled or tripled.
- Constraint: correctly state that E° is unchanged.
- Contexts: any half-reaction.
- Formats: short-answer.
- Worked instantiation: "If $\ce{Cu^2++2e- -> Cu}$ has $E^\circ=0.34$ V, what is $E^\circ$ for $\ce{2Cu^2++4e- -> 2Cu}$?" → Still $E^\circ=0.34$ V — standard reduction potential is an intensive property (like temperature or density) and does not change when a half-reaction's coefficients are scaled.

**3. Predict-the-effect — comparing two E° values**
- Variables & ranges: two half-reactions with different E° values.
- Constraint: prediction must correctly rank which is the stronger oxidizing agent.
- Contexts: any two tabulated half-reactions.
- Formats: short-answer.
- Worked instantiation: "Between $\ce{F2+2e- -> 2F-}$ ($E^\circ=+2.87$ V) and $\ce{Ag+ +e- -> Ag}$ ($E^\circ=+0.80$ V), which is the stronger oxidizing agent?" → $\ce{F2}$ — the higher E° means it is more easily reduced (a better electron acceptor), making it the stronger oxidizing agent.

**4. Error analysis**
- Variables & ranges: a student who assumes E° scales with the reaction's stoichiometric coefficients (like ΔH° or ΔG° would).
- Constraint: correction must contrast E° (intensive) with ΔH°/ΔG° (extensive).
- Contexts: any half-reaction scaling scenario.
- Formats: short-answer.
- Worked instantiation: "A student assumes doubling a half-reaction's coefficients doubles its E°, by analogy with ΔH°. What's the error?" → Unlike ΔH° or ΔG° (extensive properties that scale with the amount of reaction), E° is an intensive property — a per-electron voltage that does not change regardless of how the half-reaction's coefficients are scaled.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | Explain the SHE's role; classify 2–3 scaling scenarios. |
| Group discussion | Analyze | Debate why E° is intensive while ΔG° (computed from it via ΔG°=−nFE°) is extensive. |
| Quiz | Understand | One SHE-role explanation item. |
| Exam | Analyze | Require ranking 3+ half-reactions by oxidizing/reducing strength from their E° values. |
| Project/activity | Evaluate | Research how the SHE is constructed and why it's impractical for routine lab use (leading to reference electrodes like Ag/AgCl). |

## Objective 18.3b: Identify cathode/anode and calculate standard cell potential

### Target understanding

A student can identify the cathode (higher E°) and anode (lower E°, reversed) from two half-reactions, and calculate the overall reaction, cell diagram, and standard cell potential.

### Question guides

**1. Forward — full cell analysis**
- Variables & ranges: two half-reactions with given E° values.
- Constraint: correct cathode/anode identification, correct electron equalization, correct E°cell calculation.
- Contexts: any two half-reactions.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (Ag/Cu cell, $E^\circ_{cell}=0.46$ V).

**2. Forward — a three-metal comparison**
- Variables & ranges: three or more half-reactions with given E° values, identify strongest oxidizing/reducing agents.
- Constraint: correct ranking by E° value.
- Contexts: any set of half-reactions.
- Formats: short-answer.
- Worked instantiation: given $\ce{Al^3++3e- -> Al}$ (−1.66 V), $\ce{Fe^3++e- -> Fe^2+}$ (0.77 V), $\ce{Sn^4++2e- -> Sn^2+}$ (0.14 V), $\ce{AgBr+e- -> Ag+Br-}$ (0.07 V), identify the strongest oxidizing and reducing agents.

**3. Conceptual — why E°cell must be positive**
- Variables & ranges: any spontaneous galvanic cell.
- Constraint: explanation must connect the cathode/anode selection rule to a guaranteed positive result.
- Contexts: any half-reaction pair.
- Formats: short-answer.
- Worked instantiation: "Why is $E^\circ_{cell}$ always positive when the higher-E° half-reaction is correctly assigned as the cathode?" → Since $E^\circ_{cell}=E^\circ_{cathode}-E^\circ_{anode}$ and the cathode is defined as whichever half-reaction has the *higher* E°, the subtraction is guaranteed to be positive — this is precisely how the cathode/anode assignment rule is derived.

**4. Error analysis**
- Variables & ranges: a student who forgets to reverse the sign convention correctly (e.g., subtracts E°cell backwards).
- Constraint: correction must restate the correct subtraction order.
- Contexts: any E°cell calculation.
- Formats: short-answer.
- Worked instantiation: "A student computes $E^\circ_{cell}=E^\circ_{anode}-E^\circ_{cathode}$, getting a negative number for a cell they know is spontaneous. What's wrong?" → The formula is backwards — it should be $E^\circ_{cell}=E^\circ_{cathode}-E^\circ_{anode}$ (cathode minus anode); the student's reversed formula will always give the negative of the correct answer.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2–3 full cathode/anode/cell-potential problems. |
| Group discussion | Analyze | Rank a set of half-reactions from strongest to weakest oxidizing agent. |
| Quiz | Apply | One full cell-potential calculation from two half-reactions. |
| Exam | Analyze | Require identifying strongest oxidizing/reducing agents from a list of 4+ half-reactions. |
| Project/activity | Evaluate | Research real E° values for a galvanic cell used industrially (e.g., in metal refining) and verify its cell potential. |

## Objective 18.4a: Relate ΔG°, K, and E° for a redox reaction

### Target understanding

A student can convert between $\Delta G^\circ$, $K$, and $E^\circ$ for a redox reaction using $\Delta G^\circ=-nFE^\circ=-RT\ln K$, correctly tracking the value of $n$.

### Question guides

**1. Forward — E° to ΔG° to K**
- Variables & ranges: two half-reactions with given E°, find ΔG° and K.
- Constraint: correct value of $n$ from equalizing electrons; correct use of $F=96{,}485$ C/mol.
- Contexts: any redox reaction with tabulated half-reaction E° values.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (Sn/Cu⁺ reaction, $\Delta G^\circ=-5.606\times10^4$ J/mol, $K=6.7\times10^9$).

**2. Forward — a second worked case**
- Variables & ranges: $\ce{H2(g)+2Ag+(aq)->2H+(aq)+2Ag(s)}$.
- Constraint: correct identification that $\ce{H2}$ is the SHE reference (E°=0), simplifying the E°cell calculation.
- Contexts: any reaction involving the SHE.
- Formats: workout.
- Worked instantiation: given $E^\circ(\ce{Ag+/Ag})=0.80$ V, find $E^\circ_{cell}$, $\Delta G^\circ$, and $K$ for this reaction ($E^\circ_{cell}=0.80$ V, $\Delta G^\circ=-77.2$ kJ/mol, $K=3.4\times10^{13}$).

**3. Conceptual — qualitative prediction before calculating**
- Variables & ranges: a given E°cell (positive or negative).
- Constraint: prediction must state whether K should be greater or less than 1 before calculating.
- Contexts: any redox reaction with known E°cell.
- Formats: short-answer.
- Worked instantiation: "Without calculating, would you expect $K>1$ or $K<1$ for a reaction with $E^\circ_{cell}=-0.30$ V?" → $K<1$ — a negative $E^\circ_{cell}$ corresponds to positive $\Delta G^\circ$ (via $\Delta G^\circ=-nFE^\circ$), which in turn corresponds to $K<1$.

**4. Error analysis**
- Variables & ranges: a student who uses the wrong value of $n$ (forgetting to equalize electrons from the original half-reactions).
- Constraint: correction must trace back to the electron-equalization step.
- Contexts: any $\Delta G^\circ$/$K$ calculation from E°.
- Formats: short-answer.
- Worked instantiation: "A student combines two half-reactions (one with 2 electrons, one with 3) without equalizing, then uses $n=2$ in $\Delta G^\circ=-nFE^\circ$. What's wrong?" → Before combining, both half-reactions must be scaled so their electron counts match (in this case, to the least common multiple, 6); the value of $n$ used in every subsequent calculation must be this equalized electron count, not either original half-reaction's count.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2 full ΔG°/K/E° conversion problems. |
| Group discussion | Analyze | Debate why all three quantities (ΔG°, K, E°) must agree on the same qualitative conclusion (spontaneous or not). |
| Quiz | Apply | One E°-to-ΔG°-to-K conversion. |
| Exam | Analyze | Require the qualitative K-vs-1 prediction explicitly before the numeric answer. |
| Project/activity | Evaluate | Research a real battery half-reaction's E° and calculate its theoretical K. |

## Objective 18.4b: Apply the Nernst equation

### Target understanding

A student can apply $E=E^\circ-\frac{RT}{nF}\ln Q$ to find cell potential under non-standard conditions, correctly constructing $Q$ from the given concentrations/pressures.

### Question guides

**1. Forward — Nernst equation from given concentrations**
- Variables & ranges: a cell diagram with non-1-M concentrations, given half-reaction E° values.
- Constraint: correct construction of $Q$ matching the overall reaction's stoichiometry.
- Contexts: any non-standard-condition galvanic cell.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (Al/Cu cell, $E=1.97$ V).

**2. Conceptual — when Nernst is required**
- Variables & ranges: a cell described as at "1 M, 1 atm" vs. other concentrations.
- Constraint: explanation must state that E° alone applies only under standard conditions.
- Contexts: any galvanic cell with specified (or unspecified) conditions.
- Formats: short-answer.
- Worked instantiation: "A problem gives concentrations of 0.5 M and 2.0 M for a cell's two half-reactions. Can you just use E°cell directly?" → No — E°cell only applies when all solutes are at 1 M and gases at 1 atm; since the given concentrations are not standard, the Nernst equation must be used to find the actual E.

**3. Predict-the-effect — direction of the correction**
- Variables & ranges: a reaction where product concentrations are below standard (1 M).
- Constraint: prediction must state that E should increase above E° in this case (since Q<1, ln Q<0, making the correction term add to E°).
- Contexts: any non-standard-condition cell with low product concentrations.
- Formats: short-answer.
- Worked instantiation: "If the products of a cell reaction are at lower-than-standard concentrations (reactants closer to standard), would you expect E to be greater than or less than E°?" → Greater than E° — with lower product concentrations, $Q<1$, so $\ln Q<0$, making $-\frac{RT}{nF}\ln Q$ positive and increasing E above E°.

**4. Error analysis**
- Variables & ranges: a student who builds Q using the reduction half-reactions' coefficients instead of the overall balanced reaction's coefficients.
- Constraint: correction must require constructing Q from the final, combined overall reaction.
- Contexts: any Nernst-equation problem with a multi-electron overall reaction.
- Formats: short-answer.
- Worked instantiation: "A student builds Q using $[\ce{Al^3+}]^1$ instead of $[\ce{Al^3+}]^2$ for a reaction whose balanced overall equation has a coefficient of 2 for $\ce{Al^3+}$. What's wrong?" → Q must be constructed using the coefficients of the final, correctly balanced *overall* reaction (after equalizing electrons and combining half-reactions), not from an intermediate or unbalanced form — using the wrong exponent will give an incorrect Q and therefore an incorrect E.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 2 Nernst-equation calculations from given non-standard concentrations. |
| Group discussion | Analyze | Debate when a "non-standard" condition is close enough to standard to approximate with E° alone. |
| Quiz | Apply | One Nernst-equation calculation. |
| Exam | Analyze | Require justifying why the Nernst equation (not E° alone) applies to the given conditions. |
| Project/activity | Evaluate | Model how a real battery's voltage changes as it discharges (concentrations shift away from standard). |

## Objective 18.4c: Calculate the potential of a concentration cell

### Target understanding

A student can identify the anode and cathode in a concentration cell (dilute = anode, concentrated = cathode) and calculate its potential using $E=-\frac{RT}{nF}\ln Q$ (since $E^\circ=0$).

### Question guides

**1. Forward — concentration cell potential**
- Variables & ranges: two concentrations of the same ion/electrode pair.
- Constraint: correct identification of which side is anode vs. cathode before setting up Q.
- Contexts: any same-electrode concentration cell.
- Formats: workout.
- Worked instantiation: see the study guide's worked example (Zn concentration cell, 0.10 M/0.50 M, $E=0.0207$ V).

**2. Conceptual — why E° = 0**
- Variables & ranges: any concentration cell.
- Constraint: explanation must state that both half-reactions are identical (same electrode, same species), so their E° values are equal and cancel.
- Contexts: any concentration cell.
- Formats: short-answer.
- Worked instantiation: "Why is $E^\circ=0$ for every concentration cell, regardless of which electrode material is used?" → Both half-cells use the exact same half-reaction (same electrode material and ion), so $E^\circ_{cathode}=E^\circ_{anode}$ and $E^\circ_{cell}=E^\circ_{cathode}-E^\circ_{anode}=0$ — the entire driving force comes from the concentration difference, captured by Q alone.

**3. Predict-the-effect — as concentrations equalize**
- Variables & ranges: a concentration cell as it discharges over time.
- Constraint: prediction must state that E approaches 0 as the two concentrations approach each other.
- Contexts: any concentration cell over time.
- Formats: short-answer.
- Worked instantiation: "As a concentration cell operates, ions move from the concentrated to the dilute side. What happens to E over time?" → E decreases toward zero — as the reaction proceeds, the concentrated side's concentration decreases and the dilute side's increases, so Q approaches 1 and $\ln Q\to0$, driving E toward 0 (equilibrium, no further net driving force).

**4. Error analysis**
- Variables & ranges: a student who identifies the concentrated half-cell as the anode.
- Constraint: correction must restate the correct dilute=anode/concentrated=cathode assignment.
- Contexts: any concentration cell.
- Formats: short-answer.
- Worked instantiation: "A student assumes the more concentrated half-cell is always the anode, since 'more stuff means more reactivity.' What's the correct assignment, and why?" → The *dilute* side is the anode and the *concentrated* side is the cathode — the cell spontaneously moves ions from high to low concentration (like Le Chatelier's principle, Chapter 14), which means the concentrated side's ions are reduced (deposited, cathode) while the dilute side's electrode oxidizes and dissolves further (anode).

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Apply | 1–2 concentration-cell potential calculations. |
| Group discussion | Analyze | Discuss why concentration cells eventually "run down" to E=0. |
| Quiz | Apply | One concentration-cell calculation. |
| Exam | Analyze | Require justifying the anode/cathode assignment before calculating. |
| Project/activity | Evaluate | Research how concentration cells relate to biological membrane potentials (e.g., nerve cells). |

## Objective 18.5a: Explain corrosion, electrolysis, and batteries

### Target understanding

A student can explain corrosion as a spontaneous electrochemical process, define electrolysis as using external energy to drive a nonspontaneous redox reaction, and identify common battery types as practical galvanic cells.

### Question guides

**1. Conceptual — corrosion as electrochemistry**
- Variables & ranges: rust formation on iron.
- Constraint: explanation must identify the oxidizing agent (O₂) and note the spontaneous (galvanic-like) nature.
- Contexts: iron corrosion, or another metal's corrosion.
- Formats: short-answer.
- Worked instantiation: "Explain why rust formation is considered an electrochemical process." → Iron is oxidized (loses electrons, forming $\ce{Fe^2+}$/$\ce{Fe^3+}$) while atmospheric $\ce{O2}$ is reduced, exactly the oxidation/reduction pairing of any redox reaction — it's spontaneous, like a galvanic cell, just occurring directly on the metal surface rather than in physically separated half-cells.

**2. Conceptual — electrolysis vs. galvanic cell**
- Variables & ranges: any electrolysis example (water, molten NaCl).
- Constraint: explanation must contrast spontaneous (galvanic) vs. nonspontaneous (electrolytic, energy-requiring) directions.
- Contexts: water electrolysis, molten salt electrolysis.
- Formats: short-answer.
- Worked instantiation: "How does electrolysis differ fundamentally from a galvanic cell, even though both involve redox reactions?" → A galvanic cell harnesses a *spontaneous* redox reaction to generate electricity; electrolysis does the reverse — it uses an external electrical energy source to *force* a nonspontaneous redox reaction to occur, such as decomposing water into $\ce{H2}$ and $\ce{O2}$ (the reverse of the spontaneous combustion reaction).

**3. Forward — classify battery types**
- Variables & ranges: named battery types (dry cell, lead storage, lithium-ion, fuel cell).
- Constraint: correct identification of each as a galvanic cell, with fuel cells distinguished by requiring continuous reactant supply.
- Contexts: common battery technologies.
- Formats: short-answer.
- Worked instantiation: "How does a fuel cell differ from a typical sealed battery like a AA alkaline cell, even though both are galvanic cells?" → A sealed battery contains a fixed, finite supply of reactants and eventually depletes them; a fuel cell requires a *continuous* external supply of reactants (e.g., $\ce{H2}$ and $\ce{O2}$) to keep functioning indefinitely, as long as fuel keeps flowing in.

**4. Error analysis**
- Variables & ranges: a student who claims a negative-E°cell reaction "cannot occur under any circumstances."
- Constraint: correction must introduce electrolysis as the resolution.
- Contexts: any nonspontaneous redox reaction.
- Formats: short-answer.
- Worked instantiation: "A student says water can never decompose into $\ce{H2}$ and $\ce{O2}$ because that reaction has a negative E°cell (nonspontaneous). What resolves this apparent contradiction?" → A negative $E^\circ_{cell}$ means the reaction won't happen *spontaneously*, but it can still be driven forward by supplying external electrical energy — this is precisely how electrolysis of water works, producing $\ce{H2}$ and $\ce{O2}$ despite the reaction being thermodynamically nonspontaneous on its own.

### Design guidance by purpose

| Purpose | Cognitive level | How to design the task |
|---|---|---|
| Homework | Understand | Explain corrosion and electrolysis conceptually; classify 3–4 battery types. |
| Group discussion | Analyze | Debate real-world corrosion-prevention strategies (galvanization, sacrificial anodes) in electrochemical terms. |
| Quiz | Understand | One corrosion or electrolysis explanation item. |
| Exam | Analyze | Require connecting a nonspontaneous E°cell to the necessity of electrolysis. |
| Project/activity | Evaluate | Research a real sacrificial-anode corrosion-protection system (e.g., on a ship hull) and explain its electrochemistry. |

## Rubric Themes for Chapter 18

| Evidence of mastery | What to look for |
|---|---|
| Cathode/anode selected by E° comparison, not intuition | Student explicitly compares E° values and never guesses based on "which metal seems more reactive." |
| Anode half-reaction explicitly reversed | Student visibly rewrites the anode's tabulated reduction as an oxidation before combining half-reactions. |
| Electron count (n) equalized and reused consistently | The same, correctly equalized n appears in the combined equation, ΔG°, K, and any Nernst-equation calculation. |
| E° vs. Nernst equation correctly distinguished | Student checks whether conditions are standard (1 M, 1 atm) before deciding which formula to use. |
| Nonspontaneous ≠ impossible | Student explains a negative E°cell using electrolysis as the resolution, not as evidence the reaction "can't happen." |
| ΔG°, K, and E° treated as one connected story | Student moves fluidly between the three quantities using ΔG° = −nFE° = −RT ln K, without treating them as unrelated topics. |
