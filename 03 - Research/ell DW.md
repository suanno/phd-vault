This, togheter with [[ell]] and [[ell CC]] is a wave-lenght of the system that we can measure in simulations as a function of time.
It is defined in such a way that it represents the average lenght of the domains:
$$\ell_{DW} = \frac{L^2}{\int |\nabla u|^2 dxdy}*W$$
Where $W$ is the **thickness** (or **width**) of the interface, **defined as** the integral of the derivative of the field $u(x,y)$ along a direction perpendicular to the interface.
To understand why it represents the average domain size, you should notice that the ratio 
$$\frac{\int |\nabla u|^2 dxdy}{W}$$
is an estimate of the **total interface lenght**, as the gradient is peaked only in the regions close to the interfaces and almost zero everywhere else.
To understand why $\ell_{DW}$ represents the average domain size, think that in 1D the total interface lenght is naturally the number of kinks, and so if you divide the size of the system (that in 1D is $L$) by the number of kinks, you will get the average kink's lenght.
### Estimating the thickness (width) of the interface
It  is **NOT EASY to estimate the thickness** of the interface, but in the fast oscillations limit, a good **estimate** can be obtained by considering the stationary state with $C=\bar{C}$:
$$u_k(\xi) = \sqrt{C}\tanh(\sqrt{\frac{C}{2}}\xi)$$
$$W=\int_{-\infty}^{\infty}(\partial_{\xi}u_k(\xi))^2 d\xi = \frac23 \sqrt2 C^{\frac32}$$
(the last integral is calculated in Appendix G of the [[Master Report.pdf]]).
As the gradient is peaked in the regions close to the interfaces, $\ell_{DW}$ should estimate the ratio between the size of the system $L^2$ and the (total) length of the interfaces $\mathcal{L}$.

**NOTICE**: In the limit of slow oscillations, due to the lack of an efficient method to estimate the interface thickness, we cannot measure this wavelenght as a function of time. Although, as we expect the thickness to be almost a periodic function with the same period of $T$, we could still see look at the time dependance of $\ell_{DW}$ over a large timescale, by sampling the integral of the gradient squared once per period. 

Due to this difficulty, we considered another way of estimating the average domain lenght: [[ell CC]].