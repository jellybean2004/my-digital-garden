---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/g-normal-modes-and-small-oscillations/px-285-g7-example/","created":"2024-11-29T19:02:39.967+00:00","updated":"2024-11-29T19:53:28.214+00:00"}
---

![Pasted image 20241129195231.png|500](/img/user/pics/Pasted%20image%2020241129195231.png) 
## the inertia and stiffness matrices
- the total kinetic energy:
$$T = \frac{1}{2}m\dot x_{1}^{2} + \frac{1}{2}m\dot x_{2}^{2}$$
- the inertia matrix:
$$M = \begin{pmatrix}\frac{\partial^{2} {T}}{\partial {\dot x_{1}^{2}}} & \frac{\partial^{2} {T}}{\partial {\dot x_{1}} \partial \dot x_{2}} \\\frac{\partial^{2} {T}}{\partial {\dot x_{2}} \partial \dot x_{1}}  & \frac{\partial^{2} {T}}{\partial \dot x_{2}^{2}} \end{pmatrix} = \begin{pmatrix}m & 0 \\ 0 & m\end{pmatrix}$$
- the potential energy:
$$V = \frac{1}{2}kx_{1}^{2} + \frac{1}{2}k_(x_{2}-x_{1})^{2} + \frac{1}{2}(-x_{2})^{2}$$
- the stiffness matrix:
$$K = \begin{pmatrix}\frac{\partial^{2} {V}}{\partial { x_{1}^{2}}} & \frac{\partial^{2} {V}}{\partial { x_{1}} \partial  x_{2}} \\\frac{\partial^{2} {V}}{\partial { x_{2}} \partial x_{1}}  & \frac{\partial^{2} {V}}{\partial  x_{2}^{2}} \end{pmatrix} = \begin{pmatrix}2k & -k \\ -k & 2k\end{pmatrix}$$
- these can now be used to solve the vector euler-lagrange equation:
$$M \ddot{\vec x} = -K\vec x$$
- the solutions are sinusoidal in time $(\sim \exp(i\omega t))$ and satisfy the condition: $\det(K - \omega^{2}M) = 0$
$$\begin{vmatrix} 2k-\omega^{2}m & -k \\ -k & 2k-\omega^{2}m \end{vmatrix} = (2k-\omega^{2}m)^{2} - k^{2}  = 0$$
$$\begin{gather}
2k-\omega^{2}m  = +k \implies \omega^{(1)} = \sqrt{\frac{k}{m}} \\
2k-\omega^{2}m  = -k \implies \omega^{(3)} = \sqrt{\frac{3k}{m}} 
\end{gather}$$
- these are the first and second modes
## first mode
$$B = K - \omega^{(1)} M = \begin{pmatrix}k & -k \\ -k & k\end{pmatrix}$$
- hence, 
$$\begin{pmatrix}k & -k \\ -k & k\end{pmatrix} \vec X^{(1)} = \vec 0$$
$X^{(n)}= \begin{pmatrix}a \\ b\end{pmatrix}:$
$$\begin{align*}
	ka - kb &= 0 \\
	-ka + kb &= 0
\end{align*}$$
- these are two redundant solutions that give:
$$a = b$$
- the scale is not known, but the amplitudes are arbitrary
- thus the first mode is:
$$\vec x^{(1)}(t) = A^{(1)} \begin{pmatrix}1 \\ 1\end{pmatrix} \exp(i\omega t)$$
![Pasted image 20241129195252.png|500](/img/user/pics/Pasted%20image%2020241129195252.png)
## second mode
$$B = K - \omega^{(2)} M = \begin{pmatrix}-k & -k \\ -k & -k\end{pmatrix}$$
- hence, 
$$\begin{pmatrix}-k & -k \\ -k & -k\end{pmatrix} \vec X^{(2)} = \vec 0$$
$X^{(n)}= \begin{pmatrix}a \\ b\end{pmatrix}:$
$$\begin{align*}
	-ka - kb &= 0 \\
	-ka - kb &= 0
\end{align*}$$
- again, these are two redundant solutions that give:
$$a = -b$$
- the scale is not known, but the amplitudes are arbitrary
- thus the first mode is:
$$\vec x^{(2)}(t) = A^{(2)} \begin{pmatrix}1 \\ -1\end{pmatrix} \exp(i\omega t)$$
![Pasted image 20241129195308.png|500](/img/user/pics/Pasted%20image%2020241129195308.png)
## general solution
$$\vec x(t) = A^{(1)} \begin{pmatrix}1 \\ 1\end{pmatrix} \exp(i\omega t) + A^{(2)} \begin{pmatrix}1 \\ -1\end{pmatrix} \exp(i\omega t)$$
- considering the initial conditions: $x_{1}(t) = t$, $x_{2}(t) = -t$, and $\dot x_{1} = \dot x_{2} =0:$
$$\vec x(0) = A^{(1)} \begin{pmatrix}1 \\ 1\end{pmatrix} + A^{(2)} \begin{pmatrix}1 \\ -1\end{pmatrix} $$
- the initial conditions are only satisfied by the second mode, so: $A^{(1)}= 0$, and $A^(2)=t$

- considering the initial conditions: $x_{1}(0) = x_{2}(0) = 0$, and $\dot x_{1}(0) = \dot x_{2}(0) = \delta:$
$$\begin{gather*}
\dot{\vec x } = i\omega^{(1)} A^{(1)} \begin{pmatrix}1 \\1\end{pmatrix} \exp(i\omega^{(1 )}t ) + i\omega^{(2)} A^{(2)} \begin{pmatrix}1 \\-1\end{pmatrix} \exp(i\omega^{(2)}t ) \\
\dot{\vec x}(0) = i\omega^{(1)} A^{(1)} \begin{pmatrix}1 \\1\end{pmatrix} + i\omega^{(2)} A^{(2)} \begin{pmatrix}1 \\-1\end{pmatrix}
\end{gather*}$$
- this requires $A^{(2)}=0$ and $i\omega A^{(1)}=\delta$
$$\begin{gather}
Im(i\omega^{(1)}A^{(1)}) = \delta, & Im(A^{(2)}) = 0, \\
Re(A^{(1)}) = 0, & Re(A^{(2)}) =0
\end{gather}$$
$$\vec x(0) = A^{(1)}\begin{pmatrix}1 \\ 1\end{pmatrix} + A^{(2)} \begin{pmatrix}1 \\-1\end{pmatrix} = 0$$
$$\therefore \vec x(t) = - \frac{i\delta}{\omega^{(1)}} \begin{pmatrix}1\\1\end{pmatrix} \exp(i\omega^{(1)})  = \frac{\delta}{\omega^{(1)}}  \begin{pmatrix}1\\1\end{pmatrix}  \exp\left(i\omega^{(1)}t + \frac{3}{2}\pi \right)$$
