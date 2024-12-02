#mbc #2D #circular_island #negativeC #timedependingC #ellCC 

Here we explore **numerically** how [[Motion by curvature]] is affected by C(t) oscillations where $C$ **is positive on average BUT it takes negative values**.
For this case, where C becames negative sometimes, we have not yet a theory to describe the dynamics, so we can explore this **only with simulations**.
## What we expect
In the correspondent 1D case, we saw that those oscillations accelerate the annhilation of neighbouring kinks. So we know that those **oscillations enhance the (attractive) interaction** between kinks.
In 2D, the MBC is way faster than the **logaritmic interaction between two kinks at the OPPOSITE SIDES of the circle.** However, maybe the enhancement of this **second order effect** (in 2D is slower than MBC so it is second order) could make this second order effect significatively contributing to the evolution of the circular island.
# Simulations
We simulate the evolution of a circular domain. The radius is measured by measuring the perimeter of the circle as [[ell CC]] as in [[Motion by curvature POSITIVE oscillations]].

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
