---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-2-fluid-dynamics/j-some-approximate-solutions/px-285-j2-hydrostatic-limit-and-archimedes-principle/","noteIcon":"1","created":"2025-02-01T13:36:21.989+00:00","updated":"2025-02-01T13:52:24.037+00:00"}
---


- bernoulli's principle can be applied between any two points in the fluid:
$$P + \rho gz = \text{constant}$$
- considering an object submerged in water
- the depth of water is $z_{1}$
- air above the water exerts atmospheric pressure, $P_{atm}$

- from bernoulli's principle:
$$P(z) = P_{atm} + \rho g (z_{1}- z)$$
- $z_{1}$ can be taken to be zero, and $P_{atm}$ is constant

- the total upward force on the object, which is the projection of the force on the z-axis
$$\newcommand{\oiint}{\subset\!\supset \!\!\!\!\!\!\!\!\!\!\iint}
\vec F \cdot \hat k = - \oiint_{S} P(z) \hat k \cdot d\vec s = - \iiint_{V} \vec\nabla\cdot ( P(z) \hat k) \, dV$$
	where, $S$ is the surface of the object, and $d\vec s$ is pointed outwards; $V$ is the volume of the object

- using bernoulli's principle:
$$\iiint_{V} \vec\nabla \cdot (\rho gz \hat k ) dV = \iiint_{V}\rho g \, dV = g \iiint_{V}\rho\, dV = Mg$$
	where, $\vec\nabla\cdot z \,\hat k =1$

>[!note] archimedes' principle
> the vertical force on a submerged object is equal to the weight of the fluid displaced by the object
>$$\vec F \cdot \hat k = \iiint_{V} \rho\, dV\,g = Mg$$
> 	where, $\rho$ and $M$ are the density and the mass of the fluid

