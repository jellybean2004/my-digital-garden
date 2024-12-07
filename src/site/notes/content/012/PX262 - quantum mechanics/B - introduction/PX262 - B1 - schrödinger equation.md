---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/b-introduction/px-262-b1-schroedinger-equation/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-07T11:32:06.796+00:00"}
---

## the time-dependent equation
- a fundamental equation in QM to describe the system and the state in which it is, the schrödinger equation: 
  $$i\hbar \frac{\partial \psi(x,t)}{\partial t} = - \frac{\hbar^{2}}{2m} \frac{\partial^{2} \psi(x,t)}{\partial x^{2}}+V(x,t)\psi(x,t)$$
	where, 
		${} m= {}$ mass of the particle
		$V(x,t)=$ the potential in which it is moving
		$\psi(x,t) =$ the wavefunction which encodes all information about the state of the particle 
	
- there is a correspondence between classical energy an schrödinger equation
	- in classical mechanics: 
	  $$E = \frac{p^{2}}{2m} +V$$
	- swapping $p, V, E$ with operators: 
$$\begin{align*}
		E\to i\hbar\frac{\partial }{\partial t} \\
		\vec p \to -i\hbar \vec\nabla
	\end{align*}$$
	- putting these into the energy relation, and adding : 
## meaning of the wavefunction
- classically, it is real, and  it gives the displacement
- in QM, it can be complect, and does not directly give the displacement
- the QM wavefunction is connected to the probability of finding a particle at some position
- in some interval, between $x$ and $x+dx$, at a time, $t$, the probability of finding the particle is given by the *bohr postulates*: 
  $$P(x,t)\,dx = |\psi(x,t)|^{2}$$
- the wavefunction has to be *normalized*, ie. the probability of finding the particle in the system is fixed: 
$$\begin{gather*}
	\int_{-\infty}^{+\infty} P(x,t)\,dx = 1 \\
	\implies \int_{-\infty}^{+\infty} |\psi(x,t)|^{2}\,dx = \int_{-\infty}^{+\infty} \psi^{*}\psi\,dx=1
\end{gather*} $$
