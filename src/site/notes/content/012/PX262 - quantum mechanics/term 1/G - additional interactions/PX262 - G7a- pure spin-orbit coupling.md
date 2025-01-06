---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-1/g-additional-interactions/px-262-g7a-pure-spin-orbit-coupling/","noteIcon":"1","created":"2024-11-26T11:31:26.405+00:00","updated":"2024-12-21T14:23:31.271+00:00"}
---

- setting the external magnetic field to zero:
$$\hat H_{LS} = f(r) (\hat J^{2} - \hat L^{2} - \hat S^{2})$$
- there is no preferred axis and the energy eigenfunctions do not have to be eigenfunctions of $\hat L_z$ and $\hat S_z$
- they will still be eigenfunctions of $\hat J^{2}$, ${} \hat L^{2} {}$ and $\hat S^{2}$ operators
- the energy levels of any total angular momentum operator have the form $j(j+1)\hbar^{2}$, where, $j = n/2$ for $n\in \mathbb Z$

- the change in energy can therefore be approximated by its expectation value:
$$\delta E = \langle{f(r)}\rangle \, [j(j+1) - l(l+1) - s(s+1)] \, \hbar^{2}$$
- the three quantities are connected:
$$\begin{gather*}
	j = l+s &	\text{or, } j = |l-s| & \text{for } s = \frac{1}{2} \\
	j = l + \frac{1}{2} & \text{or, } j = l - \frac{1}{2} & \text{unless } l=0
\end{gather*}$$
- the energy levels will split into $2(2l +1) = 6$ states

![spin-orbit splitting.png|500](/img/user/pics/spin-orbit%20splitting.png)
*image: A. I. M. Rae, Quantum Mechanics 6th Edition* 

- above image shows the effect of spin-orbit coupling on the energy levels of a one-electron atom
- $l=2$ states are split into a doublet, degeneracy of either state is $(2j+1):$ $6$ for $j=5/2$, $4$ for $j=3/2$
- hence, the total number of states: $2(2 l +1) = 10$
