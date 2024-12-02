#early_dynamics #linear_regime

<!-- See more in /Research/ -->
---
### We calculate

$$\braket{q^2}=\frac1D\frac{\int q^2|u_q|^2dq}{\int |u_q|^2dq}$$

---
## In the linear regime
-  $-u^3$ can be neglected
- The **power is uniformly distributed** among the Fourier modes **in the initial state** $$|u_q|(t=0) = \bar{u}\Theta(q<q_{min})$$
where $q_{min}$ is a cutoff frequency $q_{min}=\frac{2\pi}{dx}$.

---
## Analytical result
**Until the non-linearity becames relevant**
$$\braket{q^2}(t) = \frac{1}{4t}\{1-q_{min}\frac{2^{\frac32}}{\pi^{\frac12}}t^{\frac12}\frac{e^{-2tq_{min}^2}}{erf[q_{min}(2t)^{\frac12}]}\}$$
---
### Asymptotically
- Short times: $$\braket{q^2}(t)\simeq \frac{q_{min}^2}{3}(1-\frac{8}{15}q_{min}^2t)$$
- Large times (but not so large): $$\braket{q^2}(t)\simeq\frac{1}{4t}$$
---
## Analytical prediction
![[analytical.png]]


---
## Numerical evidence
The data is fitted with $q_{min}$ a free parameter.
![[very_beginning_1D_datainit.png]]

---
# Selecting $\ell$
The linear dynamics is not affected by C(t), but the duration of this dynamics yes
![[tc.png]]

---
#### Keeping the system in the linear regime
If we keep $C=-0.1$, then the non-linearity will **never** became relevant. 
![[C=-0.1.png|500]]

---
#### Non-linear regime
![[Pasted image 20241126144234.png]]
