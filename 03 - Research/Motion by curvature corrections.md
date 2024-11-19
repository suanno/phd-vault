#mbc #2D #circular_island 
## A leading (first) order effect
Motion by curvature is a **first (leading) order effect** [[Motion by curvature]], in the limit where the **curvature $\kappa = 1/R$ is small.** So, close to the disappearance of the circular domain, when $R$ gets small, deviations from $R^2(t)=R_0^2-2t$ are expected. And **these deviations may depend on the value of $C$**, even if at leading order (MBC) there is no dependence on $C$. 
So, if we compare experiments with constant C, but with different values, it is not unexpected that the curve differ at long times, like it happens here:
![[98 - Images/circular domain/initial conditions/Cconst.png]]
## Do C(t) oscillations introduce relevant corrections?
We know **analyticaly** that:
- If $\bar{C}>0$ and the oscillations are fast respect to the dynamics
- If $C(t)>0$ and the oscillations are slow
The MBC law $\dot{R}=-R^{-1}$ still holds at leading order (==explicit what is leading order==). So 
> The **"positive" oscillations** introduce only **second order corrections** to MBC.

While **we have no theory** for the case when
- $\bar{C}>0$ but $C(t)<0$ sometimes, with oscillations that are slow
**And**
-  We are not taking care about the *intermediate* between fast and slow
- If $C(t)>0$ but sometimes it gets very close to zero, then the time scale $\tau_C\sim C^{-1}$ changes a lot (respect to the period $T$) during the simulation and so the oscillation is neither fast neither slow. This case is **not investigated** still.

Here we see, numerically, a comparison of "positive", "negative" oscillations and C constant, to answer the question

> Do negative oscillations introduce leading order corrections to the MBC or the correction is of the same order of the one you get with positive oscillations, and so of second order?


![[small_correction_2.png]]
![[small_correction_2_deviation.png]]

[[small correction.pdf]]