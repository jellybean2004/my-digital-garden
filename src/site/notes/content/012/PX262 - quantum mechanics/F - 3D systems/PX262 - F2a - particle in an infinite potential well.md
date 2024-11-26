---
dg-publish: true
---

- consider a potential well in 3D: 
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
  $$E_{n_{x}} = \frac{\hbar^{2}\pi^{2}}{8Ma^{2}}n_{x}^{2}$$
	where, $n_{x}$ is the quantum number labelling states
- and the wavefunction is: 
  $$X(x) = \frac{1}{\sqrt{a}} \left\{ \begin{matrix}\cos \\ \sin\end{matrix} \right\} \left(\frac{n_{x}\pi x}{2a}\right)$$
	where, $\left\{ \begin{matrix}\cos \\ \sin\end{matrix} \right\}$ indicate either one or the other function depending on whether $n_{x}$ is odd or even, and the fraction in the bracket is its argument

- the full solution is: 
  $$\phi(\vec r) = \frac{1}{\sqrt{abc}} \left\{ \begin{matrix}\cos \\ \sin\end{matrix} \right\} \left(\frac{n_{x}\pi x}{2a}\right) \left\{ \begin{matrix}\cos \\ \sin\end{matrix} \right\} \left(\frac{n_{y}\pi y}{2a}\right) \left\{ \begin{matrix}\cos \\ \sin\end{matrix} \right\} \left(\frac{n_{z}\pi z}{2a}\right)$$
- the energy eigenvalues are the sums of the three contributions: 
  $$E = E_{n_{x}} + E_{n_{y}} + E_{n_{z}} = \frac{\hbar^{2}\pi^{2}}{8M} \left(\frac{n_{1}^{2}}{a^{2}} + \frac{n_{2}^{2}}{b^{2}} + \frac{n_{3}^{2}}{c^{2}} \right)$$
