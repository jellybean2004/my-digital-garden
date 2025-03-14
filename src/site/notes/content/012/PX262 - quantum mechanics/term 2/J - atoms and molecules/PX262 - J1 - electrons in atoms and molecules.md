---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/j-atoms-and-molecules/px-262-j1-electrons-in-atoms-and-molecules/","noteIcon":"1","created":"2025-01-23T17:40:48.914+00:00","updated":"2025-03-13T12:22:33.676+00:00"}
---

- the schrödinger equation for a single particle:
$$i\hbar \frac{\partial \psi}{\partial t} = \left(\frac{-\hbar^{2}}{2m}\nabla^{2} + V(x,y,z)\right)\psi$$
- the stationary states: $\psi = \phi_{\lambda} \exp(iE_{\lambda}t/\hbar)$
- if the potential is spherically symmetric, $V(x,y,z) = V(r)$, use spherical polar coordinates
- eg: for hydrogen:
$$V(r) = - \frac{e^{2}}{4\pi\varepsilon_{0}r}$$
$$\hat H \phi_{nlm_{l}} (r,\theta,\rho) = E_{n}  \phi_{nlm_{l}} (r,\theta,\varphi)$$
$$\phi_{nlm_{l}} (r,\theta,\rho) = R_{nl}(r) Y(\theta,\varphi)$$
- $\hat H$, $\hat L^{2}$, $\hat L_{z}$ commute, which gives the conservation of angular momentum
- electron in a hydrogen atom:
$$\begin{gather}
\hat L^{2} Y_{lm_{l}} (\theta,\varphi) = l(l+1)\hbar^{2} Y_{lm_{l}} (\theta, \varphi) \\
\hat L_{z} Y_{lm_{l}} (\theta,\varphi) = m_{l}\hbar Y_{lm_{l}} (\theta, \varphi)
\end{gather}$$
- reminder: $l \in \mathbb Z$ up to $n-1$, $m_{l} \in [-l,  l]$

- graft on spin (electrons  = $1/2$, fermions): $\phi_{nlm_{l} \uparrow} (r, \theta, \varphi) \; , \;\phi_{nlm_{l} \downarrow} (r, \theta, \varphi)$
- for $n=2:$ 
	- $l=0, \; m_{l}= 0, \; \uparrow \downarrow$
	- $l=1, \; m_{l}= -1,0,1 \; ,\; \uparrow \downarrow$
	- this is eight fold degenerate
- for a many-electron system, electrons cannot occupy the same state in space unless they have different spin states - [[content/012/PX284 - SMETO/part 1 - statistical mechanics/L - exchange symmetry/PX284 - L2 - pauli exclusion principle\|pauli exclusion principle]]

- using the hydrogen atom to set up a model of other atoms:
$$\begin{gather}
V(r) = - \frac{e^{2}}{4\pi\varepsilon_{0}r} \\
E_{n} = - \frac{13.6}{n^{2}}\text{eV} \\
\end{gather}$$
- the model of an atom (Z-atomic number) has each of its ${} Z$ electrons moving in a potential set up by the positively charged nucleus and a symmetric cloud of negative charges from the other ${} (Z-1)$ electrons
- the net potential falls off more quickly than straight coulombic potential, ie. $-\cfrac{Ze^{2}}{4\pi\varepsilon_{0}r}$ close to the nucleus, and $-\cfrac{e^{2}}{4\pi\varepsilon_{0}r}$ far away 
- so an electron in a state which is distributed, on average, close to the nucleus will 'see' a higher charge on the nucleus than one in a state distributed further away
- this removes degeneracy of energy levels with respect to the angular momentum
- the order of the energies is such that the s-orbitals $l=0$ have lower energies than the p-orbitals $(l=1)$ and so on

- example: for sodium $Z = 11$
$$\begin{gather}
n = 1 & l = 0 & 1s^{2} & \uparrow\downarrow & 2 \\\\
n = 2 & l = 0 & 2s^{2} & \uparrow\downarrow & 2 \\
& l =1 & 2p^{6} & \uparrow\downarrow & 6 \\\\
n = 3 & l = 0 & 3s^{1} & & 1 &\text{(valence)}\\
\end{gather}$$

- example: for iron $Z = 23$
$$\begin{gather}
n = 1 & l = 0 & 1s^{2} & \uparrow\downarrow & 2 \\\\
n = 2 & l = 0 & 2s^{2} & \uparrow\downarrow & 2 \\
& l =1 & 2p^{6} & \uparrow\downarrow & 6 \\\\
n = 3 & l = 0 & 3s^{1} & \uparrow\downarrow & 1\\
& l =1 & 3p^{6} & \uparrow\downarrow & 6 \\
& l =2 & 3d^{6} & \uparrow\downarrow & 6/7 \\\\
n=4 & l =1 & 4s^{2} & \uparrow\downarrow & 2/1
\end{gather}$$
