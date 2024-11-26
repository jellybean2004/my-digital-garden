---
dg-publish: true
---

- *[[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C1 - ideal gas equation of state#ideal gas law\|ideal gas equation]]* does not predict liquification
	-  as the conditions approach $gas\to liquid/solid$ phase boundary, it fails to predict the observed properties
## things to consider
### molecules have finite volume
- eg: $1m^3 \; N_2$ gas at $STP$
	- $STP=$ "standard temperature and pressure" $=1.013\times 10^{5}Pa / 1atm$ and $0 \degree C (or \; 20 \degree C)$
	- the volumes of the molecules is $0.00075 m^3$
		- $1m^3=1000l\implies V=0.75l$
		- effect of $V$ in these conditions on observed gas properties can be assumed to be negligible 
		- as we reduce $V(density=n/V \;increases)$, and $V$ becomes significant
	- in the [[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C1 - ideal gas equation of state#ideal gas law\|ideal gas equation]], we replace $V$ with $(V-nb)$
		- where, 
			$n=$ number of moles
			$b=$ "*co-volume*" (represents the volume occupied by a mole of molecules)
### intermolecular forces
- in an ideal gas, molecules collide *elastically* and don't interact otherwise
- now, we allow for interactions between the molecules (eg: lennard-jones potential)
- we replace $p$ with $(p + a \frac{n^{2}}{V^{2}})$
	- where,
		$a$ is a constant
			$\frac{n^{2}}{V^{2}}= density^2$
		- further reading [grant+phillips : elements of physics]
## van der waal's equation of state

$$\left(p+ \frac{an^{2}}{V^{2}}\right)(V-nb)=nRT$$
- at high volumes/low densities, it is well approximate by the *[[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C1 - ideal gas equation of state#ideal gas law\|ideal gas law]]*
 