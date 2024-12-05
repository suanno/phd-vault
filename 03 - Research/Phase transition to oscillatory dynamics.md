#2D #structurefactor #coarsening #Onuki #Cahn-Hilliard

In the article of [[Onuki.pdf]] working on Model **B** (**conservative** system, **Cahn-Hilliard**) a phase transition occurs if the temperature oscillates as a function of time $T(t)$ and the **AVERAGE temperature** $\bar{T}$ crosses a critical value $T^*<T_C$ (the oscillation has an average below the critical temperature but takes **sometimes values above the critical temperature**)
- If $\bar{T} > T^*$ there is no coarsening: the wave-lenghts of the system evolve **periodically in time**.
- If $\bar{T} < T*$ there is **coarsening**: the wave-lenghts of the system grow in time. And this is consistent with the limit $A\rightarrow 0$, where the oscillation of T is completely below $T_C$.
- 
This phase transition is also observed by [[Tanaka - Periodic Spinodal Decomposition in a Binary Polymeric Fluid Mixture.pdf|H. Tanaka]] experimentally, on a system where mass is conserved (so a conservative dynamics).
# A phenomena originating from NOISE
The reason why Onuki predicts (and Tanka sees experimentally) that, when the average value of the oscillation $\bar{T}$ is sufficiently high, there is no coarsening is that Onuki considers a Cahn-Hilliard equation **with added noise** (while, for Tanaka, noise is always present in an experiment).
If $\bar{T}$ is much greater than $T_C$, then the system spends much time above the critical temperature. Here there is only one stable state ($u=0$), so the field $u(x)$ becomes very small everywhere. And if this happens and there is noise, noise's fluctuations dominate and **reset** the state to a random initial state.
So the dynamics occurring during a period is **independent** from the one experienced in the **previous period**. So there is no coarsening.
The structure factor will have a periodic evolution, ==but the real-space picture of the system will be **completely different** at each period.==

# Adapting the statement to the Cahn-Allen equation
If we consider the Cahn-Allen equation, this phase transition **will be stated like this**: 
$$C = (T_C-T)$$
so, having this phase transition would mean that there is a critical value $C^*>0$ such that
$$C(t) = \bar{C}+A\sin(2\pi t/\tau)$$
- If $0 < \bar{C} < C^*$ the state is periodic.
- If $\bar{C} > C^*$ there is coarsening. This is consistent with the limit $A\rightarrow 0$, where the oscillation of C is strictly positive.
Where, in principle, $C^*$ depends on $C^*(A,\tau)$.
==But we should not see this phenomena in simulations, as in our simulations there is no added noise!== In fact we do not see this phenomena.
### Simulations
We can check wheter there is coarsening or not by measuring $\ell = 2\pi/\sqrt{<q^2>}$ as a function of time.
**What is simulated**: 
- The **initial state** is prepared by keeping $C=0.5$ constant for a time sufficiently long to see domains. A lower value $dt=0.01$ is adopted to correctly integrate the initial dynamics such that we can see the linear growth $\ell^2 \sim t$.
- Then $C(t)$ starts to oscillate. If $\bar{C}\neq 0.5$ there will be a discontinuity in $C(t)$. So We expect a transient, but then the asymptotic dynamics I expect will not be affected by this.

With an $L=256$ simulation box, coarsening seems to stop, but increasing the size of the simulation box, we still see coarsening.

| L=256![[L=256l.png]] | L=512![[L=512l.png]] |
| -------------------- | -------------------- |
So we see that **coarsening does NOT stop** in our simulations. And if we run an even longer simulation, we see a saturation of the wavelenghts, but that is due to reaching a **stripe-like state**.

| ![[saturationN=4096.png]] | ![[saturationN=4096Stripe.png]] |
| ------------------------- | ------------------------------- |

# Conclusions
We will never see this phenomena in simulation that do not include noise. 
Anyways the result of Onuki could be interesting as it states that

> [!NOTE] Onuki's result
> Even if there is **noise**, if C(t) oscillates with a positive average but taking negative values
> $$C(t)=\bar{C}+A\sin\left( \frac{2\pi t}{T} \right);\quad 0<\bar{C}<A$$
> domains are not destroyed by noise if $\bar{C}$ is sufficiently small.

So it is **false** the following statement: ''there is no reason in studying how the system behaves under negative oscillations of C(t) with positive average, because in a **real system** noise will destroy the system when $C>0$"
