---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/q-maxwell-s-equations-in-matter/px-284-q1a-polarization/","noteIcon":"1","created":"2025-02-20T15:22:41.676+00:00","updated":"2025-02-24T16:54:21.240+00:00"}
---

- considering an atom: a positively charged nucleus ($+q$) surrounded by a negatively charged cloud $(-q)$
- if an electric field is applied, $+q$ and $-q$ shift in opposite directions, by a distance, $s$, ie. a dipole: $\vec P = q \vec s$
- now, considering in a larger scale, with many atoms
- defining polarization as the net dipole moment per unit volume:
$$\vec P = \frac{ \sum\limits_{i}\vec  P_{i}}{V}$$

- considering a polarizable material 
- upon exposure to an electric field, it will have an excess of positive charges in one end, and an excess of negative in the other
- the surface charge density:
$$\sigma_{P} = \frac{Q}{A} = \frac{(qn)\times(As)}{A} $$
	where, $q$ is the charge of an atom, $n$ is the number density, $A$ is the area, and $s$ is the displacement, so $As$ is the volume

$$\implies \sigma_{P}  = qns = |\vec P|$$
- in general:
$$\sigma_{P} = \vec P \cdot \hat n$$
	where, $\hat n$ is the outward facing unit normal to the surface

- now considering a non-uniform polarization
- two small cuboids centred at $x_0$, separated by $\delta x$

![PX284 - Q1 - polarization.png|500](/img/user/pics/PX284%20-%20Q1%20-%20polarization.png)

$$Q(x_{0})= A \left(P_{x}\left(x_{0} - \frac{\delta x}{2}\right) - P_{x}\left(x_{0}+ \frac{\delta x}{2}\right)\right)$$
- using taylor's theorem:
$$f(x) \simeq f(x_{0}) + \delta x \frac{df}{dx}\bigg|_{x=0} + \dots$$
$$Q(x_{0}) \simeq - A \delta_{x} \frac{\partial P_{x}}{\partial x} \bigg|_{x_{0}}$$
- volume charge density:
$$\rho_{P} = \frac{Q}{A\delta x} = - \frac{\partial P_{x}}{\partial x}\bigg |_{x_{0}}$$
- including contributions from ${} P_y$ and ${} P_z:$
$$\rho_{P} = - \vec\nabla\cdot\vec P$$
- differentiating it, the polarization current is obtained (and the continuity equation):
$$\frac{\partial \rho_{P}}{\partial t} + \vec\nabla \cdot \vec J_{P} = 0$$
	where, $\vec J_{P} = \cfrac{\partial \vec P}{\partial t}$ is the polarization current density

- in many materials:
$$|\vec P | \propto |\vec E|$$
- $\vec P \propto \vec E$ - 'linear', usually true at low $|\vec E|$ 

- 'isotropic':
$$\vec P \parallel \vec E \implies \vec P = \varepsilon_{0} \chi \vec E $$
	where, $\chi$ is the susceptibility

$$\vec E = \vec E_{applied} + \vec E_{P} = \vec E_{applied} - \chi \vec E$$
$$\vec E = \frac{\vec E_{app}}{1+\chi} = \frac{\vec E_{app}}{\varepsilon_{r}}$$
	where, $\varepsilon_{r}$ is called the relative permittivity
