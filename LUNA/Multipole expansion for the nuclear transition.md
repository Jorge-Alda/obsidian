# Effective Lagrangians
$$\mathcal{L}_\gamma = A_\mu(x) \mathcal{J}_\gamma^\mu (x) = A_\mu \sum_{N=p,n}\left[e Q_N \bar{N}\gamma^\mu N +  \frac{e \kappa_N}{2m_N} \partial_\nu (\bar{N}\sigma^{\mu\nu}N) \right]$$
$$\mathcal{L}_a = a(x) \mathcal{S}(x) = i a \bar{\psi}_N \gamma_5 (g_{NNa}^0 g_{NNa}^1 \tau_3)\psi_N $$

with $\kappa_N =\mu_N - Q_N$

# Spherical operators
$$\mathcal{G}_{JM} = \int d^3 \vec{r}\, j_J(kr) Y_{JM}(\theta, \varphi) \mathcal{S}(\vec{r})$$
$$\mathcal{T}^\mathrm{el}_{JM} = \frac{1}{k}\int d^3 \vec{r}\, \vec{\nabla}\times [j_J(kr) \vec{Y}_{JJM}(\theta, \varphi)] \cdot \vec{\mathcal{J}}(\vec{r})$$
$$\mathcal{T}^\mathrm{mag}_{JM} = \int d^3 \vec{r}\, j_J(kr) \vec{Y}_{JJM}(\theta, \varphi) \cdot \vec{\mathcal{J}}(\vec{r})$$

where
- $j_J$ is the vector Bessel function
- $Y_{JM}$ is the spherical harmonic
- $\vec{Y}_{JJM}$ is the vector spherical hermonic, $\vec{Y}_{JJM} \vec{r}/r$

## Reduced matrix element
The spherical operators satisfy the Wigner-Eckart theorem
$$\langle J_f M_f | \mathcal{O}_{J,-M} | J_i M_i\rangle = \frac{(-1)^{J_i-M_i}}{\sqrt{2J+1}}\langle J_f M_f; J_i, M_i| J_f J_i; J, -M\rangle \langle J_f || \mathcal{O}_J || J_i\rangle $$
with the reduced matrix element $\langle J_f || \mathcal{O}_J || J_i\rangle$ contains all the physical info of the operator, and the behaviour under rotations is controlled by the Clebsch-Gordans.

# Multipole expansion of the decay width

$$\Gamma(N_i \to N_j a) = \frac{2k}{2J_i +1} \sum_{J\geq0} |\langle J_f || \mathcal{G}_J||J_i\rangle|^2$$
$$\Gamma(N_i \to N_j \gamma) = \frac{2k}{2J_i +1} \left(\sum_{J\geq1}\sum_{t = \mathrm{el},\mathrm{mag}} |\langle J_f || \mathcal{T}^t_J||J_i\rangle|^2 \right)$$

where $k$ is the boson momentum.

# Non-relativistic limit
## $M0$ transition
[$\Delta J = 0$ and $\Delta P = -1$](Selection%20rules.md#^2136af)
$$\Gamma(N_i\to N_f a) = \frac{1}{2J_i+1}\frac{k^5}{54\pi}\left|\langle J_f|| \sum (g_{NNa}^0 + g_{NNa}^1 \tau_3)2\vec{S}_N\cdot \vec{x}_N/m_N||J_i\rangle\right|^2$$

## $M1$ transition
[$\Delta J = 1$ and $\Delta P = 1$](Selection%20rules.md#^11d8c5)

$$\frac{\Gamma(N_i\to N_f a)}{\Gamma(N_i\to N_f \gamma)} = \frac{1}{2\pi\alpha} (k/\omega)^3 \left|\frac{g_{NNa}^0 \beta + g_{NNa}^1}{(\mu_0-1/2)\beta + \mu_1 - \eta}\right|^2$$
where $\mu_{0,1} = \mu_p \pm \mu_n$ and
$$\beta = \frac{\langle J_f || \sum 2 \vec{S}_N|| J_i\rangle}{\langle J_f || \sum 2 \vec{S}_N \tau_3|| J_i\rangle}$$
$$\eta = -\frac{\langle J_f || \sum \vec{\ell}_N \tau_3|| J_i\rangle}{\langle J_f || \sum 2 \vec{S}_N \tau_3|| J_i\rangle}$$