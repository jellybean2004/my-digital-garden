---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/i-electronic-configurations/px-262-i11-energy-gaps/","noteIcon":"1","created":"2025-02-13T10:07:46.655+00:00","updated":"2025-03-02T11:53:57.264+00:00"}
---

- free electrons have the wave functions of the form: ${} \psi = A_{k}e^{ikx} {}$, where $k \in (-\infty, \infty)$
- the energies are given by:so 
$$E_{k} = \frac{\hbar^{2}k^{2}}{2m_{e}}$$
- linear combinations: $\phi_{k}^{+} = C_{k} \cos(kx)$ and ${} \phi_{k}^{-} = D_{k} \sin(kx) {}$
- these correspond to the same energy, $E_{k}$

- a 1D lattice will have the separations of $a$, and its reciprocal lattice, $2\pi/a$
- in the k-space, the first BZ: $-\pi/a \leq k \leq \pi/a$
- looking at the free electron wavefunctions' intensities with $k = \pm \pi/a$ (values at the edges of the BZ): $|\phi_{\pi/a}^{+}|^{2}$ and $|\phi_{\pi/a}^{-}|^{2}$

![PX262 - H19 - energy gaps.png|500](/img/user/pics/PX262%20-%20H19%20-%20energy%20gaps.png)

- when potentials are placed on each of the lattice points, the energy degeneracy is broken, since $|\phi_{\pi/a}^{+}|^{2}$ is distributed more closely to the potentials than the $|\phi_{\pi/a}^{-}|^{2}$ solution
- energy gaps at $k = \pm \pi/a$ are produced at the BZ boundaries
- if the [[content/012/PX262 - quantum mechanics/term 2/H - many particles/PX262 - H3 - free electron model (1D)\|free electron model (1D)]] is perturbed by a weak crystalline potential, the electronic states change 

 

- this can be plotted in the first BZ, with $k' = k - G_{n}$ ie. folding back, $G_{n} = -n\pi/a$ or ${} n\pi/a$

![PX262 - H19 - energy gaps-2.png|500](/img/user/pics/PX262%20-%20H19%20-%20energy%20gaps-2.png)

- a complementary insight can be obtained by starting with a model of a large number, $N$, of identical atoms, which are well separated. eg: Li: $1s^{2}\; 2s^{1}$
- each atom potential has a set of electronic energy levels for the valence electrons, eg: $2s\,2p \; 3s \dots$
- the energy level diagram for the whole system is set by that of a single atom, but the [[content/012/PX284 - SMETO/part 1 - statistical mechanics/L - exchange symmetry/PX284 - L2 - pauli exclusion principle\|pauli exclusion principle]] for the entire system permits each state to be occupied by up to $2N$ (2 for spin) electrons

![PX262 - H19 - energy gaps-4.png|500](/img/user/pics/PX262%20-%20H19%20-%20energy%20gaps-4.png)

- if the atoms are pushed closer together, the wavefunctions of the electrons distort and extend over more atoms
- the outermost valence electronic states accommodate $2N$ in a band of $N$ tightly spaced levels

![PX262 - H19 - energy gaps-5.png|500](/img/user/pics/PX262%20-%20H19%20-%20energy%20gaps-5.png)

- the schematic for valence electrons of Li:

![PX262 - H19 - energy gaps-7.png|500](/img/user/pics/PX262%20-%20H19%20-%20energy%20gaps-7.png)
![PX262 - H19 - energy gaps-8.png|500](/img/user/pics/PX262%20-%20H19%20-%20energy%20gaps-8.png)

- the two figures above show how, in some materials, the DOS develops a gap at the fermi energy

![PX262 - H19 - energy gaps-9.png|500](/img/user/pics/PX262%20-%20H19%20-%20energy%20gaps-9.png)


- such a material is insulating
- there are no states near $E_F$, no low-lying excitations and no conduction

- the specific heat has no electronic contribution for $k_{B}T < \Delta$
- the material is also transparent to light, with $\hbar \omega = {hc}/{\lambda} < \Delta$ and only photons with $\hbar \omega = {hc}/{\lambda} > \Delta$ will be blocked

- a material is termed as an **insulator** if $\Delta > 2$ eV, and for $\Delta \ge \sim2$ eV, the material is a **semiconductor**
