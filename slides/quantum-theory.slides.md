{{nyml
kind: document
carrier: slides
uid: doc-ku88yqgmzw93kjm0
title: Chapter 7: The Electronic Structure of Atoms
ratio: 16:9
theme: paper
}}

<!-- slide template=title -->
# The Electronic Structure of Atoms
## Building the electron's address
**General Chemistry, Chapter 7**

<!-- slide 2col -->
## Chapter Learning Objectives
<!-- @left -->
- **Objective 7.1a** — Relate wave speed, wavelength, and frequency
- **Objective 7.1b** — Calculate photon energy
- **Objective 7.1c** — Apply the photoelectric effect equation
- **Objective 7.2a** — Apply Bohr's theory to hydrogen's energy levels and emission spectrum
<!-- @right -->
- **Objective 7.2b** — Calculate an electron's de Broglie wavelength
- **Objective 7.3a** — Identify valid quantum-number sets and orbital shapes/energies
- **Objective 7.3b** — Write ground-state electron configurations
- **Objective 7.3c** — Use noble-gas-core notation and recognize transition-metal exceptions

<!-- slide template=outline -->
## Roadmap
1. Waves and photons
2. Bohr's theory and the dual nature of the electron
3. Electrons in atoms

<!-- slide -->
## Chapter Logic
{{mermaid
graph TD
  A["Waves and photons:<br/>E = hv, c = wavelength times v"] --> B["Bohr's model:<br/>quantized energy levels, emission spectra"]
  B --> C["Quantum numbers:<br/>n, l, m_l, m_s describe each electron"]
  C --> D["Electron configuration:<br/>Aufbau, Hund's rule, Pauli exclusion"]
}}
**Visual description:** waves and photons establish light is quantized; Bohr's model quantizes atomic energy levels; quantum numbers describe each orbital fully; electron configuration fills orbitals for real atoms.

<!-- slide template=section -->
# 1. Waves and Photons

<!-- slide -->
## Wave properties
$$u=\lambda\nu \qquad c=\lambda\nu\ (\text{light})$$
![EM spectrum](../assets/em_spectrum_ladder.svg =620x)

<!-- slide step -->
## Worked example — frequency and wavelength
(a) 400 nm light; (b) 5.75×10¹⁴ Hz
- $\nu=c/\lambda=7.50\times10^{14}$ Hz{{attrs[.fragment]}}
- $\lambda=c/\nu=522$ nm{{attrs[.fragment]}}

<!-- slide -->
## Photon energy
$$E=h\nu=\frac{hc}{\lambda} \qquad h=6.63\times10^{-34}\,\text{J·s}$$

<!-- slide step -->
## Worked example — photon energy
500 nm photon
- $E=hc/\lambda$ {{attrs[.fragment]}}
- **= 3.98×10⁻¹⁹ J**{{attrs[.fragment]}}

<!-- slide -->
## The photoelectric effect: what breaks the wave picture
![Threshold frequency and the KE plot](../assets/photoelectric_effect.svg =820x)
Brighter light below the threshold frequency ejects **nothing** — one photon, one electron

<!-- slide -->
## The photoelectric effect
$$E=h\nu=KE+W$$
$W$ = work function (energy to free the electron); excess becomes kinetic energy

<!-- slide template=section -->
# 2. Bohr's Theory and the Dual Nature of the Electron

<!-- slide -->
## Bohr's model
$$E_n=-R_H\left(\frac{1}{n^2}\right) \qquad \Delta E=h\nu=R_H\left(\frac{1}{n_i^2}-\frac{1}{n_f^2}\right)$$
![Bohr energy levels](../assets/bohr_energy_levels.svg =440x)

<!-- slide -->
## A real emission spectrum
![Hydrogen lamp](../assets/hydrogen_lamp.jpg =300x)
Exciting hydrogen produces its characteristic line emission spectrum

<!-- slide step -->
## Worked example — emission wavelength
$n_i=5\to n_f=2$
- $\Delta E=R_H(1/25-1/4)=-4.58\times10^{-19}$ J{{attrs[.fragment]}}
- **λ = 434 nm**{{attrs[.fragment]}}

<!-- slide -->
## Why the energies are quantized
![Standing waves on an orbit](../assets/standing_wave_orbit.svg =800x)
A wave on a closed loop must join up with itself: $2\pi r = n\lambda$, with $n$ a whole number

<!-- slide -->
## De Broglie: matter waves
$$\lambda=\frac{h}{mu} \qquad 2\pi r=n\lambda\ (\text{standing wave condition})$$

<!-- slide step -->
## Worked example — electron wavelength
68 m/s, mass 9.11×10⁻³¹ kg
- $\lambda=h/(mu)$ {{attrs[.fragment]}}
- **= 1.1×10⁻⁵ m**{{attrs[.fragment]}}

<!-- slide -->
## Quantum mechanics
:::warning
Heisenberg uncertainty principle: position and momentum cannot both be known with certainty. Quantum mechanics describes electron density ($\psi^2$), not a definite orbit.
:::

<!-- slide template=section -->
# 3. Electrons in Atoms

<!-- slide -->
## An orbital is not an orbit
![Bohr orbit vs probability cloud](../assets/orbit_vs_orbital.svg =800x)
The correction Chapter 2 promised: no path, no position — only a probability distribution

<!-- slide -->
## The four quantum numbers
- $n$ (principal): energy/size
- $l$ (angular momentum): shape (s,p,d,f)
- $m_l$ (magnetic): orientation
- $m_s$ (spin): ±½

<!-- slide -->
## Orbital shapes
![Orbital shapes](../assets/orbital_shapes.svg =560x)

<!-- slide step -->
## Worked example — quantum numbers for 3p
$n=3, l=1, m_l\in\{-1,0,1\}, m_s=\pm\tfrac12$
**6 possible combinations**{{attrs[.fragment]}}

<!-- slide -->
## The diagonal rule
![Aufbau filling order](../assets/aufbau_diagonal_rule.svg =800x)
Read the arrows and the order builds itself — note $4s$ before $3d$

<!-- slide -->
## Building the first ten elements
![Orbital boxes H to Ne](../assets/orbital_filling_h_to_ne.svg =820x)
Pauli forces opposite spins in a shared box · Hund keeps them apart until it cannot

<!-- slide -->
## Filling rules
- Aufbau: fill lowest-energy orbitals first
- Pauli exclusion: no 2 electrons share all 4 quantum numbers
- Hund's rule: fill degenerate orbitals singly before pairing

<!-- slide step -->
## Worked example — max electrons at n=3
$l=0,1,2$ → 1+3+5 = 9 orbitals
- ×2 electrons each{{attrs[.fragment]}}
- **= 18 = 2n²**{{attrs[.fragment]}}

<!-- slide -->
## Exceptions: Cr and Cu
- Cr: $[Ar]4s^13d^5$ (not $4s^23d^4$)
- Cu: $[Ar]4s^13d^{10}$ (not $4s^23d^9$)
- Extra stability of half-filled/filled $3d$

<!-- slide template=closing -->
# From light to electron configuration
Wave-particle duality shows light and matter both have wave and particle properties; Bohr's model quantizes atomic energy; quantum numbers give every orbital a full three-dimensional description; and the Aufbau/Hund/Pauli rules build up the electron configuration of most atoms — the direct foundation for periodic trends (Ch. 8) and bonding theory (Ch. 9).
