---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/f-3-d-systems/px-262-f4-separation-of-variables-in-spherical-coordinates/"}
---

- considering a spherically symmetric potential: $V(x,y,z) = V(r)$, where $r$ is the distance from the centre of potential
- the schrödinger equation in spherical coordinates: 
$$\begin{multlined}
	- \frac{\hbar^{2}}{2m} \bigg[\frac{1}{r^{2}} \frac{\partial }{\partial r}\left(r^{2}\frac{\partial \phi}{\partial r}\right) + \frac{1}{r^{2}\sin\theta} \frac{\partial }{\partial \theta}
	\left(\sin\theta \frac{\partial \phi}{\partial \theta}\right) \\+ \frac{1}{r^{2}\sin^{2}\theta} \frac{\partial^{2} {\phi}}{\partial {\phi}^{2}} \bigg] + V\phi = E\phi \tag{1}
	\end{multlined}$$
	where, $\phi = \phi(r,\theta,\phi)$
- as potential depends on a single variable, using separation of variables in the wavefunction: $$\phi(r,\theta,\phi) = R(r) \, Y(\theta,\phi)$$
- equation $(1)$ becomes:
$$
\begin{gather}
	\begin{multlined}
		-\frac{\hbar^{2}}{2m} \bigg[ \frac{Y}{r^{2}} \frac{\partial }{\partial r}\left(r^{2}\frac{\partial R}{\partial r}\right) + \frac{R}{r^{2}\sin\theta} \frac{\partial }{\partial \theta} \left(\sin\theta \frac{\partial Y}{\partial \theta}\right) \\
		+ \frac{R}{r^{2}\sin^{2}\theta} \frac{\partial^{2} {Y}}{\partial {\phi}^{2}}  \bigg] + VRY = ERY \\
	\end{multlined} \\\\
	
	\begin{multlined}
		\bigg[ -\frac{\hbar^{2}}{2m} \frac{1}{R} \frac{d }{d r}\left(r^{2}\frac{d R}{d r}\right) + r^{2}V -r^{2} E \bigg] \\
		-\frac{\hbar^{2}}{2m} \bigg[ \frac{1}{Y} \frac{1}{\sin\theta} \frac{\partial }{\partial \theta} \left(\sin\theta \frac{\partial Y}{\partial \theta}\right) + \frac{1}{Y}\frac{1}{\sin^{2}\theta} \frac{\partial^{2} {Y}}{\partial {\phi}^{2}} \bigg] = 0
	\end{multlined} \tag{2}
\end{gather}$$
- each part in a square bracket must be equal to a constant and the two constants must add up to zero
- taking the second part: 
$$-\frac{\hbar^{2}}{2m} \left[ \frac{1}{\sin\theta} \frac{\partial }{\partial \theta} \left(\sin\theta \frac{\partial Y}{\partial \theta}\right) + \frac{1}{\sin^{2}\theta} \frac{\partial^{2} {Y}}{\partial {\phi}^{2}}\right] = \lambda Y$$
- from [[content/012/PX262 - quantum mechanics/D - ladder operators and angular momentum/PX262 - E2 - eigenvalues and eigenfunctions\|here]], this is the same as the equation for the eigenvalues of the operator $\hat L^{2}:$ 
$$\frac{1}{2m} \hat L^{2} Y = \lambda Y$$
- the solutions are spherical harmonics: $Y_{lm} (\theta,\phi)$, and the eigenvalues are: 
  $$\lambda = - \frac{\hbar^{2}}{2m} l(l+1)$$
- for every system with a spherically symmetric potential, the angular part will be the same, and it will correspond to the angular momentum
- any solution will be an eigenstate of $\hat L^{2}$ and $\hat L_{z}$ operators
- substituting into equation $(2):$ 
$$\begin{align*}
	-\frac{\hbar^{2}}{2m} \frac{1}{R} \frac{d }{d r}\left(r^{2}\frac{d R}{d r}\right) +r^{2}V+\frac{l(l+1)\hbar^{2}}{2m} &= r^{2} E \\
	-\frac{\hbar^{2}}{2m} \frac{1}{r^{2}} \frac{d }{d r}\left(r^{2}\frac{d R}{d r}\right) + \left[V(r) + \frac{l(l+1)\hbar^{2}}{2mr^{2}} \right]R &= ER \tag{3}
\end{align*}$$
- making the substitution $\chi(r) = r R(r):$ 
$$\begin{gather*} 
\frac{dR}{dr} = \frac{d}{dr}\left(\frac{\chi}{r}\right) = \frac{1}{r} \frac{d\chi}{dr} - \frac{\chi}{r^{2}} \\
\therefore\frac{d}{dr}\left(r^{2} \frac{dR}{dr}\right) = \frac{d}{dr}\left(r \frac{d\chi}{dr} - \chi\right) = r \frac{d^{2}\chi}{dr^{2}}​
\end{gather*}$$
- substituting into equation $(3):$  
$$ -\frac{\hbar^{2}}{2m} \frac{d^{2}\chi}{d r^{2}} + \left[V(r) + \frac{\hbar^{2}}{2mr^{2}} l(l+1)\right] \chi = E\chi $$
- an additional boundary condition applies to avoid divergence: $\chi(r=0)=0$ 
