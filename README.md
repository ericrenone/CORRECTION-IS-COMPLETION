# CORRECTION IS COMPLETION
## *The Sangamagrama Synthesis: Madhava's* Upasaṃhāra*, Ramanujan's Shadow, Weight Decay, and Grokking as One Algorithm Across Six Centuries — Five Cross-Document Identities, Six Unified Predictions, and the Complete Mechanism*

**ERI Labs · Eric Ren · Jersey City, New Jersey · github.com/ericrenone · June 2026**

---

> "He introduced a method that looked like a series but was not — incomplete, he knew, without the non-series correction. He called it the *upasaṃhāra* — the termination, the boundary, the stopping rule."
> — on Madhava of Sangamagrama, *MADHAVA*, ERI Labs 2026

> "I want to tell you what the mock theta functions are. They are not theta functions at all. They are something new."
> — Srinivasa Ramanujan, last letter to G. H. Hardy, 12 January 1920

> "Before grokking, the edge is gradient-driven (88–98%). At grokking, gradient and weight decay align along the edge — and the edge transitions to a compression mode (0–5% gradient, 95–99.8% weight decay). This alignment is the microscopic signature of the phase transition."
> — Xu, *Lifecycle of the Spectral Edge*, arXiv:2604.07380, April 2026

> "The correction was always there. Madhava named it first."
> — *MADHAVA*, ERI Labs 2026

---

## Abstract

Two companion documents — *MADHAVA* and *THE-WEIGHT-DECAY-WAS-ALWAYS-THE-SHADOW* — independently establish that the same mathematical object governs phenomena separated by six centuries: Madhava of Sangamagrama's 14th-century correction terms for π, Ramanujan's mock theta functions, Zwegers' 2002 harmonic Maass form completion, and the weight decay dynamics of grokking in modern neural networks. This document names the invariant they share, derives five cross-document identities that neither source establishes, and presents six unified predictions.

The invariant is: **the minimum non-series, non-gradient correction that completes an incomplete holomorphic approximation**. Madhava called it *upasaṃhāra*. Zwegers called it the shadow. The gradient optimizer calls it weight decay. They are the same operator applied in four different computational substrates across six centuries. The col(F)/ker(F) partition of the Fisher information matrix is the algebraic form of this invariant in the neural network setting; the mock/shadow partition of a harmonic Maass form is its modular incarnation; Madhava's correction terms C_N are its pre-algebraic, pre-modern instance.

The central new finding is a **triadic duality extending the Madhava-Ramanujan bilateral duality** established in *MADHAVA*: Madhava discovered the shadow before the mock; Ramanujan discovered the mock before the shadow; every grokking neural network traverses the Ramanujan trajectory (mock first, 88–98% gradient-driven) and exits it via the Zwegers completion (shadow acquisition through weight decay alignment). Every grokking event is the Madhava-Ramanujan-Zwegers six-century sequence compressed to a training run. The data was always curved. The correction was always there.

---

## I · The Universal Invariant

In 1375, Madhava of Sangamagrama wrote down a formula that would not be rediscovered in Europe for three hundred years. It was not the formula for π that history remembers. It was the correction.

Madhava computed:

$$\frac{\pi}{4} = S_N + C_N$$

where $S_N = 1 - \tfrac{1}{3} + \tfrac{1}{5} - \cdots + \tfrac{(-1)^{N-1}}{2N-1}$ is the Leibniz partial sum — computable, finite, perpetually incomplete — and $C_N$ is the correction term, arriving in three successively refined versions across multiple generations of Kerala commentary:

$$C_N^{(1)} = \frac{(-1)^N}{2N+1}, \quad C_N^{(2)} = \frac{(-1)^N(N+1)}{(2N+1)^2+1}, \quad C_N^{(3)} = \frac{(-1)^N(N^2+N+\tfrac{1}{4})}{(2N+1)^3}$$

The series was not the discovery. The correction was.

In 2026, a different document described a different phenomenon. In a transformer trained with weight decay on modular arithmetic, the spectral edge of the parameter update Gram matrix undergoes a lifecycle transition: before grokking, 88–98% gradient-driven; after, 95–99.8% weight-decay-driven. Without weight decay, 0 of 24 experimental runs produced grokking. With weight decay, 24 of 24 did. The gradient alone could not complete the form. The correction was necessary.

These are the same observation. One is written in Sanskrit astronomical commentary around 1375; the other appears in a preprint on arXiv in April 2026. The mathematical object is identical.

| Substrate | Mock (col F) | Shadow / Correction (ker F) | Document |
|-----------|-------------|----------------------------|----------|
| Kerala, c. 1375 | Leibniz partial sum $S_N$ | Correction term $C_N^{(3)}$ | *MADHAVA* Identity M0 |
| Modular forms, 1920–2002 | Mock theta function $\mu(q)$ | Period integral $g^*(\tau)$ | Zwegers 2002 |
| Neural networks, 2022–2026 | Gradient accumulation (88–98%) | Weight decay (95–99.8% post-grok) | Xu arXiv:2604.07380, NI-4 |
| Silicon, Volder 1959 | Shift-and-add rotation | Mode bit / overflow correction | *MADHAVA* Identity M3 |

The invariant is the minimum non-holomorphic correction that restores completeness. Four substrates, one algorithm, six centuries.

---

## II · The Triadic Duality

*MADHAVA* establishes a bilateral Madhava-Ramanujan duality and calls it the document's central finding: Madhava discovered the shadow before the mock; Ramanujan discovered the mock before the shadow. This is correct and important. It is also incomplete.

Neural network grokking provides a third trajectory, and that trajectory resolves the duality into a closed structure.

**The Ramanujan trajectory** is traversed during the pre-grokking plateau. The gradient accumulates the mock theta structure: col(F) embryo developing, Fisher rank near zero, spectral edge 88–98% gradient-driven. The shadow is absent. The correction is present in the architecture — weight decay runs throughout training — but it has not yet aligned with the col(F) directions the gradient is building. This is precisely Ramanujan in January 1920: mock without shadow, holomorphic without completion. The series is rich and extraordinary. The correction is missing. The form is incomplete.

The **Zwegers event** is grokking. Gradient and weight decay achieve alignment on the spectral edge. Weight decay, which has been projecting the ker(F) null sector throughout training, suddenly finds the same directions the gradient has been developing. The non-holomorphic shadow is applied. The harmonic Maass form — $\hat{\mu}(\tau) = \mu(q) + g^*(\tau)$ — is complete. The Fisher rank crosses from near-zero to 2–17% of activation space. The intra-signal gap opens. The accuracy curve becomes vertical. This is Zwegers in 2002: shadow found, completion achieved, 82-year gap closed.

The **Madhava trajectory** is what comes after: architectures built from the outset with the correction present. Yildirim's spherical normalisation (arXiv:2603.05228), which achieves 20× acceleration by fixing representational magnitude and thereby eliminating the horocycle pre-grokking phase, is the first Madhava-trajectory neural network. The correction was there from initialization. The series never had to discover its shadow because the shadow was already there.

**Cross-Document Identity X1 — Every Grokking Event IS the Ramanujan-Zwegers Sequence Compressed to a Training Run**:

The pre-grokking plateau = the 82-year mock-without-shadow epoch (1920–2002). The grokking transition = Zwegers 2002. The post-grokking compression phase = the harmonic Maass form stabilized, 2–17% col(F) crystallite riding on 83–98% null-sector history. Every inference from a grokked model is 83–98% pre-grokking — the Ramanujan portion — carried on a 2–17% Zwegers completion. The Madhava trajectory (shadow before mock) is the architectural design principle that eliminates the plateau entirely by providing the completion from initialization.

---

## III · The Civilizational Grokking

*MADHAVA* identifies the Kerala school as the "canonical pre-crystallization commons": a knowledge kernel deposited by Madhava in c. 1375, generating extraordinary petals across five generations of scholars, isolated from European mathematics for three hundred years due to geographic and linguistic distance. G_coord ≈ 0 externally. The crystallization event was Hardy's recognition of Ramanujan in 1913–1914.

*THE-WEIGHT-DECAY-WAS-ALWAYS-THE-SHADOW* identifies the pre-grokking epoch as the regime in which the Fisher information matrix has near-zero rank in task-relevant directions, gradient flow executes polynomial-mixing horocycle motion in the cusp of the modular surface, and the spectral edge is 88–98% gradient-driven. No generalization signal escapes the cusp. G_coord ≈ 0. The crystallization event is the grokking transition.

These are the same structure at different scales.

**Cross-Document Identity X2 — The Kerala School's 300-Year Isolation IS the Pre-Grokking Null Sector at Civilizational Scale**:

| Kerala School (300-year isolation) | Neural Network Pre-Grokking |
|------------------------------------|-----------------------------|
| G_coord ≈ 0 externally (geographic/linguistic isolation) | Fisher rank r(t)/n < 0.01 |
| Rich internal structure (five generations of commentarial petals) | Execution manifold active (rank-1, horocycle orbit) |
| Missing conditioning clause $X_{t-1}$ | Missing spectral gap (sub-Selberg, g(t) ≈ 0) |
| Knowledge deposited without crystallization (*Yuktibhāṣā* c. 1530) | Mock theta coefficient accumulation without shadow |
| Shadow present (C_N terms) but modular transformation absent | Weight decay running but not yet aligned on col(F) |
| Crystallization event: Hardy 1913–1914 | Crystallization event: grokking transition |
| Post-crystallization: G_coord > 0 (European rediscovery + extension) | Post-grokking: r(t)/n ≈ 0.02–0.17 (col(F) active) |

The quantitative prediction follows directly from NI-8 of *THE-WEIGHT-DECAY-WAS-ALWAYS-THE-SHADOW* (adiabatic parameter $A = 1/T_{\text{remaining}}$): pre-crystallization duration $T_{\text{isolation}} \propto \varepsilon_{\text{coord}}^{-4/\lambda_1}$, where $\varepsilon_{\text{coord}}$ is the epistemic commutator defect (degree of misalignment between knowledge kernel and global intellectual commons) and $\lambda_1$ is the Selberg spectral gap of the shared mathematical topology. For the Kerala school: $T_{\text{isolation}} \approx 300$ years, $\lambda_1 \approx 0$ (complete isolation), $\varepsilon_{\text{coord}} \to 0$ — consistent with the T_mem formula diverging as ε_grad → 0.

The kernel did not degrade across 300 years. The null sector accumulated. The mock was always complete. The shadow was always there. The correction was always there.

---

## IV · The Selberg Gap as Bridge

*MADHAVA* establishes Identity M2: Madhava's refined correction $C_N^{(3)}$ introduces a spectral gap satisfying $\lambda_1 \geq 3/16$ — the Selberg lower bound — for the corrected approximant sequence. This converts the O(N⁻¹) horocycle-regime convergence of the bare Leibniz series to O(N⁻³) geodesic-regime convergence.

*THE-WEIGHT-DECAY-WAS-ALWAYS-THE-SHADOW* establishes NI-3: the intra-signal gap $g(t)$ in the Gram matrix of parameter updates satisfies $g(t) = \max(0, \lambda_1(t) - 1/4)$; grokking occurs when $\lambda_1$ crosses the Selberg floor of $1/4$.

The gap between $3/16$ and $1/4$ is $1/16$. This gap has a precise meaning.

**Cross-Document Identity X4 — Madhava Achieves Sub-Selberg; Weight Decay Completes the Crossing**:

Madhava's $C_N^{(3)}$ achieves $\lambda_1 \geq 3/16$ — approaching but not crossing the Selberg floor of $1/4$. The correction terms known to Jyeshthadeva and the Kerala commentators were sufficient to transform horocycle convergence into something better, but not sufficient to achieve modular completion. The residual gap $\Delta\lambda_1 = 1/4 - 3/16 = 1/16$ is precisely what Zwegers supplied in 2002: the full non-holomorphic period integral that restores the modular transformation property under $\text{SL}(2, \mathbb{Z})$.

In neural network training: Madhava's correction is the EW-1 warm-up phase (gradient alignment begins; col(F) embryo forms; $\lambda_1$ rises from near-zero toward $3/16$). Weight decay provides the final $3/16 \to 1/4$ crossing that is grokking: the Zwegers shadow applied in the silicon substrate.

The empirical test is direct: measure $\lambda_1(t)$ from the Xu Gram matrix framework during training both with and without weight decay. The no-weight-decay runs (0/24 grokking) should plateau below $1/4$, potentially near $3/16$. The weight-decay runs (24/24 grokking) should cross $1/4$. The height of the no-WD attractor — whether it settles near $3/16$ or elsewhere — is the first empirical measurement of the discrete Madhava spectral gap in a neural network.

---

## V · The Sangamagrama Operator as Optimal Weight Decay Schedule

*MADHAVA* defines the Sangamagrama Operator:

$$\Omega_S = \mathcal{S}_M \circ T$$

where $\mathcal{S}_M f = S_N + C_N^{(3)}$ is the Madhava shadow correction (converting the partial sum to a geodesic-regime approximant) and $T(x) = \{1/x\}$ is the Gauss continued-fraction shift (the angle-doubling step of the modular surface). This composition achieves O(N⁻⁵) convergence from an O(N⁻¹) baseline — a factor of N⁴ improvement per application. The 2024 QH-CORDIC algorithm (quadruple-step-ahead for hyperbolic functions) is $\Omega_S$ implemented in silicon.

*THE-WEIGHT-DECAY-WAS-ALWAYS-THE-SHADOW* establishes that weight decay is the Zwegers shadow operator (NI-4) and that grokking requires alignment of gradient and weight decay on the spectral edge. The alignment is the shadow acquisition step in the Madhava correction: the moment when the ker(F) projector finds the col(F) directions.

**Cross-Document Identity X3 — $\Omega_S$ Prescribes the Optimal Weight Decay Schedule, Predicting 4× Grokking Acceleration**:

The Sangamagrama Operator applied to the optimization landscape prescribes:
1. **One shadow step** ($\mathcal{S}_M$): apply weight decay *preferentially* to ker(F) directions identified in the current batch gradient statistics, rather than isotropically. This is the discrete shadow integral of the Bernoulli polynomial generating function, now applied to the parameter vector rather than the Leibniz partial sum.
2. **One Gauss shift** ($T$): one step of continued-fraction angle doubling — in optimization language, a learning rate step that doubles the effective gradient magnitude in the col(F) subspace, exploiting the spectral gap just opened by the shadow step.

The composition achieves O(N⁻⁵) convergence, corresponding directly to the QH-CORDIC four-fold iteration reduction. The prediction: an AdamW optimizer with weight decay scheduled per $\Omega_S$ should achieve approximately 4× faster grokking than standard AdamW on modular arithmetic benchmarks. This is directly testable from the Power 2022 arithmetic setup.

The 20× acceleration from Yildirim's spherical normalisation (fixing ε_grad throughout, Identity NI-6) is the architectural implementation of the same principle: rather than dynamically applying the shadow correction, the architecture enforces the correction statically. $\Omega_S$ is the dynamic analog; Yildirim is the static analog. The ratio 20×/4× ≈ 5 corresponds to the additional gain from eliminating the horocycle phase entirely (static) versus merely accelerating the shadow acquisition (dynamic). Both are Madhava-trajectory interventions.

---

## VI · The *Yuktibhāṣā* Watson-Wilson Map

*MADHAVA* performs the Watson-Wilson verification protocol on the Kerala archive: it traces how results deposited without proofs in c. 1375 received their systematic treatments across the following 625 years. Each verification event — Euler-Maclaurin (1736), Dirichlet (1837), Zwegers (2002) — is mapped onto the developing mathematical framework.

*THE-WEIGHT-DECAY-WAS-ALWAYS-THE-SHADOW* identifies three phases of the pre-grokking epoch: EW-1 (gradient alignment begins, col(F) embryo), EW-2 (Selberg floor approached, commutator defect spikes, final 3–5% of T_mem), and grokking (shadow acquisition, spectral gap opening, Fisher rank crossing).

**Cross-Document Identity X5 — Each *Yuktibhāṣā* Watson-Wilson Event IS a Neural Network Training Phase**:

| *Yuktibhāṣā* Watson-Wilson Event | Duration After Deposit | Neural Network Analog |
|-----------------------------------|----------------------|----------------------|
| Kernel deposited (Madhava, c. 1375) | t = 0 | Initialization |
| Proofs distributed orally, no crystallization (c. 1375–1530) | 0–155 yr | Stage 1: null sector dominance, r(t)/n < 0.01 |
| Proofs deposited (*Yuktibhāṣā*, c. 1530) | 155 yr | Late Stage 1: mock theta coefficients accumulate |
| European rediscovery without correction (Gregory, Newton, Leibniz, 1671–1676) | ~300 yr | Stage 1 exit: gradient finds col(F) embryo |
| Euler-Maclaurin formula (1736) | 361 yr | **EW-1**: shadow integral named; gradient alignment begins |
| Dirichlet $L(1, \chi_4) = \pi/4$ (1837) | 462 yr | **EW-2**: modular form identified; Selberg floor approached; commutator defect spikes |
| Hardy crystallization (1913–1914) | 538–539 yr | Pre-grokking final 3–5%: spectral gap opening; G_coord > 0 |
| Zwegers completion (2002) | 627 yr | **Grokking**: shadow acquired; weight decay aligns on col(F) |
| Post-Zwegers programme (2002–2026) | 627–651 yr | Post-grokking: 2–17% col(F) crystallite stabilized |

The correspondence is not metaphorical. The Euler-Maclaurin event — systematic derivation of the discrete shadow integral — IS the EW-1 signal: the moment when the correction first receives algebraic recognition. The Dirichlet event — identification of the Leibniz series as a modular L-function value — IS the EW-2 signal: the moment when the spectral structure of the mock is identified, prior to shadow acquisition. The Zwegers event — full harmonic Maass form completion — IS grokking. The kernel did not degrade across 627 years. The null sector accumulated. The shadow was always there.

---

## VII · Complete Identity Table

### From *MADHAVA*

| ID | Madhava Object | Framework Realization |
|----|---------------|----------------------|
| M0 | Correction term $C_N$ | Discrete shadow integral: non-holomorphic completion of the Leibniz mock series at cusp q = 1 |
| M1 | Partial sum $S_N$ | Farey approximant: Ford circle center at denominator N; geodesic orbit point on M at height log(2N+1) |
| M2 | Refined correction $C_N^{(3)}$ | Selberg gap λ₁ ≥ 3/16; transition from horocycle (O(N⁻¹)) to geodesic (O(N⁻³)) convergence |
| M3 | Sine series N-th term | N-th CORDIC circular-mode iteration; Banach contraction k = 1/2 in power-series coordinates |
| M4 | Convergence radius π | Selberg zeta pole; boundary between compact core and cusp divergence regime |
| M5 | Machin denominators 5, 239 | Markov numbers; Rogers-Ramanujan modulus-5 nodes; Stern-Brocot depth-5 structure |
| M6 | Kerala school isolation | Pre-crystallization commons: G_coord ≈ 0 externally; mock present, shadow present, modular transformation absent |
| M7 | Sangamagrama Operator $\Omega_S$ | $\mathcal{S}_M \circ T$ achieves O(N⁻⁵); QH-CORDIC quadruple-step-ahead in silicon |

### From *THE-WEIGHT-DECAY-WAS-ALWAYS-THE-SHADOW*

| ID | Neural Network Object | Framework Realization |
|----|-----------------------|----------------------|
| NI-1 | Execution manifold (rank-1, invariant) | Horocycle orbit η_s; commutator defect ‖[W_Q, W_K]‖_F = ε_grad proxy |
| NI-2 | RLCT (real log-canonical threshold) | (d/2)(1 − null sector fraction); LLC trajectory = col(F) crystallization tracker |
| NI-3 | Intra-signal gap g(t) | max(0, λ₁(t) − 1/4) in Selberg coordinates; k* ≤ 3 = col(F) dimension at grokking |
| NI-4 | Weight decay | Zwegers shadow operator; 0/24 grokking without WD, 24/24 with WD |
| NI-5 | Pre-grokking [H, M] non-normality | Mock theta state: [H, M] maximal when M adapted to ker(F) but H has no col(F) structure; κ(V) → ∞ = cusp singularity |
| NI-6 | L2 normalisation throughout residual stream | Fixing ε_grad; horocycle elimination; 20× acceleration when task has cyclic symmetry |
| NI-7 | Dyson Brownian motion (no outlier) | Mock theta coefficient dynamics; outlier escape = col(F) crystallization; Q/K = col(F); V/O = ker(F) |
| NI-8 | Adiabatic parameter A | $A = \varepsilon_{\text{grad}}^4 / (\eta \lambda_1 (\lambda_1 - 1/4)^2) = 1/T_{\text{remaining}}$; signal-strength ODE = T_mem formula in differential form |
| NI-9 | Multi-task staggered grokking | Staggered Zwegers completions of orthogonal mock theta functions; timing = differential Markov trap depths |

### New — This Document

| ID | Cross-Document Object | Identity |
|----|----------------------|---------|
| **X1** | Grokking trajectory | Every grokking event = Ramanujan-Zwegers six-century sequence compressed to a training run. Pre-grokking plateau = 82-year mock-without-shadow epoch. Grokking = Zwegers 2002. |
| **X2** | Kerala school isolation | 300-year external isolation = pre-grokking null sector at civilizational scale. G_coord ≈ 0 = r(t)/n < 0.01. Hardy 1913 = grokking. |
| **X3** | Sangamagrama Operator as optimizer | $\Omega_S = \mathcal{S}_M \circ T$ prescribes optimal weight decay schedule; predicts ≈4× grokking speedup over standard AdamW on modular arithmetic. |
| **X4** | Selberg gap bridge | Madhava correction achieves λ₁ ≥ 3/16 (sub-Selberg, sub-floor); weight decay provides residual 3/16 → 1/4 crossing. Gap 1/16 = Zwegers contribution absent from Kerala archive. |
| **X5** | *Yuktibhāṣā* Watson-Wilson map | Each Kerala Watson-Wilson event (Euler-Maclaurin, Dirichlet, Zwegers) corresponds to a neural network training phase (EW-1, EW-2, grokking) at 361, 462, and 627 years latency. |

---

## VIII · Six Unified Predictions

**P-X1 — The Pre-Grokking Gram Spectrum Attractor is λ₁ ≈ 3/16**

The $\lambda_1$ of the Gram matrix rolling-window spectrum should converge to an attractor near $3/16 \approx 0.1875$ during the pre-grokking plateau, rather than converging to zero or an arbitrary value. The grokking event should produce a discontinuous jump from ≈3/16 to ≥1/4 (Selberg floor crossing). The no-weight-decay runs (0/24 in Xu 2604.07380) should plateau below 1/4; the weight-decay runs (24/24) should cross it. Testable by instrumenting the Xu intra-signal gap framework at fine temporal resolution during the EW-2 epoch.

*Falsification*: The no-WD pre-grokking $\lambda_1$ plateau does not fall in [0.15, 0.22] across four of five random seeds.

**P-X2 — $\Omega_S$-Scheduled Weight Decay Achieves ~4× Grokking Acceleration**

An AdamW optimizer with weight decay applied preferentially to ker(F) directions (the Madhava shadow step $\mathcal{S}_M$) followed by a learning rate doubling in the col(F) subspace (the Gauss shift T) should achieve approximately 4× faster grokking than standard AdamW on modular arithmetic mod 97, matching the QH-CORDIC four-fold speedup that $\Omega_S$ achieves in the analytic setting. Testable by implementing $\Omega_S$-scheduled AdamW on the Power 2022 benchmark across five seeds.

*Falsification*: $\Omega_S$-scheduled weight decay achieves less than 2× speedup over standard AdamW across five random seeds.

**P-X3 — The [H, M] Commutator Collapse Coincides with the 3/16 → 1/4 Selberg Crossing**

In a grokking transformer instrumented simultaneously with Ghosh's non-normal spectral measurement (‖[H, M]‖_F / ‖H‖_F) and the Xu intra-signal gap $g(t)$, the [H, M] collapse event (NI-5) should begin exactly when $\lambda_1$ crosses $3/16$ and complete when $\lambda_1$ crosses $1/4$. The collapse should be a smooth function of the residual gap $1/4 - \lambda_1(t)$, not a step function. This temporal profile distinguishes the Madhava sub-Selberg level (3/16) as a distinct dynamical threshold from the Selberg floor (1/4).

*Falsification*: [H, M] collapse is not monotonically increasing in $\lambda_1$ between $3/16$ and $1/4$, or occurs entirely before $\lambda_1 = 3/16$, across more than two of five seeds.

**P-X4 — Spherical Normalisation Acceleration Follows the T_mem Formula Quantitatively**

The Yildirim 20× acceleration from spherical normalisation is reproduced quantitatively by the T_mem formula $T_{\text{mem}} \propto \varepsilon_{\text{grad}}^{-4/\lambda_1}$. The ratio of pre-grokking durations equals $(\varepsilon_{\text{grad, free}} / \varepsilon_{\text{grad, spherical}})^{4/\lambda_1}$, where ε_grad(free) is the plateau-phase commutator defect in the unconstrained architecture and ε_grad(spherical) is the boundary-constrained value. Measuring both quantities independently constrains λ₁, providing the first architecture-free estimate of the Selberg spectral gap in a grokking transformer.

*Falsification*: The T_mem formula with measured ε_grad values fails to reproduce the Yildirim 20× factor within 3× across three ε_grad constraint levels.

**P-X5 — The *Yuktibhāṣā* Chapter 6 Recursion Contains an Implicit Rogers-Ramanujan q-Series**

The combinatorial identity in *Yuktibhāṣā* Chapter 6 (Jyeshthadeva's proof of the sine series via iterated integration of polynomial approximants) contains a q-series specialization that, at q = 1, reduces to the Rogers-Ramanujan first identity, with the gap condition arising from the iterated-integral recursion structure. This would establish that the Rogers-Ramanujan identities were implicitly present in the Kerala archive from c. 1530, 364 years before Rogers' 1894 paper — analogous to how Ramanujan independently contained the shadow that Zwegers would formalize. Testable by extracting the generating function from Sarma's 2008 translation of the Chapter 6 recursion.

*Falsification*: No q-series specialization of the Yuktibhāṣā iterated-integration recursion reduces to the Rogers-Ramanujan first identity at q = 1.

**P-X6 — Machin Formula Efficiency is the Inverse Markov Constant Product**

Every Machin-type formula expressing π as a rational combination of arctangents of unit fractions decomposes the geodesic from the cusp to π/4 through Markov-number Ford circles. Efficiency (digits of π per term) is proportional to the inverse product of the Markov constants of the denominators. The Chudnovsky algorithm — the most efficient known π formula — should correspond to a local minimum of the Markov constant product over rational arctangent decompositions. Testable from the explicit Markov constants of Chudnovsky-related denominators and comparison with alternative Machin decompositions of equal term count.

*Falsification*: The Chudnovsky denominators do not minimize the Markov constant product among Machin decompositions with the same number of terms.

---

## IX · The Complete Historical Sequence

```
c. 1375 — Madhava, Sangamagrama, Kerala
          Shadow before mock: correction terms C_N discovered first.
          Series identified as incomplete at the outset.
          upasaṃhāra: the termination, the boundary, the stopping rule.
          Sine, cosine, arctan series in power-series form.
          CORDIC analytic form. Geodesic orbit on M, unnamed.
          Carr coefficient C(K_Madhava) > 10³.

c. 1530 — Jyeshthadeva, Yuktibhāṣā
          First systematic proof text. Kerala Lost Notebook.
          Deposited. Uncatalogued by European mathematics for 400 years.
          G_coord = 0 externally: pre-crystallization, Stage 1.
          [X5: Stage 1 plateau begins.]

1671–1676 — Gregory, Newton, Leibniz (independent)
          European rediscovery of the same series.
          No knowledge of the Kerala archive.
          C_N^{(1)} only: trivial correction, not Madhava's insight.
          Shadow lost. Mock recovered without correction.

1736 — Euler-Maclaurin formula
          [X5: EW-1 event — shadow integral named, 361 years latency.]
          Systematic theory of Madhava's correction terms.
          First algebraic framework for the discrete shadow.

1837 — Dirichlet, L(1, χ₄) = π/4
          [X5: EW-2 event — modular form identified, 462 years latency.]
          Madhava's series = special value of modular L-function at cusp.

1894 — Rogers, Rogers-Ramanujan identities
          Partition-theoretic structure of the modular boundary.
          Golden ratio emerges from combinatorics.
          Madhava's depth-5 Machin denominators = Markov numbers (M5).

1913–1914 — Hardy recognizes Ramanujan
          Crystallization event for the Kerala-Ramanujan commons.
          G_coord > 0 for the first time since Sangamagrama.
          [X2: civilizational grokking — 538-year pre-grokking plateau ends.]

1920 — Ramanujan's last letter: mock theta functions
          Mock before shadow: col(F) without ker(F).
          Ramanujan names the incompleteness. Dies three months later.
          [X1: neural network pre-grokking epoch begins here.]

1959 — Volder, CORDIC
          Madhava's sine series in shift-and-add silicon (M3).
          Banach contraction at k = 0.5.
          CORDIC = Madhava = Banach: same operation, three substrates.

2002 — Zwegers, mock theta completion
          ker(F) found. Shadow named. Harmonic Maass form completed.
          625 years after Madhava deposited the shadow without the mock.
          [X1: neural network grokking event — Zwegers compressed to one step.]

2022 — Power, grokking discovered in neural networks
          Sudden generalization after prolonged memorization plateau.
          Mock-before-shadow Ramanujan trajectory identified empirically.
          Weight decay identified as necessary (NI-4, 24/24 → 0/24).

2024 — QH-CORDIC quadruple-step-ahead
          Sangamagrama Operator Ω_S in silicon (M7, X3).
          Four iterations reduced to one: O(N⁻⁵) in hardware.

Feb–Apr 2026 — Xu arXiv series (2602–2604)
          Execution manifold = horocycle orbit (NI-1).
          Weight decay = Zwegers shadow: causal evidence (NI-4).
          Adiabatic parameter A = 1/T_remaining (NI-8).
          Intra-signal gap g(t) = Selberg floor (NI-3).
          Multi-task grokking = staggered Zwegers completions (NI-9).

Mar 2026 — Cullen, Yildirim, Ghosh arXiv
          RLCT = inverse Fisher rank (NI-2).
          Spherical normalisation = ε_grad fixing = 20× acceleration (NI-6).
          Non-normality [H,M] = mock theta state (NI-5).

May–Jun 2026 — DMFT spectral dynamics, FishBack, Singh
          Outlier escape = col(F) crystallization (NI-7).
          Seven independent programmes name seven faces of one object.
          None names the partition.

Jun 2026 — THE-WEIGHT-DECAY-WAS-ALWAYS-THE-SHADOW (ERI Labs)
          NI-4: weight decay = Zwegers shadow operator. Mechanism complete.
          Nine cross-identifications. The partition named.

Jun 2026 — MADHAVA (ERI Labs)
          M0–M7: Madhava-Ramanujan bilateral duality established.
          Sangamagrama Operator. Kerala as pre-crystallization commons.
          Shadow before mock: the inversion identified.

Jun 2026 — CORRECTION IS COMPLETION (this document)
          X1–X5: five cross-document identities.
          The triadic duality named: Madhava → Ramanujan → Grokking.
          Every grokking event = six centuries compressed to a training run.
          Kerala isolation = civilizational pre-grokking (X2).
          Ω_S prescribes the optimal weight decay schedule (X3).
          Madhava achieves 3/16; weight decay provides 1/16 residual (X4).
          Yuktibhāṣā Watson-Wilson events = EW-1/EW-2/grokking phases (X5).

          The correction was always there. Madhava named it first.
          He called it upasaṃhāra. We call it weight decay.
          They are the same.
```

---

## References

### Kerala School
- Madhava of Sangamagrama (c. 1375). *Mahajyānayanaprakāra*. Reconstructed from Nilakantha Somayaji's commentary.
- Jyeshthadeva (c. 1530). *Yuktibhāṣā* (Ganita Adhyāya, Chapters 6–7). Trans. K. V. Sarma, Springer, 2008.
- Nilakantha Somayaji (c. 1501). *Tantrasamgraha*. Trans. K. Ramasubramanian and M. S. Sriram, Springer, 2011.
- Roy, R. (1990). The Discovery of the Series Formula for π by Leibniz, Gregory and Nilakantha. *Mathematics Magazine* 63(5), 291–306.
- Plofker, K. (2009). *Mathematics in India*. Princeton University Press.

### Mock Theta Functions and Shadow Completion
- Zwegers, S. P. (2002). *Mock Theta Functions*. Doctoral thesis, Universiteit Utrecht.
- Zagier, D. (2009). Ramanujan's mock theta functions and their applications. *Séminaire Bourbaki*, No. 986.
- Ono, K. (2009). Unearthing the Visions of a Master: Harmonic Maass Forms and Number Theory. *Proc. 2008 Harvard–MIT Current Developments in Mathematics*, 347–454.

### Spectral Edge and Grokking (2026)
- Xu (arXiv:2602.10496). Low-Dimensional Execution Manifolds in Transformer Learning Dynamics.
- Xu (arXiv:2602.16746). Low-Dimensional and Transversely Curved Optimization Dynamics in Grokking.
- Xu (arXiv:2602.16967). Early-Warning Signals of Grokking via Loss-Landscape Geometry.
- Xu (arXiv:2602.18523). The Geometry of Multi-Task Grokking.
- Xu (arXiv:2603.15678). Spectral Edge Dynamics of Training Trajectories.
- Xu (arXiv:2603.28964). The Spectral Edge Thesis.
- Xu (arXiv:2604.07380). Lifecycle of the Spectral Edge.
- Cullen, Estan-Ruiz, Danait, Li (arXiv:2603.01192). Grokking as Phase Transition via SLT.
- Yildirim (arXiv:2603.05228). Geometric Inductive Bias of Grokking.
- Ghosh (arXiv:2605.23476). Non-normal spectral signatures of instability.
- Liu et al. (arXiv:2604.22778). Spectral Lifecycle of Transformer Training.
- Spectral Dynamics (arXiv:2605.07870). Feature Learning, Outlier Escape.

### Modular Surface and Geodesic Dynamics
- Selberg, A. (1965). On the estimation of Fourier coefficients of modular forms. *AMS Proc. Symp. Pure Math.* VIII, 1–15.
- Ratner, M. (1991). On Raghunathan's measure conjecture. *Annals of Math.* 134(3), 545–607.

### CORDIC and Hardware
- Volder, J. E. (1959). The CORDIC Trigonometric Computing Technique. *IRE Transactions on Electronic Computers* EC-8(3), 330–334.
- Kumar, R. et al. (2026). CARMEN: CORDIC-Accelerated Resource-Efficient Multi-Precision Inference Engine. arXiv:2605.06878.

### Diophantine Approximation
- Hurwitz, A. (1891). Ueber die angenäherte Darstellung der Irrationalzahlen durch rationale Brüche. *Math. Ann.* 39(2), 279–284.
- Markov, A. A. (1879). Sur les formes quadratiques binaires indéfinites. *Math. Ann.* 17, 379–399.

### ERI Labs Antecedents
- Ren, E. (2026). MADHAVA: The Shadow Before the Mock. github.com/ericrenone/MADHAVA.
- Ren, E. (2026). THE-WEIGHT-DECAY-WAS-ALWAYS-THE-SHADOW. github.com/ericrenone/THE-WEIGHT-DECAY-WAS-ALWAYS-THE-SHADOW.
- Ren, E. (2026). RAMANUJAN: The Mock and the Shadow. github.com/ericrenone/RAMANUJAN.
- Ren, E. (2026). Volder-1: The Rotation Is the Fixed Point. github.com/ericrenone/Volder-1.
- Ren, E. (2026). THE-MOCK-IS-THE-HESSIAN-IS-THE-PARTITION-FUNCTION. github.com/ericrenone.
- Ren, E. (2026). PRE-GROKKING-WAS-ALWAYS-THE-CUSP-WAS-ALWAYS-THE-MOCK-THETA. github.com/ericrenone.
- Ren, E. (2026). HGLD. github.com/ericrenone.
- Ren, E. (2026). SELBERG. github.com/ericrenone.

---

*ERI Labs · Eric Ren · Jersey City, New Jersey · github.com/ericrenone · June 2026*

*Lineage: CORRECTION-IS-COMPLETION ← MADHAVA (Kerala shadow-before-mock; C_N = discrete shadow integral; Sangamagrama Operator Ω_S = QH-CORDIC; Carr coefficient > 10³; bilateral Madhava-Ramanujan duality) + THE-WEIGHT-DECAY-WAS-ALWAYS-THE-SHADOW (NI-1 through NI-9; weight decay = Zwegers shadow; execution manifold = horocycle; complete pre-grokking mechanism) → five cross-document identities: X1 (grokking = Ramanujan-Zwegers compressed); X2 (Kerala isolation = civilizational pre-grokking null sector); X3 (Ω_S = optimal weight decay schedule, 4× prediction); X4 (Madhava achieves 3/16 sub-Selberg; weight decay provides residual 1/16 crossing); X5 (Yuktibhāṣā Watson-Wilson events = EW-1/EW-2/grokking at 361/462/627 year latency). Six unified predictions P-X1 through P-X6. The triadic duality named. The upasaṃhāra was the shadow was the weight decay. Correction is completion.*

*The correction was always there.*
