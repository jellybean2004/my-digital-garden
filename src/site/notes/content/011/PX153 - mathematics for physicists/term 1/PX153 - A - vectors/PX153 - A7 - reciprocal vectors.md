---
dg-publish: true
---

- relevant for non-orthogonal basis sets
	- eg: we will use it to determine components of a vector in a non-orthogonal basis set
		- $\vec a = \sum\limits a_{i}\vec e_i$
			where, $a_{i}=$ components ; $\vec e_i=$ basis vectors
		- for cartesian: $\vec e \cdot \vec e_{j}=\delta_{ij}$ and, $\vec a \cdot \underline{\hat e_x}=\vec a_x$ 
			- easy to find components
		- but in non-orthogonal: 
			$\vec e \cdot \vec e_{j}\neq\delta_{ij}$
			and, $\vec e_i \cdot \vec a \neq a_i$
				$\vec a = \sum\limits_i a_i\vec e_i$
			- not easy to find components
- define reciprocal vectors:
$$\begin{gather}
	e_{1}' = \frac{e_{2}\times e_{3}}{e_{1}\cdot(e_{2}\times e_{3})} \\
	e_{2}' = \frac{e_{3}\times e_{1}}{e_{1}\cdot(e_{2}\times e_{3})} \\
	e_{3}' = \frac{e_{1}\times e_{2}}{e_{1}\cdot(e_{2}\times e_{3})}
\end{gather}$$		
		$\vec e_i\cdot\vec e_j'=\delta_{ij}$
		$a_i=\vec e_i'\cdot a$
	