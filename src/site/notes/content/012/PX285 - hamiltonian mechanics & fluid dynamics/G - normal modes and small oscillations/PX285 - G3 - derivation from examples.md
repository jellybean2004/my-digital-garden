---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/g-normal-modes-and-small-oscillations/px-285-g3-derivation-from-examples/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T12:59:01.087+00:00"}
---

- **note:** from lecture

- often, mechanical systems are intrinsically coupled, and the displacement degrees of freedom move 'together' in a mode that has a characteristic frequency
## particle attached to a spring
- the lagrangian: 
$$L = \frac{1}{2}m\dot x^{2} - \frac{1}{2}kx^{2}$$
- the euler-lagrange equation: 
$$m\ddot x = - kx \implies \ddot x = - \omega^{2}x$$
	where, $\omega = \sqrt{\frac{k}{m}}$ 
- the solution: 
$$x = A\cos\omega t + B\sin\omega t = C\exp(i\omega t)$$
## two particles 
- the solutions: 
$$\begin{align*}
	x_{1} &= D_{1}\exp(i\omega_{1}t) \\
	x_{2} &= D_{2}\exp(i\omega_{2}t) 
\end{align*}$$
- the euler lagrange equations: 
$$\begin{align*}
	m_{1}\ddot x_{1} &= - k_{1}x_{1} \\
	m_{2}\ddot x_{2} &= - k_{2}x_{2} 
\end{align*}$$
- in matrix form: 
$$\begin{pmatrix}m_{1}\ddot x_{1} \\ m_{2}\ddot x_{2}\end{pmatrix} = \begin{pmatrix}-k_{1}x_{1} \\ -k_{2}x_{2}\end{pmatrix}$$
- to isolate $\ddot x$ an $x:$ 
$$\begin{pmatrix}m_{1} & 0 \\ 0 & m_{2}\end{pmatrix} \begin{pmatrix}\ddot x_{1} \\ \ddot x_{2} \end{pmatrix} = \begin{pmatrix}-k_{1}x_{1} \\ -k_{2}x_{2}\end{pmatrix}$$
	- the matrix is called the **inertia matrix**, $M$
- also: 
$$\begin{pmatrix}k_{1} & 0 \\ 0 & k_{2}\end{pmatrix} \begin{pmatrix} x_{1} \\ x_{2} \end{pmatrix} = \begin{pmatrix}-k_{1}x_{1} \\ -k_{2}x_{2}\end{pmatrix}$$
	- this matrix is called the **stiffness matrix**, $K$
- therefore: 
$$M \vec{\ddot x}  = -K\vec x$$
- solutions: 
$$\begin{align*}
	\vec x(t) = \begin{pmatrix}1 \\ 0\end{pmatrix} D_{1}\exp(i\omega_{1}t) \\
	\vec x(t) = \begin{pmatrix} 0 \\ 1 \end{pmatrix} D_{2}\exp(i\omega_{2}t)
\end{align*}$$
- they give the vibrations of the first and the second spring respectively
\1\n\2\n