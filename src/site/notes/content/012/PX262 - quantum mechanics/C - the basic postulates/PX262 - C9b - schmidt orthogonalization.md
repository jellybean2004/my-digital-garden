---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/c-the-basic-postulates/px-262-c9b-schmidt-orthogonalization/","noteIcon":"1","created":"2024-12-15T11:07:33.599+00:00","updated":"2024-12-15T11:07:42.905+00:00"}
---

- a way of restoring orthogonality
- considering  $\phi_{1}$ and $\phi_{2}$, which are not orthogonal, but have the same eigenvalue
- defining a new eigenfunction, which is a linear combination of the two: 
  $$\phi_{2}' = S_{12}\phi_{1}- \phi_{2}$$
	where ${} S_{12} = \int \phi_{1}^{*} \phi_{2}\,d\tau$
- checking if the new function is orthogonal to $\phi_{1}:$ 
$$\begin{align*}
	\int \phi_{1}^{*} \phi_{2}' \,d\tau &= S_{12}\int \phi_{1}^{*}\phi_{1} \,d\tau- \int\phi_{1}^{*}\phi_{2}\,d\tau \\
	&= S_{12} - S_{12} \\
	&= 0 
\end{align*}$$
- this shows that $\phi_{1}$ and $\phi_{2}'$ are orthogonal

- if there is another eigenfunction, $\phi_{3}$, with the same eigenvalue: 
  $$\phi_{3}' = s_{13}\phi_{1}+ s_{23}\phi_{2}' - \phi_{3}$$
	where, ${} s_{13} = \int \phi_{1}^{*}\phi_{3}\,d\tau {}$, and $s_{23}= \frac{\int\phi_{2}'^{*}\phi_{3}\,d\tau}{\int|\phi_{2}'|^{2}\,d\tau}$
- the factors, $s_{12}$, $s_{13}$, and $s_{23}$ are called overlap integrals
- if there are further degenerate states, the process can be continued until a full set of orthogonal functions is obtained