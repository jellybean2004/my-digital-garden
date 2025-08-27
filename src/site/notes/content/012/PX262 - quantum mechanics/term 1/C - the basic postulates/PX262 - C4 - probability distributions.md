---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-1/c-the-basic-postulates/px-262-c4-probability-distributions/","noteIcon":"1","created":"2025-08-27T13:14:15.832+01:00","updated":"2024-12-07T18:20:45.000+00:00"}
---

- taking the lowest energy state of a particle in an infinite potential well, and its wavefunction
- the position eigenfunctions are defined by the dirac delta functions, and the whole wavefunction could be viewed as a sum of an infinite number of these functions

- considering a experiment where the particle is found in one of a series of detectors of width, $\Delta$
- if the particle is measured in a particular detector, the wavefunction will be non-zero everywhere except on that detector, with a peak $h$ and width, $\Delta$
- the height is given by the fact that the probability of finding the particle in that strip is one: 
  $$ h^{2}\Delta=1 \implies h = \Delta^{-\frac{1}{2}}$$
	  **note:** $h^{2}$ comes from the fact that probability comes from $|\psi|^{2}$
	
- the $n^{th}$ wavefunction is denoted by $\phi_{n}$, which is properly normalized
- the wavefunction before such measurement is $\psi$
- if $\psi(x)$ is divided into a strips of width, $\Delta$, which can be approximated by $\psi(x_n)$ inside the $n^{th}$ strip

![Pasted image 20241207182041.png|500](/img/user/pics/Pasted%20image%2020241207182041.png)

- $\phi_n$ would represent a strip of height $h$ covering the strip, and is zero outside it:
$$\psi(x) = \sum\limits_{n} \frac{\psi(x_{n})}{h} \phi_{n} = \sum\limits_{n}a_{n}\phi_{n}$$
	where, 
$$a_{n} = \cfrac{\psi(x_{n})}{h} = \Delta^{1/2}\psi(x_{n})$$
- the weights correspond to the probability of finding the particle in each strip
- the probability of finding the particle in the $n^{th}$ strip is: 
  $$P(x_{n}) = |\psi(x_{n})|^{2}\Delta = |a_{n}|^{2}$$
- generalising to any measurement by the operator $\hat Q:$ 
  $$\psi = \sum\limits_{n}a_{n}\phi_{n} $$
- this exploits the property of hermitian operators that their wavefunctions form a complete set, and that any well-behaved function can be expressed as a liner superposition of the eigenfunctions
