---
{"dg-publish":true,"permalink":"/content/012/px-285-hamiltonian-mechanics-and-fluid-dynamics/g-normal-modes-and-small-oscillations/px-285-g4-attached-particles-on-springs/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2025-01-05T13:18:35.443+00:00"}
---

- consider two masses $(m)$ connected to a fixed wall is connected with a spring such that all springs are at rest in equilibrium conjugation, and are at equilibrium extension 

## first mode
- suppose the springs are moved in the same direction

![PX285 - G4 - attached particles on springs.png|500](/img/user/pics/PX285%20-%20G4%20-%20attached%20particles%20on%20springs.png)

- if $x_{1}=x_{2}$, the central spring is never stressed and plays no role
- hence, it can be removed

![[Pasted image 20250105131503.png\|500]]

- frequency of either mass connected to spring: $\omega = \sqrt{\frac{k}{m}}$
- there exists a mode with frequency, $\omega$, and $x_{1}=x_{2}$
- this is the **symmetric mode** with:
$$\vec x = \begin{pmatrix}x_{1} \\ x_{2}\end{pmatrix}$$

![PX285 - G4 - attached particles on springs-5.png|500](/img/user/pics/PX285%20-%20G4%20-%20attached%20particles%20on%20springs-5.png)
 
- the solution to this will be: 
$$\vec x(t) = A \begin{pmatrix}1 \\ 1\end{pmatrix} \exp(i\omega t)$$
- this is a **mode**

## second mode
- suppose the masses are moving in opposite directions

![PX285 - G4 - attached particles on springs-5.png|500](/img/user/pics/PX285%20-%20G4%20-%20attached%20particles%20on%20springs-5.png)

- this is equivalent to cutting the system in half, and fixing it to a wall as the centre of the middle spring is stationary

![PX285 - G4 - attached particles on springs-7.png|500](/img/user/pics/PX285%20-%20G4%20-%20attached%20particles%20on%20springs-7.png)

- if the mass is moved a distance, $x_1$, the central (cut) spring is compressed by $2x_1$
- the energies:
$$\begin{align*}
E_{centre} &= \frac{1}{2} k (2x_{1})^{2} \\
\implies E_{half} &= \frac{1}{2} E_{centre} = kx_{1}^{2}
\end{align*}$$