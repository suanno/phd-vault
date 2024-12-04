We say that the oscillations of C(t) are **slow**, if the time scale $\tau_C$ associated with the time variation of $C(t)$ (that, as $C(t)$ is periodic, can be identified as its **period** $T$) is l**arge compared** to the **intrinsic time-scale** of the system $\tau_{linear}$ (see [[tau_linear|here]]).
So we can define a **small parameter** $\epsilon$ as:
$$\epsilon=\frac{\tau_{linear}}{\tau_{C}}$$
# Idea
Then, assuming that $\tau_{linear}\sim 1$ (that means $\epsilon \sim \tau_{C}^{-1}$), it is natural to make a [[Multiple scales expansion]] by introducing the new time-variables 
$$t_0 = t, t_1 = \epsilon t$$
where the dependence of m(x,t) on $t_{0}$ will capture processes occurring at the intrinsic time-scale, and $t_1$ the ones occurring at the time-scale of C(t)'s oscillations.
This means that
$$\partial_t = \partial_{t_0} + \epsilon\partial_{t_{1}}$$
where
$$C(t)=\tilde{C}(t_{1}) \implies \partial_{t_0}\tilde{C}(t_{1}) = 0$$
From the relation above and the **ansatz**
$$m(x, t) = m_0(x,t) + \epsilon m_1(x,t) + O(\epsilon^2)$$
==It follows that==
$$m_0(x,t) = \sqrt{\tilde{C}(t)}\tanh(x\sqrt{\frac{\tilde{C}(t)}{2}})$$
And using the ansatz
$$m_1(x,t) = \beta_1(t)m_{k_1}(\alpha_1(t)x)\quad\text{with: }\alpha_{1}=\alpha_{0}=\sqrt{C(t)}$$
It follows that:
# ==Kink's shape correction==
$$m(x,t) = m_0(x,t) + \epsilon\beta_1(t)\tilde{m}_{k_1}(x,t) + O(\epsilon^2)$$
$$\beta_1(\tau) = \frac12 C'(\tau)C^{-\frac32}$$
$$m_{k_0} + m'_{k_0}\chi = m''_{k_1} + m_{k_1}-3m_{k_0}^2m_{k_1}'$$
Where the **numerical** solution of the last equation, giving the shape of the correction, is the **red curve**, compared with simulations.

| ![[eps10cent.png]] | ![[eps1cent.png]] |
| ------------------ | ----------------- |
