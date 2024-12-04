#twokinks #1D #negativeC #numerical

# Evidence from simulations
Simulations show that it is possible to **accelerate the annihilation** of two neighboring kinks by introducing an oscillatory C(t) with
$$C(t) = \bar{C}+A\sin(2\pi t/T)$$
- Positive average ($\bar{C}>0$)
- Such that it takes negative values during the oscillation $A>\bar{C}$
You can see, from the simulations below, that the **annhilation time $\tau_A$ is reduced** if there are oscillations of that kind.
## Simulations
To see that the annhilation time is reduced, remember that the annhilation time when C is constant is
$$t_{c}=\frac{e^{d_{0}/A}}{\alpha}=\frac{{e^{d_{0}(2C)^{0.5}}}}{48C}$$
and from the simulations below, you can see that the time it takes for the annhilation is smaller than the time you would get by putting $\bar{C}$ in the formula above.
![[T=50.png]]

**NOTICE:** Asymptotically, the plot above **does not seem to be a line**. It seems to be a little bit curved, so it is not clear if, at least asymptotically, the decay is logaritmic as in the case when C is constant.

Now we show some simulations that enhance how the parameters $T$ and $A$ affect the decay of the distance.
# Influence of the period T on $t_c$
Here we fix:
- The initial distance $d_0 = 25$;
- The Amplitude A of $C(t)$: $A=1$.
We plot the annihilation time $t_c$ as a function of the average value of the oscillation $\bar{C}$ in a log-log scale. Remember from [[Kinks effective dynamics under slow POSITIVE oscillations]] that, if $C$ is constant and positive, then
$$t_c = \frac{1}{48C}\exp{(\sqrt{2C}d_0)}$$
So, 
$$\log (t_c C)\sim \sqrt2d_0\sqrt C$$
![[varyT.png]]
(the slope of the orange (T=30) is about 10 in the semilogy scale: about variation of factor x10 in y-axis each variation of 0.1 on x-axis).

#### Comments
- In the limit of small period (fast oscillations) the data seems to move towards the curve expected for constant $C=C0$. This is coherent with what we expect in the fast oscillations limit, where the shape of the kinks does not change significatively during a period and so the calculations in [[Kinks effective dynamics under slow POSITIVE oscillations]], where the kink is assumed to propagate without changing shape, can be applied.
- The annihilation time scales too quickly with the decrease of the period, so data for short periods T or large average values $C0$ cannot be collected.
- Data seems to lay on a line, but it could be just the beginning of a square root or other functions.

# Influence of the amplitude $A$
Here we fixed $d_0=25$ and the period of the oscillation $T=30$.

![[varyA.png]]
## This is not a numerical effect
![[98 - Images/twokinks/dt.png]]