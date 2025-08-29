---
{"dg-publish":true,"permalink":"/content/012/px-280-environmental-physics/b-light-and-matter/px-280-b5-bear-lambert-law/","noteIcon":"1","created":"2025-08-27T13:15:22.684+01:00","updated":"2025-01-16T11:38:06.000+00:00"}
---

![PX280 - B5 - bear-lambert law.png|500](/img/user/pics/PX280%20-%20B5%20-%20bear-lambert%20law.png)
*image: E. Broeker & R. van Grondelle*, Environmental Physics (2011)

- consider a light beam absorbed by a thin slice of material
- due to absorption, the energy density will depend on $\omega, z, t$, ie: $W(\omega, z, t)$ 
- beam energy in the frequency interval, $\omega$ to $\omega + d\omega$, is:
 $$W(\omega, z, t) \,d\omega \cdot a\,dz$$
	where, the first term is the density of energy in the slice due to photon in range, and the second term is the volume of slice

- from equation $(7):$
$$\frac{dN_{1}}{dt} = - B_{2} W(\omega) N_{2} + A_{21}N_{2}$$

- ignoring simulated emission:
$$\implies \frac{dN_{1}}{dt} = -B_{12} W(\omega)N_{1}$$
- rate of energy loss of beam  slice = rate of energy absorbed by material of the slice
$$\boxed{\frac{\partial W}{\partial t}\cdot a\,dz\,d\omega  = B_{12}N_{1} \left(\frac{a\,dz}{V}\right)F(\omega)\,d\omega \, W(\omega, z)\,\hbar\omega} \tag{8}$$

	where, $a\,dz$ is the volume of the slice, and $V$ is the total volume of the sample, which replaced population $N_1$ in equation before with fraction within slice: $N (\cfrac{a\,dz}{V})$

- equation $2$ was rate of absorption, $[\text{s}^{-1}]$
- connected to energy absorbed per second by multiplying with $\hbar \omega$

- in practice, the atom/molecule may absorb over a range ('band') of frequencies centered on $\omega$
- therefore, a 'weight factor' is introduced:
$$\boxed{\int F(\omega)\,d\omega = 1} \tag{9}$$

- rearranging equation $(8):$
$$\boxed{\frac{\partial W}{\partial t} = - N_{1}F(\omega) B_{12} W \frac{\hbar\omega}{V}} \tag{10}$$

- in practice, the light intensity is of interest rather than the energy density

- the energy loss in the slice over a time, $dt =$ decrease of beam intensity over the slice
$$- \frac{\partial W}{\partial t}\,d\omega\,a\,dz = \underbrace{[I(z) - I(z+dz)]}_{I(\omega) \, d\omega} \,d\omega\,a = - \frac{\partial I}{\partial z}\,dz \, a\,d\omega$$
$$\implies \boxed{\frac{\partial W}{\partial t} = \frac{\partial I}{\partial z}}$$

$$\implies \frac{\partial I}{\partial z} = - N_{1}F(\omega) B_{12}W \frac{\hbar\omega}{V}$$
- intensity $[\text{J m}^{-2}]$ and energy density ${} [\text{J m}^{-3}]$ of beam:
$$W = \frac{In}{c}$$
	where, $n$ is the refractive index
$$\frac{\partial I}{\partial z}  = \frac{-B_{12}N_{1}-\hbar\omega F(\omega)n}{Vc} I = \kappa I$$
	where, $\kappa$ is independent of $z$
- $\kappa$ is the absorption cofficient:
$$\kappa = \frac{-B_{12}N_{1}-\hbar\omega F(\omega)n}{Vc} $$

$$\boxed{\therefore I(z) = I(0)e^{-\kappa z}} \tag{12}$$

