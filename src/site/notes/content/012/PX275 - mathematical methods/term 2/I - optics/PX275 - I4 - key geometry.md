---
{"dg-publish":true,"permalink":"/content/012/px-275-mathematical-methods/term-2/i-optics/px-275-i4-key-geometry/","noteIcon":"1","created":"2025-02-25T12:07:00.164+00:00","updated":"2025-02-25T12:41:53.827+00:00"}
---

#fig
- an aperture and a detector screens are in parallel, separated by a distance, $D$
- calling the direction connecting the screens $z$, so $\hat z = (0,0,1)$
- using $\vec y = (y_{1}, y_{2}, y_{3})$ to describe points on the aperture screen, such that $y_{3}$ is in $\hat z$ direction
- using ${} \vec x = (x_{1}, x_{2}, x_{3})$ to describe points on the detector screen, such that ${} x_{3}$ is in $\hat z$ direction
- $\vec r$ connects $\vec x$ with $\vec y:$ $\vec r = \vec x - \vec y$
- holes in the aperture screen will act as secondary sources
- intensity pattern on the detector, $I(\vec x) = |\vec u(\vec x)|^{2}$ is the superposition of all secondary sources

- considering a simple case of a single pinhole aperture
- so, one secondary point source emanating from aperture screen
- for convenience, setting $y_{3} = 0$, then $\vec y = (y_{1}, y_{2},0)$, where, $(y_{1}, y_{2})$ denotes the position on the screen
- if pinhole is at the centre, $\vec y_{pinhole} = (0,0,0)$, the origin

- then, for the detector screen, $\vec x = (x_{1}, x_{2}, D)$, $x_{3}=D$, as screens are parallel
- the amplitude is just that of a single point source:
$$u(x,t) = \frac{A}{r} \exp(ik(r-ct)) = \frac{A}{|\vec x-\vec y|} \exp(ik(|\vec x- \vec y|-ct))$$
- the amplitude at $\vec x = (0,0,D):$
$$u = \frac{A}{D} \exp(ik(D-ct ))$$

#fig 

- away from the pinhole, the path length is longer, so the intensity falls as $1/r^{2}$

- now, considering two pinholes


$$u(\vec x, t) = \frac{A^{1}}{|\vec x - \vec y^{1}|}\exp(ik(|\vec x - \vec y^{1}| - ct)) + \frac{A^{2}}{|\vec x - \vec y^{2}|}\exp(ik(|\vec x - \vec y^{2}| - ct))$$

- the path length differences lead to phase differences between the two secondary sources, causing interference
- different path lengths are seen in $\hat y_{1}$, but there is no difference in $\hat y_{2}$
#fig #fig 

- for a general case: considering $N$ sources at positions, $\vec y^{j}$
- if not all at the same amplitude, say $A^{j}$
- by superposition:
$$u(\vec x, t) = \sum\limits_{j=1}^{N} \frac{A^{j}}{|\vec x - \vec y^{j}|} \exp(ik(|\vec x-\vec y^{j}| - ct))$$

- this can be used to consider cases like:
	- a thin slit, considering them as a line of $N$ sources
	- a large aperture, considering them as $N$ sources
