---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-1/d-vector-integration/d3-green-s-theorem/px-275-d3c-application-of-green-s-theorem/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2025-01-07T19:11:15.416+00:00"}
---

- choosing $P$ and $Q$ such that:
$$\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y} = 1$$
- the $RHS$ of [[content/012/PX275 - mathematical methods/term 1/D - vector integration/D3 - green's theorem/PX275 - D3a - green's theorem in the plane\|green's theorem]]: 
$$\iint_{R} \left(\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y}\right)dA =\iint_{R} 1\,dA = A$$
	where, $A$ is the enclosed area
## case 1
- setting $Q = x$, $P=0:$ 
$$\oint_{C} P\,dx + Q\,dy = \oint_{C} x\,dy = \iint_{R}dA= A$$ 
## case 2
- setting $P = -y$, $Q=0:$ 
$$\oint_{C} -y\,dx = \iint_{R} dA = A$$
## case 3
- setting $P=-y$, $Q=x:$ 
$$\iint_{R} (1-(-1))dA = 2A$$
- this is usually the most useful: 
$$\begin{gather*}
	2A = \iint_{R} \left(\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y}\right) dA =\oint P\,dx + Q\,dy \\\\
	\therefore A = \frac{1}{2} \oint_{C}x\,dy - y\,dx
\end{gather*}$$
