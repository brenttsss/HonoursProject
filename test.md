Absolutely—here’s your full sheet, **keeping every item** but converted consistently to the **mostly minus convention**

$$
g_{\mu\nu}=\mathrm{diag}(+1,-1,-1,-1),\qquad
\Box\equiv \partial_\mu\partial^\mu=\partial_t^2-\nabla^2,\qquad
k^2\equiv k_\mu k^\mu=(k^0)^2-\mathbf{k}^2 .
$$

I’ve also adjusted the Klein–Gordon operator, LSZ amputators, propagators, exact 2-point function, on-shell conditions, and the canonical energy–momentum tensor to match this convention.

---

# **Formula Sheet (Mostly Minus Convention)**

### **Chapter 1: Foundations and Quantum Fields**

* **Schrödinger Equation**

  * Time evolution: $\;i\hbar\,\frac{d}{dt}\,|\psi,t\rangle=H\,|\psi,t\rangle.$
  * Free NR particle: $\;i\hbar\,\partial_t\psi(x,t)=-\frac{\hbar^2}{2m}\nabla^2\psi(x,t).$

* **Relativistic Wave Equations**

  * **Klein–Gordon** (with $\hbar=c=1$):

    $$
    (\Box+m^2)\,\phi(x)=0,\qquad \Box=\partial_\mu\partial^\mu=\partial_t^2-\nabla^2 .
    $$
  * **Dirac (first order)**:

    $$
    i\hbar\,\partial_t \psi_a(x)=\big[-i\hbar c\,(\alpha^j)_{ab}\partial_j
    +mc^2\,(\beta)_{ab}\big]\psi_b(x),
    $$

    with $\{\alpha^j,\alpha^k\}=2\delta^{jk}I$, $\{\alpha^j,\beta\}=0$, $\beta^2=I$.

* **QFT Formalism**

  * **Heisenberg picture**: $\;\phi(x,t)=e^{iHt/\hbar}\,\phi(x,0)\,e^{-iHt/\hbar}.$
  * **Creation/annihilation at position**: $a^\dagger(x),a(x)$.

    * Bosons: $[a(x),a^\dagger(x')]=\delta^3(x-x').$
    * Fermions: $\{a(x),a^\dagger(x')\}=\delta^3(x-x').$
  * **Many-body NR Hamiltonian**:

    $$
    H=\int d^3x\,a^\dagger(x)\!\left[-\frac{\hbar^2}{2m}\nabla^2+U(x)\right]\!a(x)
      +\frac12\!\int d^3x\,d^3y\,V(x-y)\,a^\dagger(x)a^\dagger(y)a(y)a(x).
    $$
  * **Number operator**: $N=\int d^3x\,a^\dagger(x)a(x)$ (conserved if $[N,H]=0$).

---

### **Chapter 2: Lorentz and Poincaré Groups**

* **Metric**: $g_{\mu\nu}=\mathrm{diag}(+1,-1,-1,-1)$.
* **Lorentz transformation**: $x'^{\mu}=\Lambda^{\mu}{}_{\nu}x^\nu$,
  condition $g_{\mu\nu}\Lambda^{\mu}{}_{\rho}\Lambda^{\nu}{}_{\sigma}=g_{\rho\sigma}$.
* **Unitary representation**: $U(1+\delta\omega)=I+\frac{i}{2\hbar}\delta\omega_{\mu\nu}M^{\mu\nu}$.
* **Poincaré algebra** (with mostly minus):

  * Rotations/boosts:

    $$
    [J_i,J_j]=i\hbar\,\epsilon_{ijk}J_k,\quad
    [J_i,K_j]=i\hbar\,\epsilon_{ijk}K_k,\quad
    [K_i,K_j]=-i\hbar\,\epsilon_{ijk}J_k.
    $$
  * Translations with Lorentz:

    $$
    [P_\mu,M_{\rho\sigma}]
    =i\hbar\,(g_{\mu\sigma}P_\rho-g_{\mu\rho}P_\sigma).
    $$
  * Translations commute: $[P_i,P_j]=0,\;[P_i,H]=0$.
* **Field transformations**

  * Scalar: $U(\Lambda)^{-1}\phi(x)U(\Lambda)=\phi(\Lambda^{-1}x)$.
  * Translation: $T(a)^{-1}\phi(x)T(a)=\phi(x-a)$, $T(a)=e^{-iP_\mu a^\mu/\hbar}$.

---

### **Chapter 3: Canonical Quantization of Scalar Fields**

* **Free relativistic Hamiltonian**: $H=\int d^3p\,\omega(p)\,\tilde a^\dagger(p)\tilde a(p)$, $\omega(p)=\sqrt{\mathbf{p}^2+m^2}$.
* **Lagrangian (real scalar, mostly minus)**:

  $$
  \mathcal{L}=\tfrac12\,\partial_\mu\phi\,\partial^\mu\phi-\tfrac12 m^2\phi^2.
  $$
* **Mode expansion** (solution of KG):

  $$
  \phi(x)=\int \tilde{d}k\;\big[a(k)e^{-ik\cdot x}+a^\dagger(k)e^{+ik\cdot x}\big],\qquad
  \tilde{d}k\equiv \frac{d^3k}{(2\pi)^3\,2\omega_k}.
  $$
* **Canonical momentum & ETCR**:

  $$
  \Pi(x)=\frac{\partial \mathcal{L}}{\partial\dot\phi}=\dot\phi(x),\qquad
  [\phi(\mathbf{x},t),\Pi(\mathbf{y},t)]=i\,\delta^3(\mathbf{x}-\mathbf{y}).
  $$
* **Operator algebra**:
  $[a(k),a^\dagger(k')]=(2\pi)^3 2\omega_k\,\delta^3(\mathbf{k}-\mathbf{k}').$
* **Hamiltonian (normal ordered)**:

  $$
  H=\int \tilde{d}k\;\omega_k\,a^\dagger(k)a(k).
  $$
* **Complex scalar**:

  $$
  \mathcal{L}=(\partial_\mu\phi^\dagger)(\partial^\mu\phi)-m^2\phi^\dagger\phi,
  \quad
  \phi(x)=\int \tilde{d}k\,[a(k)e^{-ikx}+b^\dagger(k)e^{+ikx}].
  $$

---

### **Chapters 4–5: Interactions and Scattering**

* **Microcausality**: $[H_I(x),H_I(y)]=0$ for $(x-y)^2<0$ (spacelike).
* **LSZ reduction**:

  $$
  \langle f|i\rangle = i^{n+n'}\!\int\!\cdots e^{ikx}\cdots
  (\Box_x+m^2)\,\langle 0|T\phi(x_1)\cdots|0\rangle,
  $$

  i.e. amputators are $(\Box+m^2)$ in mostly minus.
* **Field normalization (for LSZ)**:
  $\langle 0|\phi(x)|0\rangle=0,\quad \langle k|\phi(0)|0\rangle=1.$
* **Renormalized Lagrangian (example $\phi^3$)**:

  $$
  \mathcal{L}
  =\tfrac12 Z_\phi\,\partial_\mu\phi\,\partial^\mu\phi
   -\tfrac12 Z_m m^2\phi^2
   +\tfrac{1}{6} Z_g g\,\phi^3+Y\,\phi.
  $$

---

### **Chapters 6–9: Path Integrals and Perturbation Theory**

* **Transition amplitudes**

  * Phase space: $\;\langle q'',t''|q',t'\rangle=\int\mathcal{D}q\,\mathcal{D}p\;e^{i\int (p\dot q-H)dt}.$
  * Configuration space: $\;\langle q'',t''|q',t'\rangle=\int\mathcal{D}q\;e^{i\int L\,dt}.$
* **Generating functional**

  $$
  Z(J)=\int\mathcal{D}\phi\;e^{i\int d^4x\,(\mathcal{L}+J\phi)},\qquad
  \langle 0|T\phi(x_1)\cdots|0\rangle
  =\left.\prod_r \frac{1}{i}\frac{\delta}{\delta J(x_r)}\,Z(J)\right|_{J=0}.
  $$
* **Free theory**

  $$
  Z_0(J)=\exp\!\left(\frac{i}{2}\!\int d^4x\,d^4x' J(x)\,\Delta_F(x-x')\,J(x')\right),
  $$

  with **Feynman propagator (mostly minus)**:

  $$
  i\Delta_F(x-y)=\int\frac{d^4k}{(2\pi)^4}\;
  \frac{e^{-ik\cdot(x-y)}}{k^2-m^2+i\epsilon}.
  $$

  Green’s function equation: $(\Box_x+m^2)\Delta_F(x-x')=\delta^{(4)}(x-x').$
* **Wick’s theorem**:
  $\langle 0|T\,\phi(x_1)\cdots\phi(x_{2n})|0\rangle  =(1/i)^n\sum_{\text{pairings}}\Delta_F(\cdot)\cdots.$
* **Interacting theory master formula**:

  $$
  Z(J)\propto
  \exp\!\left[i\!\int d^4x\,\mathcal{L}_I\!\left(\frac{1}{i}\frac{\delta}{\delta J(x)}\right)\right] Z_0(J).
  $$
* **Connected generator**: $Z(J)=e^{iW(J)}$; $iW$ sums connected diagrams.
* **Tadpole cancellation**: choose $Y$ so that $\langle 0|\phi(x)|0\rangle=0$.

---

### **Chapters 10, 12–15, 18: Scattering, Loops, and Renormalization**

* **S-matrix element**:
  $\langle f|i\rangle=(2\pi)^4\delta^{(4)}(k_{\rm in}-k_{\rm out})\,i\,T.$
* **Momentum-space Feynman rules ($\phi^3$)**

  1. Vertex: $ig$.
  2. Internal propagator: $\displaystyle \frac{i}{k^2-m^2+i\epsilon}$.
  3. External leg: $1$.
  4. Each loop: $\displaystyle \int\!\frac{d^4\ell}{(2\pi)^4}$.
* **Mass dimensions** (in $d$ with $\hbar=c=1$):
  $[S]=0,\quad [\mathcal{L}]=d,\quad [\phi]=\tfrac{d-2}{2},\quad  [g_n]=d-\tfrac{n(d-2)}{2}.$
* **Exact propagator & self-energy $\Pi(k^2)$**

  $$
  \tilde\Delta(k^2)=\frac{1}{\,k^2-m^2+i\epsilon-\Pi(k^2)\,}.
  $$
* **On-shell renormalization (mostly minus)**:

  $$
  \Pi(m^2)=0,\qquad \Pi'(m^2)=0.
  $$
* **Lehmann–Källén representation**:

  $$
  \tilde\Delta(k^2)=\frac{1}{k^2-m^2+i\epsilon}
  +\int_{4m^2}^{\infty}\!ds\,\frac{\rho(s)}{k^2-s+i\epsilon},\quad \rho(s)\ge 0.
  $$
* **Renormalizability**: non-negative mass dimension couplings.
  **Superficial degree of divergence**: $D=dL-2I$.

---

### **Chapters 22, 30, 32: Symmetries**

* **Noether’s theorem** (global continuous symmetry):

  $$
  j^\mu=\frac{\partial\mathcal{L}}{\partial(\partial_\mu \phi_a)}\,\delta\phi_a,
  \qquad \partial_\mu j^\mu=0 \text{ (on EOM)}.
  $$
* **Energy–momentum tensor (canonical, mostly minus)**:

  $$
  T^{\mu\nu}=\frac{\partial\mathcal{L}}{\partial(\partial_\mu\phi_a)}\,\partial^{\nu}\phi_a
             - g^{\mu\nu}\mathcal{L}.
  $$
* **Ward–Takahashi identity**: quantum current conservation linking $(n+1)$-point with current insertion to $n$-point.
* **Spontaneous symmetry breaking (SSB)**:
  For $V(\phi)=\tfrac12 m^2\phi^2+\tfrac{\lambda}{24}\phi^4$ with $m^2<0$:

  $$
  v=\sqrt{\frac{6|m^2|}{\lambda}},\qquad m_\rho^2=2|m^2|.
  $$
* **Goldstone’s theorem**: one massless boson per broken generator (global symmetry).

---

### **Chapters 61, 69, 84: Gauge Theories**

* **Covariant derivative**:

  $$
  D_\mu=\partial_\mu - i e A_\mu \quad (\text{U(1)}),\qquad
  D_\mu=\partial_\mu - i g A_\mu^a T^a\quad (\text{non-Abelian}).
  $$
* **Field strength**:

  $$
  F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu \quad (\text{U(1)}),\qquad
  F_{\mu\nu}^a=\partial_\mu A_\nu^a-\partial_\nu A_\mu^a+g f^{abc}A_\mu^bA_\nu^c.
  $$

  Also $F_{\mu\nu}=\frac{i}{g}[D_\mu,D_\nu]$ (non-Abelian).
* **Gauge kinetic term**:

  $$
  \mathcal{L}_{\rm kin}=-\tfrac14\,F_{\mu\nu}F^{\mu\nu}
  \quad \text{or} \quad -\tfrac14\,F_{\mu\nu}^a F^{a\mu\nu}.
  $$
* **Scalar QED vertices**:

  $$
  \gamma\text{–}\phi\text{–}\phi:\; i e (k+k')_\mu,\qquad
  \gamma\gamma\text{–}\phi\text{–}\phi:\; -2 i e^2 g_{\mu\nu},\qquad
  \phi^4:\; -i\lambda.
  $$
* **Higgs mechanism**:

  * U(1): gauge boson mass $M=gv$.
  * Non-Abelian mass matrix:

    $$
    (M^2)^{ab}=\tfrac12 g^2\,v_i^*\,\{T_R^a,T_R^b\}_{ij}\,v_j.
    $$

---

### **General Mathematical Identities**

* **Commutator / anticommutator**: $[A,B]=AB-BA,\;\{A,B\}=AB+BA.$
* **Delta-function integral**: $\int d^3x\,e^{i\mathbf{q}\cdot\mathbf{x}}=(2\pi)^3\delta^3(\mathbf{q}).$
* **Jacobi identity**: $[[A,B],C]+[[B,C],A]+[[C,A],B]=0.$
* **Campbell–Baker–Hausdorff**: $e^{A+B}=e^A e^B e^{-\frac12[A,B]+\cdots}$.
* **Feynman parametrization (n denominators)**:

  $$
  \frac{1}{A_1\cdots A_n}=(n-1)!\int_0^1\!dx_1\cdots dx_n\,
  \frac{\delta\!\left(\sum_i x_i-1\right)}{\big(\sum_i x_i A_i\big)^n}.
  $$
* **Principal value**: $\displaystyle \frac{1}{x\pm i\epsilon}=\mathcal{P}\frac{1}{x}\mp i\pi\delta(x).$
* **Gamma function**:
  $\Gamma(n+1)=n!,\quad \Gamma\!\left(n+\tfrac12\right)=\frac{(2n)!}{n!\,2^{2n}}\sqrt{\pi}.$
  Poles: $\displaystyle \Gamma(-n+x)=\frac{(-1)^n}{n!}\!\left[\frac1x-\gamma+\sum_{k=1}^n\frac1k+O(x)\right].$
* **d-dimensional loop master integral**:

  $$
  \int\!\frac{d^d\bar q}{(2\pi)^d}\,\frac{(\bar q^2)^a}{(\bar q^2+D)^b}
  =\frac{\Gamma(b-a-\tfrac d2)\,\Gamma(a+\tfrac d2)}{(4\pi)^{d/2}\Gamma(b)\Gamma(\tfrac d2)}
   \;D^{-(\,b-a-\tfrac d2\,)}.
  $$

---

### **Notes on the Convention Changes (what flipped)**

* KG operator: $(-\,\partial^2+m^2)\to(\Box+m^2)$.
* LSZ amputators: $(-\,\partial^2+m^2)\to(\Box+m^2)$.
* Propagators: $1/(k^2+m^2-i\epsilon)\to 1/(k^2-m^2+i\epsilon)$.
* Exact 2-pt: $1/(k^2+m^2-i\epsilon-\Pi)\to 1/(k^2-m^2+i\epsilon-\Pi)$.
* On-shell point: $k^2=-m^2\to k^2=+m^2\Rightarrow \Pi(-m^2)\to \Pi(m^2)$.
* Canonical $T^{\mu\nu}$: corrected to $+\;\partial^\nu\phi$ term and $-g^{\mu\nu}\mathcal{L}$.

---

If you want, I can also **export this as a LaTeX handout** (two columns, `tcolorbox` section headers, compact spacing) or a **Markdown PDF** with a clean font—just say which format you prefer.
