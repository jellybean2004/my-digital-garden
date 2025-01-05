---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/f-hamilton-s-equations/px-285-f5-central-forces-particle-approaching-the-sun/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2025-01-05T10:09:18.113+00:00"}
---

## determining the lagrangian
- considering the position vector of the particle in polar coordinates: 
$$\vec r (t) = r(t) \begin{pmatrix}\cos\theta(t) \\ \sin\theta(t)\end{pmatrix}$$
- the velocity: 
$$\vec v = \dot r \begin{pmatrix}\cos\theta(t) \\ \sin\theta(t)\end{pmatrix}  + r\dot\theta \begin{pmatrix}-\sin\theta(t) \\ \cos\theta(t)\end{pmatrix} = \dot r \, \hat r + r\dot \theta \,\hat \theta$$
- the square of the velocity: 
$$v^{2} = \vec v \cdot \vec v = (\dot r \, \hat r + r\dot \theta \,\hat \theta)\cdot(\dot r \, \hat r + r\dot \theta \,\hat \theta)  = \dot r^{2} + (r\dot\theta)^{2}$$
- the kinetic energy: 
$$T = \frac{1}{2} m(\dot r^{2} + (r\dot \theta)^{2})$$
- and the potential energy: 
$$V = V(r)$$
- therefore, the lagrangian is: 
$$L = \frac{1}{2} m(\dot r^{2} + (r\dot \theta)^{2}) - V(r) \tag{1}$$
## formulating the euler-lagrange equations
- the components of the canonical momentum: 
$$\begin{align*}
	\frac{\partial L}{\partial \dot r} = p_{r}&= m \dot r \tag{2}\\
	\frac{\partial L}{\partial \dot \theta} = p_{\theta}&= mr^{2}\dot\theta \tag{3}
\end{align*}$$
- **note:** $p_\theta$ does not have the dimensions of canonical momentum, it is the **angular momentum**
- the time derivatives: 
$$\begin{align*}
\frac{\partial L}{\partial r} &= \dot p_{r} = mr \dot \theta^{2} - \frac{\partial V}{\partial r} \tag{4}\\ 
\frac{\partial L}{\partial \theta} &= \dot p_{\theta} = 0 \tag{5}
\end{align*}$$
- the angular momentum, $p_{\theta}$, is a conserved quantity, and it arises from the rotational invariance of the system
- from $(3): \dot\theta = \frac{p_{\theta}}{mr^{2}}$
- from $(2)$ and $(4):$ 
$$\begin{align*}
\frac{d}{dt}(m\dot r) &= mr\dot\theta^{2} - \frac{\partial V}{\partial r} \\
m\ddot r &= \frac{p_{\theta}^{2}}{mr^{3}} - \frac{\partial V}{\partial r} = -\frac{\partial V_{eff}}{\partial r} \tag{6}\\
\end{align*}$$
- the effective potential: 
$$V_{eff} = V + \frac{1}{2} \frac{p_{\theta}^{2}}{mr^{2}}$$
- equation $(6)$ can be solved for $r(t)$
## the energy of the system
- considering the energy: 
$$\begin{align*}
	H = T + V  &= \frac{1}{2}m(\dot r^{2} + (r\dot\theta)^{2}) + V(r) \\
	&= \frac{1}{2}m\left(\dot r^{2} + \frac{p_{\theta}^{2}}{m^{2}r^{2}} \right) + V(r) \\
	\therefore H(p_{r}, p_{\theta}, r, \theta) &= \frac{1}{2m}p_{r}^{2} + \frac{1}{2mr^{2}} p_{\theta}^{2} + V(r) = E \tag{7}
\end{align*}$$
- rearranging for $p_{r}:$ 
$$\begin{gather}
p_{r} = \sqrt{\left(E-V(r) - \frac{1}{2mr^{2}} p_{\theta}^{2}\right)2m} \\
\implies p_{r}=  m\dot r = \sqrt{2m(E - V_{eff}(r))} \tag{8}
\end{gather}$$
- the values of $r$ that are the roots of ${} (E-V_{eff}(r))=0$ are points above $p_{r}=0$

![PX285 - F5 - central forces.png|500](/img/user/pics/PX285%20-%20F5%20-%20central%20forces.png)
## determining the trajectory
- from equation $(3):$ 
$$\begin{align*}
	\frac{d\theta}{dt} &= \frac{p_{\theta}}{mr(t)^{2}} \\
	\int d\theta &= \int^{t} \frac{p_{\theta}}{mr(t')^{2}} dt' \\
	\theta - \theta_{0} &= \int_{0}^{t} \frac{p_{\theta}}{mr(t)^{2}}dt \tag{9}
\end{align*}$$
- from equation $(6):$ 
$$m \ddot r = \frac{p_{\theta}^{2}}{mr^{3}} - \frac{\partial V}{\partial r}$$
- to solve this equation:
	[1] adopting a parametric approach: $t \to \theta$, equivalently, changing the variables from $t$ to $\theta$
	[2] dealing with the inverse of $r$
### [1] parameterization
$$\frac{d}{dt} = \frac{d\theta}{dt} \frac{d}{d\theta} = \frac{p_{\theta}}{mr^{2}} \frac{d}{d\theta}$$
- thinking of $r(t)$ as $r(\theta)$, and from equation $(6):$ 
$$m \frac{d^{2}}{dt^{2}} r(t) = m \left(\frac{p_\theta}{mr^{2}} \frac{d}{d\theta}\right)\left(\frac{p_{\theta}}{mr^{2}} \frac{d}{d\theta}\right)r(\theta) = \frac{p_{\theta}^{2}}{mr^{3}} - \frac{\partial V}{\partial r}$$
- defining: $r' = \frac{dr}{d\theta}$, $r'' = \frac{d^{2}r}{d\theta^{2}}:$ 
$$\begin{align*}
	\frac{p_{\theta}^{2}}{mr^{3}} - \frac{\partial V}{\partial r} &= \frac{p_\theta}{r^{2}} \frac{d}{d\theta} \left(\frac{p_\theta}{mr^{2}} r'\right) \\
	&= \frac{p_{\theta}}{r^{2}} \left[\frac{p_\theta}{mr^{2}} r'' - 2\frac{p_\theta}{mr^{3}} (r')^{2}\right] \\
	\frac{p_{\theta}^{2}}{mr^{3}} - \frac{\partial V}{\partial r} &= \frac{p_{\theta}^{2}}{mr^{2}} \left[\frac{r''}{r^{2}}- \frac{2r'^{2}}{r^{3}}\right] \tag{10}
\end{align*}$$
### [2] considering the inverse
- defining $u$ as the inverse of $r:$
$$\begin{gather}
u(\theta) = \frac{1}{r(\theta)} \\
u' = \frac{d}{d\theta}\left(\frac{1}{r}\right)= - \frac{r'}{r^{2}} \\ 
u'' = \frac{d}{d\theta}\left(- \frac{r'}{r^{2}}\right)= - \frac{r''}{r^{2}} + 2 \frac{(r')^{2}}{r^{3}}
\end{gather}$$
- equation $(10)$ can be written as: 
$$\frac{p_{\theta}^{2}u^{3}}{m} - \frac{\partial V}{\partial r} = \frac{p_{\theta}^{2}u^{2}}{m} \left[ - u''\right] \tag{11}$$
- assuming $V(r) = - \frac{\alpha}{r}:$ 
$$\frac{\partial V}{\partial r} = \frac{\alpha}{r^{2}} = \alpha u^{2}$$
- using this in equation $(11):$ 
$$\begin{align*}
	\frac{p_{\theta}^{2}}{m}u^{3} - \alpha u^{2} &= - \frac{p_{\theta}^{2}}{m}u^{2}u'' \\
	-u + \frac{\alpha m}{p_{\theta}^{2}} &= u'' \\
	u'' + u &= \frac{\alpha m}{p_{\theta}^{2}} = constant \\
\end{align*}$$
- this is a second-order inhomogeneous differential equation
### solving the second-order inhomogeneous differential equation
$$ u'' + u = \frac{\alpha m}{p_{\theta}^{2}} \tag{12}$$
- considering the homogeneous part:
$$u'' + u = 0$$
- which looks like SHM with $\omega=1$
- the solutions of the complementary function will be: 
$$u_{CF} = \epsilon \cos(\theta-\theta_{0}) = A\cos\theta + B\sin\theta$$
- the particular integral: 
$$u_{PI} = \frac{\alpha m}{p_{\theta}^{2}}$$
- the full solution: 
$$u = u_{CF}+ u_{PI} = \epsilon\cos(\theta-\theta_{0}) + \frac{\alpha m}{p_{\theta}^{2}} \tag{13}$$
## case 1 
$$\begin{align*}
\epsilon &= 0 \\ 
u &= \frac{\alpha m}{p_{\theta}^{2}} \\
\implies r &= \frac{p_{\theta}^{2}}{\alpha m}
\end{align*}$$
- this is a trivial solution, which is circular orbit of constant radius, the direction given by the sign of $p_{\theta}$

![PX285 - F5 - central forces-1.png|500](/img/user/pics/PX285%20-%20F5%20-%20central%20forces-1.png)
## case 2 
$$0<\epsilon< \frac{m\alpha}{p_{\theta}^{2}}$$

![PX285 - F5 - central forces-2.png|500](/img/user/pics/PX285%20-%20F5%20-%20central%20forces-2.png)

- $u>0$ because $\epsilon<\frac{m\alpha}{p_{\theta}^{2}}$
- for **unbound** orbits, $r\to\infty: u\to0$, so this orbit is **bound**
$$\begin{align*}
	u_{max} = \epsilon + \frac{m\alpha}{p_{\theta}^{2}} &\implies r_{min} = \frac{1}{\epsilon + \frac{m\alpha}{p_{\theta}^{2}}} \\
	u_{max} = -\epsilon + \frac{m\alpha}{p_{\theta}^{2}} &\implies r_{min} = \frac{1}{-\epsilon + \frac{m\alpha}{p_{\theta}^{2}}} \\
\end{align*}$$

![PX285 - F5 - central forces-3.png|500](/img/user/pics/PX285%20-%20F5%20-%20central%20forces-3.png)
## case 3
- for 
$$\epsilon > \frac{m\alpha}{p_{\theta}^{2}}$$

![PX285 - F5 - central forces-4.png|500](/img/user/pics/PX285%20-%20F5%20-%20central%20forces-4.png)

- $u\to0$ and ${} r\to\infty$ at two special angles: $\theta_{1}, \theta_{2}$
- therefore, this is an **unbound** orbit, or a **'scattering'** event, and the particle follows a **hyperbolic orbit**

![PX285 - F5 - central forces-5.png|500](/img/user/pics/PX285%20-%20F5%20-%20central%20forces-5.png)
## case 4
$$\epsilon = \frac{m\alpha}{p_{\theta}^{2}}$$
- the particle follows a **bound parabolic** orbit

![PX285 - F5 - central forces-6.png|500](/img/user/pics/PX285%20-%20F5%20-%20central%20forces-6.png)
