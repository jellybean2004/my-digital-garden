---
dg-publish: true
---
![Pasted image 20231212141210.png](/img/user/pics/Pasted%20image%2020231212141210.png)
- two point masses, $m_1$ and $m_2$, separated by distance $r$ 
- $\vec F_{12}=$ force due to body 1 on body 2
- ${} \hat r= {}$ unit vector pointing from $m_1$ to $m_2$
## newton's law of gravity
$$\vec F_{12}= -\frac{Gm_1m_2}{r^2}\hat r$$
- attractive, so, $m_2$ is pulled towards $m_1$ in direction $-\hat r$
- $G=6.674\times 10^{-11}Nm^2kg^{-2}$
## newton's shell theorem
- consider a spherical shell
- *point mass outside the shell*: force of point mass due to the total mass of the shell is the same as if all the mass of the shell were concentrated into a point at its centre
- *point mass inside the shell*: gravitational force due to the shell precisely cancels, hence it is zero
- a solid sphere can be considered a series of concentric shells with a common centre.
- outside of the sphere can be treated as a point mass for gravitational purposes

- eg: three identical iron spheres with radius $(R)=5m$ are placed in contact ![Pasted image 20231010151132.png](/img/user/pics/Pasted%20image%2020231010151132.png)
	- to calculate: force on $A$ due to $B$ and $C$:
$$\vec F_{BA}=\frac{Gm_Am_b}{r^2}$$
	- $r=2R$, $m_A=m_B=\frac{4}{3}\pi r^3\rho$ : $$\vec F_{BA}=\frac{G\frac{16}{9}\pi^2R^6\rho^2}{4R^2}$$
$$\vec F_{BA}=\frac{4}{9}G\pi^2R^4\rho^2$$
	- putting $R=5m$, $\rho=7874 kgm^{-3}$ : $$\vec F_{BA}= \frac{4}{9} 6.674\times 10^{-11}\pi
{ #2}
 \times5^4\times (7.874\times 10^3)^{-3}$$
$$\vec F_{BA}=11.33N$$
	$$\vec F_{tot} = 2 \vec F_{BA} \cos 30\degree = 19.6 N$$
- eg: find the weight a person with mass, $m=70kg$, loses by climbing the Eiffel Tower
	$$W_{G}= \frac{G M_{E} m}{R_{E}^{2}}$$
	$$W_{T}= \frac{G M_{E} m}{(R_{E}+h)^{2}}$$
	-  $h=320m$, $R_{E}=6371km$, $M_E=5.972\times 10^24kg$
	$$W_G-W_{T} = GM_Em[\frac{(R_E+h)^2-R_E^2}{R_E^2(R_E+h)^2)}]$$
$$W_G-W_{T} = GM_{E} m \left[\frac{2R_{E}h + h^{2}}{R_{E}^{2}(R_{E}+h)^{2})}\right]$$
	- since $2R_Eh>>h^2$: $$W_G-W_{T} \approx GM_{E} m \left[\frac{2h}{R_{E}^{3} }\right] 2 \left( \frac{GM_{E}}{R_{E}^{2}} \right) m \left( \frac{h}{R_{E}} \right)$$
$$\therefore W_{G}-W_{T}\approx = 2 \left( \frac{h}{R_{E}} \right) mg = 0.07N$$
