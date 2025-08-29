---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-1-statistical-mechanics/m-fermions/px-284-m4-heat-capacity/","noteIcon":"1","created":"2025-08-27T13:15:24.884+01:00","updated":"2025-02-03T19:46:17.000+00:00"}
---

- the only accessible empty energy states are those close to $E_F$
- only the electrons very close to $E_F$ can change their momenta and carry any electrical/thermal energy
- at $T>0$, $f_{FD}$ is not a step function, but 'smeared out' by $\sim k_{B}T$, where $k_{B}T \ll E_F$

![PX284 - M4 - heat capacity.png|500](/img/user/pics/PX284%20-%20M4%20-%20heat%20capacity.png)

- roughly, the fraction of electrons that gain energy at $T \sim \cfrac{k_{B}T}{E_{F}}$
- so, the energy gained $\sim k_{B}T$
- the internal energy due to $T>0:$
$$U = N \frac{k_{B}T}{E_{F}}k_{B}T \simeq \frac{Nk_{B}^{2}T^{2}}{E_{F}}$$
$$\therefore C_\text{electron} \simeq 2 \frac{Nk_{B}^{2}T}{E_{F}}$$
- the full solution is: $c_\text{electron} =  \cfrac{\pi^{2}}{2} \cfrac{Nk_{B}^{2}T}{E_{F}}$

- therefore, for a metal at low temperature:
$$C_{total} = C_{electron} + C_{lattice} = \alpha \left(\frac{T}{T_{F}}\right) + \beta \left( \frac{T}{\theta_{D}}\right)^{3}$$
	where, ${} C_{lattice}$ comes from the [[content/012/PX284 - SMETO/part 1 - statistical mechanics/K - phonons/PX284 - K2 - debye model\|debye model]]

- so, $C_{lattice}$ dominates, except at very low temperatures