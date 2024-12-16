---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-1/px-153-a-vectors/px-153-a7-reciprocal-vectors/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2024-11-26T19:36:22.617+00:00"}
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
	