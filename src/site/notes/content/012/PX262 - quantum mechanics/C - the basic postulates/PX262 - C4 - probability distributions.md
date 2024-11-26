---
dg-publish: true
---

- taking the lowest energy state of a particle in an infinite potential well, and its wavefunction
- the position eigenfunctions are defined by the dirac delta functions, and the whole wavefunction could be viewed as a sum of an infinite number of these functions
- this can be approximated by discretizing the position, allowing the particle to be one of the several strips of a finite width, $\Delta$

![Pasted image 20241022142825.png](/img/user/pics/Pasted%20image%2020241022142825.png)

- if the particle is measured in a particular strip, strip $n$, that strip will have a non-zero height, whereas all other strips will have a height of zero
- the height is given by the fact that the probability of finding the particle in that strip is one: 
  $$ h\Delta^{2}=1 \implies h = \Delta^{-\frac{1}{2}}$$
- the $n^{th}$ wavefunction is denoted by $\phi_{n}$, which is properly normalized

- before the measurement, the wavefunction of the system is the weighted sum over all the strips: 
  $$\psi(x) = \sum\limits_{n} \frac{\psi(x_{n})}{h} \phi_{n} = \sum\limits_{n}a_{n}\phi_{n}$$
	where, $a_{n} = \frac{\psi(x_{n})}{h} = \Delta^{\frac{1}{2}}\psi(x_{n})$
- the weights correspond to the probability of finding the particle in each strip
- the probability of finding the particle in the $n^{th}$ strip is: 
  $$P(x_{n}) = |\psi(x_{n})|^{2}\Delta = |a_{n}|^{2}$$
- generalising to any measurement by the operator $\hat Q:$ 
  $$\psi = \sum\limits_{n}a_{n}\phi_{n} $$
- this exploits the property of hermitian operators that their wavefunctions form a complete set, and that any well-behaved function can be expressed as a liner superposition of the eigenfunctions