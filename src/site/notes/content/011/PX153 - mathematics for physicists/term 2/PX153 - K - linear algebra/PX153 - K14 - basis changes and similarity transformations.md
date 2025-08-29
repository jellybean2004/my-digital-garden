---
{"dg-publish":true,"permalink":"/content/011/px-153-mathematics-for-physicists/term-2/px-153-k-linear-algebra/px-153-k14-basis-changes-and-similarity-transformations/","noteIcon":"1","created":"2025-08-27T13:14:00.611+01:00","updated":"2024-11-26T19:40:37.000+00:00"}
---

- in $3\times 3$ case:
$$\begin{align*}
		\vec e' &= S_{11}\vec e_{1} + S_{12}\vec e_{2} + S_{13}\vec e_{3} \\
		\begin{bmatrix}\vec e_{1}' \\ \vec e_{2}' \\ \vec e_{3}'\end{bmatrix} &= \begin{bmatrix}S_{11} & S_{12} & S_{13} \\ S_{21} & S_{22} & S_{23} \\ S_{31} & S_{32} & S_{33}\end{bmatrix} \begin{bmatrix}\vec e_{1} \\ \vec e_{2} \\ \vec e_{3}\end{bmatrix}
\end{align*}$$
$$\begin{align*}
		\vec r' &= x_{1}' \vec e_{1}'+ x_{2}' \vec e_{2}' + x_{3}' \vec e_{3}' \\
		&= \sum\limits_{i=1}^{3} x_{i}' \vec e_{i}' \\
		&= \sum\limits_{i=1}^{3} x_{i}' \;\sum\limits_{j=1}^{3} S_{ij}\vec e_{j} \\
		&= \sum\limits_{j=1}^{3} \left(\sum\limits_{i=1}^{3} x_{i}'  S_{ij}\right)\vec e_{j}\\\\
		let,\, x_{j}&= \sum\limits_{i} x_{i}' S_{ij} \\\\
		\vec r' = \sum\limits_{j}x_{j}\vec e_{j} &= \sum\limits_{i}x_{i}'\vec e_{i}'
	\end{align*}$$
- in 3D:
$$\begin{align*}
		\begin{bmatrix}x_{1} \\ x_{2} \\ x_{3}\end{bmatrix} &= S \begin{bmatrix}x_{1}' \\ x_{2}' \\ x_{3}'\end{bmatrix} \\
		\begin{bmatrix}x_{1}' \\ x_{2}' \\ x_{3}'\end{bmatrix} &= S^{-1}\begin{bmatrix}x_{1} \\ x_{2} \\ x_{3}\end{bmatrix}\\
		but,
		\begin{bmatrix}\vec e_{1}' \\ \vec e_{2}' \\ \vec e_{3}'\end{bmatrix} &= S^{-1}\begin{bmatrix} \vec e_{1} \\ \vec e_{2} \\ \vec e_{3}\end{bmatrix}\\
	\end{align*}$$
- eg: in 2D, rescale basis vectors:
$$\begin{align*}
		\begin{bmatrix} \vec e_{1}'  \\ \vec e_{2}' \end{bmatrix} &= \begin{bmatrix}2 & 0 \\ 0 & 2\end{bmatrix} \begin{bmatrix} \vec e_{1} \\ \vec e_{2} \end{bmatrix} \\
		\begin{bmatrix} x_{1}'  \\ x_{2}' \end{bmatrix} &= \begin{bmatrix} 1/2 & 0 \\ 0 & 1/2 \end{bmatrix} \begin{bmatrix} x_{1}  \\ x_{2}\end{bmatrix} = \begin{bmatrix} \frac{x_{1}}{2} \\ \frac{x_{2}}{2}\end{bmatrix}
	\end{align*}$$
	- basis is two times larger, so the vectors will be two times smaller in the new basis
