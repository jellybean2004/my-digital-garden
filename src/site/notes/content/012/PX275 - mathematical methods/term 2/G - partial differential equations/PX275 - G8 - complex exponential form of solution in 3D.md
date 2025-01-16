---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/g-partial-differential-equations/px-275-g8-complex-exponential-form-of-solution-in-3-d/","noteIcon":"1","created":"2025-01-16T12:37:23.168+00:00","updated":"2025-01-16T12:54:11.196+00:00"}
---

## 1D case
- the wave equation in 1D:
$$\frac{\partial^{2} {u}}{\partial {t}^{2}} = c^{2} \frac{\partial^{2} {u}}{\partial {x}^{2}} \implies (A\cos kx + B \sin kx) ( C\cos\omega t + D \sin\omega t)$$
$$A\cos kx + B\sin kx = \alpha \cos(kx + \phi) = \beta \sin(kx + \phi)$$
	where, $\alpha, \beta$ are the amplitudes, and $\phi$ is the phase

- a compact alternative is to use complex exponentials

$$C\, e^{ikx}  = C(\cos kx  + i \sin kx) = |C| e^{i(kx + \phi)}$$
	where, $C = |C|e^{i\phi}$

- **note:** $\mathbf Re (|C|e^{i(kx+ \phi)}) = |C|\cos(kx + \phi)$

- same applies to the time part:
$$u(x,t) = Ce^{i(kx-\omega t)} = |C| e^{i(kx - \omega t + \phi)}$$
- physical solutions are represented by the real pert

- **note:** $Ce^{i(kx+\omega t)}$ also works!
- therefore, the full solution:
$$u(x,t) = C_{1}e^{i(kx-\omega t)} + C_{2} e^{i(kx+\omega t)}$$
- there are four degrees of freedom: $\mathbf{R}e(C_1)$, $\mathbf{I}m(C_{1})$, $\mathbf{R}e(C_{2})$, $\mathbf{I}m(C_{2})$

## generalizing to 3D
- the position vector:
$$\vec r = (x,y,z)$$

- the wave equation: 
$$\frac{\partial^{2} {u(\vec r, t)}}{\partial {t}^{2}} = \vec\nabla u(\vec r,t)$$

$$u(\vec r, t) = C_{1} \exp(i(k_{x} x + k_{y} y + k_{z}z - \omega t)) + C_{2}\exp(i(k_{x} x + k_{y} y + k_{z}z + \omega t) )$$
- defining the wavevector:
$$\vec k = (k_{x}, k_{y}, k_{z})$$
$$\implies u(\vec r, t) = C_{1}\exp(i(\vec k \cdot \vec r - \omega t)) + C_{2}\exp(i(\vec k \cdot \vec r + \omega t))$$



