---
{"dg-publish":true,"permalink":"/content/012/px-282-stars-and-solar-system/term-2-solar-system/i-planetary-motion/px-282-i3-newtons-laws/","noteIcon":"1","created":"2025-01-17T11:32:26.304+00:00","updated":"2025-01-17T11:51:50.705+00:00"}
---

- newton (1687) used [[content/012/PX282 - stars and solar system/term 2 - solar system/I - planetary motion/PX282 - I2 - kepler's laws\|kepler's laws]] to infer the **law of universal gravitation**

- simplified derivation using circular orbits
$$\begin{gather}
P^{2} = kr^{3} \\
P=2\pi \frac{r}{v} \\\\
\implies 4\pi^{2} \frac{r^{2}}{v^{2}} = kr^{3}   \\
\therefore a = \frac{v^{2}}{r} = \frac{4\pi^{2}}{k}
\end{gather}$$
- using [[content/012/PX285 - hamiltonian mechanics & fluid dynamics/term 1 - hamiltonian mechanics/C - calculus of variations/PX285 - C3 - newton's second law\|newton's second law]]:
$$F = ma = \frac{mv^{2}}{r} = \frac{4\pi ^{2}m}{kr^{2}}$$
- using [[content/011/PX155 - classical mechanics and special relativity/classical mechanics/PX155 - A - foundations of classical mechanics/PX155 - A3 - newton's third law\|PX155 - A3 - newton's third law]]:
$$F = \frac{4\pi ^{2}m}{kr^{2}} = \frac{4\pi ^{2}M}{k'r^{2}}$$
	where, $m$ is the mass of the planet, and $M$ is the mass of the sun
- **note:** the sun moving is inconsistent with kepler's laws, where the sun is fixed on a focus of the ellipse 
$$kM = k'M = k''$$
$$F = \frac{4\pi^{2}Mm}{k''r^{2}}$$
- defining ${} G = 4\pi^{2}/k'' {}$, the gravitational constant:
$$\therefore F = \frac{GMm}{r^{2}}$$
- newton was able to derive all three of kepler's laws using this law of universal gravitation (see [chapter 2, Carroll & Ostile, 2007])

- the constant in kepler's third law, assuming ${} M\gg m: {}$
$$k = \frac{k''}{M} = \frac{4\pi^{2}}{GM} \implies P^{2}  = \frac{4\pi^{2}}{GM} a^{3}$$
- this is called the **one body problem**

- kepler's third law widely used to obtain the masses of astronomical objects

- eg: 
	- for the mass of the sun: $P = 1$ yr, $a=1$ AU $\implies M_{\odot} = 1.99\times10^{30}$ kg 
	- the mass of jupiter from its moons
	- blackholes in galaxies
