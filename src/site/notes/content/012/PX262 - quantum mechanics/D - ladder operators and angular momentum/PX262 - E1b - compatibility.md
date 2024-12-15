---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/d-ladder-operators-and-angular-momentum/px-262-e1b-compatibility/","created":"2024-12-15T14:38:06.257+00:00","updated":"2024-12-15T15:09:09.733+00:00"}
---

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
- the components are mutually incompatible, but $\hat L^{2}$ is compatible with all three components
- this means that if a system is an eigenstate of one angular momentum component, it cannot simultaneously be in an eigenstate of either of the others
- but. the total angular momentum can be measured compatibly with any other component