---
{"dg-publish":true,"permalink":"/content/011/px-155-classical-mechanics-and-special-relativity/classical-mechanics/px-155-b-systems-of-particles-accelerations/px-155-b4-equations-of-motion/","noteIcon":"1","created":"2024-10-01T18:27:09.498+01:00","updated":"2024-11-26T19:55:16.422+00:00"}
---

## constant acceleration
- constant $a$ in 1D, not a function of $t,x,v$
	$a= \frac{dv'}{dt'}$
	$a\int_0^t dt'=\int_u^v dv'$

	$\implies at=v-u$
$$\implies v=u+at \; ...(1)$$
		$v= \frac{dx'}{dt'}$
		$vdt'=dx'$
		$\implies\int_{0}^{t} (u+at)dt'=\int_{0}^{s} dx'$
		$\implies [ut'+ \frac{1}{2}at'^{2}]_0^t=s$ 
	
$$\implies s=ut+ \frac{1}{2}at^{2}\; ...(2)$$
	- from $(1)$: $t= \frac{v-u}{a}$ in $(2)$:
		$s= u\frac{v-u}{a}+ \frac{1}{2}a \frac{(v+u)^2}{a^2}$
$$2as = v^2-u^2\;...(3)$$
- eg: in the UK driving theory test, the breaking distance at $70mph$ is $75m$. what is the acceleration?
		$1mile = 1600m$
		$u=1600\times 70/3600=31ms^{-1}$
	- $a= \frac{v^2-u^2}{2s}=-6.4ms^{-2}$
## time dependent acceleration
- suppose $a=a(t)= \frac{dv'}{dt'}$ 
$$\int_0^t a(t)dt'=\int_u^v dv'$$
	- $LHS$ *might* be integrable analytically
## position dependent acceleration
- if $a=a(x)=\frac{dv}{dt}$
	$\int_{u}^{v}\,dv=\int_0^s a(x)\,dt$
	$a(x)= \frac{dx}{dt} \frac{dv}{dx} = v \frac{dv}{dx}$
	$\int_0^s a(x)dx = \int_u^v v.dv$
	$$\frac{1}{2}(v^2-u^2)=\int_0^s a(x)dx$$
{ #f972e4}

## velocity dependent acceleration
- if $a=a(v)= \frac{dv}{dt}$
	$\int_u^v\frac{1}{a(v)}dv = \int_0^t dt$
- eg: starting from rest at $t=0$, an object falls through the air subject to air resistance force $F= - \frac{mv}{\tau}$ , $\tau$ is constant. find $v(t)$ and $x(t)$
	- [[content/011/PX155 - classical mechanics and special relativity/classical mechanics/PX155 - A - foundations of classical mechanics/PX155 - A2 - newton's second law\|PX155 - A2 - newton's second law]] : $mg - \frac{mv}{t}=ma$
		$a = g - \frac{v}{\tau}$
		$\int_0^{v} \frac{1}{g-\frac{v}{\tau}}dv=t$
		$t=[-\tau ln|g - \frac{v}{\tau}|]_0^v$
		$t = -\tau (ln|g - \frac{v}{\tau}|-lng)$
		$t =-\tau ln\frac{|g - \frac{v|}{\tau}}{g}$
		- rearranging for v: $e^{\frac{-t}{\tau}}=\frac{g- \frac{v}{\tau}}{g}$
			$v=g\tau(1- {e^{\frac{-t}{r}}})$
		- setting $v= \frac{dx}{dt}$, we can integrate again: $x=\int_0^tg\tau(1- {e^{\frac{-t}{r}}})$
			$=[g\tau(t+\tau e^{-t/\tau})]_0^t$
			$=g\tau [t-\tau(1-e^{-t/\tau})]$
			
		
		
		