---
{"dg-publish":true,"permalink":"/content/013/a-small-angle-scattering/a3-form-factor/","noteIcon":"1","created":"2025-08-15T07:51:16.989+01:00","updated":"2025-08-15T09:12:39.489+01:00"}
---

- assuming a homogenous particles (uniform electron density)
- each electron is a secondary wave source described as $a \exp(i\phi)$
- the amplitude, $a$, is the same for all electrons, but $\phi$ is position-dependent
- the resulting wave amplitude is:
$$A = \sum\limits_{i}a_{i}\exp(i \phi_{i})$$
- identical-phases are grouped together, all located at $\theta/2$

![A3 - form factor.png](/img/user/pics/A3%20-%20form%20factor.png)
*image: CJ Gommes, S Jakschb and S Frielinghausb (2021)*

- the scattered intensity:
$$I(q) = \left| \iiint_{particle} \exp(iqy) \rho  \,dx\,dy\,dz \right|^{2}$$
	where, $\rho$ is the electron density

- detectors measure intensity, not amplitude: $I = |A|^{2}$
- for small $q$, $\lambda^{*} =  2\pi/q \gg \lambda$, so all scattering centres scatter in phase
	- all arrows point in the same direction, maximising $I$
- for large $q$, $\lambda^{8} < \lambda$, so different parts of the particle scatter out of phase
	- arrows point in different directions, lowering $I$

- the transition from plateau (small ${} q$) to oscillatory decrease occurs where $2\pi/q  ~\sim \lambda$

- the **form factor** is the intensity scattered by an individual nanoparticle over a complete range of $q$
- customarily, the effect of $\rho$ and $V$ are factored out, so the form factor $P(q)$ is defined as:
$$I(q) = \rho^{2}V^{2} P(q)$$
- for small $q$, $P(q) = 1$
- this can be used to calculate the form factors of various spheres
- naturally particles are modelled as sphere of radius, $R$, with their form factors:
$$P(q) = \left[  3 \frac{\sin(qR) - qR\cos(qR)}{qR^{3}} \right]^{2}$$

![A3 - form factor-1.png](/img/user/pics/A3%20-%20form%20factor-1.png)
*image: CJ Gommes, S Jakschb and S Frielinghausb (2021)*

- for nonidentical nanoparticles, the conditions for constructive and destructive interference differ, giving rise to sharp oscillations
- the progressive onset of destructive interference for small $q$ obeys **guinier's law**:
$$P(q) \simeq \exp\left[- \frac{(qR_{G})^{2}}{3}\right]$$
	where, $R_{G}$ is the radius of gyration
- plotting $\ln[I(q)]$ against $q^{2}$ often yields a linear trend at low $q$, with slope $- R_{G}^{2}/3$
- obtained $R_{G}$ can be used for an intuitive understanding of particle size

- increasing $q$ beyond the validity limit of guinier's law leads to power laws of the type:
$$I \simeq q^{-\alpha}$$
![A3 - form factor-2.png](/img/user/pics/A3%20-%20form%20factor-2.png)
*image: CJ Gommes, S Jakschb and S Frielinghausb (2021)*

- the specific case of $\alpha = 4$ is **porod's law**, for structures with clear-cut interfaces
