---
{"dg-publish":true,"permalink":"/my-digital-garden/012/px-262-quantum-mechanics/d-ladder-operators-and-angular-momentum/px-262-e1-angular-momentum/","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T01:07:53.855+00:00"}
---

- in classical physics, the angular momentum is defined as: 
  $$\vec L = \vec r \times \vec p$$
- therefore, using [[content/012/PX262 - quantum mechanics/C - the basic postulates/PX262 - C2c - postulates 2 & 3\|postulate 3]], the angular momentum operator is defined as: 
  $$\hat L = \hat{\vec R} \times \hat{\vec P}$$
- the components of angular momentum are: 
$$\begin{align*}
	\hat L_{x}&= \hat Y \hat P_{z}- \hat Z \hat P_{y} \\
	\hat L_{y} &= \hat Z \hat P_{x} - \hat X \hat P_{z} \\
	\hat L_{z}&= \hat X \hat P_{y}- \hat Y \hat P_{x}\\
	\hat L^{2} &= \hat L_{x}^{2} + \hat L_{y}^{2}+ \hat L_{z}^{2} 
\end{align*}$$
- compatibility of the angular momentum operator with the position operator: 
$$\begin{gather*}
	[\hat X, \hat L_{x}] = 0 & [\hat X, \hat L_{y}] = +i\hbar \hat Z & [\hat X, \hat L_{z}] = -i\hbar \hat Y \\
	[\hat Y, \hat L_{x}] = -i\hbar \hat Z & [\hat Y, \hat L_{y}] = 0 & [\hat Y, \hat L_{z}] = +i\hbar \hat X \\
	[\hat Z, \hat L_{x}] = + i \hbar \hat Y & [\hat Z, \hat L_{y}] = -i\hbar \hat Y & [\hat Z, \hat L_{z}] = 0 \\
\end{gather*}$$
- compatibility of the angular momentum operator with the momentum operator: 
$$\begin{gather*}
	[\hat P_{x}, \hat L_{x}] = 0 & [\hat P_{x}, \hat L_{y}] = +i\hbar \hat P_{z} & [\hat P_{x}, \hat L_{z}] = -i\hbar \hat P_{y} \\
	[\hat P_{y}, \hat L_{x}] = -i\hbar \hat P_{z} & [\hat P_{y}, \hat L_{y}] = 0 & [\hat P_{y}, \hat L_{z}] = +i\hbar \hat P_{x} \\
	[\hat P_{z}, \hat L_{x}] = + i \hbar \hat P_{y} & [\hat P_{z}, \hat L_{y}] = -i\hbar \hat P_{x} & [\hat P_{z}, \hat L_{z}] = 0 \\
\end{gather*}$$
- compatibility between individual components of the angular momentum operator, and between the components and the square: 
$$\begin{align*}
	[\hat L_{x}, \hat L_{y}] &= i \hbar \hat L_{z}\\
	[\hat L_{y}, \hat L_{z}] &= i\hbar \hat L_{x} \\
	[\hat L_{z}, \hat L_{x}] &= i\hbar \hat L_{y}\\\\
	[\hat L^{2}, \hat L_{x}] = [\hat L^{2}, \hat L_{y}] &=  [\hat L^{2}, \hat L_{z}] = 0
\end{align*}$$
- this shows that the components are mutually incompatible, and $\hat L^{2}$ is compatible with all three components
- there are two operators which can have common eigenstates, and based on which the states can be labelled: $\hat L^{2}$ and $\hat L_{m},\;m\in\{x,y,z\}$, usually, $\hat L_{z}$ is taken