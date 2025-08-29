---
{"dg-publish":true,"permalink":"/content/012/px-284-smeto/part-2-electromagnetic-theory/p-em-waves/px-284-p1-introduction-to-em-waves/","noteIcon":"1","created":"2025-08-27T13:15:25.156+01:00","updated":"2025-02-23T13:23:57.000+00:00"}
---

- starting from maxwell's equations with no sources, and vector identities:
$$\begin{gather} 
\vec\nabla \times ( \vec\nabla \times \vec \omega) = \vec\nabla ( \vec\nabla\cdot\vec \omega) - \nabla^{2}\vec \omega \\\\
\vec\nabla \times (\vec\nabla \times \vec E) = \vec\nabla \times \left( - \frac{\partial  \vec B}{\partial t}\right) \\
\underbrace{\vec\nabla(\vec\nabla\cdot \vec E)}_{0} - \nabla^{2}\vec E = - \frac{\partial  }{\partial t}(\vec\nabla \times \vec B) = - \mu_{0}\varepsilon_{0} \frac{\partial^{2} {\vec E}}{\partial {t}^{2}} \\
\therefore \nabla^{2}\vec E = \mu_{0}\varepsilon_{0} \frac{\partial^{2} {\vec E}}{\partial {t}^{2}}
\end{gather}$$
- there are the wave equations for $\vec E$ and $\vec B$

- considering a generic plane wave:
$$u = u_{0} \exp(i(\vec k \cdot \vec x - \omega t))$$
- it is propagating in the direction, $\hat k$, with wavevector, $\vec k$, and angular frequency, $\omega$
- for a plane wave:
$$\begin{gather}
\vec\nabla u = + i\vec k\, u \\
\nabla^{2}u = - k^{2} u \\
\frac{\partial u}{\partial t} = -i\omega u \\
\frac{\partial^{2} {u}}{\partial {t}^{2}} = -\omega^{2}u \\
\nabla^{2} u = \frac{1}{c^{2}} \frac{\partial^{2} {u}}{\partial {t}^{2}}
\end{gather}$$
- therefore, the phase velocity of the wave is: $c = \omega/k$

- for EM waves, $c^{2} = 1/\mu_{0}\varepsilon_0$
- plugging in the values, $c$ is found to be the speed of light

$$\begin{gather}
\vec\nabla\cdot\vec E = 0 &\implies \vec k \cdot\vec E = 0 & \vec k \perp \vec E \\
\vec\nabla\cdot\vec B = 0 &\implies \vec k \cdot\vec B = 0 & \vec k \perp \vec B \\
\vec\nabla \times \vec E = - \frac{\partial \vec B}{\partial t} &\implies \vec k \times \vec E = \omega \vec B & \vec E \perp \vec B \\
\vec\nabla \times \vec B = \mu_{0}\varepsilon_{0} \frac{\partial \vec E}{\partial t} &\implies \vec k \times \vec B = -\mu_{0}\varepsilon_{0}\vec E
\end{gather}$$
- taking the curl of both sides:
$$\begin{align*}
\vec\nabla \times(\vec\nabla \times \vec B) &= - \mu_{0}\varepsilon_{0} \omega \vec\nabla\times\vec E \\
\vec k \times (\vec k \times \vec B) &= \mu_{0}\varepsilon_{0} \omega \frac{\partial \vec B}{\partial t} \\
 -k^{2}\vec B &= \mu_{0}\varepsilon_{0} \omega^{2} \vec B \\
k^{2} &= \mu_{0}\varepsilon_{0} \omega^{2} \\
\frac{\omega^{2}}{k^{2}} =c^{2} &= \frac{1}{\mu_{0}\varepsilon_{0}}
\end{align*}$$

## summary
>[!info] EM waves propagate at the speed of light:
$$c = \frac{1}{\mu_{0}\varepsilon_{0}}$$

- this is because light is an EM wave

>[!info] waves are transverse
>$$\vec E \perp \vec k \;,\; \vec B \perp \vec k$$

>[!info] the fields are perpendicular to each other and they are in phase
>$$\vec E \perp B$$

>[!info] for a given wavevector, there are two independent modes - **polarizations**

- $\vec E$ and $\vec B$ are oriented such that $\vec k \times \vec E = \omega B$
- this can form any linear combination of two modes

>[!info] 
>$$\begin{gather}
>|\vec k \times \vec E| = k |\vec E | = \omega |\vec B| \\ 
>|\vec B| = \frac{1}{c} |\vec E| \\
>\vec B = \mathcal R \frac{1}{c} \vec E
>\end{gather}$$
>where, $\mathcal R$ is a matrix that represents a $90\degree$ clockwise rotation around the direction of $\vec k$


