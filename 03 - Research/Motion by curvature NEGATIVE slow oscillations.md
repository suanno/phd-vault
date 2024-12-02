#mbc #2D #circular_island #negativeC #timedependingC #ellCC 


In this scenario
$$C(t)=\bar{C}+A\sin\left( \frac{2\pi t}{T} \right)$$
with $0<\bar{C}<A$. So the average value of the oscillation is positive, but the oscillations assumes negative values sometimes during the period. In this scenario, **we do not have any analytical theory.**

Here we explore **numerically** how [[Motion by curvature]] is affected by C(t) oscillations where $C$ **is positive on average BUT it takes negative values**.
# What we expect
In the correspondent **1D** case, we saw that those oscillations accelerate the annhilation of neighbouring kinks. So we know that those **oscillations enhance the (attractive) interaction** between kinks.
In 2D, the MBC is way faster than the **logaritmic interaction between two kinks at the OPPOSITE SIDES of the circle.** However, maybe the enhancement of this **second order effect** (in 2D is slower than MBC so it is second order) could make this second order effect significatively contributing to the evolution of the circular island.

# Simulations
We simulate the evolution of a circular domain. The radius is measured by measuring the perimeter of the circle as [[ell CC]] as in [[Motion by curvature POSITIVE slow oscillations]].

We see that 
- there are **no triangular-shaped** variations of $R^2(t)$;
- the oscillations reduce the time $t_c$ it takes for the domain to disappear ($R(t_c)=0$).
#### Effect of a different period T

| ![[big.png]] | ![[small.png]] |
| ------------ | -------------- |
#### Effect of a different amplitude A
If the amplitude is too high, we see a divergence in the measure of the radius.
We **suppose** this happens because, if C is too negative, then the plateau values of the domains are very close to zero and **numerical fluctuations** of $u(x)$ dominate, making not possible to estimate the radius with the Cauchy-Crofton formula [[ell CC]].

| ![[98 - Images/circular domain/varyA/Cbar=0.1T=50/big.png]] | ![[98 - Images/circular domain/varyA/Cbar=0.1T=50/small.png]] |
| ----------------------------------------------------------- | ------------------------------------------------------------- |

# Is it a numerical effect? NO
In the case of [[Motion by curvature POSITIVE slow oscillations]], where the analytical theory tells that, to leading order, the MBC law holds also in the presence of oscillations; we saw that the effect we used to see vanishes if dt is decreased. So that was a numerical effect.

But now, it seems **to not be a numerical** effect. Let's compare the two scenarios:
- Strictly **positive** oscillation
![[98 - Images/circular domain/positive oscillations/Cbar=1/dt.png]]
- **Negative** oscillation
![[numerical_effect.png]]

