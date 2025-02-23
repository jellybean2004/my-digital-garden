---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/p-em-waves/px-284-p4-em-waves-in-matter/","noteIcon":"1","created":"2025-02-20T15:22:41.676+00:00","updated":"2025-02-20T17:39:16.371+00:00"}
---

## polarization

- considering an atom: a positively charged nucleus ($+q$) surrounded by a negatively charged cloud $(-q)$
- if an electric field is applied, $+q$ and $-q$ shift in opposite directions, by a distance, $s$, ie. a dipole: $\vec P = q \vec s$

- considering in a larger scale, with many atoms
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
$$Q(x_{0)}= A \left(P\left(x_{0} - \frac{\delta x}{2}\right) - P\left(x_{0}+ \frac{\delta x}{2}\right)\right)$$
- using taylor's theorem:
$$f(x = f(x_{0})) + \delta x \frac{df}{dx}\bigg|_{x=0} + \dots$$
$$Q(x_{0}) \simeq - A \delta_{x} \frac{\partial P}{\partial x} \bigg|_{x_{0}}$$
- volume charge density:
$$\rho_{P} = \frac{Q}{A\delta x} = - \frac{\partial P}{\partial x}\bigg |_{x_{0}}$$
- including contributions from ${} P_y$ and ${} P_z:$
$$\rho_{P} = - \vec\nabla\cdot\vec P$$

- polarization current (and continuity equation):
$$\frac{\partial \rho_{P}}{\partial t} + \vec\nabla \cdot J_{P} = 0$$
	where, $\vec J_{P} = \cfrac{\partial \vec P}{\partial t}$ is the polarization current density

- in many materials:
$$|\vec P | \propto |\vec E|$$
- $\vec P \propto \vec E$ - 'linear', usually true at low $|\vec E|$ - 'isotropic'

$$\vec P \parallel \vec E \implies \vec P = \varepsilon_{0} \chi \vec E $$
	where, $\chi$ is the susceptibility

$$\vec E_{total} = \vec E_{applied} + \vec E_{P} = \vec E_{applied} - \chi \vec E$$
$$\vec E = \frac{\vec E_{app}}{1+\chi} = \frac{\vec E_{app}}{\varepsilon_{r}}$$
	where, $\varepsilon_{r}$ is called the relative permittivity
#fig

- applying gauss' law:
$$|\vec E_{P}| \times 2A = \sigma_{P} \frac{A}{\varepsilon_{0}} = |\vec P| \frac{A}{\varepsilon_{0}}$$

- total polarization field inside the stab:
$$\vec E_{P} = - \frac{|\vec P|}{2\varepsilon_{0}} - \frac{|\vec P|}{2\varepsilon_{0}} = - \frac{|\vec P|}{\varepsilon_{0}}$$
- total field:
$$\begin{align*}
\vec E &= \vec E_{app} + \vec E_{P} \\
\vec E_{app} - \chi \vec E  &= \vec E_{app} - \frac{\vec{P}}{\varepsilon_{0}} \\
\implies \vec E = \frac{\vec{E}_{app}}{1+\chi} &= \frac{\vec E_{app}}{\varepsilon_{r}}
\end{align*}$$
- reduction of $\vec E_{app}$ to $\vec E$ is called 'screening' $\vec E_{P}$ 
#incomplete 

- for geometries other than a slab (cuboid), eg: an ellipsoid
$$\vec E_{P} = - \alpha \frac{\vec P}{\varepsilon_{0}}$$
#incomplete 

