#twokinks #1D #costantC

When **C>0 is constant**, following the idea presented in [[Kink effective dynamics.pdf]] it is possible to describe the evolution dictated by the TDGL with an **effective law** for the velocity of each kink. If $x_n$ is the position of the n-th kink and $l_n\equiv x_{n+1}-x_n$ is the lenght of the n-th domain:
$$\dot{x_n}\simeq12\sqrt2C^{\frac12}[exp(-\sqrt{2C}l_n)-exp(-\sqrt{2C}l_{n+1})]$$
Which leads, in the case of 2 isolated kinks (that means an isolated domain), to
$$\tau_A=\frac{1}{48C}exp(\sqrt{2C}l_0)$$
$$l(t)=l_0+(2C)^{-\frac12}[\log(\tau_A-t)-\log\tau_A]$$
So the speed of the decay, meaning the prefactor of the logarithm, is $(2C)^{-\frac12}$.
This can be verified experimentally:
![[decay.png]] ![[prefactor_slope.png]]
