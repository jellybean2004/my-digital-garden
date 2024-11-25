---
dg-publish: true
---

the representation $A\vec x = \vec b$ describes a mapping of the vector space, $\vec x$, to the vector space, $\vec b$, by the matrix, ${} \vec A$
- these spaces may or may not have the same dimensions
	- if $\det A=0$, or if $A_{m\times n},\; m\neq n:$ the dimensions will be different

- an important set of vectors of the mapping with matrix $A$ (in $n\times n$ case only) is the set of eigenvectors (from equation $:A\vec x = \lambda \vec x$)
- if there is a change in the coordinate system for the vectors, matrix $A$ will have different elements for the same transformation, but matrix $A$ will have the same *eigenvector*, *eigenvalue*, and *determinant*
## examples of mapping
### rotation in 2D
- consider the effect of rotation about the $z$-axis:
$$\hat x = \begin{bmatrix}1 \\ 0\end{bmatrix} \to \begin{bmatrix}\cos\theta \\ \sin\theta\end{bmatrix},\; \hat y = \begin{bmatrix}0 \\ 1\end{bmatrix} \to \begin{bmatrix}-\sin\theta \\ \cos\theta\end{bmatrix}$$
$$\vec r' = x \begin{bmatrix}\cos\theta \\ \sin\theta\end{bmatrix} + y \begin{bmatrix}-\sin\theta \\ \cos\theta\end{bmatrix} = \begin{bmatrix}\cos\theta  & -\sin\theta \\ \sin\theta & \cos\theta\end{bmatrix} \begin{bmatrix}x \\ y\end{bmatrix}$$
- matrix $R(\theta)_{2D}$ describes rotation by $\theta$ about the $z$-axis in the anti-clockwise direction as viewed from above
### rotation in 3D about z-axis (anti-clockwise)
$$\vec r' = R(\theta_{z})\,\vec r = \begin{bmatrix}\cos\theta_{z} & -\sin\theta_z & 0 \\ \sin\theta_{z} & \cos\theta_z & 0 \\ 0 & 0 & 1\end{bmatrix} \vec r = \begin{bmatrix}x\cos\theta_{z}-y\sin\theta_{z} \\ x\sin\theta_{z}+y\cos\theta_{z} \\ z\end{bmatrix}$$
### rotation about y-axis in 3D (anti-clockwise)
$$\vec r' = R(\theta_{y})\,\vec r = \begin{bmatrix}\cos\theta_{y} & 0 & \sin\theta_y \\ 0 & 1 & 0 \\ -\sin\theta_{y} & 0 & \cos\theta_{y} \end{bmatrix}\vec r$$
### rotation about x-axis in 3D (anti-clockwise)
$$\vec r' = R(\theta_{x})\,\vec r = \begin{bmatrix} 1 & 0 & 0 \\ 0 & \cos\theta_{x} & -\sin\theta_{x} \\ 0 & \sin\theta_x & \cos\theta_{y} \end{bmatrix}\vec r$$
- **note**: 
	- $R(\theta_{x}), R(\theta_{y}), R(\theta_{z})$ can represent any arbitrary rotation in 3D
	- $\det R(\theta_{x}), \det R(\theta_{y}), \det R(\theta_{x}) =1$
### stretching/shrinking of vectors
- 2D:
$$\vec r' = \begin{bmatrix}x' \\ y'\end{bmatrix} = \begin{bmatrix}\alpha & 0 \\ 0 & \alpha\end{bmatrix} \begin{bmatrix}x \\ y\end{bmatrix}= \begin{bmatrix}\alpha x \\ \alpha y \end{bmatrix}$$
	- $\det A = \alpha^{2}$
### inversion
- $\vec r \to \vec r' = -\vec r:$
$$\begin{bmatrix}x' \\ y'\end{bmatrix} = \begin{bmatrix}-1 & 0 \\ 0 & -1\end{bmatrix} \begin{bmatrix}x \\ y\end{bmatrix} = \begin{bmatrix}-x \\ -y\end{bmatrix}$$
	- $\det A =1$
- the role of a determinant of a matrix is to give the magnification factor for the mapping of $A$ applied to a vector space

- **proof in 2D**
	- consider the effect of a matrix, $A = \begin{bmatrix}a_{11} & a_{12} \\ a_{21} & a_{22}\end{bmatrix}$, on a square, $(0,0),(0,1),(1,1),(1,0)$ 
	$$\begin{align*}
		\begin{bmatrix}a_{11} & a_{12} \\ a_{21} & a_{22}\end{bmatrix}\begin{bmatrix}1 \\ 0\end{bmatrix} &= \begin{bmatrix}a_{11} \\ a_{21}\end{bmatrix} \\
		\begin{bmatrix}a_{11} & a_{12} \\ a_{21} & a_{22}\end{bmatrix}\begin{bmatrix}0 \\ 1\end{bmatrix} &= \begin{bmatrix}a_{12} \\ a_{22}\end{bmatrix} \\
		\begin{bmatrix}a_{11} & a_{12} \\ a_{21} & a_{22}\end{bmatrix}\begin{bmatrix}1 \\ 1\end{bmatrix} &= \begin{bmatrix}a_{11}+a_{12} \\ a_{21}+a_{22}\end{bmatrix}
	\end{align*}$$
	- area of the new shape $= (a_{11},a_{21},0)\times (a_{12},a_{22},0) = (a_{11}a_{22}-a_{21}a_{12}) = \det A$ 
