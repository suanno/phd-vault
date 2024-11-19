# Focus
Understand how it looks the structure factor $S(q)$ for the **CA** equation.
So we can 
- Compare what we see with the results of Onuki about the CH equation.
- Try to understand how it evolves considering ONLY the linear part of the dynamics.
    $$S(q)\equiv u_qu_{-q}$$
    
    Then, after one period T and neglecting the non linear effects
    $$S(q,T) = S(q,t=0)e^{\bar{C}T}e^{-2q^2 T}$$
    And then, to see what happens after another period, you plug the result as $S(q,t=0)$ again.
### 1D
- Measure $S(q)$ for an **isolated (large) domain**. Do we see two peaks or the spectrum is broad?

    **NOTICE** that now, to calculate $S(q)$, you do not make an average over different initial state, because you have only one initial state.

### 2D
Measure the structure factor for random initial data. Sample it at time where domains appear and at large time.


# To do
## Two kinks (1D)

- Plot $\log d$ vs $\log\log (t_c-t)$
- Plot $\log t_c$ vs $d_0$

We see clearly that oscillations (where $A>\bar{C}>0$) accelerate the annhilation: both
- reduce the annhilation time
- increase the speed (prefacto of the log decay)

But there seems to be a correction to the logarithmic decay, that we do not know.

It will be worth to run simulations of two kinks with a value of $\bar{C}$ very slow, so the slope of the logarithmic decay when $C=\bar{C} cost.$ will be high and so maybe we see a saturation to that value by increasing $d_0$.


## Cauchy-Croft lenghtscale
- Call it $\ell_{CC}$ (without the "$-$")
- Compare with $\ell$ and $\ell_{DW}$ in Figure 3.2 of the Master report.