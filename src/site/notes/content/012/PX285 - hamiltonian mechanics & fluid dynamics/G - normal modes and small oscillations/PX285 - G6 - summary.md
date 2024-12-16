---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/g-normal-modes-and-small-oscillations/px-285-g6-summary/","noteIcon":"1","created":"2024-11-28T19:54:15.229+00:00","updated":"2024-11-28T22:42:03.855+00:00"}
---

- a vector form of the [[content/012/PX285 - hamiltonian mechanics & fluid dynamics/C - calculus of variations/PX285 - C1 - the euler-lagrange equation\|euler-lagrange equation]]:
$$M \ddot{\vec x} = - K \vec x \tag{1}$$
- the inertia and the stiffness matrices:
$$\begin{align*}
M_{ij} = \frac{\partial^{2} {T}}{\partial {\dot x_{i}}\partial \dot x_{j}} \\
K_{ij} = \frac{\partial^{2} {V}}{\partial {x_{i}}\partial x_{j}}
\end{align*}$$
- seeking oscillatory solutions, the most general form is:
$$\vec x(t) = A\, \vec X\,e^{i\omega t}$$
	where, $\vec X = (\vec x_{i}, \vec x_{2} , \dots)$, where $\vec x_{n}$ are the positions of individual masses
- substituting this into equation $(1)$, and solving it will reveal of number of modes that is equal to the number of coordinates, $\lambda$
- the general solution is the sum of all the individual solutions (modes), which may not have the same frequency
$$\vec x(t) = \sum\limits_{\lambda} A^{(\lambda)} \vec X^{(\lambda)} e^{i\omega^{(\lambda)} t} $$
$$\begin{gather*}
	\dot {\vec x} = A \vec X  = i\omega A \vec X e^{i \omega t} \\
	\ddot {\vec x} = A \vec X  = -\omega^{2} A \vec X e^{i \omega t} \equiv - \omega^{2}x
\end{gather*}$$
$$\begin{align*}
	M (-\omega^{2}\vec x) &= -K\vec x) \\
	- \omega^{2} M \vec x &= -K \vec x \\
	( K- \omega^{2} M )\vec x &= \vec 0 \\
	Ae^{i\omega t} \,(K - \omega^{2}M)\, \vec X &= \vec 0
\end{align*}$$
- $Ae^{i\omega t}$ is non-zero if $A \neq 0$
$$\begin{gather}
\underbrace{(K - \omega^{2}M)}\, \vec X = \vec 0 \\
B\vec X = 0
\end{gather}$$
- this has solutions when $\det B = 0$, ie: $\det(K-\omega^{2}M) = 0$
- this is an equation, polynomial in $\omega^{2}$, and it is called the **secular equation**
- it can be used to determine possible squared frequencies $\omega^{2}$
- $\omega^{2}$ are the eigenvalues, and $\vec X$ are the eigenvectors
