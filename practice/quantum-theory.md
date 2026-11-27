{{nyml
kind: document
format: 1
title: Chapter 7 Practice: The Electronic Structure of Atoms
}}

# Chapter 7 Practice: The Electronic Structure of Atoms

*Auto-generated from the assessment guide (`assessment-support/quantum-theory.md`), grouped by objective. 25 questions spanning multiple-choice, short-answer, and workout formats. Within each objective the questions run from easier to harder.*

:::: tabs
::: tab Q 1
{{sp[info] Objective 7.1a}} · *multiple-choice* If two light waves travel at the same speed and one has a longer wavelength, that wave has

A. a higher frequency\
B. a lower frequency\
C. the same frequency\
D. a larger amplitude
:::
::: tab Answer
**B.** Since $c=\lambda\nu$ is fixed, wavelength and frequency trade off inversely. Amplitude is independent of both.
:::
::::

:::: tabs
::: tab Q 2
{{sp[info] Objective 7.1a}} · *workout* Calculate the frequency of light with a wavelength of 650 nm.
:::
::: tab Answer
$$\nu=\frac{c}{\lambda}=\frac{3.00\times10^8\,\text{m/s}}{650\times10^{-9}\,\text{m}}=4.62\times10^{14}\ \text{Hz}$$

650 nm is red light, at the long-wavelength end of the visible range.
:::
::::

:::: tabs
::: tab Q 3
{{sp[info] Objective 7.1a}} · *workout* A microwave oven operates at 2.45 GHz. What is the wavelength, in centimeters?
:::
::: tab Answer
$2.45$ GHz $= 2.45\times10^9$ Hz.

$$\lambda=\frac{c}{\nu}=\frac{3.00\times10^8}{2.45\times10^9}=0.122\ \text{m}=12.2\ \text{cm}$$

Centimeter-scale, which is what puts it in the microwave region of Figure 7.1.
:::
::::

:::: tabs
::: tab Q 4
{{sp[info] Objective 7.1b}} · *workout* Calculate the energy of a single photon of 425 nm light.
:::
::: tab Answer
$$E=\frac{hc}{\lambda}=\frac{(6.63\times10^{-34})(3.00\times10^8)}{425\times10^{-9}}=4.68\times10^{-19}\ \text{J}$$
:::
::::

:::: tabs
::: tab Q 5
{{sp[info] Objective 7.1b}} · *workout* Which carries more energy per photon: infrared light at 1200 nm or ultraviolet at 300 nm? By what factor?
:::
::: tab Answer
Since $E = hc/\lambda$, energy is inversely proportional to wavelength — so the *shorter* wavelength carries more.

**Ultraviolet carries more**, by the ratio of the wavelengths:

$$\frac{E_{300}}{E_{1200}}=\frac{1200}{300}=4$$

**Four times as much per photon.** No calculation of the individual energies is needed; only the ratio matters.
:::
::::

:::: tabs
::: tab Q 6
{{sp[info] Objective 7.1b}} · *workout* What is the energy of one mole of photons of 700 nm light, in kJ/mol?
:::
::: tab Answer
Energy of one photon first:

$$E=\frac{(6.63\times10^{-34})(3.00\times10^8)}{700\times10^{-9}}=2.84\times10^{-19}\ \text{J}$$

Then Avogadro's number of them:

$$E_\text{mol}=(2.84\times10^{-19})(6.022\times10^{23})=1.71\times10^5\ \text{J/mol}=171\ \text{kJ/mol}$$

Well below a typical 400 kJ/mol bond energy, which is why red light does not break most chemical bonds.
:::
::::

:::: tabs
::: tab Q 7
{{sp[info] Objective 7.1c}} · *short answer* A metal is illuminated with light below its threshold frequency. What happens if the light is made ten times brighter?
:::
::: tab Answer
**Still nothing.** No electrons are ejected at all.

Brighter light means *more photons per second*, not more energetic photons. Each individual photon still carries $h\nu < W$, and since one photon ejects one electron, none of them can pay the price. Only raising the **frequency** helps.

This is precisely the observation a wave theory of light cannot explain, and it is why photons had to be introduced.
:::
::::

:::: tabs
::: tab Q 8
{{sp[info] Objective 7.1c}} · *workout* A metal has a work function of $4.50\times10^{-19}$ J. Calculate its threshold frequency and the longest wavelength of light that will eject electrons.
:::
::: tab Answer
At the threshold, all the photon's energy goes into freeing the electron and none into kinetic energy:

$$\nu_0=\frac{W}{h}=\frac{4.50\times10^{-19}}{6.63\times10^{-34}}=6.79\times10^{14}\ \text{Hz}$$
$$\lambda_0=\frac{c}{\nu_0}=\frac{3.00\times10^8}{6.79\times10^{14}}=4.42\times10^{-7}\,\text{m}=442\ \text{nm}$$

**Longest** wavelength, because longer wavelength means lower energy — anything above 442 nm has photons too weak to work.
:::
::::

:::: tabs
::: tab Q 9
{{sp[info] Objective 7.1c}} · *workout* Light of wavelength 350 nm strikes a metal whose work function is $3.00\times10^{-19}$ J. Find the kinetic energy of the ejected electrons.
:::
::: tab Answer
Photon energy first:

$$E=\frac{hc}{\lambda}=\frac{(6.63\times10^{-34})(3.00\times10^8)}{350\times10^{-9}}=5.68\times10^{-19}\ \text{J}$$

Then subtract the price of escape:

$$KE=h\nu-W=5.68\times10^{-19}-3.00\times10^{-19}=2.68\times10^{-19}\ \text{J}$$

Positive, so ejection does occur. A negative result would have meant the photon was below threshold and nothing happens.
:::
::::

:::: tabs
::: tab Q 10
{{sp[info] Objective 7.2a}} · *short answer* Why is hydrogen's emission spectrum a set of sharp lines rather than a continuous rainbow?
:::
::: tab Answer
Because the atom's energies are **quantized**. The electron may occupy only certain levels, so only certain *gaps* between levels exist.

An emitted photon carries exactly the energy of one gap, and $E=h\nu$ converts that into exactly one frequency. A discrete set of gaps therefore produces a discrete set of lines.

A continuous spectrum would require a continuous range of allowed energies — which is what classical physics predicted and what is not observed.
:::
::::

:::: tabs
::: tab Q 11
{{sp[info] Objective 7.2a}} · *workout* Calculate the energy of the photon emitted when a hydrogen electron falls from $n=4$ to $n=2$ ($R_H = 2.18\times10^{-18}$ J).
:::
::: tab Answer
$$\Delta E=R_H\left(\frac{1}{n_i^2}-\frac{1}{n_f^2}\right)=2.18\times10^{-18}\left(\frac{1}{16}-\frac{1}{4}\right)=2.18\times10^{-18}(-0.1875)=-4.09\times10^{-19}\ \text{J}$$

The negative sign confirms emission. The photon carries $4.09\times10^{-19}$ J.
:::
::::

:::: tabs
::: tab Q 12
{{sp[info] Objective 7.2a}} · *workout* Find the wavelength, in nanometers, of the photon emitted in the $n=3 \to n=2$ transition of hydrogen.
:::
::: tab Answer
$$\Delta E=2.18\times10^{-18}\left(\frac{1}{9}-\frac{1}{4}\right)=2.18\times10^{-18}(-0.1389)=-3.03\times10^{-19}\ \text{J}$$
$$\lambda=\frac{hc}{|\Delta E|}=\frac{(6.63\times10^{-34})(3.00\times10^8)}{3.03\times10^{-19}}=6.57\times10^{-7}\,\text{m}=657\ \text{nm}$$

657 nm is red — this is the bright red line that dominates hydrogen's visible spectrum.
:::
::::

:::: tabs
::: tab Q 13
{{sp[info] Objective 7.2a}} · *short answer* Is more energy required to move an electron from $n=1$ to $n=2$, or from $n=4$ to $n=5$? Explain without calculating.
:::
::: tab Answer
**From $n=1$ to $n=2$, by a large margin.**

The allowed energies go as $-R_H/n^2$, so the levels are widely spaced at small $n$ and crowd together as $n$ grows. The gap from 1 to 2 is the largest in the whole atom; the gap from 4 to 5 is small.

This is why the ground state is so stable, and why ionizing an atom from its ground state costs far more than ionizing an already-excited one.
:::
::::

:::: tabs
::: tab Q 14
{{sp[info] Objective 7.2b}} · *workout* Calculate the de Broglie wavelength of an electron ($m = 9.11\times10^{-31}$ kg) moving at $2.50\times10^6$ m/s.
:::
::: tab Answer
$$\lambda=\frac{h}{mu}=\frac{6.63\times10^{-34}}{(9.11\times10^{-31})(2.50\times10^6)}=2.91\times10^{-10}\ \text{m}$$

About 0.29 nm — comparable to the size of an atom, which is why electron waves matter inside atoms.
:::
::::

:::: tabs
::: tab Q 15
{{sp[info] Objective 7.2b}} · *workout* Calculate the de Broglie wavelength of a 0.0459 kg golf ball moving at 30.0 m/s, and explain why golf balls do not show observable wave behavior.
:::
::: tab Answer
$$\lambda=\frac{6.63\times10^{-34}}{(0.0459)(30.0)}=4.81\times10^{-34}\ \text{m}$$

That is about $10^{-34}$ m, roughly nineteen orders of magnitude smaller than an atomic nucleus. No experiment could ever resolve a wave that small.

Wave-particle duality applies to the golf ball exactly as it does to the electron. The difference is almost entirely one of mass: $\lambda = h/mu$ puts $m$ in the denominator, and Planck's constant is so small that any macroscopic mass drives the wavelength below detectability.
:::
::::

:::: tabs
::: tab Q 16
{{sp[info] Objective 7.3a}} · *multiple-choice* For $n=4$, the allowed values of $l$ are

A. 1, 2, 3, 4\
B. 0, 1, 2, 3\
C. 0, 1, 2, 3, 4\
D. −4 through +4
:::
::: tab Answer
**B.** $l$ runs from 0 to $n-1$, so $n=4$ gives 0, 1, 2, 3 — the $4s$, $4p$, $4d$, and $4f$ subshells.
:::
::::

:::: tabs
::: tab Q 17
{{sp[info] Objective 7.3a}} · *short answer* Which of these sets of quantum numbers are impossible, and why? (a) $(3,3,0,+\tfrac12)$; (b) $(2,1,+2,-\tfrac12)$; \(c) $(5,2,-2,+\tfrac12)$.
:::
::: tab Answer
**(a) Impossible.** $l$ must be less than $n$, so with $n=3$ the largest allowed $l$ is 2. There is no $3f$ orbital.

**(b) Impossible.** $m_l$ must lie between $-l$ and $+l$. With $l=1$, only $-1$, 0, $+1$ are allowed.

**\(c) Valid.** $n=5$, $l=2$ is a $5d$ orbital, $m_l=-2$ is within range, and the spin is legal.

Check in order — $l$ against $n$, then $m_l$ against $l$ — because each constraint depends on the one before it.
:::
::::

:::: tabs
::: tab Q 18
{{sp[info] Objective 7.3a}} · *workout* How many orbitals are in the $n=4$ shell, and what is its maximum electron capacity?
:::
::: tab Answer
$n=4$ allows $l = 0, 1, 2, 3$. Each subshell holds $2l+1$ orbitals:

$$1 + 3 + 5 + 7 = 16\ \text{orbitals}$$

Each orbital holds 2 electrons, so the capacity is $16\times2 = 32$.

Check against $2n^2 = 2(4)^2 = 32$. ✓
:::
::::

:::: tabs
::: tab Q 19
{{sp[info] Objective 7.3a}} · *short answer* Explain why $4s$ fills before $3d$, even though 4 is larger than 3.
:::
::: tab Answer
In a hydrogen atom it would not — with one electron, energy depends only on $n$, so all $n=3$ subshells sit below all $n=4$ subshells.

In every other atom, the inner electrons **screen** the nucleus, and they screen the different subshell shapes unevenly. An $s$ orbital penetrates closer to the nucleus than a $d$ orbital of similar size, so it feels more of the nuclear charge and is pulled lower in energy. For $4s$ against $3d$, that penetration effect is just large enough to reverse the order.

The diagonal rule captures the result: $n+l$ for $4s$ is 4, while for $3d$ it is 5, and lower $n+l$ fills first.
:::
::::

:::: tabs
::: tab Q 20
{{sp[info] Objective 7.3b}} · *workout* Write the full ground-state electron configuration of phosphorus ($Z=15$) and state its number of unpaired electrons.
:::
::: tab Answer
Fifteen electrons in Aufbau order:

$$1s^2\,2s^2\,2p^6\,3s^2\,3p^3$$

Check the total: $2+2+6+2+3 = 15$. ✓

The three $3p$ electrons go into the three separate $3p$ orbitals with parallel spins, by Hund's rule:

$$3p\ [\uparrow][\uparrow][\uparrow]$$

**Three unpaired electrons**, so phosphorus is paramagnetic.
:::
::::

:::: tabs
::: tab Q 21
{{sp[info] Objective 7.3b}} · *short answer* Draw the orbital-box diagram for the $2p$ subshell of oxygen and explain why it is not $[\uparrow\downarrow][\uparrow\downarrow][\ \ ]$.
:::
::: tab Answer
Oxygen is $1s^22s^22p^4$, so four electrons occupy the three $2p$ orbitals:

$$2p\ [\uparrow\downarrow][\uparrow][\uparrow]$$

The arrangement $[\uparrow\downarrow][\uparrow\downarrow][\ \ ]$ is wrong because it violates **Hund's rule**: electrons in orbitals of equal energy occupy separate orbitals with parallel spins before any pairing begins. Pairing forces two electrons into the same region of space, which costs energy through their mutual repulsion, so it is avoided until unavoidable.

Both arrangements obey the Pauli principle. Hund's rule is what selects between them, and only the correct one predicts oxygen's two unpaired electrons — which makes an isolated oxygen atom paramagnetic.
:::
::::

:::: tabs
::: tab Q 22
{{sp[info] Objective 7.3b}} · *short answer* Which of these is paramagnetic: Mg ($Z=12$), Si ($Z=14$), Ar ($Z=18$)?
:::
::: tab Answer
Write each configuration and look only at the outermost incomplete subshell.

- **Mg** $= 1s^22s^22p^63s^2$. The $3s$ is full and paired. **Diamagnetic.**
- **Si** $= 1s^22s^22p^63s^23p^2$. Two electrons in three $3p$ orbitals go singly, by Hund's rule: two unpaired. **Paramagnetic.**
- **Ar** $= 1s^22s^22p^63s^23p^6$. Everything is full and paired. **Diamagnetic.**

Only silicon. A filled subshell can never have unpaired electrons, so noble gases and group 2 elements (whose occupied subshells are all filled) are always diamagnetic.
:::
::::

:::: tabs
::: tab Q 23
{{sp[info] Objective 7.3c}} · *workout* Write the noble-gas-core configuration for (a) bromine ($Z=35$) and (b) strontium ($Z=38$).
:::
::: tab Answer
**(a) Bromine.** The preceding noble gas is argon ($Z=18$), leaving $35-18 = 17$ electrons. In filling order, $4s$ then $3d$ then $4p$:

$$[\ce{Ar}]4s^23d^{10}4p^5$$

Check: $2+10+5 = 17$. ✓

**(b) Strontium.** Krypton ($Z=36$) is the preceding noble gas, leaving 2:

$$[\ce{Kr}]5s^2$$

Note that strontium ends in $s^2$, exactly like calcium's $[\ce{Ar}]4s^2$ — which is why both are Group 2A metals forming $+2$ ions.
:::
::::

:::: tabs
::: tab Q 24
{{sp[info] Objective 7.3c}} · *short answer* The expected configuration of chromium ($Z=24$) is $[\ce{Ar}]4s^23d^4$, but the actual one is $[\ce{Ar}]4s^13d^5$. Explain, and name the only other first-row transition-metal exception.
:::
::: tab Answer
A **half-filled** $3d$ subshell ($3d^5$, one electron in each of the five orbitals with parallel spins) carries extra stability. The $4s$ and $3d$ energies are close enough in chromium that promoting one $4s$ electron into $3d$ costs less than the stability it gains.

The other exception is **copper** ($Z=29$), which is $[\ce{Ar}]4s^13d^{10}$ rather than $[\ce{Ar}]4s^23d^9$ — this time for the extra stability of a **completely filled** $3d$ subshell.

These two are the only first-row transition-metal exceptions expected in general chemistry. Every other element in the row follows the plain Aufbau order.
:::
::::

:::: tabs
::: tab Q 25
{{sp[info] Objective 7.3c}} · *short answer* Sodium is $[\ce{Ne}]3s^1$ and potassium is $[\ce{Ar}]4s^1$. Use this to explain why they appear in the same column of the periodic table and form the same ion.
:::
::: tab Answer
Both end in a single $s$ electron outside a noble-gas core. That outermost electron is the only one available for chemistry, so the two elements behave almost identically: each loses that one electron easily to reach a noble-gas configuration, giving $\ce{Na+}$ and $\ce{K+}$.

**Group membership is a statement about valence configuration.** Every Group 1A element is $[\text{core}]ns^1$, every Group 2A element is $[\text{core}]ns^2$, and so on — which is the reason Chapter 2 could promise that elements in a column behave alike, and the reason it had to defer the explanation to this chapter.
:::
::::
