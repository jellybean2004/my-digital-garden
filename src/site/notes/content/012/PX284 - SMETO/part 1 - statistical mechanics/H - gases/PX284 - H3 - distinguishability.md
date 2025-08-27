---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/h-gases/px-284-h3-distinguishability/","noteIcon":"1","created":"2025-08-27T13:15:24.658+01:00","updated":"2025-01-13T10:31:16.000+00:00"}
---

- considering a single particle in  a two-state system
- there are two possible configurations:
![PX284 - H3 - distinguishability.png|500](/img/user/pics/PX284%20-%20H3%20-%20distinguishability.png)
$$Z_{1} = e^{0} + e^ {-\beta \varepsilon} $$

- now, considering two *distinguishable* particles in the same system:
![PX284 - H3 - distinguishability-2.png|500](/img/user/pics/PX284%20-%20H3%20-%20distinguishability-2.png)
$$Z_{1} = e^{0} + 2e^{-\beta \varepsilon} + e^{-2\beta \varepsilon} = Z_{1} ^{2}$$

- similarly, for $N$ distinguishable particles:
$$Z_{N }= Z_{1} ^{N}$$

- now, considering two *indistinguishable* particles:
![PX284 - H3 - distinguishability-1.png|500](/img/user/pics/PX284%20-%20H3%20-%20distinguishability-1.png)
$$Z_{2} = e^{0} + e^{-\beta \varepsilon} + e^{-2\beta\varepsilon}$$
- therefore, for indistinguishable particles:
$$Z_{N }\neq Z_{1}^{N}$$
- in fact, $Z_{1}^{N}$ overcounts the number of states in which $N$ particles sit in different energy levels by a factor of $N!:$
$$Z_{N} = \frac{Z_{1}^{N}}{N!}$$
	provided that the configurations wherein more than one particles are in a state can be neglected
- this can only be done if $n \gg n_{a}$, ie. no wavefunction overlap, so a classical gas

| example                                     | type              |
| ------------------------------------------- | ----------------- |
| H$_2$ molecules at RTP                      | indistinguishable |
| spins on a regular lattice<br>(paramagnets) | distinguishable   |
