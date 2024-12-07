---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/c-the-basic-postulates/px-262-c4c-continuous-eigenvalues/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-07T16:07:30.230+00:00"}
---

- previous arguments assume that the eigenvalues of the operators have discrete values
- this is true for energy, but not for position and momentum
- taking approximation by discrete steps, but also the limit $\Delta\to0$, the eigenvalue equation becomes: 
  $$\hat Q \phi (k,x) = q(k) \phi (k,x)$$
	where, $k$ is a continuous variable that labels individual steps (like the subscript $n$)
- the equivalent wavefunction is:
$$\psi(x) = \int a(k) \phi(k,n)\,dk$$
- the probability of getting a result inside the range $dk$ in the vicinity of $k$ is:
$$p = |a(k)|^{2}\,dk$$

- the orthonormality condition is:
$$\int \phi^{*}(k,x) \phi(k',x) \,dx = \delta(k-k')$$
- the general wavefunction can be written as a liner superposition of eigenfunctions as: 
  $$\psi(x) = \int a(k)\phi(k,x)\,dk$$
