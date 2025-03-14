---
{"dg-publish":true,"permalink":"/content/012/px-262-quantum-mechanics/term-2/h-free-electron-model/px-262-h4-free-electron-model-3-d/","noteIcon":"1","created":"2025-01-13T11:11:53.829+00:00","updated":"2025-03-13T10:36:37.788+00:00"}
---

- now, considering a box of dimensions: $L_{x} \times L_{y} \times L_{z}$
$$ \begin{gather}
- \frac{\hbar^{2}}{2m} \nabla^{2} \phi(\vec r) = E \phi(\vec r) \\\\
\phi = A \exp(i(k_{x}x  + k_{y}y + k_{z}z)) \\\\
E = \frac{\hbar^{2}k^{2}}{2m_{e}} = \frac{\hbar^{2}}{2m_{e}} ( k_{x} ^{2} + k_{y}^{2} + k_{z}^{2})
\end{gather}$$
- applying periodic boundary conditions:
$$\begin{gather}
\phi(0, y, z) = \phi(L_{x}, y, z) \\
\phi(x, 0, z) = \phi(x, L_{y}, z) \\
\phi(x, y, 0) = \phi(x, y, L_{z}) \\
\end{gather}$$
- from the first condition:
$$\begin{gather}
A \exp(i (k_{x}L_{x} + k_{y}y + k_{y}z)) = A \exp(i (k_{y}y + k_{z}z) ) \\
\implies \exp(ik_{x}L_{x}) = 1
\end{gather}$$
- similarly:
$$\begin{gather}
\exp(ik_{y}L_{y}) = 1 \\
\exp(ik_{z}L_{z}) = 1
\end{gather}$$
- therefore, the **wavevector**:
$$\vec k = \left( \frac{2\pi n_{x}}{L_{x}}, \frac{2\pi n_{y}}{L_{y}}, \frac{2\pi n_{z}}{L_{z}} \right)$$
	where, $n_{x}, n_{y}, n_{z} \in \mathbb{Z}$

- the allowed states sit on a grid in wavevector-space

![PX262 - H4 - free electrons in 3D.png|500](/img/user/pics/PX262%20-%20H4%20-%20free%20electrons%20in%203D.png)

- each block, contains one allowed $\vec k$ vector (each corner shared between eight blocks)
$$\Delta k_{x} \Delta k_{y} \Delta k_{z} = \frac{8\pi^{3}}{L_{x}L_{y}L_{z}} = 8\pi^{3}/V$$
- these single electron states can be occupied by two electrons: spins $\uparrow$ and $\downarrow$
- ground state: fill all states ($\uparrow$ and $\downarrow$) up to $E = E_{F}$ or $|\vec k| \leq k_{F}$

![PX262 - H4 - free electrons in 3D-1.png|500](/img/user/pics/PX262%20-%20H4%20-%20free%20electrons%20in%203D-1.png)

- occupied states lie in a sphere in the k-space
- total number of electrons:
$$N = 2 \times \frac{\text{Vol. of sphere}}{\text{Vol. per k point}} = 2 \times \frac{4}{3}\pi k_{F}^{3} \frac{V}{8\pi^{3}} = \frac{V}{3\pi^{3}} k_{F}^{3}$$
	where, 2 is for each spin
$$\implies k_{F} = \left(\frac{3\pi^{2}N}{V}\right)^{1/3} = (3\pi^{2}\rho_{e})^{1/3}$$
	where, $\rho_{e}$ is the electron density

- $k_{F}$ is the radius of the **fermi sphere**, and also the magnitude of the **fermi wavevector**, $\vec k_F$
- fermi wavevector and fermi energy are set by the density, $\rho_{e}:$
$$E_{F} = \frac{\hbar^{2}}{2m_{e}} (3\pi ^{2}\rho_{e})^{2/3}$$
- also, the fermi velocity:
$$\vec v_{F} = \vec\nabla \omega(\vec k) = \frac{\hbar \vec k}{m_{e}}$$
- and the fermi speed: $\hbar k_F /m_e$
- this is the group velocity of the wave packet with $\vec  k$ grouped around $\vec k_F$
## density of states
- for a large $V$, it is expected that: $\Delta k_{x,y,z} \to 0$, forming a continuum of states in the space of $\vec k$ (k-space)
- the number of states with an energy below $E = \hbar^{2}k^{2}/2m_{e}:$
$$N(E) = \frac{Vk^{3}}{3\pi^{2}} = \frac{V}{3\pi^{2}} \left(\frac{2m_{e}E}{\hbar^{2}}\right)^{3/2}$$

- the number of states between $E$ and $(\Delta E + dE):$
$$n(E)\,dE = \frac{dN}{dE} \,dE = \frac{3}{2} \frac{V}{3\pi^{2}} \left(\frac{2m_{e}}{\hbar^{2}}\right)^{3/2}E^{1/2}\,dE$$
ie. the density of states:
$$n(E) = \frac{V}{2\pi^{2}} \frac{2m_{e}}{\hbar^{2}}^{3/2} E^{1/2}$$
- let ${} \alpha = \cfrac{1}{2\pi^{2}} (\cfrac{2m_{e}}{\hbar^{2}})^{3/2} {}$
$$N = \int_{0}^{E_{F}} n(E)\,dE = V \alpha E_{F}^{3/2} \frac{2}{3}$$
- $n(E)$ can be used to compute some properties
- the simplest is the total energy:
$$E_{TOT} = \int_{0}^{E_{F}} E\,n(E)\,dE = V\alpha \int_{0}^{E_{F}}E^{3/2}\,dE = V \alpha \frac{2}{5}E_{F}^{5/2}$$
- the average energy per particle:
$$\frac{E_{TOT}}{N} = \frac{3}{5} E_{F}$$

|     | $\rho_{e}$<br>(m$^{-3}$) | $E_{F}$<br>(eV) | $k_{F }$<br>(Å$^{-1}$) | $v_{F}$<br>(ms$^{-1}$) |
| --- | ------------------------ | --------------- | ---------------------- | ---------------------- |
| Li  | $4.7\times10^{28}$       | $4.74$          | $1.12$                 | $1.29\times10^6$       |
| Al  | $18.1\times10^{28}$      | $11.7$          | $1.75$                 | $2.05\times10^6$       |

- the free fermion model is relevant in other areas:
	- white dwarfs: $E_{F}\sim 0.3\times10^{6}$ eV
	- neutron stars: $E_{F}\sim 40\times10^{6}$ eV

## temperatue

**note:** $k_{B}T \leq E_{F}\sim 4.7\,\text{eV} \to 55\,000$ K
- introducing $f(E)$, probability of states with energy, $E$, are occupied

![PX262 - H4 - free electron model (3D).png|500](/img/user/pics/PX262%20-%20H4%20-%20free%20electron%20model%20(3D).png)

- for a non-zero $T$, $f$ is given by the **fermi-dirac distribution (FD)**: 
$$f(E, \mu , T) = \frac{1}{\exp\cfrac{E-\mu}{k_{B}T}  + 1}$$
	where, $\mu$ is the chemical potential

- in metals, $\mu \simeq E_{F}$
- strictly:
$$\begin{gather}
	T = 0 & N = \int_{0}^{E_{F}}n(E )\,dE & \mu = E_{F} \\
	T \neq 0 & N = \int_{0}^{E_{F}}f(E, \mu, T)\,n(E )\,dE & \mu = \text{fixed}
\end{gather}$$

## heat capacity
$$E_{TOT} (T) = \int dE\, n(E)\, E\, f(E, \mu, T) = E_{TOT}(0 ) + aT^{2} + \dots$$
- can argue that some electrons in states below $E_{F}$ thermally excited to states above $E_{F}$
- $\Delta E:$ number of excitations $\times k_{B}T \sim n(E_{F})\,k_{B}T \times k_{B}T = aT^{2}$ , where $a \sim n(E_{F})k_{B}^{2}$
	- assuming the variation of $n(E)$ within $k_{B}T$ of $E_F$ negligible
- the heat capacity:
$$C_{V} = \frac{dE_{TOT}}{dT } = 2aT$$
- linear dependence of $C_{V}$ on $T$ is characteristic of metals
