---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/l-semiconductors/px-262-l1-introduction-to-semiconductors/","noteIcon":"1","created":"2025-02-17T11:14:53.392+00:00","updated":"2025-02-17T13:02:59.762+00:00"}
---

- exploring why some materials show such a drastic bias to the direction of emf

![PX262 - I1 - introduction to semiconductors.png|500](/img/user/pics/PX262%20-%20I1%20-%20introduction%20to%20semiconductors.png)
![PX262 - I1 - introduction to semiconductors-1.png|500](/img/user/pics/PX262%20-%20I1%20-%20introduction%20to%20semiconductors-1.png)
 ![PX262 - I1 - introduction to semiconductors-2.png|500](/img/user/pics/PX262%20-%20I1%20-%20introduction%20to%20semiconductors-2.png)

- for $T \neq 0$ K, the [[content/012/PX284 - SMETO/part 1 - statistical mechanics/L - exchange symmetry/PX284 - L3 - distribution functions#^e2328b\|fermi-dirac function]]:
$$F(E, \mu, T) = \frac{1}{\exp\left(\frac{E-\mu}{k_{B}T} +1\right)}$$
- such that:
$$N = \int_{-\infty} ^{\infty} F(E,\mu, T) n(E)\, dE$$
	where, $N$ is the number of electrons, and $\mu (\simeq E_{F}\simeq E_{V} + \Delta/2)$ is the chemical potential

- each atom in group IV elements: C, Si, Ge, has  core of electrons, tightly bound to the nuclei and four loosely bound valence electrons

| element   | core                                      | valence            |
| --------- | ----------------------------------------- | ------------------ |
| $^6$C     | $1s^{2}$                                  | $2s^{2} \, 2p^{2}$ |
| $^{14}$Si | $1s^{2}\,2s^2\,2p^6$                      | $3s^2\,3p^2$       |
| $^{32}$Ge | $1s^{2}\,2s^2\,2p^6\,3s^2\,3p^6\,3d^{10}$ | $4s^2\,4p^2$       |

- considering Si: $\Delta = 1.1$ eV $=E_{C}= E_V$
- at $T= 300$ K, $\mu \simeq E_{F} = E_{V} + \Delta/2$
$$F = \frac{1}{\exp((E_{C}-E_{V}-\Delta/2)/k_{B}T)+1}= \frac{1}{\exp(\frac{\Delta}{2k_{B}T} +1)}\simeq e^-20$$

- this is very small
- therefore, semiconductors need to be **doped** to conduct easily, ie. add impurities
