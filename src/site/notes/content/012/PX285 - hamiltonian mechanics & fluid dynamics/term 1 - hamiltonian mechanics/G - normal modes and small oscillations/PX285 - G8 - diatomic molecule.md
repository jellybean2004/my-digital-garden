---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/term-1-hamiltonian-mechanics/g-normal-modes-and-small-oscillations/px-285-g8-diatomic-molecule/","noteIcon":"1","created":"2024-12-05T18:31:39.076+00:00","updated":"2024-12-06T11:21:12.810+00:00"}
---

![Pasted image 20241205225803.png|500](/img/user/pics/Pasted%20image%2020241205225803.png)
- considering a diatomic molecule - carbon monoxide (CO)
- the bond can be approximated as an ideal spring for small displacements
![Pasted image 20241205225820.png|500](/img/user/pics/Pasted%20image%2020241205225820.png)
$$\begin{gather}
V  = \frac{1}{2} k (x_{2} - x_{1})^{2} \\
T = \frac{1}{2}m_{C}\dot x_{1}^{2} + \frac{1}{2}m_{O}\dot x_{2}^{2} 
\end{gather}$$
## the inertia matrix
- using the formula:
$$M_{ij} = \frac{\partial^{2} {T}}{\partial {\dot x_{i}}\partial \dot x_j}$$
- the inertia matrix is:
$$M = \begin{pmatrix}m_{C} & 0 \\ 0 & m_{O}\end{pmatrix}$$
## the stiffness matrix
- using the formula:
$$K_{ij} =  \frac{\partial^{2}V}{\partial x_{i} \partial x_{j}}$$
- the stiffness matrix is:
$$T = \begin{pmatrix}k & -k \\ -k & k\end{pmatrix}$$
## the euler-lagrange equation in matrix form
$$M \vec{\ddot x} = K \vec x \tag{1}$$
- the value of $\vec x = \begin{pmatrix}x_1 \\ x_2\end{pmatrix}$
- guessing that there will be an oscillatory solution:
$$\vec  x = A \vec Xe^{i\omega t}$$
- substituting this into equation $(1):$
$$\begin{gather}
-\omega^{2} M \vec X  = - K\vec X \\
(\omega^{2} M - K) \vec X = \vec 0  \\
\end{gather}$$
- the secular equation:
$$\begin{gather}
\det (\omega^{2}M - K) = 0 \\
\begin{vmatrix}m_{C}\omega^{2}-k & k \\ k & m_{O}\omega^{2}-k\end{vmatrix} = 0 \\
(m_{C}\omega^{2}-k)(m_{O}\omega^{2}-k) -k^{2} = 0 \\
m_{C}m_{O}(\omega^{2})^{2} - k(m_{C} + m_{0})\omega^{2} = 0
\end{gather}$$
$$\begin{gather}
\text{either, }& m_{C}m_{O} \omega^{2} - k (m_{C}+ m_{O}) = 0 && \text{or, } &\omega^{2}=0
\end{gather}$$
## the first mode
$$\omega^{(1)} = \sqrt{ k \frac{m_{C}+m_{O}}{m_{C}m_{O}} }$$
- defining the reduced mass as:
$$\mu = \frac{m_{C}m_{O}}{m_{C}+m_{O}}$$
$$\omega^{(1)} = \sqrt{ \frac{k}{\mu }}$$
- substituting this solution into equation $(1):$
$$\begin{gather}
(M (\omega^{(1)})^{2} - K) \vec X = \vec 0 \\
\begin{pmatrix}m_{C} \cfrac{k}{\mu} -k & k \\ k & m_{O}\cfrac{k}{\mu}-k\end{pmatrix} \begin{pmatrix}a \\b\end{pmatrix} = \vec 0
\end{gather}$$
- this gives two equations:
$$\begin{gather}
(m_{C} \cfrac{k}{\mu} -k )a + kb \\
\frac{a}{b} = \frac{k}{k- \cfrac{m_{C}}{\mu}} =\dots = - \frac{m_{0}}{m_{C}} \\
\implies a = -m_{0},\; \text{and } b = m_C
\end{gather}$$
## the second mode
$$(\omega^{(2)})^{2} = 0$$
- this is a signature that is not an oscillating solution, but a translating one:
$$\omega = 0 \implies \tau = \frac{2\pi}{\omega} \to \infty$$
- this can be understood as a translational mode
$$x(t) = (A + Bt) \begin{pmatrix}1 \\1\end{pmatrix}$$
	where, $A$ is the position at $t=0$, $B$ is the velocity of translation, and the vector represents that both atoms are translating together
- the masses moving together would imply that the spring like bond is never disturbed, ie. there are no external force
- from newton's second law, the system should remain in its state of uniform motion
### more rigorously
- substituting it into  equation $(2):$
$$\begin{pmatrix}k & -k \\ -k & k\end{pmatrix} \begin{pmatrix}a \\ b\end{pmatrix} = \begin{pmatrix}0 \\ 0\end{pmatrix}$$
$$\begin{gather}
ka-kb = 0 &\implies a = b \\
\text{or, } -ka + kb = 0 &\implies a= b
\end{gather}$$
$$\therefore \vec X = \begin{pmatrix}1 \\ 1\end{pmatrix} $$
- this is a solution provided that the inertial term vanishes, ie: $F = ma = 0$
$$M \ddot{ \vec x} = \vec 0$$
- $$\begin{pmatrix}m_{C} & 0 \\ 0 & m_{O}\end{pmatrix} \begin{pmatrix}a\\ b\end{pmatrix} \ddot f(t) = 0$$
- $$\begin{gather}
	m_{C}a 
\end{gather}$$
#incomplete 