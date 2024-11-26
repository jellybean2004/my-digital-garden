---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/c-the-basic-postulates/px-262-c8-postulate-5/"}
---

## the time dependence of the wavefunction
- time dependence is given by the schrödinger equation: 
$$\begin{gather}
	- \frac{\hbar^{2}}{2m} \vec\nabla^{2}\psi + V(\vec r , t) \psi = i\hbar \frac{\partial \psi}{\partial t} \\
	H\psi = i\hbar \frac{\partial \psi}{\partial t}
\end{gather}$$
- another time dependence is when measurement is done
- at the time of the measurement, the wavefunction collapses to one of the eigenfunctions of the corresponding order
## postulate 5 
- between measurements, the development of the wavefunction is governed by the schrödinger equation 
- how it looks for a general wavefunction: 
  $$\psi(\vec r , t) = \sum\limits_{n}a_{n}(t) \phi_{n}(\vec r)$$
$$i\hbar \sum\limits_{n}\frac{da_{n}(t)}{dt} \phi_{n}(\vec r) = \sum\limits_{n}a_{n}(t) \hat H\phi_{n}= \sum\limits_{n} a_{n}(t) E_{n}\phi_{n}(\vec r)$$
	where, $\phi_{n}$ are eigenfunctions of the hamiltonian operator
$$\sum\limits_{n} \left( i\hbar \frac{da_{n}}{dt} - a_{n}E_{n} \right)\phi_{n} = 0$$
- to hold in general for all cases: 
$$\begin{align*}
	i\hbar \frac{da_{n}}{dt} - a_{n}E_{n} &= 0 \\
	i\hbar \frac{da_{n}}{dt} &= a_{n}E_{n} \\
	a_{n}(t) &= a_{n}(0) \exp\left(-\frac{iE_{n}t}{\hbar}\right)
\end{align*}$$
- the full solution: 
  $$\psi(\vec r, t) = \sum_{n}a_{n}(0) \phi_{n}(\vec r)\exp\left(- \frac{iE_{n}t}{\hbar}\right)$$