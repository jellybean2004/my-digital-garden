---
dg-publish: true
---

## introduction
- planets that orbits a star other than the sun
- $mass<13mass_{jupiter}$ (nuclear fission begins in core for larger masses)
- difficult to detect due to:
	- *faintness*: weak emission and reflection
	- very small angular separation from the brighter host star
## methods of detection
### radial velocity (RV)
- a star will have a doppler shift if it is orbited by an exoplanet
- eg:
		$r_{jupiter}=5.2\,AU$
		$r_{\odot} = \frac{1}{1000}5.2 \times 150\times10^{6}\,km = 780,000\,km$
		$P_{jupiter}= 11.9\,years$
		$v= \frac{2\pi r_\odot}{11.9} = 13\,ms^{-1}$

- in $1995$, $51\,Peg\,b$ was discovered in a very short period orbit: 'hot jupiter' with $T_{eq}\approx 1000\;to\;2000\,K$ 
	- '$b$' represents an exoplanet, '$B$' represents a binary companion
- the earth will only induce a *RV* signal on the sun at a level oh $\sim 10\,cm\,s^{-1}$
- spectrographs had precision at $\sim 1\,m\,s^{-1}$
- best spectrograph: *ESPRESSO* on *VLT* $\sim 10\,cm\,s^{-1}$
- a problem is that the surface of stars are active and dynamic, causing variations in *RV* measurements
- currently, $>1000$ exoplanets have ben discovered via the *RV* method, all have mass ($m\sin i$, minimum mass) 
## transit method
![Pasted image 20240219114807.png](/img/user/pics/Pasted%20image%2020240219114807.png)
- depth of the transit: 
$$\delta = \left(\frac{R_{p}}{R_{s}}\right)^{2}$$
- for jupiter: $\delta_{jupiter} \approx 0.01 \approx 1\%$
- *WASP* project found $100+$ 'hot jupiters' using transit method
- planets must be close to $i=90\degree$
- the radius is learned, and if *RV* is obtained, the mass is learned, which can be used to learn the *bulk density*
- currently, $>5000$ exoplanets have been discovered by the transit method. some do not have *RV* measurement

- assuming a circular orbit, $D$ is the duration of transit, $\alpha$ is the angle subtended at the centre: 
$$\begin{gather*}
		D = \frac{\alpha}{2\pi}P \\
		l = R_{s}+ R_{p} \\
		\sin\left(\frac{\alpha}{2}\right) = \frac{l}{a} = \frac{R_{p}+R_{s}}{a} \\
		\alpha = 2 \arcsin\left(\frac{R_{p}+R_{s}}{a}\right)\\
		D = \frac{P}{\pi} \arcsin \left(\frac{R_{p}+R_{s}}{a}\right)
	\end{gather*}$$
- $D_{hot\,jupiter} \simeq 4\,hrs,\; P<10\,days$
- $D_{earth-sun} \simeq 10\,hrs$
## micro-lensing
![Pasted image 20240221121218.png](/img/user/pics/Pasted%20image%2020240221121218.png)
- [[content/011/PX158 - astronomy/PX158 - G - astronomical masses/PX158 - G3 - gravitational lensing\|gravitational lensing]]: 
$$\theta_{E} = \sqrt{\frac{4GM}{Dc^{2}}}$$
	where, $\theta_{E}=$ einstein radius, $D=$ source-lens, lens-earth distance
- $D\sim 1000\,pc$, $M=0.5\,M_\odot$, $\theta_{E}\sim 1-2\,AU$
- extra lensing due to exoplanet causes a spike in flux-time plot ($\sim 1\,day$)
- the amplitude of the spike give information on the mass of the exoplanet
![Pasted image 20240221122511.png](/img/user/pics/Pasted%20image%2020240221122511.png)
## astrometry
- a star will move in a circular orbit due to an exoplanet - parallax observed: 
$$\alpha\,[''] = \frac{r_{s}\,[AU]}{d\,[pc]}$$
- eg: $\alpha = 0.01\,\frac{AU}{10\,pc} = 0.001^{''}$
- gaia can detect planets this way, but needs to way for ~full period, ie: $\sim12\,yr$ for a jupiter type planet
## direct imaging
- need to observe very nearby and young stars, ie: $d\sim 10\,pc,\; age<\sim100\,Myr$
- adaptive optics, large telescopes, and space telescopes are used

- currently, $5573$ known exoplanets (confirmed)
- radius and period of planets are biased by detection methods
