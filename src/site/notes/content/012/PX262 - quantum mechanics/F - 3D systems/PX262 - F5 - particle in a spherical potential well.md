---
dg-publish: true
---

- considering that the particle is bound to be within a sphere, the potential energy would be: 
$$V(r) = \begin{cases} 0 & r\leq a \\ \infty & r>a \end{cases}$$
- the radial schrödinger equation: 
  $$ -\frac{\hbar^{2}}{2m} \frac{d^{2}\chi}{d r^{2}} + \left[V(r) + \frac{\hbar^{2}}{2mr^{2}} l(l+1)\right] \chi = E\chi $$
- solving it for this potential: 
  $$ -\frac{\hbar^{2}}{2m} \frac{d^{2}\chi}{d r^{2}} + \frac{\hbar^{2}}{2mr^{2}} l(l+1)\chi = E\chi $$
- setting a constant: $E = \frac{\hbar^{2}k^{2}}{2m}$, and transforming: $x = kr:$ 
  $$\frac{d^{2}R(x)}{dx^{2}} + \frac{2}{x} \frac{dR(x)}{dx} + \left[ 1 - \frac{l(l+1)}{x^{2}} \right] R(x) = 0$$
- this is well known in mathematics as the **spherical bessel equation** and has solutions in the form of **spherical bessel functions**, $j_{l}(x)$, and **spherical neumann functions**, $n_{l}(x):$ 
$$\begin{align*}
	j_{0}(x) &= \frac{\sin x}{x} \\
	j_{1}(x) &= \frac{\sin{x}}{x} - \frac{\cos{x}}{x} \\
	j_{2}(x) &= \left(\frac{3}{x^{2}}- \frac{1}{x}\right)\sin{x} - \frac{3}{x^{2}}\cos{x} \\
	n_{0}&= - \frac{\cos{x}}{x}
\end{align*}$$ 
- spherical bessel functions (left), and spherical neumann functions (right): ![Pasted image 20241112114207.png](/img/user/pics/Pasted%20image%2020241112114207.png)
- it is visible that *spherical neumann functions* diverge at $x=0$, and thus, they cannot describe a wavefunction as it cannot be normalized
- therefore, *spherical bessel functions* are the only valid solutions

- imposing the boundary condition, $R(a)=0:$ 
$$j_{l}(ka) = 0$$
- the spherical bessel functions are zero at many points
- denoting the position of the $n^{th}$ crossing of zero by $x_{nl}$, the energy levels are: 
  $$E_{n,l} = \frac{\hbar^{2}x_{nl}^{2}}{2\pi a^{2}}$$
- the wavefunction: 
  $$\phi_{nlm} = j_{nl}\left(\frac{x_{nl}r}{a}\right) Y_{l,m}(\theta,\phi)$$
- there are **three quantum numbers, $n,l,m$**
- states with different $n$ and/or $l$ will have different energies
