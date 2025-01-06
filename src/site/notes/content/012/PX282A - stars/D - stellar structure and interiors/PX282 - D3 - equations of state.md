---
{"dg-publish":true,"permalink":"/content/012/px-282-a-stars/d-stellar-structure-and-interiors/px-282-d3-equations-of-state/","noteIcon":"1","created":"2024-11-25T10:50:32.000+00:00","updated":"2025-01-06T18:15:15.884+00:00"}
---

- they relate pressure, density, and temperature 
- recap: 
$$\begin{gather*}
\frac{dM_{r}}{dr} = 4\pi r^{2}\rho \\
\frac{dP}{dr} = - \rho \frac{GM_{r}}{r^{2}} \\
\frac{dL}{dr} = 4\pi r^{2} \epsilon_{N}\rho \\
\frac{dT}{dr} = - \frac{3\kappa\rho}{16ac\pi r^{2}T^{3}} L
\end{gather*}$$
## the standard equation of state
- [[content/011/PX154 - physics foundations/PX154 - C - thermal physics 2/PX154 - C1 - ideal gas equation of state\|the ideal gas law]]: 
$$P = nk_{B}T \tag{1}$$
- in terms of mass density: 
$$P = \frac{\rho}{\mu m_{H}} k_{B}T \tag{1.1}$$
	where, $\mu=$ the average mass per particle, and $m_{H}=$ mass of hydrogen

- in the sun, the mass fractions of hydrogen, $X_{\odot} \simeq 0.7$, helium, $Y_{\odot} \simeq 0.28$, and everything else ('*metals*'), $Z_{\odot} \simeq 0.02$
	- for a fully ionized hydrogen, $\mu = \frac{1}{2}$ (2 particles per $m_{H}: 1p,1e$)
	- for $He: \mu = \frac{4\,m_{H}}{3\,particles} = \frac{4}{3}$ (1 nucleus and 2 electrons)
	- for $Z: _{6}^{12}C, \;_{8}^{16}O \to \mu \simeq 2$
	- overall: $\mu_{\odot} \simeq 0.6$

## the equation of state for radiation
- the radiation pressure:
$$P = \frac{1}{3}aT^{4} \tag{2}$$
	where, $a = \frac{4\sigma}{c}$
## the equation of state for a degenerate gas
- for an ideal gas, $T\to0$ as $P\to0$
- consequently, the average particle speed, and hence the average momentum also tend to zero
- from [[content/012/PX262 - quantum mechanics/term 1/A - recap/PX262 - A7 - the uncertainty principle\|the uncertainty principle]]: 
$$\Delta x \Delta p \simeq \hbar$$
- so, as $\Delta p \to 0, \; \Delta x \to \infty$, which is impossible
- hence, there is a minimum $\Delta p$
- this is relevant for neutron stars and white dwarfs

- a gas is *degenerate* when the average thermal energy is less than the *fermi energy*:
$$\frac{3}{2} k_{B}T  < \epsilon_{p} \propto \rho^{{2}/{3}}$$
- this translates to: 
$$T\rho^{\frac{2}{3}} < 1261 \, Km^{2}kg^{- {2}/{3}}$$
- lower $T\rho^\frac{2}{3}$ equates to more degenerate gas
- the degeneracy pressure for non-relativistic electrons: 
$$P \propto n_{e}^{{5}/{3}} $$
- for relativistic electrons, $v_{e} \to c:$ 
$$P \propto n_{e}^{4/3}$$
- for the sun: $T\rho^{2/3}= 5300 >1251$
	$P_{degen\,\odot} = 2.4\times10^{15}\,Nm^{-2}$
	$P_{ideal\,\odot} = nk_{B}T = 1.4\times10^{16}\,Nm^{-2}$
	${} \cfrac{P_{ideal}}{P_{degen}} = 5.8 {}$
	$P_{rad} = 1.5\times10^{13}\,Nm^{-2}$

- for a white dwarf:
	$R\simeq R_{\oplus}$, 
	$M\simeq M_{\odot}$, 
	$T\simeq 10^{7}\,K$, 
	$\rho \simeq 1.8\times10^{9}\,kgm^{-3}$ , 
	$\mu \simeq 2\, \text{mass units}/e^{-}$
	$n_{e} \simeq \cfrac{\rho}{\mu m_{H}} = 5.4\times10^35\,m^{-3}$ 
	$\therefore P_{degen,\,non-rel} \simeq 8.4\times10^{21}\,Nm^{-2}$ and $P_{degen,\,rel} \simeq 1.1\times10^{22}\,Nm^{-2}$
