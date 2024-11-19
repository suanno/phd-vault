## Comparing $\ell$, $\ell_{DW}$ and $\ell_{CC}$
#### Beginning of the linear regime
At short times, the linear analysis without further approximation does not predict a linear growth of $\braket{q^2}$ from the beginning. Instead in [[Linear analysis.pdf]] it is calculated that
$$\braket{q^2}(t) = \frac{1}{4t}\{1-q_{min}\frac{2^{\frac32}}{\pi^{\frac12}}t^{\frac12}\frac{e^{-2tq_{min}^2}}{erf[q_{min}(2t)^{\frac12}]}\}$$
where $q_{min}$ is the cut-off frequency of the lattice and, evaluating the expression at $t=0$ is
$$q_{min}^2 = 3\braket{q^2}(t=0)$$
- CHECK numerically if this is the shape of $\braket{q^2}$ at **very short** times.
- FIT the curve using the above model BUT keeping $q_{min}$ as a free parameter of the fit. Then compare this estimate of $q_{min}$ with $\frac{2\pi}{L}$.
NOTE: You can simulate a 1D system, as the calculations that lead to the above result do not depend on the dimension D of the system.

#### $\ell_{CC}$ seems to scale the same both in linear and non-linear regimes
Notice that $\ell_{CC}$ is the **"area" of the level set** $u(x)=0$.
- CHECK, by zooming at the time of the transition between linear and non-linear regime,  if there is a change of slope or not.
- PLOT $\ell_{CC}$ instead of $\ell_{DW}$ in the comparison in the asymptotic regime.
- SIMULATE **C "constant and negative"**. We expect, in this case, to rest in the linear regime. So we know that $\ell\sim t^{\frac12}$ but how do $\ell_{CC}$ and $\ell_{DW}$ evolve?
## Structure factor
- Plot $S(q)q^2$ v.s. $q$ both for 1D and 2D. So we see how the different modes q weight in computing $\braket{q^2}$.
The shape of the structure factor in 1D and 2D is the same:
- At t=0 it is flat
- At t=1 ($C=\frac12$) it is a gaussian (parabola in semi-logy)
#### Linear tail of $S(q)$
- At large times it shows some **linear tails**, while close to $q=0$ is still a parabola.
- There is a value of q at which the linear tail starts. There $S(q)$ changes shape. And this value moves with time towards $q=0$, never reaching it.
- Olivier believes that this change of shape of $S(q)$ represents the information on the interfaces, while the information around $q=0$ represents the large-scale information.
#### Data collapse
As the wavelenghts of the system evolve, due to coarsening (dimensional analysis finds the exponent) as $\ell \sim t^{\frac12}$, then if I plot $S(q)$ v.s. $q*t^{\frac12}$ for different times t, I should see that all the curves collapse on each other. BUT I expect this **only close to $q=0$**, as the scale invariance is true only at large-scales (so far that the interfaces appear without thickness).
#### Structure factor of some shapes
- 1D: Periodic structure of kinks: prepare it like $\tanh(\cos(x))$, let it evolve a little bit with $C=1$ constant and then compute the structure factor.
- 1D: Single kink
- 2D: Circular island

## Accelerating the 1D coarsening
**CONTROL IDEA**: We can exploit this effect of accelerating the coarsening in 1D to rapidly increase the characteristic wavelenght of the system and then, once we reach the desired one, we keep C constant (and positive) so the coarsening is (almost) stopped.
This is another way of selecting the characteristic lenght of the system, but we work in the non-linear regime instead of the linear one.

- COUNT the number of zeros of $u(x)$ in 1D. Call it $\ell_{CC}$ and check both linear and non linear behaviours.
#### $\tau_C(d_0)$
We see, in 1D simulations, that oscillating $C(t)$ with
- Slow oscillation $T>>\tau_{\bar{C}}$
- Positive average $\bar{C}>0$
- That takes negative values $A>\bar{C}$
$$\tau_c \sim exp(\alpha d_0)$$
where **$\alpha$ is reduced by increasing the amplitude A or the period T of $C(t)$.** As $\tau_C$ has an exponential dependance on $d_0$, then the coarsening is still logarithmic, **but with a different prefactor**.
We can get a $\tau_C$ that is way smaller than the one we have if $C$ is constant or if $C(t)$ oscillates strictly positively or fast.

Olivier says that **also in 2D**, when you have a circular island, while the leading order effect is MBC, there must be a **second order contribution** to the motion that is given **by the interaction of opposite kinks**. Likely, this interaction leads to a logaritmic coarsening (as in 1D is like this) and **so it can be enhanced by using an high period or amplitude.**
This is coherent with what we see in the [[Master Report.pdf]] in Appendix F, where, on average, the MBC is faster if $C(t)$ is oscillating taking negative values.
- SIMULATE the coarsening of an isolated circular island with C oscillating taking negative values and increasing A and T.
If the $\tau_C$ is comparable with the collapse time due to MBC, I expect this second order effect to be clearly visible.

## Onuki phase transition
- SIMULATE oscillating $C(t)$ with very low $\bar{C}$ starting from strongly biased initial conditions (to see droplet-like decomposition).