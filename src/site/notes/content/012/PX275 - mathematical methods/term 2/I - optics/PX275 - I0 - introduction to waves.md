---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/i-optics/px-275-i0-introduction-to-waves/","noteIcon":"1","created":"2025-02-18T12:39:31.536+00:00","updated":"2025-02-18T22:30:02.559+00:00"}
---

- a stationary plane wave:
$$e^{\pm ikx}$$
	where, $k = 2\pi/\lambda$
$$\exp(\pm i(kx \pm \omega t))$$
	where, $\omega = kx$

- considering 1D plane waves:
$$u(x,t) = A\exp(\pm i(kx - \omega t)) = A\exp(\pm ik(x - ct))$$
- and 3D plane waves:
$$u(\vec r, t) = C \exp(\pm) i (\vec k \cdot \vec r \pm) \omega t$$
	where, $C$ is the complex amplitude
- the dispersion relation is given by:
$$\omega = |\vec k | c$$
## FT of a plane wave
- the FT:
$$\tilde u(k,\omega) = \iint_{-\infty}^{\infty} \exp(-i(kx+\omega t)) \,u(x,t) \, dx\, dt$$
- also, the inverse FT:
$$u(x,t) = \left(\frac{1}{2\pi}\right)^{2} \iint_{-\infty}^{\infty} \exp(i(kx+\omega t)) \, \tilde u(k,\omega) \, dk\, d\omega$$
- let $u(x,t) = A \exp(k'x - \omega't)$
- taking its FT:
$$\begin{align*}
\tilde u(k,\omega) &= \iint_{-\infty}^{\infty} \exp(-i(kx+\omega t)) \,A \exp(k'x - \omega't) \, dx\, dt \\
&= A \int_{-\infty}^{\infty} \exp(i(k'-k))\,dx \int_{-\infty}^{\infty}\exp(-i(\omega'+\omega)t)\,dt \\\\
\implies \tilde u(k,\omega) &\propto A \, \delta(k-k') \, \delta(\omega + \omega')
\end{align*}$$
- so, a pure plane wave with wave number, $k'$, and frequency, $\omega'$, maps to the product of delta functions in reciprocal space

- physical phenomena with wave-like properties:
	- surface waves on a fluid
	- pressure waves in a compressible fluid
	- optics: propagation, interference and diffraction of light waves
	- quantum mechanics wavefunction
	- wave-like properties of particles

