#twokinks #1D #negativeC #numerical 

We have an analytical formula for the kink's **dynamics** in the limit of strictly **positive** C(t) and **slow** oscillations [[Kinks effective dynamics under slow POSITIVE oscillations]]
$$\dot{d}(t)\simeq-24\sqrt{2} C^{\frac12}(t)e^{-2^{\frac12}C(t)^{\frac12}d}$$
## Comparison with experiments
Here we verify if, in the case where C(t) assumes sometimes negative values (but with a positive average: $0<\bar{C}<A$) the law is still valid, **assuming that the kinks do not move while C<0**:

![[distance_analytical_exp_comparison.png]]
Clearly, the distance changes significatively when C is negative, so our assumption does not hold at all! And so there is no match between the two curves.
## Slightly positive C
Notice that the orange curve changes significatively only when C gets very close to zero. This suggests to plot the function $\dot{d}$ as a function of C
![[dddt.png]]
You can see that there is a **power-law** **divergence of the kinks velocity** if $C \rightarrow 0^+$. This suggests that we could accelerate the kinks annhilation **with strictly positive oscillations**. But notice that, as $\tau_{C} \sim C^{-1}$, it will be necessary to consider a long period T in order to keep the _slow oscillations_ approximation valid.
## Divergence at C=0
Notice that the analytical law plotted above diverges if $C\rightarrow 0$, so when comparing the analytically expected $d(t)$ with the data, you must be aware that if $C(t)$ crosses zero, ==**the numerical error on the plotted analytical curve will explode.**==
