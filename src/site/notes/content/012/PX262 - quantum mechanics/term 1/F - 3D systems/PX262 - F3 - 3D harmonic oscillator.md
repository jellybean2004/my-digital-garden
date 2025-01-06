---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-1/f-3-d-systems/px-262-f3-3-d-harmonic-oscillator/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2025-01-06T18:15:14.644+00:00"}
---

- the potential energy operator: 
  $$\hat V(\vec r) = \frac{1}{2}k_{x}x^{2} + \frac{1}{2}k_{y}y^{2} + \frac{1}{2}k_{z}z^{2} = \hat V_{x}(x) + \hat V_{y}(y) + \hat V_{z}(z)$$
	where, $k_{x}, k_{y}, k_{z}$ are effective spring constants in the respective directions  
- solving the time-independent schrödinger equation by separation of variables: 
  $$- \frac{\hbar^{2}}{2m} \nabla^{2}(XYZ) + V(\vec r) XYZ = E\, XYZ$$
- dividing by $XYZ$ and grouping terms with like coordinates: 
  $$\left[\frac{-\hbar^{2}}{2m} \frac{1}{X} \frac{\partial^{2} {X}}{\partial {x}^{2}} + V_{x}\right] + \left[\frac{-\hbar^{2}}{2m} \frac{1}{Y} \frac{\partial^{2} {Y}}{\partial {y}^{2}} + V_{y}\right] + \left[\frac{-\hbar^{2}}{2m}  \frac{1}{Z} \frac{\partial^{2} {Z}}{\partial {z}^{2}} + V_{z} \right] = E$$
- this can be split into three [[content/012/PX262 - quantum mechanics/term 1/B - introduction/PX262 - B6 - 1D harmonic oscillator\|1D harmonic oscillator]] equations, with three quantum numbers, $n_{x}, n_{y}, n_{z}$
- the energy eigenstates are: 
  $$E_{n_{x}n_{y}n_{z}} = \left(n_{x}+ \frac{1}{2}\right)\hbar\omega_{x} + \left(n_{y}+ \frac{1}{2}\right)\hbar\omega_{y}  + \left(n_{z}+ \frac{1}{2}\right)\hbar\omega_{z} $$
	where, $\omega_{i}$ is related to the spring constant, $k_{i}$
- the wavefunctions are: 
  $$\phi(\vec r) = H_{n_{x}}(x') H_{n_{y}}(y') H_{n_{z}}(z') \exp(- \frac{1}{2}(x'^{2}+ y'^{2}+ z'^{2}))$$
	where, $i' = (\frac{M\omega_{i}}{\hbar})^\frac{1}{2}$ for $i = \{x,y,z\}$
- it can be observed that non-different $k_{i}$ values will lead to degenerate systems
