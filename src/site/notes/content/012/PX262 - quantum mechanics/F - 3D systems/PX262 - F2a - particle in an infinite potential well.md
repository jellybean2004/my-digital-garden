---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/f-3-d-systems/px-262-f2a-particle-in-an-infinite-potential-well/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-12-15T11:40:32.615+00:00"}
---

s- consider a potential well in 3D: 
  $$V(\vec r) = \begin{cases} 0  & if & -a \leq x \leq a ,\; -b \leq y \leq b \; \text{and } -c \leq z \leq c, \\ \infty &  & \text{elsewhere}.\end{cases}$$
- using separation of variables for the wavefunction: 
  $$\phi(\vec r) = X(x) Y(y) Z(z)$$
- substituting into the time-independent schrödinger equation: 
$$\begin{align*}
	\frac{-\hbar^{2}}{2m} \left[YZ \frac{\partial^{2} {X}}{\partial {x}^{2}} + XZ \frac{\partial^{2} {Y}}{\partial {y}^{2}} + XY \frac{\partial^{2} {Z}}{\partial {z}^{2}}\right] &= E XYZ \\
	\underbrace{\frac{-\hbar^{2}}{2m} \frac{1}{X} \frac{\partial^{2} {X}}{\partial {x}^{2}}}_\text{only dependent on x} + \underbrace{\frac{-\hbar^{2}}{2m}  \frac{1}{Y} \frac{\partial^{2} {Y}}{\partial {y}^{2}}}_\text{only dependent on y} + \underbrace{\frac{-\hbar^{2}}{2m}  \frac{1}{Z} \frac{\partial^{2} {Z}}{\partial {z}^{2}}}_\text{only dependent on z} &= E \\
\end{align*}$$
- each term should be equal to a constant, and the three constants should add up to $E$
- looking at the $x$-dependent term: 
  $$- \frac{\hbar^{2}}{2m} \frac{\partial^{2} {X}}{\partial {x}^{2}} = E_{1}X$$
- this is exactly the same as the equation for [[content/012/PX262 - quantum mechanics/B - introduction/PX262 - B4 - particle in an infinite square well\|the 1D potential well]], and the solution is: 
  $$E_{n_{1}} = \frac{\hbar^{2}\pi^{2}}{8Ma^{2}}n_{1}^{2}$$
	where, ${} n_{1} {}$ is the quantum number labelling states
- and the wavefunction is: 
  $$X(x) = \frac{1}{\sqrt{a}} \left\{ \begin{matrix}\cos \\ \sin\end{matrix} \right\} \left(\frac{n_{1}\pi x}{2a}\right)$$
	where, $\left\{ \begin{matrix}\cos \\ \sin\end{matrix} \right\}$ means cosine for odd and sine for even values of $n_1$
- the full solution is: 
  $$\phi(\vec r) = \frac{1}{\sqrt{abc}} \left\{ \begin{matrix}\cos \\ \sin\end{matrix} \right\} \left(\frac{n_{1}\pi x}{2a}\right) \left\{ \begin{matrix}\cos \\ \sin\end{matrix} \right\} \left(\frac{n_{2}\pi y}{2a}\right) \left\{ \begin{matrix}\cos \\ \sin\end{matrix} \right\} \left(\frac{n_{3}\pi z}{2a}\right)$$
- the energy eigenvalues are the sums of the three contributions: 
  $$E = E_{n_{1}} + E_{n_{2}} + E_{n_{3}} = \frac{\hbar^{2}\pi^{2}}{8M} \left(\frac{n_{1}^{2}}{a^{2}} + \frac{n_{2}^{2}}{b^{2}} + \frac{n_{3}^{2}}{c^{2}} \right)$$
