---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-relativity/special-relativity/px-155-h-the-lorentz-transformations/px-155-h5-the-twin-paradox/","created":"2024-10-01T18:27:09.778+01:00","updated":"2024-11-26T19:58:39.214+00:00"}
---

## not a paradox: proof
- alice and bobs are twins. alice travels to a distant star and returns to find bob many years older then her
- ***but*** isn't time dilation reciprocal? shouldn't they both observe time running slowly for the other
- use *[[content/011/PX155 - classical mechanics and special relativity/special relativity/PX155 - H - the lorentz transformations/PX155 - H1 - lorentz transformation\|LTs]]* to rectify:
	- assume alice uses a spaceship that accelerates instantly to cruising speed
	- frames :
		- $S =$ bob's rest frame
		- $S'=$ alice's outbound rest frame, $+u$ relative to bob
		- $S''=$ alice's inbound rest frame, $-u$ relative to bob
	- events::
		- **$I$** : alice leaves earth, $x=x'=x''=0$ , $t'=t''=0$
		- **$II$** : alice reaches the star, $x=L$, where, $L$ is the position of the star; $t=\frac{L}{u}$
		- **$III$** : alice returns to earth, $x=0$ , $t=2 \frac{L}{u}$
	- need $t' = \gamma (t- \frac{ux}{c^{2}})$ ,  $t'' = \gamma (t+ \frac{yx}{c^{2}})$

| time  | event 1, $x=0$ | event 2 $x=L$                              | event 3 $x=0$          |
| ----- | -------------- | ------------------------------------------ | ---------------------- |
| $t$   | $0$            | $\frac{L}{u}$                              | $2 \frac{L}{u}$                |
| $t'$  | $0$            | $\gamma (\frac{L}{u} - u \frac{L}{c^{2}})$ | $2\gamma\frac{L}{u}$ |
| $t''$ | $0$            | $\gamma (\frac{L}{u} + u \frac{L}{c^{2}})$ | $2\gamma\frac{L}{u}$ |

- time elapsed for:
	- bob:
$$\Delta t_{B} = (t_{2}-t_{1}) +(t_{3}-t_{2}) = 2 \frac{L}{u}$$
	- alice:
$$\Delta t_{A} = (t_{2}'-t_{1}') +(t_{3}''-t_{2}'') = \frac{2L\gamma}{u} \left( 1- \frac{u^{2}}{c^{2}} \right) = \frac{2L}{\gamma u} =  \frac{\Delta t_{B}}{\gamma}$$
	- $\gamma>1 \implies$ less times experienced by alice than by bob
	- ***note***: in frames $S'$ and $S''$, $\Delta t' = \gamma \Delta t_{B}$ ; $\Delta t'' = \gamma \Delta t_{B}$
## twin paradox by doppler shift
- alice and bob have identical clocks that they carry with them. each has a telescope with which they count ticks on each other's clock
- bob's view of bob's clock:
	- clock ticks with proper frequency $f_{0}$
	- $N_{B}(B) = \frac{2L_{B}}{u} f_{0}$
- bob's view of alice's clock:
	- subsequent ticks occur farther away for outbound journey
	- for outbound frequency:
$$f_{1} = \frac{f_{0}}{\gamma(1+ \frac{u}{c})}$$
	- for inbound frequency:
$$f_{2} = \frac{f_{0}}{\gamma(1- \frac{u}{c})}$$
	- in frame $S$, bob receives last tick at $f_{1}$ at time, $\frac{L}{c}$ *after* it is emitted
	- total ticks:
$$N_{B}(A) = (\frac{L}{u} + \frac{L}{c})f_{1}+ \left( \frac{L}{u} - \frac{L}{c}\right)f_{2}$$
	$$N_{B}(A) = \frac{f_{0}}{\gamma} \left[ \frac{\frac{L}{u}+\frac{L}{c}}{1+ \frac{u}{c}} + \frac{\frac{L}{u}-\frac{L}{c}}{1-\frac{u}{c}} \right]$$
	$$N_{B}(A) = \frac{f_{0}}{\gamma(1- \frac{u^{2}}{c^{2}})} \left[ (\frac{L}{u}+ \frac{L}{c})(1- \frac{u}{c}) + (\frac{L}{u}- \frac{L}{c})(1+ \frac{u}{c})\right]$$
	$$N_{B}(A) = \frac{f_{0}}{\gamma(1- \frac{u^{2}}{c^{2}})} \left[ 2\frac{L}{u} - 2 \frac{Lu}{c^{2}} \right]$$
	$$N_{B}(A) = \frac{2L}{u\gamma}$$
- alice's view of alice's clock:
	- for alice, length of he journey contracts to $\frac{L}{\gamma}$
	- time taken $\Delta t_{A}' = 2\frac{L}{\gamma u}$
	- so ticks on her own clock:
$$N_{A}(A)= \frac{2L}{\gamma u}f_{0}$$
