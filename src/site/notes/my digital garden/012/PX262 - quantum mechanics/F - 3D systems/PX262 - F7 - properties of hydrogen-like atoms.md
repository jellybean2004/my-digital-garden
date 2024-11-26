---
{"dg-publish":true,"permalink":"/my-digital-garden/012/px-262-quantum-mechanics/f-3-d-systems/px-262-f7-properties-of-hydrogen-like-atoms/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T01:08:31.595+00:00"}
---

- the solution the schrödinger equations for a single electron in coulomb potential is: 
  $$\phi_{nlm} = R_{nl}(r) \,Y_{lm}(\theta,\varphi)$$
- three quantum numbers are needed to label the states:
	- the main quantum number: $n\in \mathbb{Z}>0$
	- the orbital quantum number: $l \in \mathbb{Z} \geq 0$
	- the magnetic quantum number: $m \in [-l,l]$
- the energies if individual eigenstates: 
  $$E_{1} = - \frac{me^{4}}{2(4\pi\epsilon_{0})^{2}\hbar^{2}} = - \frac{me^{4}c^{2}}{2(4\pi\epsilon_{0})^{2}\hbar^{2}c^{2}}$$
- defining the fine structure constant:
  $$\alpha = \frac{e^{2}}{4\pi\epsilon_{0}\hbar c^{2}} = \frac{1}{137}$$
- the energy level becomes: 
  $$E_{1} = - \frac{mc^{2}\alpha^{2}}{2} = -13.6\,eV$$
- **note:** the energy is negative as the electron is bound inside the atom
- the energies for other states: 
  $$E_{n} = E_{1} \frac{1}{n^{2}}$$
- states get closer in energy as $n$ increases, but they will always stay negative
- for atoms other than hydrogen the energy scales by $Z^{2}$
- to determine the  number of states: 
	- if $n=1$, $l=0$, and there is only a single state
	- if $n=2$, $l= \{0,1\}$, ${} m_{l=0}=\{0\}, \; m_{l=1}=\{-1,0,1\} {}$
- for a given $l$, there are $2l+1$ states
- an often used notation for orbital quantum numbers, $l=0,1,2,3\dots$ is $s,\;p,\;d,\;f\dots$
- the notation for states:
	- $1s \Leftrightarrow n=1,l=0$ 
	- $2p \Leftrightarrow n=2,l=1$ 

- **comment:** $l<n$ is not a general requirement, and it depends on the potential and there are systems in which it does not hold, eg: spherically symmetric potential wells
## shape wavefunctions
- it was found that:
	- the angular part are described by the spherical harmonics: $Y_{lm}(\theta,\varphi)$
	- the radial parts are described by the laguerre polynomials: $R_{nl}(r) = F_{nl}(\rho) \exp(- \frac{\rho}{2})$
- the probability of finding the particle: 
  $$P(r) = \int_{0}^{2\pi}\int_{0}^{\pi} \phi^{2}_{nlm} r^{2}\sin\theta\,d\theta\,d\varphi$$
- this can be solved numerically
