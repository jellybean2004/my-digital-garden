---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/h-many-particles/px-262-h11-molecules/","noteIcon":"1","created":"2025-01-30T10:30:05.368+00:00","updated":"2025-01-30T12:02:37.140+00:00"}
---

- **approximation:** neglecting the kinetic energy o the nuclei and solving the electronic problem
- nuclei take the positions where the sum of electronic energy and nuclear coulomb energy is minimized, electrons bond the nuclei
- types of bonding:
	- covalent
	- ionic

- considering a covalent bond in H$_{2}$
- the two protons are fixed at $\vec R_{A}$ and $\vec R_{B}$, and the two electrons at $\vec r_{1}$ and $\vec r_{2}$
- the distance from $B$ to ${} A: {}$ ${} \vec R = \vec R_{A} - \vec R_B$
- building a model of the electrons' ground state from hydrogen states which complies with [[content/012/PX284 - SMETO/part 1 - statistical mechanics/L - exchange symmetry/PX284 - L2 - pauli exclusion principle\|pauli exclusion principle]]
## covalent bond
- for one hydrogen atom:
$$\phi_{100, \sigma}^{A} (\vec r_{1}) = \frac{1}{\sqrt{\pi a_{0}^{3}}} \exp\left( - \frac{|\vec r_{1} - \vec R_{A}|}{a_{0}}\right)$$
	where, $\sigma = \uparrow , \,\downarrow$

- in the molecule, approximating the ground state two electron wavefunction:
$$\phi(\vec r_{1}, \sigma_{1} , \vec r_{2}, \sigma_{2}) = C(R) \underbrace{(\phi_{100}^{A} (\vec r_{1})  \, \phi_{100}^{B} (\vec r_{2}) + \phi_{100}^{A}(\vec r_{2}) \, \phi_{100}^{B} (\vec r_{1}))}_\text{spatial} \times \underbrace{(u_{1\uparrow} \, u_{2\downarrow} - u_{1\downarrow} \, u_{2\uparrow})}_\text{spin}$$

- the charge is concentrated between the protons and each electron is more delocalized than in an isolated atom

#fig 

- $R_{0}$ is the bond length in the H$_2$ molecule $\sim 0.74$ Å
