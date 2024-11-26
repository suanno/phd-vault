#twokinks #1D #negativeC

# Evidence from simulations
Simulations show that it is possible to **accelerate the annihilation** of two neighboring kinks (this annhilation is a process that it's described, in the case when C is constant and positive, with an effective law in [[Effective dynamics of kinks]]) by introducing an oscillatory C(t) with
$$C(t) = \bar{C}+A\sin(2\pi t/T)$$
- Positive average ($\bar{C}>0$)
- Such that it takes negative values during the oscillation $A>\bar{C}$
You can see, from the simulations below, that the **annhilation time $\tau_A$ is reduced** if there are oscillations of that kind.

**Remarks**
- In the first plot $C$ is constant and take different values for each curve (starting from left to right: 0.5, 0.6, 0.7, 0.8, 1). If $\bar{C}=0.5$, two kinks at a distance $l_0=10.8$ take a time $\tau_A \simeq 2*10^3$ to annihilate.
- In the second plot C is time dependent. The amplitude of the oscillation $A=1$ is higher than the average value $\bar{C}=0.5$, such that C is sometimes negative. You can see that two kinks at a distance higher than the precedent case $l_0=20>10.8$ take a time $\tau_A\simeq 800$ to annihilate, that is lower than the times in the first plot.
Additionally, you can see that the experimental curve, for times close to $t_c$ (at the left of the plot) lies **below** the dashed black line, that represents a linear fit of the tail of the experimental data's distribution. This is a clear evidence that the process is accelerated by the oscillations. 
![[decay.png]]|![[T=50.png]]

Now we show some simulations that enhance how the parameters $T$ and $A$ affect the decay of the distance.
# Influence of the period T
Here we fix:
- The initial distance $d_0 = 25$;
- The Amplitude A of $C(t)$: $A=1$.
We plot the annihilation time $t_c$ as a function of the average value of the oscillation $\bar{C}$ in a log-log scale. Remember from [[Effective dynamics of kinks]] that, if $C$ is constant and positive, then
$$t_c = \frac{1}{48C}\exp{(\sqrt{2C}d_0)}$$
So, 
$$\log (t_c C)\sim \sqrt2d_0\sqrt C$$
![[varyT.png]]
(the slope of the orange (T=30) is about 10 in the semilogy scale: about variation of factor x10 in y-axis each variation of 0.1 on x-axis).

#### Comments
- In the limit of small period (fast oscillations) the data seems to move towards the curve expected for constant $C=C0$. This is coherent with what we expect in the fast oscillations limit, where the shape of the kinks does not change significatively during a period and so the calculations in [[Effective dynamics of kinks]], where the kink is assumed to propagate without changing shape, can be applied.
- The annihilation time scales too quickly with the decrease of the period, so data for short periods T or large average values $C0$ cannot be collected.
- Data seems to lay on a line, but it could be just the beginning of a square root or other functions.

# Influence of the amplitude $A$
Here we fixed $d_0=25$ and the period of the oscillation $T=30$.

![[varyA.png]]