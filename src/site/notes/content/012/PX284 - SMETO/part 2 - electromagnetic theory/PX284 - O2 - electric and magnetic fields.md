---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/px-284-o2-electric-and-magnetic-fields/","noteIcon":"1","created":"2025-02-12T09:49:06.088+00:00","updated":"2025-02-13T15:26:26.879+00:00"}
---

- electric ($\vec E(\vec r, t)$) and magnetic ($\vec B(\vec r, t)$) are vector fields that affect charged particles, given by the [[content/011/PX157 - electricity and magnetism/PX157 - C - magnetic fields/PX157 - C1a - the lorentz force\|lorentz force]]:
$$\vec F = q (\vec E + \vec v \times \vec B)$$

## maxwell's equations (integral form)
### gauss' law
- [[content/011/PX157 - electricity and magnetism/PX157 - B - electric fields/I - field/PX157 - B5a - gauss's law\|PX157 - B5a - gauss's law]]
- the electric field through a closed surface is given by:
$\newcommand{\oiint}{\subset\!\supset \!\!\!\!\!\!\!\!\!\!\iint}$
$$\oiint_{S} \vec E \cdot d\vec S = \frac{Q_\text{encl.}}{\varepsilon_{0}} = \iiint_{V} \frac{\rho}{\varepsilon_{0}} \, dV $$
	where, 
		$Q_\text{encl.}$ is the charge enclosed by the surface $S$,
		$\varepsilon_{0}$ is the permittivity of free space,
		$\rho$ is the charge density,
		$V$ is the volume enclosed by the surface $S$.
### solenoidal condition
-  AKA the **'law with no name'**
- the magnetic field through a closed surface is given by:
$$\oiint_{S} \vec B \cdot d\vec S = 0$$
- this says that there are no **magnetic monopoles**, ie. magnetic charges
### faraday-lenz law
- the emf around a circuit is given by:
$$\epsilon = \oint_{C} \vec E \cdot d\vec l = - \frac{d}{dt} \iint_{S} \vec B \cdot d\vec S$$
- ie. it is the rate of change of magnetic flux
### ampere's law
- the magnetic field around a closed loop is given by:
$$\oint_{C}\vec B \cdot d\vec l = \mu_{0} I_\text{encl.} = \mu_{0} \iint_{S} \vec J \cdot d\vec S$$
	where, $I_\text{encl.}$ is the current enclosed by the loop, $\mu_0$ is the permeability of free space, and $\vec J$ is the current density
