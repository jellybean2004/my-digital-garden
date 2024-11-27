---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/d-ladder-operators-and-angular-momentum/px-262-e2-eigenvalues-and-eigenfunctions/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-27T23:10:39.790+00:00"}
---

- using spherical coordinates: 
$$\begin{gather}
	x = r\sin\theta\cos\phi \\
	y = r\sin\theta\sin\phi \\
	z = r\cos\theta
	\end{gather}$$
$$\vec\nabla = \hat r\frac{\partial }{\partial r} + \frac{1}{r}\hat \theta \frac{\partial}{\partial \theta} + \frac{1}{r\sin\theta} \hat \phi \frac{\partial }{\partial \phi}$$
$$\begin{gather}
	\hat r \times \hat r = 0 \\
	\hat \theta \times \hat r = - \hat \phi \\
	\hat \phi \times \hat r = \hat \theta
\end{gather}$$
- the angular momentum operator: 
$$\begin{align*}\hat{\vec L} = - i\hbar \hat r \times \vec\nabla &= -\hbar \left(\hat\phi \frac{\partial }{\partial \theta} - \frac{1}{\sin\theta} \hat\theta \frac{\partial }{\partial \phi}\right)\\
\implies \hat L_{z} &= \hat z \cdot \hat{\vec L} = -i\hbar \frac{\partial }{\partial \phi}
\end{align*}$$
- the angular momentum squared operator: 
$$\begin{align*}
	\hat{\vec L}^{2} &= -\hbar^{2} (\hat r \times \vec\nabla) \cdot (\hat r \times \vec\nabla) \\
	&= -\hbar^{2} \left[ \frac{1}{\sin\theta} \frac{\partial }{\partial \theta} \left(\sin\theta \frac{\partial}{\partial \theta} \right) + \frac{1}{\sin^{2}\theta} \frac{\partial^{2}}{\partial \phi^{2}}  \right]
\end{align*}$$
- to solve the eigenvalues equations: 
$$\begin{align*}
	\hat{\vec L}^{2} Y &= \lambda Y \\
	\hat L_{z} Y &= \nu Y 
\end{align*}$$
- using separation of variables: 
  $$Y(\theta,\phi) = \Theta(\theta) \, \Phi(\phi)$$
- taking the eigenvalue equation for $\hat L_{z}:$ 
$$\begin{align*}
	-\hbar \frac{\partial }{\partial \phi} \Theta(\theta)\,\Phi(\phi) &= \nu\,\Theta(\theta)\,\Phi(\phi) \\
	-\hbar \frac{\partial \Phi(\phi)}{\partial \phi} &= \nu\,\Phi(\phi)
\end{align*}$$
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
- substituting $v = \cos\theta:$
  $$\frac{d}{d\theta}= -\sin\theta \frac{d}{dv} = - (1-v^{2})^{\frac{1}{2}} \frac{d}{dv}$$
- $\Theta(\theta)$ can be rewritten as $P(v):$ 
  $$\hbar^{2} \frac{d}{dv}\left[ (1-v^{2})^{\frac{1}{2}} \frac{dP(v)}{dv}\right] + \left[\lambda - \frac{\hbar^{2}m^{2}}{1-v^{2}}\right] = 0$$
- solving explicitly for $m=0$, looking at the solution in the form $P(v) = \sum\limits_{p=0}^{\infty} a_{p}v^{p}:$ 
  $$\lambda = \hbar^{2}l(l+1)$$
	where, $l$ is a positive integer
- the functions, ${} P(v)$, are well known polynomials, *legendre polynomials*: 
$$\begin{align*}
	P_{0}(v) &= 1 \\
	P_{1}(v) &= v \\
	P_{2}(v) &= \frac{1}{2}(3v^{2}-1) \\
	P_{3}(v) &= \frac{1}{2}(5v^{3}-3v) \\
	\vdots
\end{align*}$$
- functions for $m\neq0$ follow the same steps, but the maths is quite complicated, hence the details are skipped

- the solutions in terms of $P(v)$, given by functions: 
  $$P_{l}^{m } (v) = (1-v^{2})^{\frac{|m|}{2}} \frac{d^{|m|}P_{l}}{dv^{|m|}}$$
- if $|m|>l$, the derivative will be zero, therefore making the solution zero, therefore the values of $m$ are restricted to $|m|\leq l$
- the eigenfunctions of $\hat L^{2}$ and $\hat L_{z}$ are: 
  $$Y_{l,m}(\theta,\phi) = (-1)^{m} \left[ \frac{2l+1}{4\pi} \frac{(l-|m|)!}{(l+|m|)!} \right]^{\frac{1}{2}} P_{l}^{|m|} (\cos\theta)\,\exp(im\phi)$$
- the functions, $Y_{l,m}(\theta,\phi)$, are called *spherical harmonics*
- the factor in the brackets is the normalization factor such that: 
  $$\int_{0}^{2\pi} \int_{0}^{\pi} |Y_{l,m}(\theta,\phi)|^{2} \,\sin\theta\,d\theta\,d\phi =1$$
- $(-1)^{m}$ is purely a convention

- these functions are orthogonal and form a complete set, so any general wavefunction can be written as a linear combination of $Y_{lm}(\theta,\phi)$ 
- the eigenvalue equations are: 
$$\begin{align*}
	\hat L_{z} Y_{l,m}(\theta,\phi) &= \hbar m \, Y_{l,m}(\theta,\phi) \\
	\hat {\vec L^{2}} Y_{lm}(\theta,\phi) &= \hbar^{2}l(l+1) \, Y_{lm}(\theta,\phi)
\end{align*}$$
- $l$ and $m$ are often used as quantum numbers to label states, referred to as orbital and magnetic quantum numbers respectively
- spherical harmonics for $l\leq 2:$
 ![Pasted image 20241106212214.png](/img/user/pics/Pasted%20image%2020241106212214.png)
- for two neighbouring states with the same $l$, $\Delta m = m_{1}-m_{2}$, is constant
- another analogue of latter operators can be defined: 
$$\begin{align*}
	\hat L_{+} &= \hat L_{x} + i \hat L_{y} \\
	\hat L_{-} &= \hat L_{x} - i \hat L_{y} 
\end{align*}$$
$$\hat L_{\pm} Y_{l,m}(\theta,\phi) = \sqrt{(l\mp m)(l\pm m+1 )} \hbar \, Y_{l,m+1 }(\theta,\phi) $$

![Pasted image 20241106211601.png](/img/user/pics/Pasted%20image%2020241106211601.png)