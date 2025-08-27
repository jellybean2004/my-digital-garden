---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/j-atoms-and-molecules/px-262-j3-molecules/","noteIcon":"1","created":"2025-08-27T13:15:23.304+01:00","updated":"2025-03-13T12:26:21.000+00:00"}
---

- **approximation:** neglecting the kinetic energy of the nuclei and solving the electronic problem
- nuclei take the positions where the sum of electronic energy and nuclear coulomb energy is minimized, electrons bond the nuclei
- types of bonding:
	- covalent
	- ionic
- considering a covalent bond in H$_{2}$
- the two protons are fixed at $\vec R_{A}$ and $\vec R_{B}$, and the two electrons at $\vec r_{1}$ and $\vec r_{2}$
- the distance from $B$ to ${} A: {}$ ${} \vec R = \vec R_{A} - \vec R_B$
- building a model of the electrons' ground state from hydrogen states which complies with the [[content/012/PX284 - SMETO/part 1 - statistical mechanics/L - exchange symmetry/PX284 - L2 - pauli exclusion principle\|pauli exclusion principle]]
## covalent bond
- for one hydrogen atom:
$$\phi_{100, \sigma}^{A} (\vec r_{1}) = \frac{1}{\sqrt{\pi a_{0}^{3}}} \exp\left( - \frac{|\vec r_{1} - \vec R_{A}|}{a_{0}}\right)$$
	where, $\sigma = \uparrow , \,\downarrow$

- in the molecule, approximating the ground state two electron wavefunction:
$$\phi(\vec r_{1}, \sigma_{1} , \vec r_{2}, \sigma_{2}) = C(R) \underbrace{(\phi_{100}^{A} (\vec r_{1})  \, \phi_{100}^{B} (\vec r_{2}) + \phi_{100}^{A}(\vec r_{2}) \, \phi_{100}^{B} (\vec r_{1}))}_\text{spatial} \times \underbrace{(u_{1\uparrow} \, u_{2\downarrow} - u_{1\downarrow} \, u_{2\uparrow})}_\text{spin}$$
- the charge is concentrated between the protons and each electron is more delocalized than in an isolated atom
- $R_{0}$ is the bond length in the H$_2$ molecule $\sim 0.74$ Å

![PX262 - H11 - molecules.png|500](/img/user/pics/PX262%20-%20H11%20-%20molecules.png)

## ionic bond
- for a NaCl molecule:
	Na : $1s^{2}\; 2s^{2}\, 2p^{6}\; 3s^{1}$
	Cl : $1s^{2}\; 2s^{2}\, 2p^{6}\; 3s^{2}\, 3p^{5}$

- the molecule is well described by the Na $3s^1$ valence electron transferring to the Cl $3p$ shell so that both atoms have filled shell configurations
- Na becomes positively charged, and Cl, negatively 
- this is called an **ionic bond**
