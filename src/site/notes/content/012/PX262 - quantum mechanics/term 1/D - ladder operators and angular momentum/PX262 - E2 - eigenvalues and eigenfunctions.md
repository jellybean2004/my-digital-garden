---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-1/d-ladder-operators-and-angular-momentum/px-262-e2-eigenvalues-and-eigenfunctions/","noteIcon":"1","created":"2025-08-27T13:14:15.867+01:00","updated":"2024-12-15T17:12:41.000+00:00"}
---

- using spherical coordinates: 
$$\begin{gather}
	x = r\sin\theta\cos\phi \\
	y = r\sin\theta\sin\phi \\
	z = r\cos\theta\\
	\vec\nabla = \hat r\frac{\partial }{\partial r} + \frac{1}{r}\hat \theta \frac{\partial}{\partial \theta} + \frac{1}{r\sin\theta} \hat \phi \frac{\partial }{\partial \phi}
\end{gather}$$
$$\begin{gather}
	\hat r \times \hat r = 0 \\
	\hat \theta \times \hat r = - \hat \phi \\
	\hat \phi \times \hat r = \hat \theta
\end{gather}$$
- the angular momentum operator: 
$$\begin{align*}\hat{\vec L} = - i\hbar \hat{\vec r} \times \vec\nabla &= -\hbar \left(\hat\phi \frac{\partial }{\partial \theta} - \frac{1}{\sin\theta} \hat\theta \frac{\partial }{\partial \phi}\right)\\
\implies \hat L_{z} &= \hat z \cdot \hat{\vec L} = -i\hbar \frac{\partial }{\partial \phi}
\end{align*}$$
- the angular momentum squared operator can be expressed using the vector identity: 
$$\begin{align*}
	\hat{ L}^{2} &= -\hbar^{2} (\hat r \times \vec\nabla) \cdot (\hat r \times \vec\nabla) \\
	&= -\hbar^{2} \hat r \cdot [\vec\nabla \times  (\hat r \times \vec\nabla) ]\\
	
	&= -\hbar^{2} \left[ \frac{1}{\sin\theta} \frac{\partial }{\partial \theta} \left(\sin\theta \frac{\partial}{\partial \theta} \right) + \frac{1}{\sin^{2}\theta} \frac{\partial^{2}}{\partial \phi^{2}}  \right]
\end{align*}$$
- to solve the eigenvalues equations: 
$$\begin{align*}
	\hat L^{2} Y &= \lambda Y \\
	\hat L_{z} Y &= \nu Y 
\end{align*}$$
- using separation of variables: 
  $$Y(\theta,\phi) = \Theta(\theta) \, \Phi(\phi)$$
- taking the eigenvalue equation for $\hat L_{z}:$ 
$$\begin{align*}
	-i\hbar \frac{\partial }{\partial \phi} \Theta(\theta)\,\Phi(\phi) &= \nu\,\Theta(\theta)\,\Phi(\phi) \\
	-i\hbar \frac{\partial \Phi(\phi)}{\partial \phi} &= \nu\,\Phi(\phi)
\end{align*}$$
{ #2a5506}

- the general solution for this equation is: 
  $$\Phi = C\exp\left(\frac{i\nu\phi}{\hbar}\right)$$
	where $C$ is the normalization constant
- with $\phi$ being the angle, the answer should stay the same after a rotation by $2\pi$, ie: $\Phi(\phi+2\pi) = \Phi(\phi)$
- therefore, it is required that $\frac{\nu}{\hbar}=m$, where $m$ is an integer
- normalizing the function: 
$$\begin{align*}
	1 &= \int_{0}^{2\pi} \Phi^{*}\Phi\,d\phi \\
	&= C^{2} \int_{0}^{2\pi} e^{im\phi} e^{-im\phi}\,d\phi \\
	&= C^{2}2\pi \\
	\therefore C &= \frac{1}{\sqrt{2\pi}}
\end{align*}$$
- therefore, the eigenfunctions have the form: 
  $$\Phi = \frac{1}{\sqrt{2\pi}} e^{im\phi}$$
	where the eigenvalues would be: $\nu = \hbar m$
	
- with $\phi$-dependence fixed, looking at $\hat{\vec L}^{2}:$ 
$$\begin{align*}
	-\hbar^{2} \left[\frac{1}{\sin\theta} \frac{\partial }{\partial \theta} \left(\sin\theta \frac{\partial }{\partial \theta}\right) + \frac{1}{\sin^{2}\theta} \frac{\partial^{2} {}}{\partial {\phi}^{2}} \right] \Theta(\theta)\Phi(\phi) &= \lambda\Theta(\theta)\Phi(\phi) \\
	-\hbar^{2} \left[\frac{1}{\sin\theta} \Phi(\phi) \frac{\partial }{\partial \theta} \left(\sin\theta \frac{\partial \Theta(\theta)}{\partial \theta}\right) + \frac{\Theta(\theta)}{\sin^{2}\theta} \frac{\partial^{2} {\Phi(\phi)}}{\partial {\phi}^{2}} \right] &= \lambda\Theta(\theta)\Phi(\phi) \\
	-\hbar^{2} \left[\frac{1}{\sin\theta} \Phi(\phi) \frac{\partial }{\partial \theta} \left(\sin\theta \frac{\partial \Theta(\theta)}{\partial \theta}\right) + \frac{\Theta(\theta)}{\sin^{2}\theta} (-m^{2}\Phi(\phi)) \right] &= \lambda\Theta(\theta)\Phi(\phi) \\
	-\hbar^{2}\sin\theta \frac{d}{d\theta}\left(\sin\theta \frac{d\Theta(\theta)}{d\theta}\right) + \hbar^{2}\Theta(\theta) m^{2} - \lambda \sin^{2}\theta \, \Theta(\theta) &= 0
\end{align*}$$
{ #136af2}

- substituting $v = \cos\theta:$
  $$\frac{d}{d\theta}= -\sin\theta \frac{d}{dv} = - (1-v^{2})^{\frac{1}{2}} \frac{d}{dv}$$
- $\Theta(\theta)$ can be rewritten as $P(v):$ 
  $$\hbar^{2} \frac{d}{dv}\left[ (1-v^{2})^{\frac{1}{2}} \frac{dP(v)}{dv}\right] + \left[\lambda - \frac{\hbar^{2}m^{2}}{1-v^{2}}\right] = 0$$
- solving explicitly for $m=0$, looking at the solution in the form: 
$$P(v) = \sum\limits_{p=0}^{\infty} a_{p}v^{p}$$
- following the same logic as for the [[content/012/PX284 - SMETO/part 1 - statistical mechanics/E - single-particle partition function/PX284 - E3 - harmonic oscillator in 1D\|harmonic oscillator]], substituting $P$ into the differential equation will lead to a recursive relation between coefficients
- it will be found that the expansion diverges at $v=1$, so, the coefficients after some value of $p$ must be cut off
- this can be done by setting:
  $$\lambda = \hbar^{2}l(l+1)$$
	where, $l$ is a positive integer
- the functions, ${} P(v)$, are well known polynomials, *legendre polynomials*
- the first few legendre polynomials are: 
$$\begin{align*}
	P_{0}(v) &= 1 \\
	P_{1}(v) &= v \\
	P_{2}(v) &= \frac{1}{2}(3v^{2}-1) \\
	P_{3}(v) &= \frac{1}{2}(5v^{3}-3v) 
\end{align*}$$
- functions for $m\neq0$ follow the same steps, but the maths is quite complicated, hence the details are skipped

- the solutions in terms of $P(v)$ are given by functions: 
$$P_{l}^{|m| } (v) = (1-v^{2})^{|m|/2} \frac{d^{|m|}P_{l}}{dv^{|m|}}$$
- if $|m|>l$, the derivative will be zero, and the whole wavefunction will be zero over all space, which is physically unrealistic
- therefore the values of $m$ are restricted by the condition:
$$|m|\leq l$$
- the eigenfunctions of $\hat L^{2}$ and $\hat L_{z}$ are: 
  $$Y_{lm}(\theta,\phi) = (-1)^{m} \left[ \frac{2l+1}{4\pi} \frac{(l-|m|)!}{(l+|m|)!} \right]^{{1}/{2}} P_{l}^{|m|} (\cos\theta)\,\exp(im\phi)$$
	where, $(-1)^{m}$ is purely a convention

- the functions, $Y_{lm}(\theta,\phi)$, are called *spherical harmonics*
- the factor in the brackets is the normalization factor such that: 
  $$\int_{0}^{2\pi} \int_{0}^{\pi} |Y_{lm}(\theta,\phi)|^{2} \,\sin\theta\,d\theta\,d\phi =1$$

- these functions are orthogonal and form a complete set, so any general wavefunction can be written as a linear combination of $Y_{lm}(\theta,\phi)$ 
- the eigenvalue equations are: 
$$\begin{align*}
	\hat L_{z} Y_{l,m}(\theta,\phi) &= \hbar m \, Y_{l,m}(\theta,\phi) \\
	\hat L^{2} Y_{lm}(\theta,\phi) &= \hbar^{2}l(l+1) \, Y_{lm}(\theta,\phi)
\end{align*}$$
- $l$ and $m$ are often used as quantum numbers to label states, referred to as orbital and magnetic quantum numbers respectively
- spherical harmonics for $l\leq 2:$
$$\begin{align*}
Y_{00}(\theta,\phi) &= \frac{1}{\sqrt{4\pi }}\\
Y_{10}(\theta,\phi) &= \mp \sqrt{\frac{3}{4\pi }} \cos\theta \\
Y_{1\pm1}(\theta,\phi) &= \mp \sqrt{\frac{3}{8\pi }} \sin\theta e^{\pm i \phi}\\
Y_{20}(\theta,\phi) &= \mp \sqrt{\frac{5}{16\pi }} (3\cos^{2}\theta - 1)\\
Y_{2\pm1}(\theta,\phi) &= \mp \sqrt{\frac{15}{8\pi }} \cos\theta  \sin\theta \, e^{\pm i \phi} \\
Y_{2\pm2}(\theta,\phi) &= \mp \sqrt{\frac{15}{32\pi }}  \sin^{2}\theta \,e^{\pm 2i \phi} \\
\end{align*}$$
- for two neighbouring states with the same $l$, $\Delta m = m_{1}-m_{2}$, is constant
- another analogue of ladder operators can be defined for angular momentum operator as: 
$$\begin{align*}
	\hat L_{+} &= \hat L_{x} + i \hat L_{y} \\
	\hat L_{-} &= \hat L_{x} - i \hat L_{y} 
\end{align*}$$
$$\hat L_{\pm} Y_{l,m}(\theta,\phi) = \sqrt{(l\mp m)(l\pm m+1 )} \hbar \, Y_{l,m+1 }(\theta,\phi) $$

![Pasted image 20241106211601.png](/img/user/pics/Pasted%20image%2020241106211601.png)
*image: Q. Wang, K. Birod, C. Angioni, et al. PLoS ONE 6(7): e21554. https://doi.org/10.1371/journal.pone.0021554*
