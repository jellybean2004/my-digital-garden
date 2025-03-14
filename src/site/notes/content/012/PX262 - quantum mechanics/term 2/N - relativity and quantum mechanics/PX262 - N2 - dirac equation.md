---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/n-relativity-and-quantum-mechanics/px-262-n2-dirac-equation/","noteIcon":"1","created":"2025-03-10T11:47:17.092+00:00","updated":"2025-03-10T11:47:24.399+00:00"}
---

- the klein-gordon equation contains a second order time derivative, as opposed to the schrödinger has just a first order time derivative
- special relativity implies that the wave equation must treat space and time on an equal footing
- ie. should be linear in both space and time derivatives

- dirac proposed:
$$\hat H = \alpha_{x} c \, \hat p_{x} + \alpha_{y}c \, \hat p_{y} + \alpha_{z}c \, \hat p_{z} + \beta mc^{2}$$
- $\hat H \psi = i\hbar \frac{\partial \psi}{\partial t}$ has the same form as the schrödinger equation
- choosing $\alpha_{x}, \alpha_{y}, \alpha_{z}, \beta$ such that $\hat H \psi = - \hbar^{2}\partial^{2}_{t} \psi$ becomes the klein-gordon equation
- this requires 
$$\begin{gather}
\alpha_{x}^{2} = \alpha_{y}^{2} = \alpha_{z}^{2} = \beta^{2} = 1 \\
 \alpha_{x}\alpha_{y} = - \alpha_{y}\alpha_{x}\\
 \alpha_{x}\alpha_{z} = - \alpha_{z}\alpha_{x} \\
 \alpha_{y}\alpha_{z} = - \alpha_{z}\alpha_{y} \\
 \alpha_{i}\beta = - \beta \alpha_{i} \; i\in\{x,y,z\}
\end{gather}$$
- ie: $\alpha_{x}\alpha_{z} + \alpha_{z}\alpha_{x} = 0$ and $\alpha_{x}\beta + \beta \alpha_{x} = 1$, etc

- dirac proposed that the coefficients be taken as $4\times4$ matrices and find the set of matrices to meet these conditions
- the results from the pauli spin matrices look promising: 
$$\begin{gather} 
\sigma_{x}\sigma_{z}+ \sigma_{z}\sigma_{x}= 0 \\
\sigma_{x}^{2} = I
\end{gather}$$
- these meet the conditions:
$$\begin{gather}
\alpha_{x} = \begin{pmatrix}0 & 0 & 0 & 1\\ 0 & 0 & 1 & 0 \\ 0 & 1 & 0 & 0 \\ 1 & 0 & 0 & 0 \end{pmatrix} = \begin{pmatrix}0 & \sigma_{x}\\ \sigma_{x}& 0 \end{pmatrix}\\
\alpha_{y} = \begin{pmatrix}0 & \sigma_{y}\\ \sigma_{y}& 0 \end{pmatrix} \\
\alpha_{z} = \begin{pmatrix}0 & \sigma_{z}\\ \sigma_{z}& 0 \end{pmatrix} \\
\beta = \begin{pmatrix}1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & -1 & 0 \\ 0 & 0 & 0 & -1 \end{pmatrix} = 
\begin{pmatrix}I & 0\\ 0& -I \end{pmatrix}
\end{gather}$$
- the dirac equation is:
$$\left[- i\hbar c \left(\alpha_{x}\frac{\partial }{\partial x} + \alpha_{y} \frac{\partial }{\partial y} + \alpha_{z} \frac{\partial }{\partial z}\right) + \beta mc^{2}\right] \psi = i\hbar \frac{\partial \psi}{\partial t}$$

- $\vec \alpha = (\alpha_{x}, \alpha_{y}, \alpha_{z})$ and $\beta$ are matrices
- $\psi(\vec r, t)$ must have four components, called the**dirac spinors**:
$$\psi = \begin{pmatrix} \psi_{1} \\ \psi_{2}\\ \psi_{3} \\ \psi_{4}\end{pmatrix}
= \begin{pmatrix} u_{1}(p) \\ u_{2}(p)\\ u_{3}(p) \\ u_{4}(p)\end{pmatrix} \exp\left(i \frac{(\vec p \cdot \vec r - \vec k t)}{\hbar}\right)$$
- in the non-relativistic limit ($1/c^{2}\to0$), the dirac equation reduces to the schrödinger equation, but now, for a particle with a spin, $\hbar/2$
$$\psi(x, y,z,t) = \begin{pmatrix}u_{1} \\ u_{2}\end{pmatrix} \exp\left(i \frac{(\vec p \cdot \vec r - Et)}{\hbar}\right)$$
	where, $u_{3}, u_{4}\to 0$ as $c^{2} \to \infty$, and $u_{1}$ and $u_{2}$ become independent of the momentum
- thus, spin is explained
- by looking at the leading relativistic corrections, spin-orbit coupling is also described
- by comparing with the continuity equation:
$$\vec\nabla\cdot\vec  j = - \frac{\partial \rho}{\partial t}$$
- the probability density:
$$\rho  = |\psi_{1}^{2} | + |\psi_{2}|^ {2} + |\psi_{3}|^ {2}+ |\psi|^{4}$$
