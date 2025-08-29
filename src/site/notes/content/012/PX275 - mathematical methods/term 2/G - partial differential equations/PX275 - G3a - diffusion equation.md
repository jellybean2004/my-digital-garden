---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/g-partial-differential-equations/px-275-g3a-diffusion-equation/","noteIcon":"1","created":"2025-08-27T13:15:23.624+01:00","updated":"2025-01-23T18:52:21.000+00:00"}
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

![PX275 - G3a - diffusion equation.png|500](/img/user/pics/PX275%20-%20G3a%20-%20diffusion%20equation.png)

- considering the particle flux, $j(x)$, then the net flux $=$ number of particles moving right - number of particles moving left
- **fick's law:**
$$j(x)\propto - \frac{\partial c}{\partial x}$$

	where, ${} j(x)$ is the local flux at $x$, and the negative sign works to reduce the gradient, $\frac{\partial c}{\partial x}$
- the proportionality constant is defined to be $D$, the diffusivity of the medium:
$$j(x) = - D \frac{\partial c}{\partial x}$$
- the continuity must be satisfied
- considering a small part, $\Delta x$
- the change in the number of particles over $\Delta x$ at a fixed time:
$$\Delta j = j (x,t) - j(x + \Delta x ,t )$$
- over time, $\Delta t:$
$$\Delta j \, \Delta t= [j (x,t) - j(x + \Delta x ,t)]  \Delta t \tag{1}$$
- recalling that $N=c\Delta x$, so the change in the number within $\Delta x$ across time, $\Delta t$, is:
$$-[c(x,t) - c(x, t + \Delta t)] \Delta x \tag{2}$$
- combining equation $(1)$ and $(2):$
$$\begin{gather}
[j (x,t) - j(x + \Delta x ,t)]  \Delta t = -[c(x,t) - c(x, t + \Delta t)] \Delta x \\\\
\Delta j \, \Delta t= - \Delta x\, \Delta c
\end{gather}$$
$$\lim_{\Delta x, \Delta t \to 0} \frac{\partial j}{\partial x} = - \frac{\partial c}{\partial t}$$
- from fick's law:
$$\boxed{\frac{\partial c}{\partial t} = D \frac{\partial^{2} {c}}{\partial {x}^{2}}}$$
- this is the diffusion equation for a 1D concentration field, $c(x,t)$, in a medium with a constant diffusivity, $D$

![PX275 - G4 - wave equation.png|500](/img/user/pics/PX275%20-%20G4%20-%20wave%20equation.png)
## dimensions of the diffusion constant
$$\left[\frac{\partial c}{\partial t}\right] = [T]^{-1} \; and \; \left[\frac{\partial^{2} {c}}{\partial {x}^{2}}\right] = [L]^{-2}$$
$$\therefore [D] = [L]^{2}[T]^{-1}$$

- it has been assumed that $D$ is constant
- if $D$ is not constant:
$$\frac{\partial c}{\partial t} = \frac{\partial }{\partial x}\left(D(x) \frac{\partial c}{\partial x}\right)$$
- if there is a source or sink of particles:
$$\frac{\partial c}{\partial t} = \frac{\partial }{\partial x}\left(D\frac{\partial c}{\partial x}\right) + S(x,t)$$
