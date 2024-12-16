---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/b-introduction/px-262-b6-1-d-harmonic-oscillator/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-07T12:53:06.390+00:00"}
---

- in classical physics: 
  $$V(x) = \frac{1}{2}kx^{2}$$
	where, $k$ is the spring constant, $x$ is the displacement from the equilibrium position
- a particle with a mass, ${} m$, will be oscillating with an angular frequency, $\omega_{c} = \sqrt{\frac{k}{m}}$
- the time independent schrödinger equation: 
$$\begin{align*}
	- \frac{\hbar^{2}}{2m} \frac{d^{2}\phi(x)}{dx} + \frac{1}{2}m \omega_{c}^{2}x^{2}\phi(x) &= E\,\phi(x) \\
	\frac{d^{2}\phi(y)}{dy^{2}} + (\alpha-y^{2})\phi(y) =0
\end{align*}$$
	where, $y = \sqrt{\frac{M\omega_{c}}{\hbar}}x$, and $\alpha = \frac{2E}{\hbar\omega_{c}}$
- looking at the asymptotic case, $|y| >> \alpha:$ 
$$\frac{d^{2}\phi}{dy^{2}} - y^{2}\phi = 0$$
- try solution in form: 
$$\begin{gather*}
	\phi = y^{n}e^{-\frac{y^{2}}{2}} \\\\
	\implies \frac{d\phi}{dy} = ny^{n-1} e^{- \frac{y^{2}}{2}} - ye^{- \frac{y^{2}}{2}} 	= \frac{n}{y}\phi(y) - y \phi(y)\\\\
	\implies \frac{d^{2}\phi}{dy^{2}} = - \frac{n}{y^{2}} \phi(y) + \frac{n}{y}\left(\frac{n}{y}\phi(y)-y\phi(y)\right)-\phi(y) -y\left(\frac{n}{y}\phi (y) -y\phi(y)\right) \\
	= \frac{n(n-1)}{y^{2}}\phi(y) - (2n+1)\phi(y) + y^{2}\phi(y)
\end{gather*}$$
- if $y$ is very large: 
$$\frac{d^{2}\phi(y)}{dy^{2}} \approx y^{2}\phi(y)$$
	- also, $\phi\approx 0$ due to the $e^\frac{-y^{2}}{2}$ term

- for all values  of $y$, the general solution can be written as: 
  $$\phi(y) = H(y)e^{- \frac{y^{2}}{2}}$$
	where, $H(y)$ is a function that needs to be determined
- substituting $H$ in the TISE: 
  $$H'' - 2yH' + (\alpha-1)H=0$$
- any well behaved wavefunctions in quantum mechanics can be written as a power series: 
  $$H(y) = \sum\limits_{p=0}^{\infty} a_{p}y^{p}$$
	where, $a_p$ is  constant to be determined
- differentiating $H:$ 
$$\begin{align*}
	H' &= \sum\limits_{p=1}^{\infty}a_{p}py^{p-1} \\\\
	H'' &= \sum\limits_{p=1}^{\infty}a_{p}p(p-1)y^{p-2} \\
	&= \sum\limits_{p=2}^{\infty}a_{p}p(p-1)y^{p-2} \\
	&= \sum\limits_{p'=0}^{\infty} a_{p'+2}(p'+2 )(p'+1)y^{p'} \\
\end{align*}$$
- substituting into the differential equation: 
$$\begin{gather*}
	\sum\limits_{p=0}^{\infty} [(p+1)(p+2) a_{p+2} - (2p+1-\alpha)]y_{p} =  0 \\
	(p+1)(p+2) a_{p+2} - (2p+1-\alpha)a_{p} = 0 \\\\
\frac{	a_{p+2}}{a_{p}} = \frac{2p+1-\alpha}{(p+1)(p+2)}

\end{gather*}$$
- $H$ will tend to $e^{y^{2}}$, which diverges as $y\to\infty:$ 
  $$\implies \phi(y) = e^{\frac{-y^{2}}{2}}e^{y^{2}}= e^{\frac{y^{2}}{2}}$$
- this cannot describe a valid wavefunction as the integral would be infinite
- the number of contributing terms need to be restricted by stopping the sum at some point
- this can be done by making all constants, $a_{p} = 0$ for $p>n$
- setting the numerator, $2n + 1 - \alpha =0 \implies \alpha = 2n+1$
- substituting the value of $\alpha$ gives the allowed energies: 
  $$E_{n}= \left(n + \frac{1}{2}\right)\hbar\omega_c$$
- the condition $\alpha =2n+1$ removed even/odd terms, but not both

- the lowest state has $n=0$, and its energy is called the **zero-point energy**: 
  $$E_{0}= \frac{1}{2}\hbar \omega_{c}$$
- the energy levels are evenly spaced with the difference, $\hbar\omega_c$
- the polynomials $H(y)$ are called **hermite polynomials**: 
$$\begin{gather}
		H_{0}=1 && H_{1}=2y \\ H_{2}=4y^{2}-2 && H_{3}=8y^{3}-12y
\end{gather}$$
- these are multiplied by $e^{-y^{2}}$ in full wavefunctions
- quantum oscillators can go beyond the classical limit in displacement
$$\begin{align*}
	\phi_{0} &= \left(\frac{M\omega}{\hbar\pi}\right)^{\frac{1}{4}}\exp\left(\frac{-M\omega x^{2}}{2\hbar} \right) \\
	\phi_{1} &= \left(\frac{4}{\pi}\right)^{\frac{1}{4}} \left(\frac{M\omega}{\hbar\pi}\right)^{\frac{1}{4}}\exp\left(\frac{-M\omega x^{2}}{2\hbar}\right) \\
	\phi_{2} &= \left(\frac{M\omega}{4\pi\hbar}\right)^{\frac{1}{4}} \left[\frac{2M\omega}{\hbar}x^{2}-1\right] \exp\left(\frac{-M\omega x^{2}}{2\hbar}\right)
\end{align*}$$

![Pasted image 20241207125243.png|500](/img/user/pics/Pasted%20image%2020241207125243.png)
*image: avtar sehra*
