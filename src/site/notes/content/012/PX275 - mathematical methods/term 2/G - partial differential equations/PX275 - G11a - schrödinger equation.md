---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/g-partial-differential-equations/px-275-g11a-schroedinger-equation/","noteIcon":"1","created":"2025-01-29T12:14:17.297+00:00","updated":"2025-01-29T12:55:51.118+00:00"}
---

[[content/011/PX156 - quantum phenomena/PX156A - quantum phenomena/PX156 - C - quantum mechanics/PX156 - C1 - the schrodinger equation\|PX156 - C1 - the schrodinger equation]]
- in 3D:
$$i \hbar \frac{\partial \psi}{\partial t} = - \frac{\hbar^{2}}{2m} \nabla^{2}\psi + V \psi$$
- considering a case without potential, ie: $V=0$, and let $D = i\hbar/2m:$
$$\frac{\partial \psi}{\partial t} = D \nabla^{2} \psi$$
- this is identical to the [[content/012/PX275 - mathematical methods/term 2/G - partial differential equations/PX275 - G3a - diffusion equation\|diffusion equation]]

- using separation of variables:
$$\psi(\vec r, t) = R(\vec r) \, T(t) = X(x)Y(y)Z(z)\, T(t)$$
$$\begin{gather}
i\hbar R \frac{dT}{dt} = - \frac{\hbar^{2}}{2m} T \nabla^{2} R + VRT \\
\frac{i\hbar}{T} \frac{dT}{dt} = - \frac{\hbar^{2}}{2mR} \nabla^{2} R + V = \text{ constant}
\end{gather}$$

- rather than deriving solutions for positive, negative and zero constant, considering special, physically-meaningful solutions
- suppose the constant of separation is $E$, the energy associated with $\psi$

- the time dependent part:
$$\begin{gather}
\frac{dT}{dt} = - \frac{i}{\hbar}TE  \\
\implies T(t) = C \exp(- \frac{iE}{\hbar}t)
\end{gather}$$
- the spatial part, for ${} E>V$:
$$\frac{1}{R}\nabla^{2} R = - \frac{2m}{\hbar^{2}}(E - V) = -k^{2}$$
- trial solution: $$\begin{gather}
R = C\exp(i\vec k \cdot \vec r) \\\\
\nabla^{2} R = - k^{2}R \\
\implies\frac{\hbar^{2}k^{2}}{2m} +V = E \\
\frac{p^{2}}{2m} + V  = E
\end{gather}$$
	where, $p = \hbar k$ is the [[content/012/PX262 - quantum mechanics/term 1/A - recap/PX262 - A5 - debroglie waves\|debroglie momentum]]
- the above equation represents the total energy with the first term being the kinetic energy:
$$T + V = E$$

## particle in a potential well
- considering a 1D case:
$$\begin{gather}
\frac{1}{X} \frac{d^{2}X}{dx^{2}} = - \frac{2m}{\hbar^{2}} (E-V) = - k^{2} \\
\implies X = A\cos kx + B\sin kx
\end{gather}$$
- the boundary conditions de to the well:
$$\begin{gather}
\psi(x = 0,t) = \psi(x = L, t) = 0 \;\forall t \\\\
X(0) = 0 \implies A = 0 \\
X(L ) = 0 \implies  k = \frac{n\pi}{L} \\\\
\therefore \psi(x,t) = \sum\limits_{n}B_{n} \sin\left(\frac{n\pi x}{2}\right)\exp\left(- \frac{iEt}{\hbar}\right)
\end{gather}$$
- now, considering a 3D case:
$$\begin{gather}
\frac{1}{R}\nabla^{2} R = - \frac{2m}{\hbar^{2}} (E-V) = -k^{2} \\\dots \\
\frac{1}{X} \frac{d^{2}X}{dx^{2}} + \frac{1}{Y} \frac{d^{2}Y}{dy^{2}} + \frac{1}{Z} \frac{d^{2}Z}{dz^{2}} = - k^{2} \\
\frac{1}{X} \frac{d^{2}X}{dx^{2}} = - k^{2} - \frac{1}{Y} \frac{d^{2}Y}{dy^{2}} - \frac{1}{Z} \frac{d^{2}Z}{dz^{2}} = -k_{x}^{2}
\end{gather}$$
- the solutions for $X:$
$$X(x) = A\cos k_{x}x  + B \sin k_{x}x$$
- similarly for $Y$ and $Z:$
$$\begin{gather}
\frac{1}{Y} \frac{d^{2}Y}{dy^{2}} = - k^{2} - \frac{1}{X} \frac{d^{2}X}{dx^{2}} - \frac{1}{Z} \frac{d^{2}Z}{dz^{2}} = -k_{y}^{2} \\
Y(y) = C \cos k_{y}y + D \sin k_{y}y \\\\
\frac{1}{Z} \frac{d^{2}Z}{dz^{2}} = - k^{2} - \frac{1}{X} \frac{d^{2}X}{dx^{2}} - \frac{1}{Y} \frac{d^{2}Y}{dy^{2}} = -k_{z}^{2} \\
Z(z) = E \cos k_{z}z + F \sin k_{z}z \\\\
k^{2} = k_{x}^{2}+ k_{y}^{2} + k_{z}^{2} = \frac{2m}{\hbar^{2}} (E-V)
\end{gather}$$

$$\psi(\vec r , t) = \sum\limits_{n}\sum\limits_{m}\sum\limits_{l} A_{nml} \sin\left(\frac{n\pi x}{L}\right) \sin\left(\frac{m\pi y}{L}\right)\sin\left(\frac{l\pi z}{L}\right) \exp\left(\frac{- iEt}{\hbar}\right)$$

- considering a special case, $V = 0$ inside the box:
$$\begin{gather}
k^{2} = \frac{2mE}{\hbar^{2}} \\
E = \frac{\hbar^{2}}{2m} \frac{\pi}{L}^{2} (n^{2}+ m^{2} + l^{2} )
\end{gather}$$
- this is the quantization of energy in 3D
