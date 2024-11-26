---
dg-publish: true
---

- includes galaxies, comets, planets
- surface brightness $=$ flux per angle$^{2} =$ magnitude / arc-second$^{2}$
- brightness in the telescope: 
$$\frac{\pi r^{2} S_{B} \alpha^{2}}{l^{2}} = \frac{\pi D^{2}S_{B}\alpha^{2}}{4l^{2}} = \frac{\pi D^{2}S_{B}\alpha^{2}}{4\alpha^{2}f^{2}} = \frac{\pi D^{2}S_{B}}{4f^{2}} = \frac{\pi S_{B}}{4} \frac{1}{(\frac{f}{D})^{2}}$$
	where, $\frac{f}{D}=focal\;ratio$ 
- "$f/8$" means $focal\;ratio=8$
- a "slow" focal ratio is a high number, and a "fast" focal ratio is a low number
- fast optics are difficult and quite expensive to make
## angular magnification
- due to the wave nature of light, diffraction occurs in telescopes
- bessel found that the diffraction limit for a *circular* aperture as: 
$$\alpha_{min} = 1.22 \frac{\lambda}{D}$$

- eg: what is the minimum angular resolution of the human eye?
	$$\alpha_{min} = 1.22 \frac{500\,nm}{5\,mm} = 0.000122\,rad \times \frac{180}{\pi\,rad}\times 3600 ^{''} = 25^{''}$$
	- this is the limit, but more typical value $\approx 60^{''}$

- eg: what is the $\alpha_{min}$ for the *VLT*?
		$D=8\,m$
	$$\alpha_{min} = 0.016^{''}$$

- for ground based telescopes, the atmospheric turbulence limits the angular resolution. this effect is called "*seeing*"
- a good site will have "*seeing*"$=1^{''}$
- adaptive optics can help correct this effect using deformable mirrors
## adaptive optics
- measuring the 'blurring' due to earth's atmosphere (by bright stars and/or laser guide stars) and correct it via deformable mirrors (millisecond corrections)
- telescopes are situated on high mountains to reduce these effects of earth's atmosphere 
- space telescopes do not suffer from this effect but they are very expensive to create, launch, and operate
![Pasted image 20240130102513.png](/img/user/pics/Pasted%20image%2020240130102513.png)
$$magnification= \frac{\alpha_{2}}{\alpha_{1}} = \frac{f_{1}}{f_{2}}$$
- eg: what is the angular magnification for celestron, $D=90\,mm$, ${} focal\,length=1250\,mm {}$, $eyepiece=32\,mm$? what is the diffraction limit?
	$$\frac{\alpha_{1}}{\alpha_{2}} = \frac{1250}{32}\approx 39$$
	$$\alpha_{min} = 1.22 \frac{\lambda}{D} = 1.22 \frac{500\,nm}{90\,mm} \approx 14^{''}$$
	