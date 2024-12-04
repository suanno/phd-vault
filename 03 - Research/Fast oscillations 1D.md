We say that the oscillations of C(t) are **slow**, if the time scale $\tau_C$ associated with the time variation of $C(t)$ (that, as $C(t)$ is periodic, can be identified as its **period** $T$) is **SMALL compared** to the **intrinsic time-scale** of the system $\tau_{linear}$ (see [[tau_linear|here]]).
So we can define a **small parameter** $\epsilon$ as:
$$\epsilon=\frac{\tau_{C}}{\tau_{linear}}$$
# Idea
Then, assuming that $\tau_{linear}\sim 1$ (that means $\epsilon \sim \tau_{C}$), it is natural to make a [[Multiple scales expansion]] by introducing the new time-variables 
$$t_0 = t, t_{-1} = \epsilon^{-1} t$$
where the dependence of m(x,t) on $t_{0}$ will capture processes occurring at the intrinsic time-scale, and $t_{-1}$ the ones occurring at the time-scale of C(t)'s oscillations.
This means that
$$\partial_t = \partial_{t_0} + \epsilon^{-1}\partial_{t_{-1}}$$
where
$$C(t)=\tilde{C}(t_{-1}) \implies \partial_{t_0}\tilde{C}(t_{-1}) = 0$$
From the relation above and the **ansatz**
$$m(x, t) = m_0(x,t) + \epsilon m_1(x,t) + O(\epsilon^2)$$
==It follows that==
==$$m_0(x,t) = \sqrt{\bar{C}}\tanh(x\sqrt{\frac{\bar{C}}{2}})$$==
==But we could not find an equation for the first order correction $\epsilon m_{1}(x,t)$==
