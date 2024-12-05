# C is constant
If $C$ is constant and we consider the linearized Cahn-Allen equation
$$\partial_{t}u=\partial_{xx}u + Cu$$
Then the dispersion relation is
$$\sigma(q)=i\omega = C-q^2$$
And we can identify a characteristic time-scale of the system as the growth rate of the faster growing mode. The growth rate is $\frac{1}{\sigma(q)}$ and so $q=0$ is the fastest mode. The intrinsic time-scale of the system will be
$$\tau_{linear}=C^{-1}$$
# C(t) is oscillating
In this case is not clear how to identify the time-scale of the system, these are **some options we could consider**:
- The time-scale $\tau_{linear}$ has a time dependance and $$\tau_{linear}=C(t)^{-1}$$
- If 
	- The system is initially a random fluctuation around zero
	- $C(t)$ has a positive average and a sufficiently high amplitude such that, after some oscillations, the non-linear term $-u^3$ will became relevant. 
	If the time it takes for this to happen (duration of the linear approximation) is **much greater** than the time-scale of $C(t)$'s oscillations $\tau_{C}$, then we can approximate $$\int_{0}^tdt' C(t')\simeq \int_{0}^tdt' \bar{C}=\bar{C}t$$$$u_{q}(t)=u_{q}(0)e^{\int_{0}^{t}dt' (C(t')-q^2)}\simeq u_{q}(0)e^{(\bar{C}-q^2)t}$$
		So the time-scale we identify here will be
		$$\tau_{linear}=\bar{C}^{-1}$$

It is 