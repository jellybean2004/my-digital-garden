---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/j-photons/px-284-j2-statistical-mechanics-of-photons/","noteIcon":"1","created":"2025-08-27T13:15:24.748+01:00","updated":"2025-01-20T10:45:49.000+00:00"}
---

- the energy density:
$$u = \frac{U}{V} = \frac{1}{V} \int_{0}^{\infty}g(\omega) \langle{E(\omega)}\rangle \, d\omega$$

[[content/012/PX284 - SMETO/part 1 - statistical mechanics/H - gases/PX284 - H1 - density of states (DOS)\|PX284 - H1 - density of states (DOS)]]

$$g(k) \, dk = \frac{Vk^{2}}{2\pi^{2}} \, dk \times 2$$
- the factor of $2$ accounts for the two polarisations of light

- to convert to $\omega$, the dispersion relation is required
- for photons:
$$\omega  = ck$$
$$g(\omega) \, d\omega = \frac{V(\omega/c)^{2}}{2\pi^{2}} \, \frac{d\omega}{c} \times 2 = \frac{V\omega^{2}}{\pi^{2}c^{2}}\,d\omega$$
- modelling photons has simple harmonic oscillators with:
$$\varepsilon_{n} = \left(n + \frac{1}{2}\right) \hbar \omega$$
$$\langle{\varepsilon(\omega)}\rangle = U_{SHO} = \hbar\omega \left[ \frac{1}{2} + \frac{1}{\exp(\beta\hbar\omega)-1}\right]$$
- ignoring the ZPE:
$$u = \int_{0}^{\infty} \frac{\hbar}{\pi^{2}c^{3}} \frac{\omega^{3}}{\exp(\beta\hbar\omega)-1} \,d\omega \tag{1}$$

- using $\omega = 2\pi \nu$ and $\nu = c/\lambda:$
$$U_{\lambda} \,d\lambda = \frac{8\pi h c}{\lambda^{5}} \frac{1}{\exp(\beta h/\lambda)-1} \,d\lambda$$
- this is **planck's radiation distribution**

## consequences
- light is quantized into packets of $\hbar\omega$, giving birth to quantum mechanics

- **stefan-boltzmann** law: substituting $x = \beta\hbar\omega$ and $dx = \beta \hbar \, d\omega$ in equation $(1):$
$$u = \frac{\hbar}{\pi^{2}c^{3}} \left(\frac{1}{\hbar\beta}\right)^{4} \underbrace{\int_{0}^{\infty} \frac{x^{3}}{e^{x}-1} \,dx}_{\text{standard integral} = \pi^{4}}{15} = \frac{\pi^{2}k_{B}^{4}}{15c^{3}\hbar^{3}} T^{4}$$
$$\therefore u  = \frac{4\sigma}{c} T^{4}$$
	where, $\sigma$ is the stefan-boltzmann constant determined from experiments

- **wien's displacement law:** maximising $u_{\lambda} \implies \lambda_{max}T = 2.897$ mm K

- **planck's constant:** planck used the experimentally measured value of $\sigma$ and wien's law to evaluate $h$ and $k_{B}$
