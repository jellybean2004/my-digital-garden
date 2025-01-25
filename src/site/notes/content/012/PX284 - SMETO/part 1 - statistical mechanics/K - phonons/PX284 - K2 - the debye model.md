---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/k-phonons/px-284-k2-the-debye-model/","noteIcon":"1","created":"2025-01-23T15:33:31.697+00:00","updated":"2025-01-23T17:04:58.567+00:00"}
---

## assumptions
- lattice vibrations are waves with dispersion relation:
$$\omega = v_{s}q$$
	where, $v_{s}$ is the speed of sound, and $q$ is the wavevector

- thus, the DOS is given by:
$$g(q)\,dq = \frac{Vq^{2}}{2\pi^{2}} \, dq \times 3$$
- the factor of $3$ corresponds to three polarizations of vibration - 2 transverse and a longitudinal
$$g(\omega)\,d\omega = \frac{3V\omega^{2}}{2\pi^{2}v_{S}^{2}}\,d\omega$$
- debye also assumed a cut-off frequency, $\omega_{D}$, so as to enforce $3N$ modes
$$\begin{align*}
\int_{0}^{\omega_{D}} g(\omega)\, d\omega &= 3N \\
\frac{V\omega_{D}^{3}}{2\pi^{2} v_{s}^{3}} &= 3N \\
\omega_{D} &= \left(\frac{6N\pi^{2}v_{s}^{3}}{V}\right)^{1/3}\\
\text{or, } g(\omega)\, d\omega &= \frac{9N\omega^{2}}{\omega_{D}^{3}} d\omega
\end{align*}$$
- defining debye temperature, $\theta_{D} = \hbar\omega_{D}/k_{B}$

$$U = \int_{0}^{\omega_{D}} g(\omega) U_{SHO} \, d\omega$$

- ignoring ZPE:
$$U = \frac{9N\hbar}{\omega_{D}^{3}} \int_{0}^{\omega_{D}} \frac{\omega^{3}}{\exp(\beta\hbar\omega)-1} d\omega$$
$$C_{V}= \frac{9N\hbar}{\omega_{D}} \int_{0}^{x_{D}} \frac{x^{4}\exp(x)}{(\exp(x)-1)^{2}}\,dx$$
	where $x = \beta\hbar\omega$ and $x_{D} = \beta\hbar\omega_{D} = \theta_{D}/T$

- $T \to 0: x_{D} \to \infty$
- integral is standard $= 4\pi^{4}/15$
$$C_{V} = \frac{12\pi^{4}}{5} Nk_{B} \left(\frac{T}{\theta_{D}}\right)^{3}$$
- ie: $C_{V}\sim T^{4}$ at low temperatures

- $T \to \infty$ #incomplete 