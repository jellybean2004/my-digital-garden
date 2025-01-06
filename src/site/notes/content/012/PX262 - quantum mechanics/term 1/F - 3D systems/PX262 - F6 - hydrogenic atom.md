---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-1/f-3-d-systems/px-262-f6-hydrogenic-atom/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-15T14:14:36.543+00:00"}
---

- **hydrogen-like atoms** are systems with a **single electron in the coulomb potential** of the nucleus, eg: $He+$, $Li^{2+}$, etc.
- it is reasonable to state that the nucleus is much heavier than the electron, and its size is negligible compared to the distance to electrons, hence the nucleus can be assumed to be a point charge
- considering the case of a positively charged nucleus, where the potential is given by the atomic charge: 
  $$V(r) = - \frac{Ze^{2}}{4\pi\epsilon_{0}r}$$
	where, $r$ is the distance from the nucleus, and $Z$ is the atomic number
	
- solving the schrödinger equation for this potential, the angular part has already been solved, and the solution is: 
  $$\phi(r,\theta\,\varphi) = R(r)\, Y_{l,m} (\theta,\varphi)$$
- the radial equation after the transformation $\chi(r) = r\,R(r):$ 
  $$ -\frac{\hbar^{2}}{2m} \frac{d^{2}\chi}{d r^{2}} + \left[ - \frac{Ze^{2}}{4\pi\epsilon_{0}r} + \frac{l(l+1)\hbar^{2}}{2mr^{2}} \right] \chi = E\chi $$
- **note:** 
	- in the textbook, reduced mass $(\mu = \frac{m_{N}m_{e}}{m_{N}+m_{e}})$ is used instead of the electron mass
	- this is because both nucleus and electron will move under due to mutual attraction
	- since $m_{N}>>m_{e},\; \mu \approx m_{e} = m$
- defining a new variable: 
  $$\rho = \left(- \frac{8mE}{\hbar^{2}}\right)^{\frac{1}{2}} r$$
- so, the second derivative becomes: 
  $$\frac{d^{2}\chi}{dr^{2}}= - \frac{8mE}{\hbar^{2}} \frac{d^{2}\chi}{d\rho^{2}}$$
- and the radial equation becomes: 
  $$\frac{d^{2}\chi}{d\rho^{2}}- l(l+1) \frac{\chi}{\rho^{2}} + \left(\frac{\beta}{\rho} - \frac{1}{4}\right)\chi = 0 \tag{1}$$
	where, the constant $\beta$ is defined as: 
	$$\beta = \left(- \frac{m}{2E}\right)^{\frac{1}{2}} \frac{Ze^{2}}{4\pi\epsilon_{0}\hbar}$$
- the boundary conditions are: $\chi(0) = 0$, and $\chi(\infty) \to 0$
- similar to the harmonic oscillator, starting with the behaviour at large $\rho:$ 
  $$\frac{d^{2}\chi}{d\rho^{2}} = \frac{1}{4}\chi \implies \chi \sim \exp\left(-\frac{\rho}{2}\right)$$
- **note:** $\exp\left(\frac{\rho}{2}\right)$ is rejected as it tends to infinity at large $\rho$
- the trial solution is: 
  $$\chi(\rho) = F(\rho) \exp\left(- \frac{\rho}{2}\right)$$
	where, $F(\rho)$ is the function defining the details at small $\rho$

- substituting the trial solution into equation $(1):$ 
  $$\frac{d^{2}F}{d\rho} - \frac{dF}{d\rho} - \frac{l(l+1)}{\rho^{2}}F + \frac{\beta}{\rho}F = 0 \tag{2}$$
- $F$ can be written as a power series: 
  $$F(\rho) = \sum\limits_{p=1}^{\infty} a_{p}\rho^{p}$$
- $\chi$ must be zero at ${} \rho=0 {}$
- if the sum starts at $p=0$, $F$ and, hence, $\chi$ would not be zero at $\rho=0$
- therefore, it starts at $p=1$

- calculating the derivatives: 
$$\begin{align*}
	\frac{dF}{d\rho} &= \sum\limits_{p=1}^{\infty} p a_{p}\rho^{p-1} \\
	\frac{d^{2}F}{d\rho^{2}} &= \sum\limits_{p=1}^{\infty} p(p-1) a_{p}\rho^{p-2} \\
	&= \sum\limits_{p'=1}^{\infty} (p'+1)p' a_{p'+1}\rho^{p'-1}
\end{align*}$$
- here, $p'=p+1$ is just a dummy variable, and can be written as $p$
- also: 
  $$\frac{F}{\rho^{2}}= \sum\limits_{p=1}^{\infty} a_{p}\rho^{p-2} = a_{1}\rho^{-1} + \sum\limits_{p=1}^{\infty} a_{p+1}\rho^{p-1}$$
- substituting into equation $(2):$ 
  $$\sum\limits_{p=1}^{\infty} \bigg[ (p+1)pa_{p+1} - pa_{p} - l(l+1)a_{p+1} + \beta a_{p} \bigg]\rho^{p-1} - l(l+1) a_{1}\rho^{-1} = 0 $$
- coefficient of each power of $\rho$ must vanish, so: $a_{1}=0$ unless $l=0$, and: 
  $$\frac{a_{p+1}}{a_{p}}= \frac{p-\beta}{p(p+1) - l(l+1)}$$
-  **notes**:
	- this tends to $\frac{1}{p}$ as $p\to\infty$
	- the $RHS$ denominator is zero if $p=l$, which means that  for $p>l, \; a_{p}=\infty$, unless $a_{l}=0$
	- but if $a_{l}=0$, ${} a_{p}$ for $p<l$ must also be zero
	- therefore, to represent a physically realistic wavefunction, $a_{p}=0$ for $p\leq l$

- the full power series with an infinite number of terms diverges like $\exp(\rho)$
- if $\chi = \exp(\rho) \exp\left(- \frac{\rho}{2}\right) = \exp(\frac{\rho}{2})$,  the wavefunction cannot be normalized as it diverges for large $\rho$
- therefore, the power series needs to be cut off somewhere
- fixing $\beta$ such that at some point, $a_{p+1}$ becomes zero
- suppose, it is fixed at $\beta=n>l$, the expressions for discrete energy levels of the hydrogen-like atom is found: 
  $$E_{n}= - \frac{mZ^{2}e^{4}}{2(4\pi\epsilon_{0})^{2}\hbar^{2}n^{2}}$$
- **note:** this is independent of the quantum numbers $m$ and $l$ ($m$ in the equation is the electron mass)
- after working through constants, it is found that the energy levels agree with the experimentally obtained energy levels for hydrogen: 
  $$E_{n}= -2\pi \hbar c R_{0} \frac{1}{n^{2}}$$
	where, $n\in Z > 0$, and $R_{0}$ is the rydberg constant

- the function $F$ starts at ${} l+1$ and terminates at $n:$ 
  $$F_{n}(\rho) = \sum\limits_{p=l+1}^{n} a_{p}\rho^{p}$$
- the wavefunction: 
  $$\phi_{nlm} = R_{nl}Y_{lm}(\theta,\varphi) = F_{nl}(\rho) \exp\left(- \frac{\rho}{2}\right) Y_{lm}(\theta,\varphi)$$
	where, $Y_{lm}$ are **the spherical harmonics**, and $F_{nl}$ are **the laguerre polynomials**

- the wavefunctions of the first five lowest states determined are:
$$
\begin{align}
\phi_{1,0,0} &= \left( \frac{Z^3}{\pi a_0^3} \right)^{1/2} \exp\left( -\frac{Zr}{a_0} \right), \\
\phi_{2,0,0} &= \left( \frac{Z^3}{8\pi a_0^3} \right)^{1/2} \left( 1 - \frac{Zr}{2a_0} \right) \exp\left( -\frac{Zr}{2a_0} \right), \\
\phi_{2,1,0} &= \left( \frac{Z^3}{32\pi a_0^3} \right)^{1/2} \frac{Zr}{a_0} \cos\theta \exp\left( -\frac{Zr}{2a_0} \right), \\
\phi_{2,1,\pm 1} &= \pm \left( \frac{Z^3}{\pi a_0^3} \right)^{1/2} \frac{Zr}{8a_0} \sin\theta \exp(\pm i\varphi) \exp\left( -\frac{Zr}{2a_0} \right).
\end{align}
$$
- $a_0$ is called the **bohr radius**:
$$a_0 = \frac{4\pi \epsilon_0 \hbar^2}{\mu e^2} = 0.5291766 \times 10^{-10} \, \text{m}$$
