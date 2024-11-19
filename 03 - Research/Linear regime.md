#early_dynamics #linear_regime

In [[Linear analysis.pdf]] we **calculate analytically** how the characteristic wavelenght
$$\braket{q^2}=\frac1D\frac{\int q^2|u_q|^2dq}{\int |u_q|^2dq}$$
evolves in time **if** 
- the non-linearity $-u^3$ can be neglected
- AND the **power is uniformly distributed** among the Fourier modes in the initial state $$|u_q|(t=0) = \bar{u}\Theta(q<q_{min})$$
where $q_{min}$ is a cutoff frequency, that we expect to have since the simulation box is finite.
The calculations, predict that, **until the non-linearity becames relevant** (and eventually it happens because large-wavelenght modes grow in time if $C>0$)
$$\braket{q^2}(t) = \frac{1}{4t}\{1-q_{min}\frac{2^{\frac32}}{\pi^{\frac12}}t^{\frac12}\frac{e^{-2tq_{min}^2}}{erf[q_{min}(2t)^{\frac12}]}\}$$
That gives the asymptotic behaviours:
- Short times: $$\braket{q^2}(t)\simeq \frac{q_{min}^2}{3}(1-\frac{8}{15}q_{min}^2t)$$
- Large times (but not so large such that the non-linearity becomes non-negligible): $$\braket{q^2}(t)\simeq\frac{1}{4t}$$
![[analytical.png]]
## Simulations $\braket{q^2}$
#### 1D
Here I show a simulation of a 1D system. 
The initial state is prepared starting from random initial conditions, without any bias. While $C=1$ is kept constant during the whole simulation. *"1D/.saves/24_11_6_A"*.
The data (in orange) is fitted with the formula presented above (the long one) (green line) where $q_{min}$ is a free parameter.
![[very_beginning_1D_datainit.png]]
There is agreement between the model and the data, but the estimated value of $q_{min}$ is way far from the smallest q-vector due to the discreteness of the lattice $2\pi/L\simeq 0.15$ as $L=N*dx=409.6$.
Notice that we are able to see **correct very early dynamics** only if $dt$ is small enough!

#### 2D
The expected very early behavior of $\braket{q^2}$ is verified also in 2D.
Also in 2D, we see that we need to go to small values of $dt$ to capture the **non-power law initial decay** of $\braket{q^2}$.
We also see that the fitted $q_{min}$ does not depend on the size of the lattice $L$, while the smallest q-vector, due to the finiteness of the lattice depends over $L$: $q_{min}=2\pi/L$.

![[very_beginning_2D_datainit_L=1024.png|300]]![[very_beginning_2D_datainit_L=2048.png|300]]
## Simulations (the state (2D))
Above we showed how the time discretization $dt$ affects the time evolution of $\braket{q^2}$. Now I will show actual pictures of the state (and its structure factor) at time $t=0.2$ , for different values of $dt$. Here L=1024; dx=0.1; C=1 constant, as in the previous plot.

| dt=1e-1![[very_beginning_2D_datainit_dt=0.1.png]]       | dt=1e-2![[very_beginning_2D_datainit_dt=0.01.png]]       |     |
| ------------------------------------------------------- | -------------------------------------------------------- | --- |
| **dt=1e-3**![[very_beginning_2D_datainit_dt=0.001.png]] | **dt=1e-4**![[very_beginning_2D_datainit_dt=0.0001.png]] |     |
# Keeping the system in the linear regime 
If we keep $C=-0.1$, then the non-linearity will never became relevant. We have an analytical formula for the evolution of $\ell$ in this regime, but what happens to the length of the zero level-set $\mathcal{L}=L^2/\ell_{CC}$ in the linear regime?
This question makes sense, because once the domains emerge, there is coarsening and we expect $\ell_{CC}\sim t^{\frac12}$. But what about the linear regime, where the lenght of the interfaces $\mathcal{L}$ seems to make no sense?
![[C=-0.1.png]]