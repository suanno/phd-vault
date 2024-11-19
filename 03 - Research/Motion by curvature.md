#2D #circular_island #mbc

In the limits of
- Slow oscillations and $C(t)>0$ strictly
- Fast oscillations and $\bar{C}>0$
We prove that, up to leading order, the dynamics is dictated by motion by curvature (**MBC**), that means the velocity of an interface between domains is proportional to the local curvature $\kappa$
$$v=-\kappa$$
## Circular domain
![[R0=50L=4096.png]]
If the MBC law is applied to the case of an (isolated) circular domain with initial radius $R_0$, then the curvature is $R^{-1}$, while the interface velocity is $\partial_t R$, so
$$R^2(t)-R_0^2=-2t$$
This means that $R^2$ decays linearly with time and the island eventually disappears at a time $t_c = R_0^2/2$. However, in the proof of MBC we assume that the curvature $\kappa$ is small everywhere, but when the island becomes very small, then $R$ is small and so $\kappa=R^{-1}$ is very large. So, close to $t_c$, we do not expect the MBC law to hold, so the actual $t_c$ will be different than the predicted one (in particular, simulations show that $t_c < R_0^2/2$).
### How to measure $R$
It is possible to use the **Cauchy-Crofton (CC) formula** to estimate the lenght of the interface $\mathcal{L}$ (that is the perimeter of the circle) and then estimate 
$$R(t)=\mathcal L/(2\pi)$$
### Effects of $C(t)$ oscillations
Here I consider the case where $C(t)$ oscillates taking also negative values, but on average it is positive ($\bar{C}>0$). And we consider the oscillations to be slow (in the fast oscillations limit we know that MBC is the leading order effect).
In the correspondent 1D case, we saw that those oscillations accelerate the annhilation of neighbouring kinks. So we know that those **oscillations enhance the (attractive) interaction** between kinks.
In 2D, the MBC is way faster than the **logaritmic interaction between two kinks at the OPPOSITE SIDES of the circle.** However, maybe the enhancement of this **second order effect** (in 2D is slower than MBC so it is second order) could make this second order effect significatively contributing to the evolution of the circular island.
#### Simulation
We see that 
- there are **no triangular-shaped** variations of $R^2(t)$;
- the oscillations reduce the time $t_c$ it takes for the domain to disappear ($R(t_c)=0$).
![[MBC correction big.png]]

| ![[MBC correction.png]] | ![[MBC correction medium.png]] |
| ----------------------- | ------------------------------ |


I would like to see if with an oscillation that is strictly positive, but where $C(t)$ gets very close to zero, if the coalescence time $t_c$ of the circular domain is still reduced.
Also I would like to see how this effect depends on the period and on the amplitude of the oscillation.

### Varying the period T
Also in the simulations below, the state was prepared with $u_0=\sqrt{\bar{C}}$.
Here we show the evolution of $R^2(t)$ under an oscillating $C(t)$ :
$$C(t)=\bar{C}+A\sin(2\pi t/T)$$
where, in all the simulations, we keep fixed
- $\bar{C}=0.1$
- $A=1$
While $T$ is different in each simulation:

| ![[big.png]] | ![[small.png]] |
| ------------ | -------------- |
### Varying the amplitude A

we keep fixed
- $\bar{C}=0.1$
- $T=50$
While $A$ is different in each simulation:

| ![[98 - Images/circular domain/varyA/Cbar=0.1T=50/big.png]] | ![[98 - Images/circular domain/varyA/Cbar=0.1T=50/small.png]] |
| ----------------------------------------------------------- | ------------------------------------------------------------- |
### Strictly positive oscillation of $C(t)$
Maybe this result depends on how the initial state is prepared.
In this case, it was prepared such that the initial thickness of the interface is the one associated to $C=0.1$, while the average value of the oscillation here is $\bar{C}=1$.
Explicitly, if you evaluate $u(x,y,t=0)$ along a line that passes through the origin, such that $y=0$:
$$u(x,t=0)\sim \sqrt{0.1}\tanh(\sqrt{\frac{0.1}{2}}(x-R_0))$$
close to the interface.

| ![[u0=0.001_big.png]] | ![[u0=0.001_small.png]] |
| ----------------------------- | ----------------------------------- |
|                               |                                     |
But if, instead, we prepare the initial state such that the thickness of the kink is the one associated to $C=1$, then we do not see any deviation from the MBC law:
![[positive_oscillation_u0=1.png]]