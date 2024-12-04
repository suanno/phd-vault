#2D #structurefactor #coarsening #Onuki #Cahn-Hilliard

## Information from articles (about conservative dynamics (Cahn-Hilliard))
In the article of [[Onuki.pdf]] working on Model **B** (**conservative** system, **Cahn-Hilliard**) a phase transition occurs if the temperature oscillates as a function of time $T(t)$ and the **AVERAGE temperature** $\bar{T}$ crosses a critical value $T^*<T_C$
- If $\bar{T} > T^*$ there is no coarsening, as the evolution of the state **is periodic**.
- If $\bar{T} < T*$ there is **coarsening**. And this is consistent with the limit $A\rightarrow 0$, where the oscillation of T is completely below $T_C$.

This phase transition is also observed by [[Tanaka - Periodic Spinodal Decomposition in a Binary Polymeric Fluid Mixture.pdf|H. Tanaka]] experimentally, on a system where mass is conserved (so a conservative dynamics).

## Check the phenomena in my code (NON conservative dynamics)
Even if we are working on a non conservative dynamics, we would like to check if this phase transition takes place.

In TDGL,
$$C = (T_C-T)$$
so we verify if there is a critical value $C^*>0$ such that
$$C(t) = \bar{C}+A\sin(2\pi t/\tau)$$
- If $0 < \bar{C} < C^*$ the state is periodic.
- If $\bar{C} > C^*$ there is coarsening. This is consistent with the limit $A\rightarrow 0$, where the oscillation of C is strictly positive.
==Where, in principle, $C^*$ depends on $C^*(A,\tau)$.==
### How we measure this?
We can check wheter there is coarsening or the state returns periodically to the same "image" by measuring $\ell = 2\pi/\sqrt{<q^2>}$ as a function of time. If it continues to grow, it means that coarsening is happening, if it stops then it is not.

**What is simulated**: 
- The **initial state** is prepared by keeping $C=0.5$ constant for a time sufficiently long to see domains. A lower value $dt=0.01$ is adopted to correctly integrate the initial dynamics such that we can see the linear growth $\ell^2 \sim t$.
- Then $C(t)$ starts to oscillate. If $\bar{C}\neq 0.5$ there will be a discontinuity in $C(t)$. So We expect a transient, but then the asymptotic dynamics I expect will not be affected by this.

With an $L=256$ simulation box, coarsening seems to stop, but increasing the size of the simulation box, we still see coarsening.

- L = 256; dx = 0.1
![[L=256l.png]]
- L = 512; dx = 0.1

| ![[L=512l.png]] | ![[L=512lDW.png]] |
| --------------- | ----------------- |
So we see that **coarsening does NOT stop** in our simulations. And if we run an even longer simulation, we see a saturation of the wavelenghts, but that is due to reaching a **stripe-like state**.

| ![[saturationN=4096.png]] | ![[saturationN=4096Stripe.png]] |
| ------------------------- | ------------------------------- |

## Conclusion
==We do not see any phase transition.== 
Additionally, we cannot consider values of $\bar{C}$ that are too small, as the duration of the linear dynamics $\tau_{linear}\sim\bar{C}^{-1}$ will be longer in that case and so a longer simulation will be needed to study the non linear dynamics.

### Possible solutions
- **Fixing $\tau_{linear}$**: Instead of fixing A,T and changing $\bar{C}$ among the simulation, we could fix the averge value and change the amplitude $A$.
In this way, $\bar{C}$ is fixed but the critical value $C^*$ changes.
- **Speed up the code**: (1D) We could measure in time the minimum distance between kinks and the maximum kink width. Comparing them we can find out if two kinks are close to annhilate (so we should adopt a small dt) or no (so we can adopt an higher dt).
But $dt$ must be lower than 1, and we are already using $dt=0.1$.
- **==Asymmetric==** initial state: in the article of H. Tanaka, we see droplet-like spinodal decomposition. Maybe this phase transition happens only for droplet-like decomposition and not for bicontinuos.