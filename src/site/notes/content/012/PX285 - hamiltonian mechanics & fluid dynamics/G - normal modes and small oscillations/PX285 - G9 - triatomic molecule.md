---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/g-normal-modes-and-small-oscillations/px-285-g9-triatomic-molecule/","created":"2024-12-05T19:21:44.356+00:00","updated":"2024-12-06T13:02:15.185+00:00"}
---

## the euler-lagrange equation and modes
![Pasted image 20241205225850.png|500](/img/user/pics/Pasted%20image%2020241205225850.png)
- now, considering a carbon dioxide molecule (CO$_2$)
$$\begin{gather}
T = \frac{1}{2}m_{O}\dot{\vec x_{1}}^{2} +\frac{1}{2}m_{C}\dot{\vec x_{2}}^{2} + \frac{1}{2}m_{O}\dot{\vec x_{3}}^{2} \\
V = \frac{1}{2}k(x_{2}-x_{1})^{2} + \frac{1}{2}k(x_{3}-)
\end{gather}$$
- the inertia matrix:
$$M = \begin{pmatrix}m_{O} & 0 & 0 \\ 0 & m_{C}& 0 \\ 0 & 0 & m_{O}\end{pmatrix}$$
- the stiffness matrix:
$$K = \begin{pmatrix}k & -k & 0 \\ -k & 2k & -k \\ 0 & -k & k\end{pmatrix}$$
- the euler-lagrange equation in matric form:
$$M \ddot{\vec x} = -K\vec x \tag {1}$$
- assuming $\vec x (t) = A \vec X e^{i\omega t}$, so, $\ddot{\vec x} = - \omega^{2}\vec x$
- substituting into equation $(1):$
$$ - \omega^{2}M A \vec X e^{i\omega t} = - A K \vec X e^{i\omega t}$$
- this should be equal for all time
- for an arbitrary non-zero amplitude, $A:$
$$\begin{gather}
A e^{i\omega t} [\omega^{2}M\vec X - K\vec X] = \vec 0  \\
\implies (\omega^{2}M - K)\vec X = \vec 0
\end{gather}$$
- considering the secular equation:
$$\begin{gather*}
\det (\omega^{2}M - K) = 0 \\
\begin{vmatrix}\omega^{2}m_{O} - k & k & 0 \\ k & \omega^{2}m_{C}-2k & k \\ 0 & k & \omega^{2}m_{O}-k\end{vmatrix} = 0 \\\\
\implies (\omega^{2}m_{O} - k)\bigg((\omega^{2}m_{C}-2k)(\omega^{2}m_{O} - k) -k^{2} \bigg) = 0 \\
\text{and } -k \bigg( k(\omega^{2}m_{O}-k)-0\bigg) = 0 \\
\end{gather*}$$
- this results in a cubic in $\omega^{2}$, so expect three roots with corresponding frequencies
- from the first equation:
$$(m_{0}\omega^{2}-k) \omega^{2} \left[\omega^{2}- \frac{k}{\gamma}\right] m_{O} m_{C} = 0$$
	where, $\gamma  = \cfrac{m_{O}m_{C}}{2m_{O}+m_{C}}$
- this gives three solutions:
$$\begin{align*}
	\omega^{(1)} &= \sqrt{\frac{k}{m_{O}} } \\
	\omega^{(2)} &= 0 \\
	\omega^{(3)} &= \sqrt{\frac{k}{\gamma}}
\end{align*}$$
## the first mode
- substituting it to equation $(1)$ will yield:
$$\begin{gather}
b = 0 \\
a = -c \\
\end{gather}$$
$$\therefore \vec X ^{(1)}= \begin{pmatrix}a \\ b \\ c\end{pmatrix} = a\begin{pmatrix}1\\ 0 \\ -1\end{pmatrix}$$
## the second mode
- $\omega^{(2)}$ represents translation 
- $M\ddot{\vec x} = 0$ is recovered for $\vec x(t) = A \vec X f(t)$, with $f(t) = 1 + \frac{B}{A} t$
- $-K \vec X = \vec 0:$
$$\begin{pmatrix}k & -k & 0 \\ -k & 2k & -k \\ 0 & -k & k\end{pmatrix} \begin{pmatrix}1 \\ a \\b\end{pmatrix} = \vec 0$$
$$\begin{gather}
	k(1-a) = 0 &\implies &a=1 \\
	k(-1 + 2a - b) = 0 &\implies &b =2a-1 =1 \\
	k(-a+b) = 0 &\implies &a=b
\end{gather}$$
$$\therefore \vec X^{(2)} = \begin{pmatrix}1\\1\\1\end{pmatrix}$$
- the general solution:
$$ \vec x (t) = (A^{(2)} + B^{(2)}t) \begin{pmatrix}1 \\ 1 \\ 1\end{pmatrix} t$$
## the third mode
\1\n\2\n