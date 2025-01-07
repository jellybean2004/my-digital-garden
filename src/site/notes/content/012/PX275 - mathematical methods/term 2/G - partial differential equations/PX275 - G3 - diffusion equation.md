---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/g-partial-differential-equations/px-275-g3-diffusion-equation/","noteIcon":"1","created":"2025-01-07T12:41:44.605+00:00","updated":"2025-01-07T19:44:08.444+00:00"}
---

- considering the **diffusion problem**: spatial and temporal variation of a density function, $\rho(x,t)$
- with $N$ particles in a volume, $V$, the volume density, $n = \cfrac{N}{V}$, is the number of particles per unit volume (3D)

- many cases can be considered in 1D

![PX275 - G3 - diffusion equation.png|500](/img/user/pics/PX275%20-%20G3%20-%20diffusion%20equation.png)
- considering a bar of length, $L$, and cross-section, $A$, with only one variation in the spatial dimension, say $x$
- the concentration of particle: $c = n \times A$
- $c(x,t)$ describes the physical (1D) concentration of particles in this  medium at $x$ and $t$
- the number of particles in the red box: $N = c\Delta x$
- in general:
$$N = \int_{0}^{L} c(x,t)\,dx$$
- if there is no source or sink, $N$ is constant

![PX275 - G3 - diffusion equation-1.png|500](/img/user/pics/PX275%20-%20G3%20-%20diffusion%20equation-1.png)

- diffusion acts to reduce gradients in concentration
- gradients will lead to a flux of particles

![PX275 - G3 - diffusion equation-2.png|500](/img/user/pics/PX275%20-%20G3%20-%20diffusion%20equation-2.png)
