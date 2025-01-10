---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/h-introduction-to-fluids/px-285-h5-fluid-element/","noteIcon":"1","created":"2025-01-10T12:36:43.533+00:00","updated":"2025-01-10T12:51:54.815+00:00"}
---

- a fluid element is a parcel of a fluid, which can be visualised by some shape, eg: a cube
- it moves with a flow and may deform in time, but the same molecules remain in the parcel and its mass remains the same

![[Pasted image 20250110124028.png\|500]]

- two approaches to fluid parcels:
	- lagrangian
	- eulerian
## lagrangian
- a lagrangian fluid element moves with the fluid in such a way, into or out of the element
- constant mass
- the velocity depends only on time

![PX285 - H5 - fluid element-1.png|500](/img/user/pics/PX285%20-%20H5%20-%20fluid%20element-1.png)

- the displacement:
$$\vec s = \vec r(t) - \vec r_0$$
- therefore, the velocity: 
$$\vec u = \frac{d}{dt}(\vec r(t) - \vec r_{0}) = \frac{dx}{dt}\hat i + \frac{dy}{dt}\hat j + \frac{dz}{dt}\hat k$$
- the lagrangian coordinate system is fixed with a fluid
## eulerian 
- it is fixed in space and does not move with the flow
- the velocity:
$$\vec u = \vec u (t, \vec r)$$
- the flow can come into this element or go out
- so, the eulerian coordinate system remains the same, whereas the lagrangain system deforms with the fluid

- eg: 
	- "a cold wind is coming from scotland" - lagrangian
	- "in coventry, the wind is $10$ ms$^{-1}$" - eulerian

