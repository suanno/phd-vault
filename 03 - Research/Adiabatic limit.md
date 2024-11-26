
If $C(t)$ oscillates, **strictly positively**, at a timescale $T$ that is **much larger** than the intrinsic timescale of the system $\tau_{C}=C^{-1}$ (as $C(t)$ is time-dependent, this must hold for the smallest value that $C(t)$ takes) then we expect that

> The system has time to adapt/relax to the changes of C(t), so it will **follow adiabatically** the stationary state with $C=C(t)$  

$$u_{adiabatic}(x,t) = \sqrt{C(t)}\tanh{[x\sqrt{\frac{C(t)}{2}}]}$$

  

That is the stationary state you expect for **constant** C, but you evaluate it in $C=C(t)$.

## A zeroth order statement
As the period T is finite, then also the ratio $T/\tau_C$ is finite, so we expect that the dynamics contains **corrections** to the adiabatic behaviour, that decrease as  $T/\tau_C$ increases. So we reasonably expect the adiabatic limit to be a **zeroth** order approximation of the **slow oscillations limit**. What we expect is confirmed in the analytical study of teh slow oscillations limit.
  

## When the adiabatic condition is not valid?
  $$T >> \tau_{C(t)} = C(t)^{-1}$$
is not satisfyied if $C(t)$ is varying close to zero, as when $C$ is constant and close to zero then $\tau$ is big, we expect the system to not evolve adiabatically at times $t$ when $C(t)\simeq 0$. Even if the period $T$ is very big.