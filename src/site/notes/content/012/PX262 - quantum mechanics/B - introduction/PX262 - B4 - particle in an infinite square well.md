---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/b-introduction/px-262-b4-particle-in-an-infinite-square-well/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T01:30:54.474+00:00"}
---

- considering an infinite square potential well: 
  $$V(x) = \begin{cases} 0 & for & |x|<a, \\ \infty & for & |x|>a. \end{cases}$$
- infinite potential means that particles cannot be in that region, ie: $\phi =0$
- inside the well: 
  $$-\frac{\hbar^{2}}{2m} \frac{d^{2}\phi(x)}{dx^{2}} = E\phi(x)$$
- the solution has the form: $\phi(x) = A\cos(kx)+B\sin(kx)$
	where, $A$ and $B$ are constants; $k=\sqrt{\frac{2mE}{\hbar^{2}}}$
- the boundary conditions require that the function is continuous at the border of the potential well: $\phi(-a) = \phi(a)=0$
$$\begin{gather*}
	A\cos(ka)+ B\sin(kx) = 0 \\
	A\cos(-ka)+ B\sin(-kx) = 0 \\
	2A\cos(ka) = 0 \\
	2B\sin(ka) = 0 \\
\end{gather*}$$
- two options to satisfy this: 
	- $B=0$, ${} \cos(ka)=0 \implies k = \frac{n\pi}{2a},n\in odd {}$
	- ${} A=0$, $\sin(ka)=0 \implies k = \frac{n\pi}{2a},n\in even$

- wave function (after normalization): 
  $$\phi_{n}(x) = \begin{cases}
	 \frac{1}{\sqrt{a}}\cos\left(\frac{n\pi x}{2a}\right) & \text{for } n\in \text{odd,} \\
	\frac{1}{\sqrt{a}}\sin\left(\frac{n\pi x}{2a}\right) & \text{for } n \in \text{even,} \\
	0 & \text{for } |x|>a.
	\end{cases}$$
	- the index in the labels give the state of the system

- substituting into the schrödinger equation: 
  $$\begin{gather*}
\vdots \\
E_{n}= \frac{\hbar^{2}\pi^{2}}{8ma^{2}}n^{2}
\end{gather*}$$
- **note:** 
	- a particle in the system can only have specific, discrete energies
	- the probabilities of finding the particle at different positions will depend on the energies

- typical values for electron, $M=9.1\times10^{-31}\,kg$, in an atom of size, $10^{-10}m:$ $E_{n}=9.4\,eV\,n^{2}$

- more macroscopic: $M=10^-10\,kg$; $a = 10^{-6}\,m \implies E_{n}= 1.4\times10^{-46}\,n^{2}\,J$
	- thermal energy at $1K \sim 10^-23\,J$, $n$ must be $3\times10^{11}$
	- differences between energies and positions are so small that they cannot be distinguished experimentally

- **correspondence principle:** when going towards macroscopic objects, the quantum mechanical description will result in something resembling classical physics
