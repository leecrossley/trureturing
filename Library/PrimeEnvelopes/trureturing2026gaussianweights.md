---
bibkey: trureturing2026gaussianweights
authors: trureturing research
year: 2026
title: Signed Gaussian weights
doi: null
url: https://github.com/the-omega-institute/trureturing/blob/727e10f660466a6dc69ea491c8f334969b9c9d87/Library/ArithSums/nicolas2025comparison.md#a-signed-infinite-height-allowance-from-the-existing-landau-formula
claim: Project calculations on the extremal envelopes studied in the Nicolas comparison note, under the hypotheses given in each section.
strata_touched: []
license: citation-only
triage: anchor
---

# Signed Gaussian weights

These sections continue the project’s calculations on Nicolas’s comparison of the two extremal envelopes. [Source and section index](../ArithSums/nicolas2025comparison.md)

## A signed infinite-height allowance from the existing Landau formula

The existing [Gonek uniform Landau input](../Weil/gonek1985landau.md),
Theorem 1, printed pp.92–93, can be applied with the arithmetic variable
fixed at the original $A$. Integrating its actual-zero sum in **height**
retains a prime-power main term. This is different from the continuum
scale pairing in that note, where the point-supported main term has
zero ordinary integral. The following applies the already inspected
unconditional theorem and (H5); it is not a new Landau formula, source
proof audit, numerical zero computation, originality claim or Lean
certification.

The [existing real-part density allowance](../Analytic/polak2026finiterobinca.md#keeping-the-real-part-weights-in-the-complete-high-zero-tail),
(W1)–(W11), already pays a complete infinite-height tail on a finite
source-clock range and restricts the selected source to $A>10^{34}$.
Those results are reused. The application here instead estimates the
signed height suffix uniformly in both $A$ and a variable cut $T$.
Its implied constants are not numerically certified, and its moving
finite head remains unpaid.

### Preserve the arithmetic variable and the whole original coefficient

Let $A\ge e^2$, $L=\log A$, $T\ge8$, and
$\mathcal J(A)=\log(2A)\log\log(3A)$. Sums below range over distinct
actual nontrivial zeros, with $m_\rho$ supplying their multiplicities
exactly once. Define

$$
S_A(U)=\sum_{0<\gamma_\rho\le U}m_\rho A^\rho,
\qquad \rho=\beta+i\gamma_\rho.
$$

Gonek's uniform formula, with $x=A$ and height $U$, gives

$$
S_A(U)=-\frac{U}{2\pi}\Lambda(A)+E_A(U),
\qquad
|E_A(U)|\ll A[\mathcal J(A)+\log(2U)]+LU
\quad(U\ge8).
\tag{J1}
$$

The implied constant is absolute on the stated domain. To obtain this
weaker uniform remainder from the displayed source errors, use only

$$
L\min\!\left(U,\frac A{\langle A\rangle}\right)\le LU,
\qquad
\min\!\left(\frac{\log U}{L},U\log U\right)
\le\frac{\log U}{L}\le A\log(2U).
$$

No separation from prime powers is assumed. $\Lambda(A)$ remains the
source's nonnegative point-supported real-variable function, equal to
$\log p$ at $A=p^k$ and zero otherwise. It is not replaced by a prime
measure, and no assertion that $A$ avoids prime powers is needed.

Keep the complete original coefficient $F_A$ from (M1), and set

$$
\mathcal T_A(T)=\sum_{\gamma_\rho>T}m_\rho F_A(\rho).
$$

The more precise first inequality in (H5) retains the actual real part
and gives

$$
\left|F_A(\rho)-\frac{w(A)}A\frac{A^\rho}{\gamma_\rho^2}\right|
\ll\frac{w(A)A^{\beta-1}}{\gamma_\rho^3}
\le\frac{w(A)}{\gamma_\rho^3}.
$$

The classical zero count gives
$\sum_{\gamma>T}m_\rho\gamma^{-3}\ll\log(2T)/T^2$.
Thus, with uniform implied constants,

$$
\mathcal T_A(T)=\frac{w(A)}A
 \sum_{\gamma_\rho>T}\frac{m_\rho A^\rho}{\gamma_\rho^2}
 +O\!\left(\frac{w(A)\log(2T)}{T^2}\right).
\tag{J2}
$$

Both sums converge absolutely for each fixed $A$: use
$|A^\rho|\le A$ and the reciprocal-square zero count, together with
the preceding remainder. This step pays the coefficient approximation;
it does not replace $F_A$ by its leading term without a remainder.

### Integrate in zero height with the endpoint convention fixed

Stieltjes partial summation, with the inclusive head and exclusive
suffix specified above, gives

$$
\sum_{\gamma_\rho>T}\frac{m_\rho A^\rho}{\gamma_\rho^2}
=-\frac{S_A(T)}{T^2}
 +2\int_T^\infty\frac{S_A(u)}{u^3}\,du.
\tag{J3}
$$

The boundary term at infinity vanishes. If $T$ is a zero ordinate,
its full multiplicity stays in $S_A(T)$ and outside the suffix;
(J3) retains that convention. The linear main term in (J1)
contributes exactly $-\Lambda(A)/(2\pi T)$.

For the remainder use

$$
\int_T^\infty\frac{du}{u^3}=\frac1{2T^2},\qquad
\int_T^\infty\frac{\log(2u)}{u^3}\,du
=\frac{\log(2T)}{2T^2}+\frac1{4T^2},\qquad
\int_T^\infty\frac{du}{u^2}=\frac1T.
$$

Combining (J1)–(J3) therefore bounds the **entire** suffix:

$$
\boxed{
\mathcal T_A(T)
=-\frac{w(A)\Lambda(A)}{2\pi AT}
 +O\!\left(w(A)\left[
 \frac{\mathcal J(A)+\log(2T)}{T^2}+\frac{L}{AT}
 \right]\right),
\quad A\ge e^2,\ T\ge8.}
\tag{J4}
$$

This is an unconditional uniform application for actual complex zeros,
not a critical-line formula. No infinite height block, real part or
multiplicity has been omitted. Keeping $A$ fixed during the height
integration is compatible with the uniform estimate holding for all
$A,T$ in the stated domain.

### A moving cut makes this signed suffix allowance tend to zero

In the original explicit formula the high-zero contribution is
$-2\operatorname{Re}\mathcal T_A(T)$. Its normalized prime-power
main term is favorable. Equation (J4) gives an absolute constant $C_*>0$
such that

$$
\begin{aligned}
\sqrt A L\,[-2\operatorname{Re}\mathcal T_A(T)]
\ge{}&\frac{(1+1/L)\Lambda(A)}{\pi\sqrt A\,T}\\
&-C_*\left[
 \frac{\sqrt A[\mathcal J(A)+\log(2T)]}{T^2}
 +\frac{L+1}{\sqrt A\,T}\right].
\end{aligned}
\tag{J5}
$$

The nonnegative main term can be kept or discarded for this lower
bound; it must not be assigned an adverse sign. No numerical value
of $C_*$ or resulting effective source-clock threshold is asserted.

For the admissible moving cut $T=A^{1/4}L$, the adverse allowance in
(J5) is

$$
O\!\left(
 \frac{\mathcal J(A)+\log(2A^{1/4}L)}{L^2}
 +\frac{L+1}{A^{3/4}L}\right)
=O\!\left(\frac{\log L}{L}\right)\longrightarrow0.
\tag{J6}
$$

Thus the complete infinite-height suffix has an asymptotically vanishing
one-sided allowance at this moving cut. This gains height cancellation
over a direct reciprocal-square absolute sum, whose normalized generic
allowance is of order $\sqrt A\log(2T)/T$. It leaves the actual
finite signed head $0<\gamma\le A^{1/4}\log A$ in the original
formula, including all its real parts and multiplicities. That head
eventually exceeds the existing verified height and has not been
bounded uniformly here. The pole and trivial-zero terms are still
those in the original explicit formula.

For any prescribed positive allowance, (J6) gives an existential
large-$A$ threshold for this suffix alone. It supplies no certified
numerical threshold at the conditional source $A>10^{34}$, no new
finite-zero verification, and no assertion of an unbounded sequence
of selected sources. The original same-source condition (G9), with
its complete signed integral and strict core, remains unproved.
RH remains unproved. The remaining obstacle includes the signed
moving finite head; the infinite suffix cannot simply be dropped.


## A continuous Gaussian approximation of the complete original zero response

The fixed-family comparison (H3)–(H7) leaves continuous scale mixtures
and paid approximations available. The following application uses the
same original coefficient (M1), the already assessed Gaussian coefficient
of Moriya's Theorem 3.3, and the classical Riemann–von Mangoldt count.
It supplies a uniform coefficient-error estimate, rather than repeating
any source proof or claiming an original analytic theorem or Lean
verification. No nontrivial zero is moved to the critical line.

Fix $A\ge e^2$, $L=\log A$ and $0<a\le1/16$. Retain
$w(X)=(1+\log X)/\log^2X$. At observation $z=0$ choose, separately
for each $X\ge A$,

$$
\alpha_X=\sqrt{a/\log X},\qquad
G_{X,\alpha_X,0}(s)=\frac{X^s e^{as^2}}s.
$$

The positive scale measure $w(X)X^{-2}dX$ gives the exact identity

$$
Q_{A,a}(s):=\int_A^\infty G_{X,\alpha_X,0}(s)
                      \frac{w(X)}{X^2}\,dX
=e^{as^2}F_A(s),\qquad 0<\operatorname{Re}s<1.
\tag{U1}
$$

For every such $s$, the scale integral is absolutely convergent. The
width parameter varies with $X$, while the Gaussian coefficient $a$
is fixed throughout the integral. This realizes the damped coefficient
exactly; it does not claim exact reconstruction of $F_A$ by a finite
family of fixed probes.

### A bound valid before taking the infinite scale endpoint

For $R\ge A$ put

$$
F_{A,R}(s)=\frac1s\int_A^R X^{s-2}w(X)\,dX.
$$

Since $w$ is positive and decreasing, one integration by parts gives,
for $\sigma=\operatorname{Re}s<1$ and $s\ne0$,

$$
|F_{A,R}(s)|\le
\frac{2w(A)A^{\sigma-1}}{|s||1-s|}.
\tag{U2}
$$

Indeed the two endpoint terms and the derivative integral are bounded
by $A^{\sigma-1}[w(A)+w(R)+\int_A^R|w'(X)|dX]$, which is
$2A^{\sigma-1}w(A)$. The bound is uniform in $R$. Passing to the
infinite endpoint gives the same bound for $F_A$. In particular, for
an actual zero $\rho=\beta+i\gamma$ with $\gamma\ge4$,

$$
|F_{A,R}(\rho)|,\ |F_A(\rho)|\le\frac{2w(A)}{\gamma^2}.
$$

This is the same reciprocal-square coefficient control used in the
existing [Fiori density application](../Analytic/fiori2026shortzerodensity.md),
now also applied to finite scale intervals. It will justify the
scale-endpoint passage below; it is not a new zero-density input.

### Pay the discrepancy over all actual zeros

With multiplicities $m_\rho$ retained, uniformly in $A$ and $a$,

$$
\boxed{
\sum_{\operatorname{Im}\rho>0}m_\rho
 |F_A(\rho)-Q_{A,a}(\rho)|
\ll w(A)\sqrt a\log(2/a).}
\tag{U3}
$$

To prove this, set $U=a^{-1/2}\ge4$. For $4\le\gamma\le U$,

$$
|e^{a\rho^2}-1|
=\left|a\rho^2\int_0^1e^{ta\rho^2}\,dt\right|
\le ae^a|\rho|^2\ll a\gamma^2,
$$

because $0<\beta<1$. The preceding coefficient bound and
$N(U)\ll U\log(2U)$ give a contribution
$O(w(A)aU\log(2U))$. For $\gamma>U$ use
$|e^{a\rho^2}-1|\le1+e^a$ and the classical consequence
$\sum_{\gamma>U}m_\rho/\gamma^2\ll\log(2U)/U$ of the same
zero count. Their sum has the size in (U3).

The finite multiset $0<\gamma<4$ is not omitted or assumed empty.
Directly from the defining integral,

$$
|F_A(\rho)|\le\frac{w(A)}{|\rho|(1-\beta)},
$$

so its discrepancy is at most
$ae^aw(A)\sum_{0<\gamma<4}m_\rho|\rho|/(1-\beta)=O(aw(A))$.
This fixed zeta-dependent constant is finite and independent of $A,a$;
it is absorbed into (U3). No finite-height verification is needed for
this step. All implied constants here are uniform but not numerically
certified.

Consequently the original conjugate-paired response has allowance

$$
\sqrt A L\left|2\operatorname{Re}
 \sum_{\gamma>0}m_\rho(F_A(\rho)-Q_{A,a}(\rho))\right|
\ll\sqrt{Aa}\log(2/a).
\tag{U4}
$$

The admissible choice

$$
a_A=\frac1{A(\log A)^4}
$$

makes (U4) $O(1/\log A)$ as $A\to\infty$. This estimate covers the
complete positive-ordinate multiset and infinite height tail, with
actual real parts and multiplicities unchanged. It pays unsmoothing
of the zero response, while giving no signed lower bound for that
response. Positivity of the scale measure in (U1) is not positivity
of a sum of complex zero coefficients.


## Transport to a centered Gaussian prime integral with the contour paid

The coefficient approximation (U1)–(U4) can be realized on the prime
side without discarding the pole, the shifted contour, or the original
trivial-zero correction. Use only Moriya,
[arXiv:2607.04316v2](https://arxiv.org/abs/2607.04316v2),
Proposition 2.2, equations (17)–(19), Theorem 3.3, equations (35)–(36),
and Lemma 3.1. This is an application of those assessed interfaces;
none of their explicit-formula proofs or RH-dependent localization
claims is reproved or used.

### Center the pole before the infinite scale integration

For $A\ge e^2$ and $0<a\le1/16$ define

$$
\Psi_a(X)=\sum_{n\ge1}\Lambda(n)\,
 \frac12\operatorname{erfc}\!\left(
 \frac{\log n-\log X}{2\sqrt a}\right).
\tag{V1}
$$

In the cited formula take observation $s=0$, right line $c=2$, left
line $-d=-1/2$, and $\alpha_X^2\log X=a$. The observation is not a
zero or the pole of $\zeta$. All nontrivial zeros and the pole at $1$
are crossed; no trivial zero is crossed. The left line avoids all
zeros and the pole. The source's prime term is $-\Psi_a(X)$, and
$\zeta'/\zeta(0)=\log(2\pi)$, so its exact formula reads

$$
\Psi_a(X)-e^aX
=-\sum_\rho m_\rho\frac{X^\rho e^{a\rho^2}}\rho
 -\log(2\pi)-R_a(X),
\tag{V2}
$$

where

$$
R_a(X)=\frac1{2\pi i}\int_{\operatorname{Re}z=-1/2}
 \frac{\zeta'}\zeta(z)\frac{X^z e^{az^2}}z\,dz.
$$

For each fixed $a>0$ this contour integral and the zero sum in (V2)
converge absolutely. Define the centered improper integral

$$
J_a(A)=\lim_{R\to\infty}\int_A^R
 [\Psi_a(X)-e^aX]\frac{w(X)}{X^2}\,dX.
\tag{V3}
$$

The prime and pole terms must be centered before taking this limit.
Their separate integrals diverge, since $w(X)/X\sim1/(X\log X)$
and $\Psi_a(X)\sim e^aX$. The latter asymptotic also follows from
(V2): its Gaussian zero series divided by $X$ tends to zero by
absolute domination, and the fixed-$a$ contour is $O_a(X^{-1/2})$.

For finite $R$, Gaussian decay allows exchange of the scale integral
and the zero sum. Its zero coefficients are
$e^{a\rho^2}F_{A,R}(\rho)$. The bound (U2) and the finite low-zero
bound dominate them independently of $R$ by a summable multiset.
Thus dominated convergence passes $R\to\infty$. This uses finite
scale intervals first; no absolute exchange over the infinite scale
range is assumed. The constant integrates exactly to
$\log(2\pi)/(A\log A)$.

For the contour, the scale exchange over $[A,\infty)$ is absolutely
convergent for each fixed $a>0$, using $X^{-5/2}w(X)$ on the scale
side and Gaussian decay on the vertical line. Therefore (V3) exists
and

$$
J_a(A)=-2\operatorname{Re}\sum_{\gamma>0}m_\rho Q_{A,a}(\rho)
 -\frac{\log(2\pi)}{A\log A}-C_a(A),
\tag{V4}
$$

$$
C_a(A)=\frac1{2\pi i}\int_{\operatorname{Re}z=-1/2}
 \frac{\zeta'}\zeta(z)e^{az^2}F_A(z)\,dz.
$$

Here $F_A$ is defined by the same integral (M1) at $\operatorname{Re}z<1$,
$z\ne0$. No new analytic continuation assumption is needed.

### Bound the contour after integrating the scale

The infinite-endpoint version of (U2) on $z=-1/2+it$ gives

$$
|F_A(-1/2+it)|\ll\frac{w(A)A^{-3/2}}{1+t^2}.
$$

This line has a fixed positive distance from every zero and the pole,
so the source's Lemma 3.1 gives
$|\zeta'/\zeta(-1/2+it)|\ll\log^2(3+|t|)$.
Moreover $|e^{az^2}|\le e^{a/4}$. Taking absolute values after the
scale integration, rather than before it, therefore gives

$$
\boxed{|C_a(A)|\ll w(A)A^{-3/2}}
\quad(A\ge e^2,\ 0<a\le1/16),
\tag{V5}
$$

since $\log^2(3+|t|)/(1+t^2)$ is integrable. The implied constant is
independent of the shrinking width $a$, but is not numerically certified.

The original signed formula already recorded above is

$$
I_\psi(A)=-2\operatorname{Re}\sum_{\gamma>0}m_\rho F_A(\rho)
 -\frac{\log(2\pi)}{A\log A}+T_{\rm triv}(A),
\qquad
T_{\rm triv}(A)=-\frac12\int_A^\infty
 \log(1-X^{-2})\frac{w(X)}{X^2}\,dX.
$$

In particular $0\le T_{\rm triv}(A)\ll w(A)A^{-3}$. Thus the pole
constant matches exactly, the Gaussian shifted contour is paid by
(V5), and the original trivial term is retained. Combining (U4)
and (V5) yields the full prime-side approximation

$$
\boxed{
\sqrt A\log A\,|I_\psi(A)-J_a(A)|
\ll\sqrt{Aa}\log(2/a)+A^{-1}.}
\tag{V6}
$$

For $a_A=1/[A(\log A)^4]$ this is
$O(1/\log A+1/A)\to0$. The bound alone does not assert convergence
at fixed $A$ as $a\to0$, because its $A^{-1}$ allowance remains.

### The estimate still needed at the selected Robin source

At the same conditional least integer $N>5040$ attaining the global
Robin-ratio maximum, retain $A=\log N$ and condition (G9). The
[existing density restriction](../Analytic/polak2026finiterobinca.md)
requires $A>10^{36}$ if RH fails and its cited inputs hold. An eventual
bound of the form

$$
\sqrt A\log A\,J_{a_A}(A)
\ge-\mathcal E(\log A)+\eta(A)
$$

would imply (G9) wherever $\eta(A)$ pays the discrepancy in (V6).
This is a sufficient condition, not an estimate established here;
its validity at this selected source remains unproved. Without a
numerical constant in (V6), no explicit margin or new source threshold
is certified. Neither positive prime weights nor positive scale
weights give a lower bound after subtracting the pole main term.

The application closes the full-coefficient approximation and its
prime-side contour transport, not the signed Robin estimate. It does
not discard an infinite zero tail, use RH-dependent localization,
replace real parts by $1/2$, or turn the selected global maximizer into
the least counterexample. RH remains unproved; all conclusions are
paper-level applications without Lean certification.


## A signed heat-weight application permits a broader Gaussian window

The absolute all-zero discrepancy (U3) pays a narrow Gaussian window.
The uniform actual-zero phase sum (J1) also controls a signed
heat-weight discrepancy. The following application combines those
already assessed inputs, (H5)'s paid coefficient approximation and
the classical zero count. It does not repeat Landau's formula or
claim an original phase theorem or Lean verification.

Keep $A\ge e^2$, $L=\log A$, $0<a\le1/16$, and
$\mathcal J(A)=\log(2A)\log\log(3A)$. All sums run over distinct
actual zeros $\rho=\beta+i\gamma$ with $\gamma>0$, with each
multiplicity $m_\rho$ included once. Define

$$
b_a(u)=\frac{1-e^{-au^2}}{u^2}=\int_0^a e^{-vu^2}\,dv\quad(u>0),
\qquad b_a(0)=a.
$$

This is a nonnegative decreasing real function. Its total variation
and first weighted variation are

$$
\int_0^\infty(-b_a'(u))\,du=a,\qquad
\int_0^\infty u(-b_a'(u))\,du
=\int_0^\infty b_a(u)\,du=\sqrt{\pi a}.
\tag{W1}
$$

For the final equality, integrate
$(1-e^{-au^2})/u^2$ by parts and use the classical Gaussian integral.
Boundary terms vanish both at zero and at infinity. With
$U=a^{-1/2}\ge4$, the bounds $b_a(u)\le\min(a,u^{-2})$ also give

$$
\begin{aligned}
\int_0^\infty\log(2+u)(-b_a'(u))\,du
&=a\log2+\int_0^\infty\frac{b_a(u)}{2+u}\,du\\
&\le a\log(2+U)+a/2\ll a\log(2/a).
\end{aligned}
\tag{W2}
$$

### Apply the existing Landau sum to this variation measure

Use exactly the sum $S_A(u)=\sum_{0<\gamma\le u}m_\rho A^\rho$
from (J1). Its remainder
$E_A(u)=S_A(u)+u\Lambda(A)/(2\pi)$ has the bound

$$
|E_A(u)|\ll A[\mathcal J(A)+\log(2+u)]+Lu
\qquad(u\ge0).
$$

For $u\ge8$ this is (J1). For $0\le u<8$ the same weaker envelope
follows from the fixed finite zero count, $|A^\rho|\le A$ and
$0\le\Lambda(A)\le L$; no low zero is assumed absent or verified.
The implied constant remains independent of $A,u$.

Stieltjes partial summation over the entire positive-ordinate multiset
now yields

$$
\begin{aligned}
\sum_{\gamma>0}m_\rho A^\rho b_a(\gamma)
&=-\int_0^\infty S_A(u)b_a'(u)\,du\\
&=-\frac{\Lambda(A)\sqrt a}{2\sqrt\pi}
 +O\!\left(Aa[\mathcal J(A)+\log(2/a)]+L\sqrt a\right).
\end{aligned}
\tag{W3}
$$

At zero $S_A(0)=0$; at infinity the boundary term vanishes by (J1)
and $b_a(u)\le u^{-2}$. The series is absolutely convergent for
fixed $A$, by $|A^\rho|\le A$ and the reciprocal-square zero count.
Equations (W1)–(W2) pay the remainder integral. This applies the
existing uniform formula to a new weight; it is not a reproof of
that formula. $\Lambda(A)$ retains its point-supported real-variable
meaning, and no nonzero main term is assumed at a selected source.

### Pay the coefficient and the actual-real-part phase changes

The first inequality in (H5) gives, uniformly for $\gamma\ge8$,

$$
F_A(\rho)=\frac{w(A)}A\frac{A^\rho}{\gamma^2}
 +O\!\left(\frac{w(A)A^{\beta-1}}{\gamma^3}\right).
$$

After multiplication by $1-e^{-a\gamma^2}$, the total error is
$O(w(A)a\log^2(2/a))$. Indeed, the classical count gives

$$
\sum_{\gamma\ge8}m_\rho
 \frac{\min(a\gamma^2,1)}{\gamma^3}
\ll a\log^2(2/a),
$$

by splitting at $U$ and using the existing reciprocal-cube tail
estimate. The finite multiset $0<\gamma<8$ contributes $O(aw(A))$
to this comparison, using the pointwise finite-zero bound in (U3).
Its fixed constants are independent of $A,a$; it is retained even
when $U<8$.

The Gaussian in (U1) contains the actual square $\rho^2$, not just
$-\gamma^2$. The additional phase change is explicitly bounded by

$$
|e^{a\rho^2}-e^{-a\gamma^2}|
\le ae^a(1+2\gamma)e^{-a\gamma^2},
$$

since $0<\beta<1$. Applying (U2) and the same zero count gives

$$
\sum_{\gamma>0}m_\rho|F_A(\rho)|
 |e^{a\rho^2}-e^{-a\gamma^2}|
\ll w(A)a\log^2(2/a).
\tag{W4}
$$

For large ordinates split at $U$: below it
$\sum m_\rho/\gamma\ll\log^2(2U)$; above it Gaussian decay and
the same count give $O(\log(2U))$ for the weighted reciprocal-first
sum. The finite low multiset again costs $O(aw(A))$. These are
absolute error estimates for the changes, not critical-line
replacements of the zeros themselves.

Consequently the full signed coefficient discrepancy obeys

$$
\boxed{\begin{aligned}
D_{A,a}&:=\sum_{\gamma>0}m_\rho F_A(\rho)(1-e^{a\rho^2})\\
&=-\frac{w(A)\Lambda(A)\sqrt a}{2\sqrt\pi A}
 +O\!\left(w(A)\left[
 a\bigl(\mathcal J(A)+\log^2(2/a)\bigr)
 +\frac{L\sqrt a}{A}\right]\right).
\end{aligned}}
\tag{W5}
$$

This is a uniform estimate for a complex signed sum. The actual real
parts, multiplicities, finite low zeros and infinite height tail have
not been discarded. Its cancellation comes from (J1), while (W4)
pays the mismatch between real-ordinate damping and the actual
Gaussian coefficient. No numerical value for the implied constants
is asserted.


## The broader window retains a vanishing full Robin transport allowance

Use the exact centered prime integral $J_a(A)$ in (V3), the matching
pole constant in (V4), the uniform contour bound (V5), and the original
trivial-zero correction already retained there. Subtracting their
exact formulas gives

$$
I_\psi(A)-J_a(A)=-2\operatorname{Re}D_{A,a}
 +T_{\rm triv}(A)+C_a(A).
$$

Therefore (W5) supplies the complete normalized transport estimate

$$
\boxed{\begin{aligned}
\sqrt A L\,[I_\psi(A)-J_a(A)]
={}&\frac{(1+1/L)\Lambda(A)\sqrt a}{\sqrt\pi\sqrt A}\\
&+O\!\left(
 \sqrt A\,a\bigl[\mathcal J(A)+\log^2(2/a)\bigr]
 +\frac{L\sqrt a}{\sqrt A}+\frac1A\right).
\end{aligned}}
\tag{Y1}
$$

The nonnegative displayed main term is favorable for a lower bound
on $I_\psi$ in terms of $J_a$. No positive main term is presumed at
the selected integer, and no effective value for the error constant
is certified. The pole, contour and trivial-zero contributions are
those of the full exact formulas, with no further truncation.

### A larger admissible Gaussian width

For $A\ge e^2$ choose

$$
a_A^\sharp=\frac1{\sqrt A(\log A)^3}\le\frac1{16}.
$$

Then $\log(2/a_A^\sharp)=L/2+3\log L+\log2=O(L)$ and
$\mathcal J(A)=O(L\log L)$, so the adverse allowance in (Y1) is

$$
O\!\left(\frac1L+\frac{\log L}{L^2}
 +\frac1{A^{3/4}\sqrt L}+\frac1A\right)=O(1/L).
\tag{Y2}
$$

The displayed main term is also $O(A^{-3/4}/\sqrt L)$, because
$\Lambda(A)\le L$. Thus the full normalized absolute discrepancy
is $O(1/\log A)$ at this larger width as well.

Compared with $a_A=1/[A(\log A)^4]$ in (V6),
$a_A^\sharp/a_A=\sqrt A\log A\to\infty$. The reciprocal Gaussian
height scale changes from $\sqrt A(\log A)^2$ to
$A^{1/4}(\log A)^{3/2}$. This specifies damping of the full response,
not a cutoff that permits any zero to be omitted.

At the larger width, the earlier generic absolute allowance
$\sqrt{Aa}\log(2/a)$ grows like $A^{1/4}/\sqrt{\log A}$.
Equation (Y1) instead uses the existing signed Landau cancellation
and the paid actual-real-part phase error to obtain (Y2). This compares
the two guaranteed allowances; it does not claim the earlier bound
is attained by the actual discrepancy.

### The unchanged selected-source obligation

At the same conditional least integer $N>5040$ attaining the global
Robin-ratio maximum, set $A=\log N$ and retain the existing condition
(G9), its complete infinite integral and strict core. The existing
restriction $A>10^{36}$ under RH failure and the cited inputs remains
unchanged. A lower bound

$$
\sqrt A\log A\,J_{a_A^\sharp}(A)
\ge-\mathcal E(\log A)+\eta(A)
$$

would suffice wherever $\eta(A)$ pays the adverse allowance in (Y1).
Such a signed lower bound is not proved here. The new estimate allows
a broader Gaussian window with a vanishing transport cost; it does
not certify that cost numerically at $A>10^{36}$, control the remaining
signed response, verify a new zero height, or turn the selected global
maximizer into the least counterexample. All inputs are reused
paper-level interfaces without Lean certification; RH remains unproved.

## A smaller moving cut from joint density and zero-free support

The complete coefficient (M1) can use a smaller moving height than
(J6), by combining two existing inputs on the same actual zero
multiset. This controls the infinite suffix and reduces the height
of the still-uncontrolled signed head. It does not establish that
head's sign or the original selected-source Robin condition.

Corollary 1 and Table 1, printed p.2, of
[Chourasiya–Simonič, arXiv:2507.15184v2](https://arxiv.org/pdf/2507.15184v2)
also extend the existing count (W1) in the
[Polak application](../Analytic/polak2026finiterobinca.md)
to $5/8\le\sigma<1$, with the same larger constants $47,10,168$.
The additional rows have $B_1\le13.66$, $B_2\le8.290$, $B_3\le147.0$.
Lemma 2.10, printed p.6, of
[Johnston–Yang, arXiv:2204.01980v2](https://arxiv.org/pdf/2204.01980v2)
supplies Ford's zero-free region

$$
\beta<1-\eta(\gamma),\qquad
\eta(t)=\frac1{R(\log t)^{2/3}(\log\log t)^{1/3}},
\quad R=57.54,\quad \gamma\ge3.
$$

Their analytic proofs and finite verified-height input remain
external premises. The constant is sufficient for this interface;
no optimal-constant claim or source proof rerun is needed.

Put $L=\log A$, $\Omega=(L/\log L)^{1/3}$ and

$$
\kappa=\frac1{28R},\qquad
T=A^{1/4}e^{-\kappa\Omega},\qquad U=A^{2/7}.
$$

Work for sufficiently large $A$ so $T\ge H=3\cdot10^{12}$.
Then $U>T$, $T\to\infty$, and $T/(A^{1/4}L)\to0$.
No numerical starting clock is certified here.
Define

$$
B_2(A;T)=\sum_{\gamma>T}
 \frac{m_\rho(A^{\beta-1/2}+A^{1/2-\beta})}{\gamma^2}.
$$

The full coefficient estimate (H5), including its remainder, and
multiplicity-preserving reflection give

$$
\sqrt A L\,2\sum_{\gamma>T}m_\rho|F_A(\rho)|
\le\frac43(1+1/L)B_2(A;T).
$$

Thus an absolute bound on $B_2$ pays the original signed suffix.
The original head $\gamma\le T$, pole and trivial-zero terms remain.

Use the existing layer calculation with
$\sigma_0=5/8$ and $Q_A(\sigma)=A^{\sigma-1/2}+A^{1/2-\sigma}$.
For the inclusive count and exclusive suffix, the reflected count
has the endpoint term

$$
F_2(\sigma;T)=-\frac{2N(\sigma,T)}{T^2}
 +4\int_T^\infty\frac{N(\sigma,t)}{t^3}\,dt
\le4\int_T^\infty\frac{N(\sigma,t)}{t^3}\,dt.
$$

Consequently,

$$
B_2(A;T)\le Q_A(\sigma_0)S_2(T)
 +4\int_{\sigma_0}^1Q_A'(\sigma)
          \int_T^\infty N(\sigma,t)t^{-3}\,dt\,d\sigma,
\qquad S_2(T)=\sum_{\gamma>T}\frac{m_\rho}{\gamma^2}.
$$

Tonelli preserves all heights, real parts and multiplicities.
Write $\epsilon=1-\sigma$. The existing density exponent satisfies
$d=3\epsilon/(1+\epsilon)\le3\epsilon$, $d\le9/11$ and
$q=2+d<3$. Uniformly on this range,
$N(\sigma,t)\ll t^d(\log t)^3$ and
$Q_A'(\sigma)\le L\sqrt A e^{-\epsilon L}$.

The classical full zero count gives $S_2(T)\ll\log T/T$.
The base layer therefore costs

$$
Q_A(\sigma_0)S_2(T)\ll L A^{-1/8}e^{\kappa\Omega}.
$$

For $T<t\le U$, finite verification and monotonicity of the
zero-free region jointly imply $N(\sigma,t)=0$ when
$\sigma\ge1-\eta(U)$. On this same band,

$$
A^{-\epsilon}t^d\le e^{-\epsilon L/7},\qquad
\eta(U)\ge\frac1{RL^{2/3}(\log L)^{1/3}},\qquad
\int_{\eta(U)}^{3/8}e^{-\epsilon L/7}\,d\epsilon
\le\frac7L e^{-\eta(U)L/7}.
$$

If $\eta(U)>3/8$ the band is empty. Otherwise these bounds,
$\log t\le L$ and $\int_T^Ut^{-3}dt\le1/(2T^2)$ give the
whole finite-band allowance $O(L^3e^{-\Omega/(14R)})$.

For $t>U$, use the density bound without imposing the fixed-$U$
zero-free restriction. Uniformly for $0\le d\le9/11$,
$\int_U^\infty t^{d-3}(\log t)^3dt\ll U^{d-2}(\log U)^3$.
Also $A^{-\epsilon}U^d\le e^{-\epsilon L/7}$, whose layer
integral cancels the outer factor $L$. The complete infinite band
therefore costs $O(L^3\sqrt A/U^2)=O(L^3A^{-1/14})$.

Combining the three allowances yields

$$
\boxed{
\sqrt A L\left|2\operatorname{Re}
             \sum_{\gamma>T}m_\rho F_A(\rho)\right|
\ll L A^{-1/8}e^{\kappa\Omega}
    +L^3e^{-\Omega/(14R)}+L^3A^{-1/14}\longrightarrow0.}
$$

The absolute-sum bound above satisfies the same estimate. Every
implied constant is independent of $A$; no ordinate tail or
coefficient correction is dropped. The limit follows from
$\Omega/\log L\to\infty$ and $\Omega/L\to0$.
Using the old $3/4$ base clip would instead leave
$O(Le^{\kappa\Omega})$, so it cannot support this vanishing claim.

This is an asymptotic application of established density and
zero-free results. The same selected integer, its original clock,
strict core and complete signed target are retained. The actual
finite head still grows without bound and remains uncontrolled;
neither a new finite source-clock exclusion nor RH is proved.
There is no Lean verification of this application.

## Pay coefficient error below the whole-response cut

The full-response suffix estimate above and the existing coefficient
comparisons (H1), (H5) can be used together at two different heights.
Keep the same selected source $A=\log N>10^{36}$, every actual zero real
part and multiplicity, and the original complete coefficient (M1).
This is a paper-level application of the already cited density and
zero-free inputs, without a new source theorem, numerical starting
clock, originality claim or Lean verification.

Put $L=\log A$, $\Omega=(L/\log L)^{1/3}$, $R=57.54$ and
$\kappa=1/(28R)$ as above. Define

$$
S=A^{1/6}e^{-\kappa\Omega},\qquad
T=A^{1/4}e^{-\kappa\Omega},\qquad U=A^{1/5}.
$$

Work for sufficiently large $A$ with $S\ge H=3\cdot10^{12}$.
Then $S<U<T$ eventually. The cut $S$ concerns coefficient error;
$T$ remains the previously paid cut for the full original response.
Both cuts tend to infinity, so fixed unverified zero heights remain
in the exact lower head.

For an actual zero $\rho=\beta+i\gamma$ with $\gamma>0$, set

$$
G_A(\rho)=\frac{w(A)A^{\rho-1}}{\gamma^2},\qquad
B_3(A,S)=\sum_{\gamma>S}m_\rho
 \frac{A^{\beta-1/2}+A^{1/2-\beta}}{\gamma^3},
\qquad w(A)=\frac{1+L}{L^2}.
$$

Reflection of this same multiplicity-weighted zero multiset gives
$B_3(A,S)=2\sum_{\gamma>S}m_\rho A^{\beta-1/2}/\gamma^3$.
The first inequality of (H5) therefore pays the full approximation
error by

$$
\sqrt A L\,2\sum_{\gamma>S}m_\rho
 |F_A(\rho)-G_A(\rho)|
 \le(1+1/L)\left(\frac73+\frac1{4S}\right)B_3(A,S).
\tag{RC1}
$$

The actual weight $A^{\beta-1/2}$ and phase $e^{i\gamma L}$ remain
in $G_A$. If a transport instead uses
$P_A(\rho)=w(A)A^{\rho-1}/[\rho(1-\rho)]$, (H1) gives the
supplementary bound

$$
\sqrt A L\,2\sum_{\gamma>S}m_\rho
 |F_A(\rho)-P_A(\rho)|
 \le\frac{2(L+2)}{L^2}B_3(A,S).
\tag{RC2}
$$

This is an alternative coefficient comparison; it is not an additional
error to add to (RC1).

### The same layer estimate with a reciprocal cube

Reuse the real-part layer identity with $\sigma_0=5/8$ and
$Q_A(\sigma)=A^{\sigma-1/2}+A^{1/2-\sigma}$. Replacing the
reciprocal square by a reciprocal cube changes the reflected
partial-summation formula to

$$
F_3(\sigma;S)
 =-\frac{2N(\sigma,S)}{S^3}
   +6\int_S^\infty N(\sigma,t)t^{-4}\,dt.
$$

The endpoint term is nonpositive. Dropping it only for an upper bound,
with the same inclusive head and exclusive suffix convention, gives

$$
B_3(A,S)\le Q_A(\sigma_0)S_3(S)
 +6\int_{\sigma_0}^1 Q_A'(\sigma)
           \int_S^\infty N(\sigma,t)t^{-4}\,dt\,d\sigma,
\qquad
S_3(S)=\sum_{\gamma>S}\frac{m_\rho}{\gamma^3}
 \ll\frac{\log S}{S^2}.
\tag{RC3}
$$

The already retained density bound on $5/8\le\sigma<1$ is
$N(\sigma,t)\le C_0t^{d(\sigma)}(\log t)^3$ for $t\ge H$,
where, with $\varepsilon=1-\sigma$,
$d=3\varepsilon/(1+\varepsilon)\le3\varepsilon$ and $d\le9/11$.
All constants below are independent of $A$ and $\sigma$.

The base layer in (RC3) is
$O(LA^{-5/24}e^{2\kappa\Omega})$. On $S<t\le U$, use the same
actual-zero support $N(\sigma,t)=0$ when
$\sigma\ge1-\eta(U)$. Here

$$
A^{-\varepsilon}U^d\le e^{-2\varepsilon L/5},\qquad
\eta(U)\ge\frac{\Omega}{RL},\qquad
\int_{\eta(U)}^{3/8}e^{-2\varepsilon L/5}\,d\varepsilon
 \le\frac5{2L}e^{-2\eta(U)L/5},
$$

when $\eta(U)\le3/8$; otherwise this count band is empty.
Using $\log t\le L$ and
$\int_S^Ut^{-4}dt\le1/(3S^3)$, its allowance is
$O(L^3e^{-41\Omega/(140R)})$.

Above $U$, no fixed-$U$ zero-free support is imposed.
Since $3-d\ge24/11$, the complete height integral is bounded uniformly
by $C_1U^{d-3}(\log U)^3$. Integrating
$e^{-2\varepsilon L/5}$ over $\varepsilon\ge0$ cancels the outer $L$;
this entire infinite band costs $O(L^3A^{-1/10})$. Thus

$$
B_3(A,S)\ll
 LA^{-5/24}e^{2\kappa\Omega}
 +L^3e^{-41\Omega/(140R)}+L^3A^{-1/10}
 \longrightarrow0.
\tag{RC4}
$$

All three terms vanish because $\Omega/\log L\to\infty$.
Equations (RC1) and (RC2) pay complete absolute coefficient errors above
$S$, rather than just at the larger whole-response cut $T$.

### Retain the exact lower head and the oscillatory middle

Let $Z_{\rm orig}(A)=2\operatorname{Re}\sum_{\gamma>0}
 m_\rho F_A(\rho)$ denote the original paired zero sum, and set

$$
Z_{\rm split}(A)=2\operatorname{Re}\left[
 \sum_{0<\gamma\le S}m_\rho F_A(\rho)
 +\sum_{S<\gamma\le T}m_\rho G_A(\rho)\right].
$$

Its contribution to $I_\psi$ is $-Z_{\rm orig}$; the approximation
there uses $-Z_{\rm split}$ with the same sign. All elementary terms
remain unchanged. Combining (RC1) with the already retained
complete absolute suffix estimate gives

$$
\sqrt A L\,|Z_{\rm orig}(A)-Z_{\rm split}(A)|
 \le(1+1/L)\left(\frac73+\frac1{4S}\right)B_3(A,S)
 +\sqrt A L\,2\sum_{\gamma>T}m_\rho|F_A(\rho)|
 \longrightarrow0.
\tag{RC5}
$$

This restores every coefficient error and every infinite height.
It reduces the range requiring exact-coefficient treatment while
preserving the actual signed oscillatory middle. Its sign, the exact
lower head, the original full sufficient Robin bound and RH remain
unproved. This asymptotic reduction does not certify a finite numerical
clock exclusion or a uniform safe margin.

## Localized complex Mellin transport of the moving middle

Reuse (RC2), (RC4) and the complete original suffix above $T$;
their density and zero-free-region proofs are not repeated. The
following application of Mellin inversion keeps the actual real
parts and multiplicities. It supplies a finite-frequency interface
to the unconditional Theorem 2 of
[Garunkštis–Sourmelidis–Steuding, version 1](https://arxiv.org/abs/2505.14228v1),
without repeating that theorem's proof or using its RH-conditional
corollary. This is a paper-level transport, with no originality or
Lean-verification claim.

Keep $A,L,S,T,B_3$ as in (RC1)–(RC5), and assume $A$ is sufficiently
large that $S\ge H$, $S\ge L\ge1$ and $L/\log S\le7$. These are
eventual conditions, not a certified numerical starting threshold.
Partition $(S,T]$ into disjoint bands $(V,W]$, where $V=2^jS$ and
$W=\min(2V,T)$. A zero at a shared endpoint belongs to exactly one
band. Every sum below retains $m_\rho$.

### Localize the kernel and pay the compensating weight

For $\rho=\beta+i\gamma$ put

$$
r=i(1/2-\rho)=\gamma+i\delta,\qquad
\delta=1/2-\beta,\qquad
f_L(r)=\frac{e^{iLr}}{r^2+1/4}.
$$

The rational coefficient from (RC2) satisfies the exact identity
$\sqrt A L P_A(\rho)=(1+1/L)f_L(r)$.
For each band set $c_{\rm loc}=3/2$, $a_V=L/V^2$ and

$$
f_V(r)=e^{-a_V(r-c_{\rm loc}V)^2}f_L(r),\qquad
h_V(v)=\frac{e^{a_V(v-c_{\rm loc}V)^2}}v,\qquad
J_V(\tau)=\sum_{V<\gamma\le W}m_\rho
 h_V(\gamma)r^{-i\tau}.
\tag{LM1}
$$

All complex powers use the principal logarithm in $\operatorname{Re}r>0$.
The kernel reconstructed with this height weight is

$$
h_V(\gamma)r f_V(r)
 =\frac r\gamma e^{E_\rho}f_L(r),\qquad
E_\rho=a_V\delta^2-2ia_V\delta(\gamma-c_{\rm loc}V).
$$

Since $|\delta|\le1/2$ and $|\gamma-c_{\rm loc}V|\le V/2$,
$|E_\rho|\le L/(4V^2)+L/(2V)\le3L/(4V)\le1$.
Using $|e^z-1|\le e|z|$ on $|z|\le1$ and $e<3$ gives

$$
\left|\frac r\gamma e^{E_\rho}-1\right|
 \le\frac{4L}V.
$$

Also $|r^2+1/4|=|\rho(1-\rho)|\ge\gamma^2$ and
$|e^{iLr}|=A^{\beta-1/2}$. Thus $\gamma\le2V$ and reflection
in $\beta=1/2$ give the complete paired approximation allowance

$$
2(1+1/L)\sum_{\text{bands}}\sum_{V<\gamma\le W}m_\rho
 |h_V(\gamma)r f_V(r)-f_L(r)|
 \le8(1+1/L)L B_3(A,S)\longrightarrow0.
\tag{LM2}
$$

The final limit uses the explicit terms of (RC4), which remain
vanishing after multiplication by $L$. This error pays both the
local Gaussian compensation and the outer $\gamma$ versus $r$
weight. No replacement $\beta=1/2$ is made.

### Absolute inversion on the actual complex zeros

Define the real-axis Mellin transform

$$
M_V(\tau)=\int_0^\infty
 e^{-a_V(u-c_{\rm loc}V)^2}\frac{e^{iLu}}{u^2+1/4}u^{i\tau}\,du.
$$

In the logarithmic coordinate the profile is $g_V(z)=e^z f_V(e^z)$.
Shift its Fourier contour to $\operatorname{Im}z=\pm\alpha_V$,
where $\alpha_V=1/V$. There are no poles in this strip and
$\cos(2/V)\ge1/2$. On either boundary line the real part of
the exponential exponent is at most

$$
-a_V\cos(2/V)u^2+b u-a_Vc_{\rm loc}^2V^2,
\qquad b\le2a_Vc_{\rm loc}V+L/V=4L/V.
$$

Completing the square bounds it by
$8L-9L/4=23L/4<6L$.
The denominator satisfies
$|u^2e^{\pm2i/V}+1/4|\ge\tfrac12(u^2+1/4)$;
the integral of $(u^2+1/4)^{-1}$ on $(0,\infty)$ is $\pi$.
Consequently

$$
|M_V(\tau)|\le2\pi e^{6L}e^{-|\tau|/V}.
\tag{LM3}
$$

The vertical contour sides vanish: near zero the logarithmic
profile is $O(e^{\operatorname{Re}z})$, and at infinity the positive
$\cos(2/V)$ gives quadratic damping. Fourier inversion and analytic
continuation therefore give

$$
f_V(r)=\frac1{2\pi r}\int_{\mathbb R}
 M_V(\tau)r^{-i\tau}\,d\tau
\qquad(|\arg r|<1/V).
$$

For every actual zero in the band,
$|\arg r|\le1/(2\gamma)\le1/(2V)$, so this inverse converges
absolutely. Define

$$
Q_V=\frac{1+1/L}{\pi}\operatorname{Re}
 \int_{\mathbb R}M_V(\tau)J_V(\tau)\,d\tau.
$$

Finite summation with multiplicity commutes with the absolute integral,
and exactly
$Q_V=2(1+1/L)\operatorname{Re}\sum_{V<\gamma\le W}
m_\rho h_V(\gamma)r f_V(r)$.

### Pay the entire frequency tail within a fixed source range

Let $n_V=\sum_{V<\gamma\le W}m_\rho$ and let $Q_{V,K}$ use
only $|\tau|\le K$. Since

$$
h_V(\gamma)\le e^{L/4}/V,\qquad
|J_V(\tau)|\le\frac{n_V e^{L/4}}V e^{|\tau|/(2V)},
$$

(LM3) pays the complete two-sided omitted frequency integral:

$$
|Q_V-Q_{V,K}|
 \le8(1+1/L)n_V e^{25L/4}e^{-K/(2V)}.
$$

Choose $K_V=20VL$. Then this allowance is
$8(1+1/L)n_V A^{-15/4}$.
The bands are disjoint, so $\sum n_V\le N_0(T)\ll T\log T$.
Using the retained $T=A^{1/4}e^{-\kappa\Omega}$ gives

$$
\sum_{\text{bands}}|Q_V-Q_{V,K_V}|
 \ll LA^{-7/2}\longrightarrow0.
\tag{LM4}
$$

Moreover $K_V/(V\log V)=20L/\log V\le140$ under the stated
eventual conditions. The positive frequencies lie within the fixed
$O(V\log V)$ range of GSS Theorem 2; its implied constants must
be those for this prescribed fixed range. Reflection preserves
$h_V(\gamma)$ and sends $r$ to $\overline r$, hence
$J_V(-\tau)=\overline{J_V(\tau)}$. This accesses negative frequencies
without assuming RH. The frequency-range statement alone supplies
no signed bound.

### Height weights, endpoint atoms and the remaining source error

For $V\le v\le W$ let
$I_V(v,\tau)=\sum_{V<\gamma\le v}m_\rho r^{-i\tau}$.
Ordinary finite partial summation yields

$$
J_V(\tau)=h_V(W)I_V(W,\tau)
 -\int_V^W h_V'(v)I_V(v,\tau)\,dv,
\qquad
|h_V'(v)|\le\frac{e^{L/4}(L+1)}{V^2}.
$$

The source uses $[V,v)$ rather than $(V,v]$. Define the exact atom
$E_z(\tau)=\sum_{\gamma=z}m_\rho r^{-i\tau}$. Then

$$
I_V(v,\tau)=I_{\rm GSS}(V,v,\tau)+E_v(\tau)-E_V(\tau).
$$

Keep these atoms in the endpoint term and in the partial-summation
integral. In that integral $E_v$ is supported on finitely many
ordinates and contributes zero as a Lebesgue integral; the lower
$E_V$ term and the upper $E_W$ term still require their exact
contributions. Equivalently, the exact weighted correction to the
source partial sum is $h_V(W)E_W(\tau)-h_V(V)E_V(\tau)$.
At $v=V$, use the empty sum. Every other pair $(V,v)$
is comparable; the whole interval $(S,T]$ is never substituted as
a comparable source interval.

Fix the independent GSS splitting parameter $c_{\rm GSS}=1/2$;
its low/high-frequency transition is $\tau=V\log2/2$.
GSS's high-frequency remainder includes

$$
e^{\tau/(2V)}
 \left((\log V)^2+(\tau/V)^2\log V\right)
 +\frac{\tau^{3/2}}V e^{\tau/(2V)-\tau/v}.
$$

Its low-frequency remainder is $O((\log V)^2)$.
Retain both, as well as the main prime sum and the exact endpoint
atoms. The elementary absolute envelope (LM3) combined with
the displayed height-weight bounds gives, for the integrated
source remainder on one band, only the coarse allowance

$$
O\!\left(A^{25/4}
 \left(L^3+V^{1/2}L\right)\right).
$$

For example the first term uses
$\int_0^\infty e^{-\tau/(2V)}
[(\log V)^2+(\tau/V)^2\log V]d\tau=O(VL^2)$;
the second uses $v\le2V$ and
$\int_0^\infty\tau^{3/2}e^{-\tau/V}d\tau=O(V^{5/2})$.
The partial-summation weight has total bound
$e^{L/4}(L+2)/V$.
There are $O(L)$ bands and $\sum\sqrt V=O(\sqrt T)$, so the
corresponding allowance for the entire middle is
$O(A^{25/4}(L^4+\sqrt T\,L))$.
This growing upper allowance does not control the desired signed
response. It is neither a lower bound for the actual remainder nor
an impossibility result for cancellation or a sharper transport.

### Restore the complete original response

Put

$$
Y(A)=\sqrt A L\,2\operatorname{Re}
 \sum_{0<\gamma\le S}m_\rho F_A(\rho)
 +\sum_{\text{bands}}Q_{V,K_V}.
$$

(RC2), (LM2), (LM4) and the retained complete original suffix give

$$
\begin{aligned}
|\sqrt A L Z_{\rm orig}(A)-Y(A)|
\le{}&\left(\frac{2(L+2)}{L^2}+8(1+1/L)L\right)B_3(A,S)\\
&+\sqrt A L\,2\sum_{\gamma>T}m_\rho|F_A(\rho)|
 +O(LA^{-7/2})\longrightarrow0.
\end{aligned}
\tag{LM5}
$$

Every actual real part, multiplicity, coefficient and height is
retained or covered by an explicit error. The contribution to
$I_\psi$ is $-Z_{\rm orig}$, so its normalized approximation is
$-Y(A)$; all elementary terms and the strict core remain unchanged.
The exact low head, the signed transformed middle and its integrated
GSS prime and error contributions are still unpaid. This interface
does not prove the full signed Robin estimate, a numerical threshold,
a uniform strict margin or RH.

## A norm floor for the local GSS absolute endpoint allowance

The local inversion permits a sharper method diagnosis than the
growing sufficient allowance displayed above. Retain exactly the
kernel, height weight and cutoff in (LM1)–(LM5), on the same bands
$S\le V<W\le\min(2V,T)$, with the same eventual
conditions. Put $\tau_0=V\log2/2$, the fixed GSS splitting point.
As in (R5)–(R7), distinguish a positive majorant allowance from the
actual signed source error. The following is a paper-level application
of the existing inverse, with no originality or Lean-verification claim.

### The actual transform has an in-range weighted norm floor

Use the analytic test point
$r_*=c_{\rm loc}V-i/2$, with $c_{\rm loc}=3/2$.
It is not an asserted zeta zero. Since $|\arg r_*|\le1/(3V)$,
the absolute inverse from (LM3) gives

$$
\int_{\mathbb R}|M_V(\tau)|e^{|\tau|/(2V)}\,d\tau
 \ge2\pi|r_*f_V(r_*)|\ge\frac{2\pi\sqrt A}{3V}.
\tag{LM6}
$$

For the last inequality write $x=c_{\rm loc}V\ge1$.
The Gaussian factor has modulus $e^{a_V/4}\ge1$ and
$|e^{iLr_*}|=\sqrt A$. Moreover

$$
\frac{|r_*|}{|r_*^2+1/4|}
 =\frac{\sqrt{x^2+1/4}}{x\sqrt{x^2+1}}
 \ge\frac1{2x}=\frac1{3V}.
$$

This uses the chosen analytic kernel at a test point, without replacing
any actual zero's real part.

The floor cannot be assigned only to frequencies outside GSS's retained
range. In the defining real-axis integral for $M_V$, split at $V/2$.
On the lower part the Gaussian is at most $A^{-1}$; on the upper
part $(u^2+1/4)^{-1}\le4/V^2$ and the complete real Gaussian
integral is $\sqrt\pi V/\sqrt L$. Thus, for every real $\tau$,

$$
|M_V(\tau)|\le\frac\pi A+\frac{4\sqrt\pi}{V\sqrt L}.
$$

Consequently the weighted norm on $|\tau|\le\tau_0$ is at most
$2\pi V/A+8\sqrt\pi/\sqrt L$. From (LM3), the entire weighted
norm beyond $K_V=20VL$ is at most

$$
\int_{|\tau|>K_V}|M_V(\tau)|e^{|\tau|/(2V)}\,d\tau
 \le8\pi V e^{6L-K_V/(2V)}=8\pi V A^{-4}.
$$

Subtract both parts from (LM6) to obtain

$$
\begin{aligned}
\int_{\tau_0<|\tau|\le K_V}|M_V(\tau)|e^{|\tau|/(2V)}\,d\tau
\ge{}&\frac{2\pi\sqrt A}{3V}-\frac{2\pi V}A
 -\frac{8\sqrt\pi}{\sqrt L}-8\pi V A^{-4}\\
\ge{}&\frac{\pi\sqrt A}{3V}
\qquad\text{eventually, uniformly for }S\le V\le T.
\end{aligned}
\tag{LM7}
$$

Indeed $\sqrt A/V\ge A^{1/4}e^{\kappa\Omega}$ grows, whereas
each subtracted bound vanishes uniformly. The source range and
negative-frequency reflection are precisely those already retained
in (LM4); no new source theorem or range calculation is required.

### The defined endpoint budget cannot tend to zero

GSS's high-frequency remainder includes the positive majorant shape
$e^{\tau/(2V)}(\log V)^2$. Define the **unit-coefficient allowance**
for its term-by-term absolute propagation through the weighted
height endpoint by

$$
\mathcal B^{\rm GSS}_V(A)=\frac{1+1/L}{\pi}
 h_V(W)(\log V)^2
 \int_{\tau_0<|\tau|\le K_V}
 |M_V(\tau)|e^{|\tau|/(2V)}\,d\tau.
$$

Since $h_V(W)\ge1/W\ge1/(2V)$, (LM7) gives

$$
\mathcal B^{\rm GSS}_V(A)
 \ge\frac{\sqrt A(\log V)^2}{6V^2}
 \ge\frac{L^2e^{2\kappa\Omega}}{294}
 \longrightarrow\infty.
\tag{LM8}
$$

Here $\log V\ge\log S\ge L/7$ and
$V\le T=A^{1/4}e^{-\kappa\Omega}$.
Multiplying the printed majorant shape by any fixed positive source
coefficient multiplies this floor by that coefficient. No numerical
value for it or effective starting threshold follows from big-$O$
notation. No unbounded sequence of selected integer sources is
asserted, nor a failure at a particular selected $A$.

This is a lower bound for the explicitly defined allowance, not for
the actual remainder, its integral, the total propagated error or a
Robin violation. The second printed source-error shape, derivative
terms and endpoint atoms retain their roles in (LM5).
Because (LM8) uses the actual transform, merely sharpening its crude
upper bound $e^{6L}$ cannot make this same absolute endpoint budget
tend to zero. Joint cancellation, stronger source information,
another kernel or a favorable bound for the combined main and exact
low head could change the budget comparison; none is excluded or
supplied here. The original full signed Robin condition and RH remain
unproved, with all coefficients, real parts, multiplicities and
height ranges unchanged.

### A shrinking strip improvement alone leaves the first-band allowance large

Retain the kernel and complete frequency range of (LM1)–(LM8).
Grant, only for this comparison, a strengthened source endpoint
majorant in which $e^{|\tau|/(2V)}$ is replaced by
$e^{(1/2-\delta(V))|\tau|/V}$, where $\delta(V)\ge0$ and
$\delta(V)\to0$. No such strengthened GSS estimate is inferred merely
from a zero-free region. Define $\mathcal B_{V,\delta}$ by this
replacement in the same unit-coefficient absolute allowance
$\mathcal B^{\rm GSS}_V$.

Since the retained range has $|\tau|\le K_V=20VL$, direct comparison
of the existing positive integrals gives

$$
\mathcal B_{V,\delta}(A)
\ge e^{-20\delta(V)L}\mathcal B^{\rm GSS}_V(A)
\ge e^{-20\delta(V)L}\frac{\sqrt A(\log V)^2}{6V^2}.
$$

On the first band, $V=S=A^{1/6}e^{-\kappa\Omega}$ and eventually
$W=2S\le T$, the already retained $\log S\ge L/7$ therefore yields

$$
\mathcal B_{S,\delta}(A)
\ge\frac{L^2}{294}
 \exp\!\left(\frac L6+2\kappa\Omega-20\delta(S)L\right)
\longrightarrow\infty.
$$

Here $S\to\infty$, $\delta(S)\to0$ and $\Omega=o(L)$.
For example, the existing gap $\delta(V)=\eta(2V)$ from the
Vinogradov–Korobov input above has these properties. Thus even granting
this exponential improvement, while retaining the other endpoint
prefactors, cannot make the same independently absolute allowance
uniformly bounded on all middle bands. Any fixed positive source
coefficient preserves the conclusion.

This is a direct application of (LM8), not a new norm, density or
zero-free theorem. The lower bound concerns only the defined
allowance; it is not a lower bound for the actual remainder, a Robin
violation or a failure at a certified numerical clock. Additional
prefactor savings, joint signed cancellation, other kernels or a
favorable combined head/main bound retain their roles. The original
complete signed estimate and RH remain unproved.

### Actual zero jumps obstruct a uniform inverse-height prefactor

The classical jump principle gives a further application boundary for
the retained source interface. Reuse GSS Theorem 2, printed p.3 of
[arXiv:2505.14228v1](https://arxiv.org/pdf/2505.14228v1), and its
Riemann–von Mangoldt inputs (3)–(4), printed p.2. No source proof is
repeated. This evaluates a proposed strengthening of that particular
interface; it is not a mathematical originality claim or an improved
Robin estimate.

With the source's half-open convention, write

$$
I(V,v,\tau)=\sum_{V\le\gamma<v}m_\rho r_\rho^{-i\tau},
\qquad r_\rho=\gamma+i(1/2-\beta),
$$

and retain its complete high-frequency main term

$$
P(V,v,\tau)=
\frac{e^{i(\tau+\pi/4)}\tau^{1/2-i\tau}}{\sqrt{2\pi}}
\sum_{e^{\tau/v}\le n\le e^{\tau/V}}
\frac{\Lambda(n)(\log n)^{i\tau}}{n^{1/2}\log n}.
$$

Here sums over $\rho$ list distinct zeros and attach their actual
multiplicities $m_\rho$. Suppose one attempted to strengthen only the
first printed error shape by a factor $V^{-1}$, leaving the main term
and second shape unchanged:

$$
|I(V,v,\tau)-P(V,v,\tau)|
\le C\left[
 V^{-1}e^{\tau/(2V)}
 \left((\log V)^2+(\tau/V)^2\log V\right)
 +\frac{\tau^{3/2}}{V}e^{\tau/(2V)-\tau/v}
\right].
\tag{JP1}
$$

The proposed $C$ is fixed and uniform in $v,\tau$ on the same
comparable-height source range, including
$21V/20<v<6V/5$ and the frequencies used below. Such a uniform
strengthening cannot hold, unconditionally and even under RH.

For every sufficiently large $V$, the cited count gives an actual
zero ordinate $\Gamma\in(21V/20,23V/20)$. Choose

$$
\frac74V\log V<\tau<\frac74V\log V+V
$$

outside the finitely many values $\Gamma\log n$ in this interval.
Then $P(V,v,\tau)$ is locally constant as $v$ crosses $\Gamma$:
its lower cutoff crosses no integer there, and its upper cutoff and
coefficients are independent of $v$. The frequency lies in the
printed fixed $O(V\log V)$ regime. For $S\le V\le T$ it also lies
below the retained $K_V=20VL$ eventually, using the existing scale
relations, without changing that frequency range.

By contrast, the two one-sided values of $I$ differ by the exact atom

$$
J_\Gamma(\tau)=\sum_{\Im\rho=\Gamma}
 m_\rho\bigl(\Gamma+i(1/2-\beta)\bigr)^{-i\tau}.
$$

The actual functional-equation reflection
$\rho\mapsto1-\overline\rho$ preserves this ordinate and
multiplicity and sends $r_\rho$ to $\overline r_\rho$.
For a reflected noncritical pair, with the usual logarithm in the
right half-plane, its contribution is

$$
m_\rho(r^{-i\tau}+\overline r^{-i\tau})
=2m_\rho\cosh(\tau\arg r)\,e^{-i\tau\log|r|}.
$$

A critical-line zero is counted once, with its original
multiplicity and phase $e^{-i\tau\log\Gamma}$. Since
$|1/2-\beta|<1/2$, every reflected pair has phase displacement
from this central phase at most

$$
0\le\tau\log(|r|/\Gamma)
\le\frac{\tau}{8\Gamma^2}
=O(\log V/V).
$$

Choose $k\in\{0,1,2,3\}$ so that the central phase after
multiplication by $i^k$ is within $\pi/4$ of the positive real axis.
Eventually every pair and critical-line contribution is within
$\pi/3$, and $2\cosh(\tau\arg r)\ge2$. Therefore

$$
\operatorname{Re}\bigl(i^kJ_\Gamma(\tau)\bigr)
\ge\frac12\sum_{\Im\rho=\Gamma}m_\rho\ge\frac12.
\tag{JP2}
$$

The four phases here are output observation directions. This
projection does not assert a new intertwining between the FIB
operators $M,J,C=MJ$ and the actual zeta spectrum.

For $v$ on either side sufficiently close to $\Gamma$, take
$v\le6V/5$. The two proposed majorants in (JP1) satisfy

$$
V^{-1}e^{\tau/(2V)}
 \left((\log V)^2+(\tau/V)^2\log V\right)
=O\!\left(V^{-1/8}(\log V)^3\right),
$$

$$
\frac{\tau^{3/2}}V e^{\tau/(2V)-\tau/v}
=O\!\left(V^{-1/12}(\log V)^{3/2}\right).
$$

Both tend to zero, uniformly in this neighborhood. A locally
constant main and two vanishing one-sided residuals cannot produce
the nonvanishing jump (JP2). More explicitly, one of the actual
one-sided residual magnitudes is at least $|J_\Gamma|/2\ge1/4$.
This contradicts (JP1) for any fixed $C$. The conclusion also rules
out a still smaller first shape obtained by combining this factor
$V^{-1}$ with a nonnegative exponential reduction $\delta(V)$.

The preceding allowance comparison separately shows why this
restricted prefactor question matters. If its first shape alone
were multiplied by $V^{-p}$, with fixed $p\ge0$ and
$\delta(V)\to0$, its defined first-band allowance would have the
lower bound

$$
S^{-p}\mathcal B_{S,\delta}(A)
\ge\frac{L^2}{294}
 \exp\!\left(
 \frac{1-p}{6}L+(2+p)\kappa\Omega-20\delta(S)L
 \right).
\tag{JP3}
$$

For every fixed $p<1$ this diverges. Thus a uniform pure
inverse-height-power repair of the first shape cannot supply the
required bounded independent allowance: powers below one retain
this allowance floor, while powers at least one encounter the
actual-jump obstruction. This is not a sufficiency equivalence;
the unchanged second shape and all other terms still matter.

The lower bound $1/4$ concerns the actual pointwise residual near
the chosen zero jumps, not its signed Mellin integral or its
height-weighted integral. Restricted parameter ranges, smoothing,
explicit atomic main terms, joint signed cancellation and other
kernels can escape this particular model. Keep the exact endpoint
atoms in (LM5), the actual real parts and multiplicities, the
original rational coefficient, the low head and all heights. The
complete signed Robin estimate and RH remain unproved. These
application calculations are paper-level and have no Lean
verification or certified numerical starting clock.

### Scope of the Gaussian single-zero-sum formula

Kamiya–Suzuki, *An asymptotic formula for a sum involving zeros of
the Riemann zeta-function*, Publications de l'Institut Mathématique
76(90) (2004), 81–88,
[DOI 10.2298/PIM0476081K](https://doi.org/10.2298/PIM0476081K),
[primary text](http://elib.mi.sanu.ac.rs/files/journals/publ/96/n090p081.pdf),
studies

$$
H(u,v)=\sum_\rho e^{u\rho^2-v\rho}.
$$

Theorem 1.1 is unconditional and retains actual zero real parts and
multiplicities. Its $u\downarrow0$ resonance estimates at
$v=\pm\log m$ have constants depending on the fixed integer $m>2$;
its off-resonance estimates are uniform on fixed closed intervals
contained in the positive or negative half-line and avoiding the
corresponding prime-power logarithms. These intervals exclude zero.
Neither statement
supplies uniform control when the frequency parameter grows with $A$.
The subsequent RH specialization is an illustration, not a hypothesis
of the theorem.

Lemma 2.1 gives the exact Gaussian explicit formula for every $u>0$
and real $v$. It is a special case of Weil's formula, already available
as an interface. Lemma 3.1 bounds its real convolution residual between
zero and one; this does not bound the complete prime and archimedean
contributions.

For the localized kernel above, put $a=L/V^2$, $c=3/2$ and
$r=i(1/2-\rho)$. Its numerator has the exact parameter correspondence

$$
e^{-a(r-cV)^2+iLr}
=e^{a/4-L/2+iacV-ac^2V^2}
 e^{a\rho^2-v_V\rho},\qquad
v_V=a-L+2iacV.
$$

Here $v_V$ is complex, while the printed lemma takes real $v$.
Analytic continuation of an identity alone supplies no uniform signed
estimate in this moving parameter range. The rational denominator
$r^2+1/4=\rho(1-\rho)$, the height restrictions and the compensating
weight $h_V(\gamma)$ also remain to be transported. Thus the printed
Gaussian results do not pay the signed middle, its combined prime and
error contribution, or the exact low head in (LM5). They are reused
within their stated scope, without excluding a future weighted
application or establishing the original Robin bound or RH.

### A real-parameter heat integral transports the rational high response

The exact real-parameter formula of Kamiya–Suzuki, Lemma 2.1, can
also be used with a different kernel. Keep the original selected
integer, $A,L,S$ and complete coefficient $F_A$. Reuse (RC2)–(RC4),
the reciprocal-square zero count and the printed Gaussian formula;
their source proofs are not repeated. This application pays a
transport error, not the sign of the resulting prime expression.
It makes no mathematical originality or Lean-verification claim.

Put

$$
u_*=\frac{L}{S^2},\qquad
\mathcal H(u,v)=\sum_\rho m_\rho e^{u\rho^2-v\rho},\qquad
\mathcal H_{\le S}(u,v)=
 \sum_{|\operatorname{Im}\rho|\le S}m_\rho e^{u\rho^2-v\rho}.
$$

These sums list distinct nontrivial zeros, with their actual
multiplicities. Both conjugate signs of the ordinate are included.
The head includes every zero at the cut. Work eventually with
$L\ge2$, $S\ge H$ and $u_*\le1/16$; no numerical starting clock is
certified. The head below $S$ includes unverified heights above $H$
and is retained exactly.

For an actual $\rho=\beta+i\gamma$,
$\operatorname{Re}[\rho(1-\rho)]=\gamma^2+\beta(1-\beta)>0$.
Consequently the elementary scalar resolvent identity gives

$$
\frac{A^{\rho-1/2}}{\rho(1-\rho)}
=A^{-1/2}\int_0^\infty
 e^{u\rho^2-(u-L)\rho}\,du.
\tag{HR1}
$$

The Gaussian parameter $v=u-L$ is real throughout. No continuation
of the printed lemma to complex $v$ is needed. Its fixed-parameter
asymptotic theorem is not used in this moving range.

For $|\gamma|>S$, the modulus of the normalized integrand in
(HR1) is at most $\sqrt A e^{-u\gamma^2}$. Thus summation and
integration are absolutely interchangeable, since
$\sum_{\gamma>S}m_\rho/\gamma^2\ll\log S/S$. The entire discarded
heat-time suffix, still summing every zero height, has allowance

$$
\begin{aligned}
A^{-1/2}\int_{u_*}^\infty
 \sum_{|\gamma|>S}m_\rho
  |e^{u\rho^2-(u-L)\rho}|\,du
&\le2\sqrt A\,e^{-u_*S^2}
 \sum_{\gamma>S}\frac{m_\rho}{\gamma^2}\\
&\ll A^{-1/2}\frac{\log S}{S}\longrightarrow0.
\end{aligned}
\tag{HR2}
$$

Here $e^{-u_*S^2}=A^{-1}$. This truncates heat time, not the zero
height range. In particular every zero above the previously paid
whole-response cut $T$ is included before this bound is applied.

Write

$$
\mathcal G_u(t)=\frac{e^{-t^2/(4u)}}{\sqrt{4\pi u}},
\qquad
\mathcal D_{A,u_*}=A^{-1/2}\int_0^{u_*}
 \left[A-\sum_{n\ge2}\Lambda(n)
       \mathcal G_u(\log n-L+u)\right]du.
\tag{HR3}
$$

The pole is centered at the same arithmetic clock as the primes.
Indeed the continuous background is exactly

$$
\int_0^\infty\mathcal G_u(\log x-L+u)\,dx=A.
$$

Retain this difference as a combined signed expression; its
definition gives no estimate for its sign or size. The integrated
prime terms are not replaced by an average over other clocks.

At $v=u-L$, the two pole terms in the literal source formula are
$A+1$. Its first prime sum is precisely the one in (HR3). Its
remaining terms contribute a vanishing allowance after multiplying
by $A^{-1/2}$ and integrating over $0<u<u_*$. To see this using
only the printed interfaces, its logarithmic archimedean term becomes

$$
\frac{e^{-u/4}}{2\pi}\int_{\mathbb R}
 \log|1/4+it/2|\,e^{-ut^2+itL}\,dt.
$$

Since $|\log|1/4+it/2||\ll\log(2+|t|)$, its complete absolute
integral over heat time is

$$
O\!\left(\int_0^{u_*}u^{-1/2}\log(2/u)\,du\right)
=O\!\left(\sqrt{u_*}\log(2/u_*)\right)
\longrightarrow0.
$$

The source's Lemma 3.1 gives
$0\le(E*\mathcal G_u)(u-L)\le1$. Its convolution term and the
constant pole $1$ together cost at most $2A^{-1/2}u_*$.
The $\log\pi$ term and the second prime sum have allowance

$$
O\!\left(A^{-1/2}\sqrt{u_*}
           e^{-L^2/(16u_*)}\right).
$$

For the second sum this follows from $L-u\ge L/2$ and
$(L-u)/(2u)\ge1$:

$$
\sum_{n\ge2}\frac{\Lambda(n)}n
 e^{-(u-L-\log n)^2/(4u)}
\le e^{-L^2/(16u)}
     \sum_{n\ge2}\frac{\log n}{n^2},
$$

where the last series is finite. All these terms retain the signs
and coefficients of Lemma 2.1; only their absolute propagation
is bounded. Because $S=A^{1/6}e^{-\kappa\Omega}$,
$\sqrt{u_*}\log(2/u_*)=O(L^{3/2}/S)\to0$.

No endpoint value at $u=0$ is substituted. For each fixed $A$,
the Gaussian zero sum is integrable on this finite heat interval:
the reciprocal-square count controls its high part, and its head is
finite. All other source terms just bounded are integrable there.
The nonnegative first prime sum is consequently integrable by the
exact source identity; Tonelli then permits its prime summation and
heat integral to be interchanged. This includes the case where $A$
is exactly a prime power, without importing fixed-resonance
asymptotics. Integrating the two pole terms separately to infinite
heat time would diverge and is not used.

Define the exact combined head

$$
\mathcal J_{\rm head}(A)=
 \sqrt A L\,2\operatorname{Re}
      \sum_{0<\gamma\le S}m_\rho F_A(\rho)
 -(1+1/L)A^{-1/2}\int_0^{u_*}
      \mathcal H_{\le S}(u,u-L)\,du.
\tag{HR4}
$$

The finite subtraction belongs to the same zero multiset and
clock; it is not an independently optimized head allowance.
Combining (HR1)–(HR4) with the single coefficient comparison (RC2)
gives the complete original response

$$
\boxed{
\sqrt A L\,Z_{\rm orig}(A)
=\mathcal J_{\rm head}(A)
 +(1+1/L)\mathcal D_{A,u_*}+o(1).}
\tag{HR5}
$$

More precisely, the absolute discrepancy is at most

$$
\frac{2(L+2)}{L^2}B_3(A,S)
 +O\!\left(
 A^{-1/2}\frac{\log S}{S}
 +\sqrt{u_*}\log(2/u_*)
 +A^{-1/2}u_*
 +A^{-1/2}\sqrt{u_*}e^{-L^2/(16u_*)}
 \right),
\tag{HR6}
$$

which tends to zero by the already retained (RC4). All actual real
parts, conjugate and reflected multiplicities, original coefficient
errors and infinite zero heights are covered. No complex-v
extension, GSS pointwise remainder or independent GSS endpoint
allowance is used in this alternative transport.

The nontrivial-zero contribution to the original $I_\psi$ is still
$-Z_{\rm orig}$. Paying (G9) through (HR5) requires an upper bound for
its combined right side, plus the positive elementary correction $r_A$
defined after (G9) and an allowance for the signed discrepancy (HR6).
The strict core at the same integer remains the one already proved.
Neither $\mathcal D_{A,u_*}$ nor $\mathcal J_{\rm head}$ is bounded
here by the required margin. In particular the head subtraction
does not establish positivity or an estimate for the unverified
head. The full original Robin bound and RH remain unproved.

### The heat prime response has a paid finite arithmetic window

The positive kernel in (HR3) permits an unconditional localization
of its prime sum. This uses only $\Lambda(n)\le\log n$, the
Gaussian bound below and the same $A,L,S,u_*$. It is an application
estimate for this profile, not a new prime-distribution theorem,
an originality claim or a Lean-verified result.

For $0<U\le1/16$ and $d\in\mathbb R$, put

$$
K_U(d)=\int_0^U\mathcal G_u(d+u)\,du.
$$

Expanding the square inside the Gaussian gives

$$
0\le K_U(d)
=e^{-d/2}\int_0^U
 \frac{e^{-d^2/(4u)-u/4}}{\sqrt{4\pi u}}\,du
\le\sqrt{U/\pi}\,e^{-d/2}e^{-d^2/(4U)}.
\tag{HR7}
$$

For $A\ge e^2$, $L=\log A$ and any $D>0$, split the last
Gaussian exponent into two equal parts. On $|d|>D$ one part is
at most $e^{-D^2/(8U)}$. Consequently

$$
\sum_{|\log(n/A)|>D}\Lambda(n)K_U(\log(n/A))
\ll\sqrt U\,e^{-D^2/(8U)}\sum_{n\ge2}f_{A,U}(n),
$$

where

$$
f_{A,U}(x)=\log x\,(A/x)^{1/2}
 \exp\!\left[-\frac{(\log x-L)^2}{8U}\right],\qquad x\ge1.
$$

This nonnegative function vanishes at $1$ and at infinity and
has just one maximum. Indeed, for $t=\log x>0$, its logarithmic
derivative with respect to $t$ is
$1/t-1/2-(t-L)/(4U)$, which is strictly decreasing from positive
infinity to negative infinity. The elementary unimodal
sum–integral comparison therefore gives

$$
\sum_{n\ge2}f_{A,U}(n)
\le\int_1^\infty f_{A,U}(x)\,dx
    +2\sup_{x\ge1}f_{A,U}(x).
$$

Write $d=\log x-L$. Completing the square first with
$e^{-d/2}$ and then with $e^{d/2}$ gives, uniformly in the stated
parameters,

$$
\sup_{x\ge1}f_{A,U}(x)
\le e^{U/2}(L+2U+2\sqrt U)\ll L+1,
$$

$$
\begin{aligned}
\int_1^\infty f_{A,U}(x)\,dx
&\le A e^{U/2}\int_{\mathbb R}
 (L+|d|)e^{-(d-2U)^2/(8U)}\,dd\\
&\ll A\sqrt U(L+1).
\end{aligned}
$$

These comparisons account for the integer grid as well as the
continuous background. Combining them with (HR7) proves the
complete positive arithmetic tail bound

$$
\boxed{
\sum_{|\log(n/A)|>D}\Lambda(n)K_U(\log(n/A))
\ll (L+1)(AU+\sqrt U)e^{-D^2/(8U)}.}
\tag{HR8}
$$

No prime powers outside the displayed window are dropped before
this bound is applied, and no prime-counting asymptotic or average
over $A$ is assumed.

Now use the same $U=u_*=L/S^2$ as (HR1)–(HR6), and take

$$
D_*=4\sqrt{u_*L}=\frac{4L}{S},\qquad
\mathcal W_A=\{n\ge2:Ae^{-D_*}\le n\le Ae^{D_*}\}.
$$

Keep both endpoints in this finite window. Define

$$
\mathcal D^{\rm loc}_{A,u_*}
=A^{-1/2}\left[
 Au_*-\sum_{n\in\mathcal W_A}\Lambda(n)
       K_{u_*}(\log(n/A))\right].
$$

Since $e^{-D_*^2/(8u_*)}=A^{-2}$, (HR8) yields

$$
0\le\mathcal D^{\rm loc}_{A,u_*}-\mathcal D_{A,u_*}
\ll(L+1)\left(\sqrt A\,u_*+
 \frac{\sqrt{u_*}}{\sqrt A}\right)A^{-2}
\longrightarrow0.
\tag{HR9}
$$

The direction is relevant to Robin: removing the outside positive
prime terms increases $\mathcal D$, hence gives an upper estimate
for its contribution to $Z_{\rm orig}$ and a lower estimate for
the corresponding contribution $-Z_{\rm orig}$ to $I_\psi$.
The separate bound in (HR9) also pays the absolute discrepancy.
Together with (HR5)–(HR6), it gives

$$
\sqrt A L\,Z_{\rm orig}(A)
=\mathcal J_{\rm head}(A)
 +(1+1/L)\mathcal D^{\rm loc}_{A,u_*}+o(1),
\tag{HR10}
$$

with no discarded zero heights or unpaid arithmetic tail.

The relative log window $D_*=4L/S$ tends to zero. Its continuous
arithmetic width is asymptotic to $8AL/S$; this is a window at
$A=\log N$, not a window at the original integer $N$. The weighted
prime-power sum within it is still not estimated by the required
signed margin. Nor is the exact unknown head in (HR4) paid by
localization. The original selected-source joint estimate, strict
core, all actual real parts and multiplicities remain unchanged,
and RH remains unproved. All limits are eventual, with no
certified numerical starting clock.

## Whole multiplicative sums do not control prescribed prime blocks

Granville–Lamzouri, *Large values of exponential sums with
multiplicative coefficients*,
[arXiv:2604.02306v1](https://arxiv.org/pdf/2604.02306v1),
Corollary 1.1 and Example 1.2, printed pp.5–6, give a useful one-way
interface. Write $e(t)=\exp(2\pi it)$ and

$$
S_f(x,\alpha)=\sum_{n\le x}f(n)e(\alpha n),\qquad
f:\mathbb N\to\{z:|z|\le1\}\text{ multiplicative}.
$$

For fixed $\epsilon\in(0,1/10)$, Corollary 1.1 assumes
$|\alpha-a/q|\le1/(qx)$, $(a,q)=1$ and
$(\log x)^{2+\epsilon}\le q\le x/(\log x)^{3+\epsilon}$.
An inequality $|S_f(x,\alpha)|\ge cx/\log x$, with fixed
$c\in(0,1)$, forces a dyadic prime sum with large modulus for some
positive integer harmonic $h\ll c^{-2}\log(1/c)$ and a block location
$c^2x/\log(1/c)\ll z\le x/(2h)$. This is an existential conclusion,
not a bound for a prescribed prime block.

The source's Example 1.2 supplies a completely multiplicative $f$
with $|f|\le1$, a cutoff $y\sim3x/4$, $z=y/2$ and
$\delta\in\{0,1\}$ such that

$$
S_f(x,\alpha)=e(\alpha)+\delta,\qquad
\sum_{z<p\le2z}f(p)e(\alpha p)\sim\frac{x}{4\log x}.
$$

Thus multiplicativity and cancellation of the whole integer sum alone
do not imply cancellation of each prime block. This printed
counterexample is reused directly; it concerns the source's selectable
coefficients, not a counterexample for the actual
$\Lambda(n)n^{-it}$ Gaussian response.

The actual von Mangoldt weight is not multiplicative:
$\Lambda(6)=0$ while $\Lambda(2)\Lambda(3)>0$; multiplication by a fixed
nonzero scalar preserves that obstruction. Putting $n^{-it}$ into an
admissible multiplicative coefficient instead leaves the prime support,
$\Lambda$ weight, Gaussian cutoff and signed transport to be justified.
Corollary 1.1 supplies no such bridge or original-kernel estimate.
The same selected integer, complete rational coefficient, actual zero
real parts and multiplicities, exact low head and all remaining height
ranges therefore retain their roles in (LM5) and (G9). The required
joint signed estimate and RH remain unproved.


### The same-source price minimum gives a nonnegative heat cost

The existing unrestricted price pressure and selected-source contact
can be transported into the real heat kernel (HR7). This application
identifies the direction and scale of the resulting constraint. It
reuses the pressure, derivative and limit in the
[FIB theory volume, §98](../../docs/develop/theory/FIBONACCI_ATOMIC_RELATION_GENERATION.md),
the actual tangent optimum (G1), and (HR1)–(HR10). It does not
reprove those results or the
[packet and cone theorems](../Analytic/mantovanelli2026primeworkload.md).
No mathematical originality or Lean verification is claimed.

Keep the same conditional least global Robin-ratio maximizer $N>5040$,
$A=\log N$, $L=\log A$ and $U=L/S^2$. Write

$$
g(x)=\frac1{x\log x},\qquad
q(x)=-g'(x)=\frac{\log x+1}{x^2(\log x)^2},
$$

$$
\mathcal B(\epsilon)=\max_{m\ge1}
 \{\log Z(m)-\epsilon\log m\},\qquad
\mathcal P(x)=\gamma+\log\log x-g(x)x-\mathcal B(g(x)).
$$

Here $\mathcal P$ is the existing $\mathfrak D$, and $q$ is its
positive derivative weight, not the price. Let
$a_C(x)=\log C_x$ for an unrestricted optimum at price $g(x)$;
ties may use either consistent prefix convention. Local finiteness
of activation events and the existing pressure derivative give

$$
\mathcal P'(x)=q(x)[x-a_C(x)]\quad\hbox{almost everywhere},
\qquad \mathcal P(x)\longrightarrow0.
$$

The selected $N$ attains the optimum at $g(A)$, so
$\mathcal P(A)=\gamma+\log\log A-\log Z(N)$.
Choose a fixed $x_0>1$ such that every optimum for $x\ge x_0$
exceeds $5040$; it suffices that the first thirteen $2$-layers
are strictly active. The actual global Robin maximum and the
concavity tangent for $b(t)=\gamma+\log\log t$ imply

$$
0\le\mathcal P(x)-\mathcal P(A)\le c_A(x)
\quad(x\ge x_0),\qquad
c_A(x)=\log\log x-\log\log A+g(x)(A-x).
\tag{PH1}
$$

For the lower inequality use the Robin comparison at this same
$C_x$ and $b(a_C)\le b(x)+g(x)(a_C-x)$.
For the upper inequality insert the same $N$ as a competitor in
$\mathcal B(g(x))$. Concavity gives $c_A(x)\ge0$ for all $x>1$.
The global comparison does not cover optima at most $5040$;
their fixed interval is paid below, not included in (PH1).

#### A positive kernel row with the correct atom

Put $\ell=\log x$, $d=\log(x/A)$ and
$a(\ell)=\ell^2/(\ell+1)$. The integrated Gaussian obeys, in
the distributional sense on the $d$-line,

$$
K_U''(d)+K_U'(d)=\mathcal G_U(d+U)-\delta_0(d).
$$

Indeed, this is the heat equation integrated over $0<u<U$;
the initial Gaussian is a unit atom. Its one-sided derivatives are

$$
K_U'(d)=
\begin{cases}
 \tfrac12e^{-d}\operatorname{erfc}((-d+U)/(2\sqrt U)),&d<0,\\
 -\tfrac12e^{-d}\operatorname{erfc}((d-U)/(2\sqrt U)),&d>0.
\end{cases}
$$

Thus the derivative jumps by $-1$ at $0$. Define

$$
h(x)=x\,a(\ell)K_U'(d),\qquad
r(x)=a(\ell)\mathcal G_U(d+U)+a'(\ell)K_U'(d).
$$

Using one-sided values at $A$ gives the exact row identity

$$
dh=r(x)\,dx-Aa(L)\delta_A,
\qquad
\pi_{A,U}(dx)=\frac{r(x)}{Aa(L)}\,dx.
\tag{PH2}
$$

The atom has coefficient $Aa(L)$, including the Jacobian
$\delta_0(\log(x/A))=A\delta_A(x)$.
For $d<0$ every term in $r$ is nonnegative. For $d>0$ put
$t=(d-U)/(2\sqrt U)\ge-1/8$, using $U\le1/16$. Then

$$
\frac{-K_U'(d)}{\mathcal G_U(d+U)}
 =\sqrt{\pi U}\,e^{t^2}\operatorname{erfc}(t)
 \le5\sqrt U.
$$

For $t\ge0$ use $e^{t^2}\operatorname{erfc}(t)\le1$;
for $-1/8\le t<0$ use $\operatorname{erfc}(t)\le2$ and
$e^{t^2}\le e^{1/64}$. Since $x>A$, $L\ge2$ and

$$
\frac{a(\ell)}{a'(\ell)}
 =\frac{\ell(\ell+1)}{\ell+2}\ge\frac32
 >5\sqrt U,
$$

we again have $r\ge0$. Moreover $h(1+)=h(\infty)=0$;
the Gaussian decay controls the latter endpoint. Integrating
(PH2) therefore gives $\int_1^\infty r(x)\,dx=Aa(L)$.
Consequently $\pi_{A,U}$ is an actual nonnegative probability
measure on $(1,\infty)$, formed from the same $A$ and kernel.
It is not an average over independently selected extremal integers.

#### The arithmetic correction vanishes at the paid heat scale

Write $\Delta(x)=\psi(x)-a_C(x)$, so

$$
\psi(x)-x=-\frac{\mathcal P'(x)}{q(x)}+\Delta(x).
$$

Only a crude uniform activation estimate is needed here.
The first active prime layer differs from the cutoff $p\le x$
only for $x-1<p\le x$: use
$1/(p+1)<\log(1+1/p)<1/p$ in the activation rule.
Every active higher layer satisfies $p^j\log p<x\log x$,
so there are $O(\log x)$ layers and all their primes lie below
$\sqrt{x\log x/\log2}$. With the elementary
$\vartheta(t)\le t\log t$, the higher layers of $a_C$ and
$\psi$ give the uniform bound

$$
|\Delta(x)|\ll\sqrt x\,[\log(2x)]^{5/2}\qquad(x>1).
$$

This estimate follows from activation, not from imposing GA1
on every intervening CA prefix. In particular it uses neither
a new source-selector theorem nor a square-root PNT error.
For $d\ne0$, differentiating the integral defining $K_U$ and
taking absolute values gives the almost-everywhere estimate

$$
e^{d/2}|K_U'(d)|
\le\int_0^U
 \left(\frac{|d|}{2u}+\frac12\right)
 \mathcal G_u(d)e^{-u/4}\,du.
$$

Gaussian moments and $0<U\le1/16$ therefore imply

$$
\int_{\mathbb R}e^{d/2}(1+|d|)^{5/2}|K_U'(d)|\,dd
 \ll\sqrt U.
$$

At $d=0$ use the one-sided jump in (PH2); differentiation under
the integral there does not supply either one-sided derivative.

After $x=Ae^d$, the complete arithmetic correction satisfies

$$
A^{-1/2}\left|\int_1^\infty\Delta(x)
 \frac{K_U'(\log(x/A))}{x}\,dx\right|
\ll(L+1)^{5/2}\sqrt U
=O(L^3/S)\longrightarrow0.
\tag{PH3}
$$

All actual prime powers are present in this comparison. No
fixed-beta or zero-height simplification is made.

#### Exact direction and the remaining upper requirement

Stieltjes integration by parts in (HR3), including the interval
$0<x\le1$, yields

$$
\mathcal D_{A,U}=A^{-1/2}
 \left[\int_0^1K_U(\log(x/A))\,dx-K_U(-L)
 +\int_1^\infty(\psi(x)-x)
   \frac{K_U'(\log(x/A))}{x}\,dx\right].
$$

The first two terms have allowance
$O(\sqrt U e^{-L^2/(4U)})$ by (HR7).
For the pressure term, $1/(xq(x))=xa(\ell)$, so
integration by parts with (PH2) gives

$$
-A^{-1/2}\int_1^\infty\mathcal P'(x)h(x)\,dx
=\sqrt A\,a(L)\left[\int\mathcal P(x)\,\pi_{A,U}(dx)
 -\mathcal P(A)\right].
$$

There are no pressure atoms at activation events: the existing
pressure is continuous and locally absolutely continuous.
Near $1$, $\mathcal B(g(x))=0$ and
$\mathcal P(x)=\gamma+\log\ell-1/\ell$, while
$a(\ell)=O(\ell^2)$ and $a'(\ell)=O(\ell)$.
These facts justify the lower boundary and integrability.
At infinity reuse $\mathcal P(x)\to0$ and Gaussian decay.

Set the independently nonnegative cost

$$
V_{A,U}=\int_{x_0}^\infty
 [\mathcal P(x)-\mathcal P(A)]\,\pi_{A,U}(dx)\ge0.
$$

The omitted fixed interval $1<x<x_0$ costs at most
$O_{x_0}(U^{-1/2}e^{-(L-\log x_0)^2/(4U)})=o(1)$
after multiplying by $\sqrt A a(L)$. To obtain this bound,
use the preceding integrability at $1$, boundedness of
$\mathcal P(A)$ from its existing limit, and the negative-$d$
derivative formula. No small-prefix Robin comparison is used.
Together with (PH3), this proves the specific transport

$$
\boxed{\mathcal D_{A,U}=\sqrt A\,a(L)V_{A,U}+o(1).}
\tag{PH4}
$$

Combining with (HR5)–(HR10) retains the exact same-source head:

$$
\boxed{\sqrt A L Z_{\rm orig}
 =\mathcal J_{\rm head}
  +(1+1/L)\sqrt A\,a(L)V_{A,U}+o(1).}
\tag{PH5}
$$

All actual zero real parts, multiplicities and heights remain
as specified in those equations. In particular the unknown
head above the verified height is not paid by (PH4).

The existing support gap in (PH1) does give an upper allowance,
but not one of Robin strength. Since $c_A(A)=0$ and
$c_A'(x)=q(x)(x-A)$, (PH2) and integration by parts give

$$
\begin{aligned}
0\le\sqrt A\,a(L)V_{A,U}
&\le\sqrt A\,a(L)\int_1^\infty c_A(x)\,\pi_{A,U}(dx)\\
&=A^{-1/2}\left[\int_1^\infty K_U(\log(x/A))\,dx
 -(A-1)K_U(-L)\right]\\
&\le\sqrt A\,U
=L A^{1/6}e^{2\kappa\Omega}.
\end{aligned}
\tag{PH6}
$$

The final normalization uses the already fixed
$S=A^{1/6}e^{-\kappa\Omega}$.
The displayed allowance diverges. This is not a lower bound
on the actual cost and does not rule out a sharper joint estimate.
It is the same ceiling obtained by merely dropping positive
prime terms in (HR3); the price constraint has not improved it.

Thus the price minimum supplies $\mathcal D_{A,U}\ge-o(1)$.
To apply (G9), retain the elementary correction $r_A>0$ defined there.
Let $\varepsilon_{\rm PH5}(A)$ be the signed discrepancy in (PH5),
so $\varepsilon_{\rm PH5}(A)=o(1)$ by (HR6), (PH3) and the fixed-prefix
allowance. The exact complete response is

$$
-\sqrt A L\,I_\psi(A)
=\mathcal J_{\rm head}
 +(1+1/L)\sqrt A\,a(L)V_{A,U}
 +r_A+\varepsilon_{\rm PH5}(A).
$$

Consequently the remaining joint target, equivalent to (G9), is

$$
\mathcal J_{\rm head}
 +(1+1/L)\sqrt A\,a(L)V_{A,U}
 +r_A+\varepsilon_{\rm PH5}(A)\le\mathcal E(L).
$$

For any proved allowance $\delta(A)\ge|\varepsilon_{\rm PH5}(A)|$,
a sufficient upper estimate is

$$
\mathcal J_{\rm head}
 +(1+1/L)\sqrt A\,a(L)V_{A,U}
 \le\mathcal E(L)-r_A-\delta(A).
$$

The absolute allowance is sufficient, not necessary. Its constants
have not been numerically certified at the selected finite clock.
A vanishing discrepancy alone does not establish (G9) without enough
signed slack; the strict core remains the one already proved.
No such bound, numerical starting clock, unbounded sequence of
selected sources, or proof of RH is established here. The
nonnegative quantity is independently constructed; naming it
does not prove that its size fits the available Robin budget.

## An unconditional primary source already contains the full response coefficient

Akatsuka, *Maximal order for divisor functions and zeros of the Riemann
zeta-function*, [arXiv:2411.19259v1](https://arxiv.org/abs/2411.19259v1),
Proposition 4.4, printed p.15, supplies an unconditional explicit formula
at divisor-weight exponent $1$. Write $\nu$ for the paper's $\kappa$;
this exponent is distinct from the moving-cut constant used above.
This application reuses that proposition and the project's existing
finite-tail identity; it does not reprove the explicit formula or claim
new mathematical content. The selected source statements, exponential
integral convention and parameter correspondence were inspected, not
the complete source proofs or a Lean implementation.

Let $P(X)=\sum_{2\le n\le X}\Lambda(n)/(n\log n)$, using the
prime-power cutoff rather than the full Euler-product logarithm.
Equations (4.9) and (4.11) give

$$
P(X)-\frac{\psi(X)-X}{X\log X}
=\log\log X+\gamma+Z_{\rm Ak}(1;X)+R_{\rm Ak}(1;X),
$$

where

$$
Z_{\rm Ak}(1;X)=-\sum_\rho\left[
 \operatorname{Ei}((\rho-1)\log X)
 -\frac{X^{\rho-1}}{\rho\log X}\right],
$$

$$
R_{\rm Ak}(1;X)=\frac{\zeta'(0)}{\zeta(0)X\log X}
-\sum_{k\ge1}\left[
 \frac{X^{-2k-1}}{2k\log X}
 +\operatorname{Ei}(-(1+2k)\log X)\right].
$$

The zeros retain their actual complex values and multiplicities.
The exponential integral defined immediately before Proposition 4.4
uses the cut $[0,\infty)$ and the horizontal integral from left infinity.
That convention matters: adding a lateral $i\pi$ constant would change
the individual coefficient and its absolute-convergence statement.

For the existing $A=\log N$, $L=\log A$, write (M1) in the source's
convention:

$$
F_A(s)=\frac{A^{s-1}}{sL}-\operatorname{Ei}((s-1)L),
\qquad 0<\Re s<1.
$$

This is the defining integral in the source's convention: the endpoint
term at infinity vanishes in this strip. Thus
$Z_{\rm Ak}(1;A)=Z_{\rm orig}$ with the **complete** $F_A$,
without replacing it by a leading asymptotic term or moving zeros onto
the critical line. Substitution into the existing finite-tail identity
retains the other explicit terms as well:

$$
I_\psi(A)=-Z_{\rm Ak}(1;A)-R_{\rm Ak}(1;A).
$$

The source's maximal-order Theorem 1 concerns fixed
$\nu\in[1/2,1)$; its boundedness condition is equivalent to the stated
zero-free half-plane, not an unconditional upper estimate. Definition
2.1 optimizes $\sigma_\nu(n)/n^{\nu(1+\varepsilon)}$, so its
half-power extremum is not identified with the selected ordinary Robin
extremum. Lemma 4.5 gives $O_\nu$ bounds only for $0<\nu<1$;
it supplies neither a uniform limit as $\nu\to1$ nor the missing signed
bound at exponent $1$. The formula above is an available primary
representation of the original response. The required same-source
upper bound on $Z_{\rm Ak}(1;A)+R_{\rm Ak}(1;A)$, equivalently the
original lower bound on $I_\psi(A)$, remains unproved, as do the strict
Robin margin and RH.

## Quantitative Tauberian hypotheses for the complete response

Pierce, Turnage-Butterbaugh and Zaman, *A guide to Tauberian theorems for arithmetic applications*, [arXiv:2504.16233v4](https://arxiv.org/html/2504.16233v4), §2.3, Hypothesis B and Theorem B, give a quantitative result for a general Dirichlet series $D(s)=\sum_j a_j\lambda_j^{-s}$ with nonnegative coefficients. Write their parameters as $\alpha_{\rm T}>0$, $0<\delta_{\rm T}<\alpha_{\rm T}$, $k_{\rm T}>0$ and $m\ge1$ for the quoted positive-growth version, to distinguish them from the FIB atoms and the moving-cut parameter. Hypothesis B permits $k_{\rm T}=0$ as well. Its assumptions require analytic continuation throughout $\Re s\ge\alpha_{\rm T}-\delta_{\rm T}$ except for the pole of order $m$ at the single real point $\alpha_{\rm T}$, the strip bound

$$
|(s-\alpha_{\rm T})^mD(s)|\le M_1\exp(|s|^{M_2}),\qquad
\alpha_{\rm T}-\delta_{\rm T}\le\Re s\le\alpha_{\rm T},
$$

and, on the left boundary, a uniform bound

$$
|D(s)|\le C(1+|\Im s|)^{k_{\rm T}}
 (\log(3+|\Im s|))^{m-1}.
$$

Under these hypotheses, for $X\ge2$,

$$
\sum_{\lambda_j\le X}a_j
=\operatorname*{Res}_{s=\alpha_{\rm T}}\frac{D(s)X^s}{s}
+O\!\left(X^{\alpha_{\rm T}-\delta_{\rm T}/(k_{\rm T}+1)}
 (\log X)^{m-1}\right).
$$

The implied constant depends on $\alpha_{\rm T},\delta_{\rm T},k_{\rm T},m,C,D(\alpha_{\rm T}+\delta_{\rm T})$, and is independent of $M_1,M_2$. Remark 9.3.1 gives the $k_{\rm T}=0$ version with remainder $O(X^{\alpha_{\rm T}-\delta_{\rm T}}(\log X)^m)$. The parameters are fixed; applying the result to a changing family requires controlling this dependence. In particular, the stated saving is $\delta_{\rm T}/(k_{\rm T}+1)$, rather than a saving of $\delta_{\rm T}$ from analytic continuation alone.

Theorems B.4–B.5 supply limiting examples for $k_{\rm T}>1/2$: general Dirichlet series satisfying Hypothesis B can have a remainder of size $\Omega(X^{\alpha_{\rm T}-\delta_{\rm T}/(k_{\rm T}+1/2)}(\log X)^{m-1})$, including examples with $0\le a_j\le1$. These examples do not identify the exact optimum between the two displayed exponents. The B.4 construction can use integer frequencies when $(k_{\rm T}+1/2)/\delta_{\rm T}$ is a positive integer. The B.5 bounded-coefficient construction uses general real frequencies without giving this integer-frequency guarantee. Neither result asserts a counterexample for the Riemann zeta function or the selected Robin integer.

For the direct prime-counting series $D(s)=-\zeta'(s)/\zeta(s)$, $\lambda_j=j$, $a_j=\Lambda(j)$ and $\alpha_{\rm T}=m=1$. Each actual zeta zero in the proposed half-plane is an additional pole, so the single-pole hypothesis must be verified for all heights. A finite zero subtraction supplies no such verification for the remaining zeros. Applying Theorem B to a resulting remainder also requires a proved nonnegative-coefficient representation and the stipulated uniform growth bounds; none is supplied by this source application.

The same conditional least integer $N>5040$ attaining the global Robin-ratio maximum remains fixed, with $A=\log N>10^{36}$ and $L=\log A$. The original complete $\sqrt A\,L\,I_\psi(A)$ lower allowance, or equivalently the full zero-plus-remainder upper allowance above, has not been obtained from these hypotheses. The actual zero real parts and multiplicities, every height, all remaining explicit terms and the strict core remain present. The published theorem and examples are reused without reconstructing their proofs; this applicability check supplies neither a new prime-error estimate nor a Robin/RH proof.

## A bounded-shape Gamma mixture retains an original coefficient remainder

Balanzario, Cárdenas Romero and Chacón Serna,
*A smooth version of Landau's explicit formula*,
[arXiv:2311.04347v1](https://arxiv.org/abs/2311.04347v1),
Theorem 1, supplies the Gamma density

$$
w_{\alpha,\lambda}(x)
=\frac{x^{\alpha-1}e^{-x/\lambda}}{\lambda^\alpha\Gamma(\alpha)},
\qquad
G_{\alpha,\lambda}(s)
=\lambda^{s-1}\frac{\Gamma(\alpha+s-1)}{\Gamma(\alpha)}.
$$

For $\alpha,\lambda>0$, $\alpha\notin\mathbb N$ and
$\mu=\alpha\lambda$, the stated formula is

$$
\sum_{n\ge1}\Lambda(n)w_{\alpha,\lambda}(n)
=1-\sum_\rho m_\rho G_{\alpha,\lambda}(\rho)-R(\mu,\alpha).
$$

This statement has no RH premise. The source defines $R$ by two separate
series involving falling factorials and $\zeta'/\zeta$; those terms
remain present, with no assumed sign or uniform budget. Its Theorem 2,
which gives a finite-ordinate formula near a natural-number center
$\mu$, assumes RH and fixes its window parameters. That truncated
formula is not an unconditional supplier at $A=\log N$.

The existing algebraic lower bound (H2) also specifies a restriction on
exact replacement by these Gamma coefficients. Fix $A\ge e^2$ and a
finite $B>0$. Let $\nu_A$ be a locally finite signed or complex measure on

$$
\{(\alpha,\lambda):0<\alpha\le B,
\ \alpha\notin\mathbb N,\ \lambda>0\}
$$

which is fixed as the zero height varies, and assume only the critical-line
absolute moment

$$
M_A=\int\lambda^{-1/2}\,d|\nu_A|(\alpha,\lambda)<\infty.
$$

This does not require finite total mass or moments at the endpoints of
the critical strip. Set

$$
Q_A(1/2+it)=\int G_{\alpha,\lambda}(1/2+it)
                         \,d\nu_A(\alpha,\lambda),\qquad t\ne0.
$$

The standard vertical-line Stirling formula,
[DLMF 5.11.9](https://dlmf.nist.gov/5.11.E9), is uniform for bounded real
arguments. Here $\alpha-1/2\in[-1/2,B-1/2]$ and
$1/\Gamma(\alpha)$ is bounded for $0<\alpha\le B$. Consequently,
for a constant $C_B$ and sufficiently large $|t|$,

$$
|Q_A(1/2+it)|
\le C_BM_A|t|^{B-1}e^{-\pi|t|/2}.
$$

In contrast, (H2) on this same line gives, for $|t|\ge4$,

$$
|F_A(1/2+it)|
\ge\frac{2w(A)}{3\sqrt A(t^2+1/4)},
\qquad w(A)=\frac{1+\log A}{(\log A)^2}.
$$

Exponential decay is eventually smaller than this algebraic bound.
Hence there is a threshold depending on $A,B,M_A$ such that

$$
|F_A(1/2+it)-Q_A(1/2+it)|
\ge\frac{w(A)}{3\sqrt A(t^2+1/4)}
$$

above that threshold. There are unconditionally infinitely many actual
critical-line zeros, as recalled in
[DLMF §25.10(i)](https://dlmf.nist.gov/25.10.i).
Thus the mismatch occurs at actual zeros of arbitrarily large height;
it is not merely an off-spectrum difference on the whole strip. Their
positive multiplicities do not remove the coefficient difference.

This applies even to infinitely many scales and to complex mixture
weights under the stated absolute moment. It reuses (H2), uniform
Stirling and the classical critical-line zero theorem; no new version
of those results or mathematical originality is claimed. Shapes and
weights may depend on $A$, but their bound is fixed at each such $A$.
The conclusion concerns exact coefficient matching at every actual zero.
It does not give a sign for a paired residual or exclude equality of an
aggregate signed sum, unbounded shape support, nonabsolute constructions,
or approximation on a finite height range with a paid remainder.
In particular the original suffix above $T$ is already paid independently;
this restriction does not invalidate that transport or prohibit a useful
approximation of its lower head. The complete same-selected-source signed
Robin estimate and RH remain unproved. This application is not Lean
verified.
