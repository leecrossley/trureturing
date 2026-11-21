---
bibkey: trureturing2026gammaresponse
authors: trureturing research
year: 2026
title: Gamma response
doi: null
url: https://github.com/the-omega-institute/trureturing/blob/727e10f660466a6dc69ea491c8f334969b9c9d87/Library/ArithSums/nicolas2025comparison.md#uniform-control-of-the-combined-gamma-remainder
claim: Project calculations on the extremal envelopes studied in the Nicolas comparison note, under the hypotheses given in each section.
strata_touched: []
license: citation-only
triage: anchor
---

# Gamma response

These sections continue the project’s calculations on Nicolas’s comparison of the two extremal envelopes. [Source and section index](../ArithSums/nicolas2025comparison.md)

## Uniform control of the combined Gamma remainder

The two remainder series in Balanzario, Cárdenas Romero and Chacón
Serna, [arXiv:2311.04347v1](https://arxiv.org/abs/2311.04347v1),
Theorem 1, need not be integrated separately. Their combined remainder
has a uniform bound under the existing canonical scale measure. The
following is a `repo-derived` paper-level application of that theorem, the classical
explicit formula displayed as equation (1) in the same source, the
existing coefficient estimate (H5), and unconditional PNT bounds. It
does not reconstruct those source proofs or claim mathematical
originality or Lean verification.

Let $A\ge e^2$, $L=\log A$, and retain (M2):

$$
h_A(\mu)=\frac1{\max(A,\mu)\log\max(A,\mu)},\qquad
k(u)=\frac{1+\log u}{u^2\log^2u}.
$$

For noninteger $\alpha\ge4$, write the source's prime response as

$$
P_\alpha(\mu)=\sum_{n\ge1}\Lambda(n)
 \frac{(\alpha/\mu)^\alpha n^{\alpha-1}e^{-\alpha n/\mu}}
      {\Gamma(\alpha)}
=1-\sum_\rho m_\rho G_{\alpha,\mu/\alpha}(\rho)
 -R(\mu,\alpha).
$$

The sum indexes distinct zero locations, and $m_\rho$ carries their
actual multiplicities. No zero is moved to the critical line. Define

$$
\overline R_\alpha(A)
 =\int_0^\infty h_A(\mu)R(\mu,\alpha)\,d\mu,
\qquad
M_3(\alpha)=\frac{\alpha^3}
 {(\alpha-1)(\alpha-2)(\alpha-3)}.
$$

This integral exists absolutely for each such $\alpha$. There is an
absolute constant $K$, independent of both $A$ and $\alpha$, for which

$$
\boxed{
\left|\overline R_\alpha(A)
 -\frac{\log(2\pi)}{A\log A}\frac{\alpha}{\alpha-1}\right|
 \le\frac{K M_3(\alpha)}{A^3\log A}.}
\tag{GR1}
$$

Since $M_3(\alpha)\le32/3$ and $\alpha/(\alpha-1)\le4/3$,
this is uniform even when the noninteger shape grows with $A$ or
approaches an integer. In particular,

$$
\sqrt A\log A\,\overline R_\alpha(A)
 =\frac{\log(2\pi)}{\sqrt A}\frac{\alpha}{\alpha-1}
  +O(A^{-5/2})\longrightarrow0
\tag{GR2}
$$

uniformly over the stated shapes. The constant is not numerically
certified; no finite starting clock follows.

### Convergence and the dilation representation

Put $D(x)=\psi(x)-x$. Reuse an unconditional PNT bound in the global
form

$$
|D(x)|\le C_\psi\frac{x}{\log^2(2+x)}\qquad(x>0).
\tag{GR3}
$$

An absolute $C_\psi$ exists by PNT with a fixed logarithmic saving,
with the bounded initial interval absorbed into the constant. This is
not a square-root prime-error estimate. Integration by parts against
the fixed-shape Gamma density, splitting its argument at $\sqrt\mu$,
gives $P_\alpha(\mu)-1=O_\alpha((\log\mu)^{-2})$ at infinity.
At zero, $P_\alpha(\mu)=O_\alpha(\mu^{-\alpha}e^{-\alpha/\mu})$.
Consequently $h_A(1-P_\alpha)$ is absolutely integrable. These
convergence constants may depend on the fixed shape; they are not used
as the uniform constants in (GR1).

For fixed $\alpha$, vertical-line Stirling gives exponential decay of
the Gamma coefficient. Moreover (M2) implies, for $0<\beta<1$,

$$
F_A(\beta)\le\frac{A^{\beta-1}}L
 \left(\frac1\beta+\frac1{1-\beta}\right).
$$

The already cited zero-free region and its reflection bound the two
reciprocal endpoint distances by powers of logarithms of the ordinate.
Together with the classical zero count this makes

$$
\sum_\rho m_\rho\int_0^\infty h_A(\mu)
 |G_{\alpha,\mu/\alpha}(\rho)|\,d\mu<\infty.
$$

The source identity therefore proves absolute convergence of the
combined $\overline R_\alpha(A)$, without integrating either printed
remainder series term by term. It also justifies

$$
\overline R_\alpha(A)
 =J_\alpha(A)-\sum_\rho m_\rho H_\alpha(\rho)F_A(\rho),
\quad
J_\alpha(A)=\int_0^\infty h_A(\mu)(1-P_\alpha(\mu))\,d\mu,
\tag{GR4}
$$

where the existing coefficient identity is
$H_\alpha(s)=\Gamma(\alpha+s-1)/[\Gamma(\alpha)\alpha^{s-1}]$.
The constant pole and the prime response have been kept together.

Let $C>0$ have Gamma shape $\alpha$ and rate $\alpha$, so its mean is
one. The source primitive and its negative moments are

$$
U_\alpha(\mu)=\mathbb E\frac{\psi(C\mu)}C,
\qquad U_\alpha'(\mu)=P_\alpha(\mu),
\qquad
\mathbb E C^{-1}=\frac{\alpha}{\alpha-1},
\quad \mathbb E C^{-3}=M_3(\alpha).
$$

The derivative follows by differentiating the Gamma integral for each
prime-power jump. Thus integration by parts gives

$$
J_\alpha(A)=\mathbb E J_C(A),\qquad
J_c(A)=-\frac1c\int_A^\infty D(cu)k(u)\,du.
\tag{GR5}
$$

Here the exchange is an absolute one. For $u\ge A$, (GR3) and the
split $C\ge u^{-1/2}$ or $C<u^{-1/2}$ give

$$
\mathbb E\frac{|D(Cu)|}C
 \le C_\psi u\left[\frac4{\log^2u}
       +\frac{M_3(\alpha)u^{-3/2}}{(\log2)^2}\right].
$$

Multiplication by $k(u)$ is integrable. The same bound pays the
integration-by-parts boundary at infinity; the boundary at zero
vanishes by $|D(x)|\ll x$. No separate infinite-mass integral of the
pole term has been taken.

### A bound valid on both sides of the unit cutoff

For each $c>0$, define the absolutely convergent zero sum and its
arithmetic remainder

$$
Z_c(A)=\sum_\rho m_\rho c^{\rho-1}F_A(\rho),\qquad
r_c(A)=J_c(A)-Z_c(A).
$$

The existing (H5) and $\sum_\rho m_\rho/\gamma^2<\infty$ give

$$
|Z_c(A)|\le\sum_\rho m_\rho |c^{\rho-1}F_A(\rho)|
 \le\frac{C_0}L\max\{1,(cA)^{-1}\}.
\tag{GR6}
$$

If $cA\ge1$, applying the classical explicit formula to (GR5) gives

$$
r_c(A)=\frac{\log(2\pi)}{cA L}
 +\frac12\int_{cA}^\infty\log(1-x^{-2})
 \frac{1+\log(x/c)}{x^2\log^2(x/c)}\,dx.
\tag{GR7}
$$

Take finite scale endpoints first and use the existing finite-endpoint
bound (U2), then dominated convergence for the zero coefficients. The
prime-power half-value convention changes no integral.
At $cA=1$ the logarithmic singularity is integrable. For $1\le cA\le2$,
use

$$
\int_1^\infty\frac{-\log(1-x^{-2})}{x^2}\,dx
 =2-2\log2<1.
$$

For $cA\ge2$, use $-\log(1-x^{-2})\le4/(3x^2)$.
Since $\log(x/c)\ge L$, both ranges give

$$
\left|r_c(A)-\frac{\log(2\pi)}{cA L}\right|
 \le\frac{K_1}{(cA)^3L}\qquad(cA\ge1).
\tag{GR8}
$$

For $cA<1$, do not extend the explicit formula below one. There
$D(x)=-x$. Substitution $x=cu$ in (GR5) and direct integration over
$[cA,1]$ give, with $d=-\log(cA)>0$,

$$
\int_{cA}^1\frac{1+\log(x/c)}{x\log^2(x/c)}\,dx
 =\log(1+d/L)+\frac1L-\frac1{L+d}
 \le\frac{d+1}L\le\frac2{cA L}.
$$

On $x\ge1$, (GR3) bounds the remaining absolute integral by

$$
\frac{C_1}L\int_1^\infty\frac{dx}{x\log^2(2+x)}
 \le\frac{C_2}L.
$$

Together with (GR6), this yields
$|r_c(A)|\le C_3/(cA L)$. Because $(cA)^{-1}\le(cA)^{-3}$ in this
range, (GR8), with a larger absolute constant, holds for every $c>0$.
This pays the entire small-scale contribution, including $cA<1$.

Finally, $\mathbb E C^{\rho-1}=H_\alpha(\rho)$.
Equation (GR6) and $\mathbb E C^{-1}<\infty$ justify averaging the
complete zero series. Equations (GR4)–(GR5) therefore give
$\overline R_\alpha(A)=\mathbb E r_C(A)$. Average (GR8) and use the
exact inverse-third moment to obtain (GR1).

The result bounds the combined source remainder, not its individual
series. It adds no Gamma coefficient approximation or replacement for
the existing complete Gaussian transport. At the same conditional
least global Robin maximizer $N>5040$, $A=\log N>10^{36}$, the full
centered prime response and any signed comparison of
$H_\alpha(\rho)F_A(\rho)$ with the original $F_A(\rho)$ still require
control. All actual zeros, multiplicities, heights, original pole and
trivial terms, and the strict core remain present. The complete signed
Robin estimate and RH remain unproved.


## A directed prime-weight comparison for the complete Gamma response

The combined-remainder estimate (GR1) can be paired with a one-sided
arithmetic comparison. This `repo-derived` application uses the same
canonical measure (M2), nonnegative von Mangoldt weights, the standard
unconditional Chebyshev bound, and the Gamma law already used in
(GR4)–(GR5). It does not replace the original coefficient by a pointwise
approximation or claim mathematical originality or Lean verification.

Keep $A\ge e^2$, $L=\log A$ and noninteger $\alpha\ge4$. Let $C$ have
Gamma shape $\alpha$ and rate $\alpha$, and put

$$
h_A(t)=\frac1{\max(A,t)\log\max(A,t)},\qquad
w_c(t)=\frac1c h_A(t/c),\qquad
\Delta_\alpha(t)=\mathbb E w_C(t)-h_A(t).
$$

The resulting complete signed comparison is

$$
\boxed{
-I_\psi(A)\le J_\alpha(A)
 +\frac{\psi(A)}{(\alpha-1)A\log A}.}
\tag{GP1}
$$

Here $J_\alpha$ is the centered prime response in (GR4), not the
uncentered integral of its pole or prime terms. No source extremality
assumption is needed for (GP1); it therefore applies at the same
selected Robin integer without changing that integer.

### A global tangent majorant on the infinite prime tail

Fix $t\ge A$ and write $s=t/A\ge1$, $v=\log t$. As a function of the
dilation $c>0$, the transported prime weight is

| Dilation | *f*<sub>*t*</sub>(*c*) = *w*<sub>*c*</sub>(*t*) |
| --- | --- |
| 0 &lt; *c* ≤ *s* | 1 / (*t* · (*v* − log *c*)) |
| *c* ≥ *s* | 1 / (*A* · *L* · *c*) |

On $0<c<s$,

$$
f_t''(c)=\frac{2-(v-\log c)}
 {t c^2(v-\log c)^3}\le0,
$$

because $v-\log c\ge L\ge2$. Thus its tangent at $c=1$ majorizes
the first branch:

$$
f_t(c)\le \frac1{tv}+\frac{c-1}{tv^2}\qquad(0<c\le s).
$$

The same affine function is increasing and majorizes $f_t(s)$. The
second branch decreases for $c\ge s$, so this is a global majorant,
even though $f_t$ is not globally concave. At $s=1$ use the left
tangent and the same argument. Since $\mathbb EC=1$, averaging gives

$$
\Delta_\alpha(t)\le0\qquad(t\ge A).
\tag{GP2}
$$

For $0<t<A$, $h_A(t)=1/(A L)$ and $h_A(t/c)\le1/(A L)$.
The existing inverse-first Gamma moment therefore gives

$$
\Delta_\alpha(t)\le
 \frac{\mathbb EC^{-1}-1}{A L}
 =\frac1{(\alpha-1)A L}.
\tag{GP3}
$$

### Centering and absolute convergence of the full prime difference

The pole and prime integrals are not subtracted as separate infinite
quantities. First fix $c>0$ and set $T=A\max(1,c)$. Reuse a fixed
unconditional bound $\psi(x)\le Bx$. Below $T$, the absolute
prime-weight difference is bounded by

$$
\sum_{n\le T}\Lambda(n)|w_c(n)-h_A(n)|
\le\frac{B}{L}(1+c^{-1})\max(1,c).
$$

For $n>T$ both weights use their logarithmic branch, and

$$
|w_c(n)-h_A(n)|
 =\frac{|\log c|}{n\log n\,\log(n/c)}
 \le\frac{|\log c|(1+|\log c|/L)}{n\log^2n}.
$$

Partial summation with the same Chebyshev bound gives
$\sum_{n>T}\Lambda(n)/(n\log^2n)\le2B/L$. Since
$|\log c|+(\log c)^2\ll c+c^{-1}$, these estimates yield an absolute
constant $B_1$ such that

$$
\sum_{n\ge2}\Lambda(n)|w_c(n)-h_A(n)|
 \le\frac{B_1}{L}(c+c^{-1}).
\tag{GP4}
$$

The analogous Lebesgue integral is also absolutely convergent.
Changing variables in finite integrals shows

$$
\int_0^\infty(w_c(t)-h_A(t))\,dt=0:
$$

for sufficiently large $R$, the difference of integrals up to $R$
is $\log\log(R/c)-\log\log R$, which tends to zero. Integration by
parts against $D(t)=\psi(t)-t$, using (GR3) at infinity and $D(t)=-t$
below one, therefore gives

$$
J_1(A)-J_c(A)
 =\sum_{n\ge2}\Lambda(n)[w_c(n)-h_A(n)],
\qquad J_1(A)=-I_\psi(A).
$$

The $J_c$ here is the deterministic dilation in (GR5); $J_1$ is its
value at dilation one, not a Gamma response with shape one. All
boundary terms vanish. Equation (GP4), $\mathbb EC=1$ and
$\mathbb EC^{-1}<\infty$ justify averaging and termwise summation.
Reusing (GR5) yields the absolutely convergent identity

$$
-I_\psi(A)-J_\alpha(A)
 =\sum_{n\ge2}\Lambda(n)\Delta_\alpha(n).
\tag{GP5}
$$

Apply (GP2) to the entire infinite tail, (GP3) to the finite lower
part, and $\Lambda(n)\ge0$ to prove (GP1). An atom at $n=A$ has the
nonpositive sign in (GP2); using $\psi(A)$ in the upper allowance
remains valid.

### Pay the remainder and retain the original signed target

Define the complete real zero response

$$
Z_\alpha(A)=\sum_\rho m_\rho H_\alpha(\rho)F_A(\rho),
\qquad
H_\alpha(s)=\frac{\Gamma(\alpha+s-1)}
 {\Gamma(\alpha)\alpha^{s-1}}.
$$

Its absolute convergence and reality under conjugate pairing follow
from the existing fixed-shape argument in (GR4). No zero real part,
multiplicity or height is changed. Since
$J_\alpha=Z_\alpha+\overline R_\alpha$, (GR1) and (GP1) give

$$
\boxed{\begin{aligned}
\sqrt A L[-I_\psi(A)]\le{}&\sqrt A L Z_\alpha(A)
 +\frac{\psi(A)}{(\alpha-1)\sqrt A}\\
&+\frac{\log(2\pi)}{\sqrt A}\frac\alpha{\alpha-1}
 +\frac{K M_3(\alpha)}{A^{5/2}}.
\end{aligned}}
\tag{GP6}
$$

This is a directed bound for the original full response, with a paid
finite prime budget and the complete combined remainder. It is not an
absolute coefficient approximation, a bound on the sum of coefficient
moduli, or a deletion of the original explicit-formula terms.

For shapes with $\alpha(A)/\sqrt A\to\infty$, the added allowance in
(GP6) tends to zero by the existing PNT bound. This gives a sufficient
transfer from a full signed Gamma-response upper estimate to (G9),
provided the estimate has enough slack to pay the displayed allowance.
The signed upper estimate on $Z_\alpha(A)$ is not established here.
At the same conditional least global Robin maximizer $N>5040$,
$A=\log N>10^{36}$, the original strict core, complete infinite
response and target remain unchanged. Neither (G9) nor RH is proved.


## An explicit one-sided bound for the combined Gamma remainder

For finite source clocks, the absolute constant in (GR1) need not be
assigned an unproved numerical value. The following upper bound instead
uses the existing finite-height verification and zero-count constants in
[(F3) of the Polak application](../Analytic/polak2026finiterobinca.md#reusing-the-complete-residual-envelope),
together with (U2), (GR5) and (GR7). These inputs are reused without a new
zero computation or reconstruction of their source proofs.

Put $H=3\cdot10^{12}$, and let every zero sum retain the full actual
nontrivial-zero multiset, with multiplicities. Write

$$
c_0=2+\gamma-\log(4\pi)<0.05,\qquad
S_2(H)=\sum_{\Im\rho>H}\frac{m_\rho}{(\Im\rho)^2}
 <1.48\cdot10^{-12}.
$$

The same sources supply criticality up to $H$ and the classical identity
$\sum_\rho m_\rho/[\rho(1-\rho)]=c_0$.
For $\rho=\beta+i\gamma$ in the critical strip,

$$
\Re\frac1{\rho(1-\rho)}
=\frac{\gamma^2+\beta(1-\beta)}{|\rho(1-\rho)|^2}>0.
$$

On the verified head the denominator is the positive real number
$\gamma^2+1/4$. On the remaining zeros,
$|\rho||1-\rho|\ge\gamma^2$.
Consequently the complete absolute weight obeys

$$
\mathcal C_\zeta:=\sum_\rho
 \frac{m_\rho}{|\rho||1-\rho|}
\le c_0+2S_2(H)<0.051.
\tag{GE1}
$$

The factor two accounts for the two ordinate signs, not an additional
independently chosen zero population.

Keep $A\ge e^2$ and $L=\log A$. For the same deterministic dilation
$r_c(A)=J_c(A)-Z_c(A)$ in (GR5)–(GR7), one has the uniform upper bound

$$
\boxed{r_c(A)<\frac5{cAL}\qquad(c>0).}
\tag{GE2}
$$

If $cA\ge1$, (GR7) immediately gives
$r_c(A)\le\log(2\pi)/(cAL)<2/(cAL)$, since its logarithmic integral
is nonpositive. This includes the integrable endpoint $cA=1$.

If $cA<1$, put $B=1/c>A$ and $d=\log(B/A)>0$.
Since $\psi(cu)-cu=-cu$ on $A<u<B$, (GR5) gives exactly

$$
r_c(A)=\log(1+d/L)+\frac1L-\frac1{L+d}
 +r_c(B)-\sum_\rho m_\rho c^{\rho-1}F_{A,B}(\rho).
\tag{GE3}
$$

The initial elementary term is at most $2/(cAL)$, as already computed
in the proof of (GR8). At $cB=1$, (GR7) gives
$r_c(B)<2/\log B\le2/(cAL)$.
The finite-endpoint bound (U2), (GE1) and
$(cA)^{\beta-1}\le(cA)^{-1}$ give

$$
\left|\sum_\rho m_\rho c^{\rho-1}F_{A,B}(\rho)\right|
\le\frac{2(1+1/L)\mathcal C_\zeta}{cAL}
\le\frac{3\mathcal C_\zeta}{cAL}<\frac{0.153}{cAL}.
$$

Thus (GE2) also holds below the unit cutoff. In particular, no classical
explicit formula has been extended to $cu<1$ and no small Gamma scales
have been discarded.

For the same noninteger shapes $\alpha\ge4$ as in (GR1), averaging (GE2)
by (GR5) and the existing inverse-first Gamma moment yields

$$
\overline R_\alpha(A)
\le\frac{5M_1(\alpha)}{AL},\qquad
M_1(\alpha)=\frac\alpha{\alpha-1}.
\tag{GE4}
$$

This is an explicit upper bound, not an absolute bound or a replacement
for the sharper asymptotic assertion (GR1). With the original full
prime-integral comparison (GP1), it gives the finite inequality

$$
\boxed{\sqrt A L[-I_\psi(A)]
\le\sqrt A L Z_\alpha(A)
 +\frac{\psi(A)}{(\alpha-1)\sqrt A}
 +\frac{5M_1(\alpha)}{\sqrt A}.}
\tag{GE5}
$$

The full elementary and trivial contributions are paid through
$\overline R_\alpha$; the left side is the original complete integral.
No signed main estimate or unbounded source-clock conclusion follows
from (GE5) alone.


## A larger finite clock from the verified-height Gamma response

The explicit directed inequality (GE5) can be paired with a uniform
Gamma modulus estimate. It bounds the original signed integral on a
larger finite interval, while keeping the same conditional least integer
$N>5040$ attaining the global Robin-ratio maximum. This is not a reduction
to the least counterexample or an all-integer finite Robin verification.
No arithmetic profiles or zero ordinates are newly enumerated.

### Uniform damping with the actual real parts retained

Use the classical product
[NIST DLMF 5.8.3](https://dlmf.nist.gov/5.8.E3), for $x>0$:

$$
\left|\frac{\Gamma(x+it)}{\Gamma(x)}\right|
=\prod_{k=0}^\infty
 \left(1+\frac{t^2}{(x+k)^2}\right)^{-1/2}.
$$

The summand $\log(1+t^2/(x+u)^2)$ is positive and decreasing in $u$.
Using $\log(1+v)\ge v/(1+v)$ in its integral gives

$$
\sum_{k=0}^\infty\log\left(1+\frac{t^2}{(x+k)^2}\right)
\ge |t|\arctan(|t|/x)
\ge\frac{t^2}{x+|t|}.
$$

The last inequality uses $\arctan v\ge v/(1+v)$ for $v\ge0$.
For $0<\beta<1$, the already used Gamma law has
$\mathbb E C^{\beta-1}\le(\mathbb EC^{-1})^{1-\beta}\le M_1(\alpha)$
by Hölder. Set $x=\alpha+\beta-1\le\alpha$ in the product. It follows that

$$
\boxed{|H_\alpha(\beta+it)|
\le M_1(\alpha)
 \exp\left(-\frac{t^2}{2(\alpha+|t|)}\right).}
\tag{GH1}
$$

This is uniform over the whole actual critical strip. Criticality is
used only on the already verified head below $H$.

Passing to the infinite endpoint in the existing (U2) gives

$$
\sqrt A L|F_A(\rho)|
\le2(1+1/L)\frac{A^{\beta-1/2}}{|\rho||1-\rho|}.
\tag{GH2}
$$

The function $t^2/[2(\alpha+t)]$ increases for $t>0$.
Split the complete $Z_\alpha$ at the verified height $H$.
Use the positive $c_0$ identity on the critical head, and (GH1), (GH2),
$\beta<1$, and $2S_2(H)$ on every remaining zero. This gives

$$
\sqrt A L|Z_\alpha(A)|
\le2M_1(\alpha)(1+1/L)
 \left[c_0+2\sqrt A\,S_2(H)
   \exp\left(-\frac{H^2}{2(\alpha+H)}\right)\right].
\tag{GH3}
$$

Every height beyond $H$ is included to infinity. Replacing the actual
$A^{\beta-1/2}$ by $\sqrt A$ in this upper bound does not assume RH
outside the verified head.

### Pay the constants at the same selected source

Take the exact noninteger shape and clock range

$$
\alpha=10^{23}+\frac12,\qquad
10^{36}<A\le10^{45},\qquad L=\log A.
$$

Then $L>78$, $\sqrt A<3.2\cdot10^{22}$,
$M_1(\alpha)<1.0001$, and

$$
\frac{H^2}{2(\alpha+H)}>40,\qquad e^{40}>10^{17}.
$$

The latter follows from $e>8/3$ and
$8^{40}>10^{17}3^{40}$.
The two contributions in (GH3) are bounded by the rational inequalities

$$
2(1.0001)(1.02)(0.05)<0.103,
$$

$$
4(1.0001)(1.02)(3.2\cdot10^{22})
 (1.48\cdot10^{-12})10^{-17}<0.000003.
\tag{GH4}
$$

For the prime-comparison allowance, reuse Dusart's
[Theorem 5.2, $k=0$, and Proposition 3.2](../Weil/dusart2010estimates.md):
$\vartheta(A)<2A$ and
$\psi(A)-\vartheta(A)<1.00007\sqrt A+1.78A^{1/3}$.
On this range they give $\psi(A)<2.01A$. Therefore

$$
\frac{\psi(A)}{(\alpha-1)\sqrt A}
<\frac{2.01(3.2\cdot10^{22})}{0.9999\cdot10^{23}}<0.644,
\qquad
\frac{5M_1(\alpha)}{\sqrt A}<6\cdot10^{-18}.
\tag{GH5}
$$

Combining (GE5) and (GH3)–(GH5) pays the full original signed integral:

$$
\boxed{-\sqrt A L I_\psi(A)
<0.103+0.000003+0.644+6\cdot10^{-18}<\frac34
\qquad(10^{36}<A\le10^{45}).}
\tag{GH6}
$$

The same selected source still satisfies
$\Delta(N)=I_\psi(A)+D^*(A)$ and the strict core (G6).
The already proved bound
[(X5) in the Polak application](../Analytic/polak2026finiterobinca.md#pay-the-full-signed-margin-with-the-same-strict-core)
gives $\mathcal E(L)>0.778$ for every $L\ge78$.
Thus at this actual source and clock,

$$
\boxed{\sqrt A L\Delta(N)>0.778-0.75=0.028
\qquad(10^{36}<A\le10^{45}).}
\tag{GH7}
$$

The existing restriction $A>10^{36}$ and (GH7) therefore force
$\log N>10^{45}$ for the same hypothetical least global maximizer.
This conclusion is specific to that selected source; it does not assert
strict Robin for every integer below $\exp(10^{45})$.

This application reuses the published finite-height verification,
zero-count and prime estimates, the classical Gamma product, and the
existing core and directed-transport results. It makes no mathematical
priority claim and has no Lean certification. The fixed shape and verified
height give no uniform bound as $A\to\infty$: the comparison and high-zero
allowances in (GE5), (GH3) still grow with $\sqrt A$.
The full unbounded signed Robin target and RH remain unproved.


## A one-sided entire envelope retaining the original cutoff

The original prime weight has a derivative jump at its cutoff. A signed
mixture of published power-function extremals gives entire lower and
upper envelopes with an exact error while retaining that cutoff. Use
the power-function corollary in Carneiro, Littmann and Vaaler,
[arXiv:1008.4969v2](https://arxiv.org/abs/1008.4969v2), Part III,
“Extremal Functions for $|x|^\sigma$”, can instead be applied before
mixing the actual second-derivative measure. This is a paper-level
application of that published corollary and elementary signed-measure
integration, with no mathematical priority or Lean-verification claim.

Retain $A\ge e^2$, $L=\log A$, and the original weight and derivative

$$
H_A(x)=\frac1{\max(A,|x|)\log\max(A,|x|)},\qquad
k(t)=\frac{1+\log t}{t^2\log^2t},\qquad
\kappa_A=k(A).
$$

The distributional second derivative is the signed measure

$$
\mu_A=\mu_A^+-\mu_A^-,\qquad
\mu_A^+(du)=-k'(|u|)\mathbf1_{\{|u|>A\}}\,du,
\qquad
\mu_A^-=\kappa_A(\delta_{-A}+\delta_A).
\tag{CE1}
$$

Here $k'<0$. Both parts have mass $2\kappa_A$, and
$\int(1+|u|)\,d|\mu_A|(u)<\infty$. The negative cutoff atoms have
not been dropped. Direct integration gives the absolutely convergent
potential representation

$$
\boxed{H_A(x)=\frac12\int_{\mathbb R}|x-u|\,d\mu_A(u).}
\tag{CE2}
$$

For example, differentiation off $\pm A$ gives the original derivative;
the value at zero is
$-A\kappa_A+\int_A^\infty u[-k'(u)]\,du=1/(AL)$.
These facts and continuity identify the potential with $H_A$.

Use the source corollary at $\sigma=1$, where its normalization is
$\gamma(-1)=-2\pi$ and $\gamma(2)=1/\pi$. Reversing the inequalities
when dividing by $-2\pi$, and then rescaling, provides even real entire
functions $P_\delta,Q_\delta$ of exponential type at most $2\pi\delta$
for every $\delta>0$, satisfying

$$
P_\delta(x)\le |x|\le Q_\delta(x),\qquad
\int_{\mathbb R}(|x|-P_\delta(x))\,dx=\frac1{6\delta^2},\qquad
\int_{\mathbb R}(Q_\delta(x)-|x|)\,dx=\frac1{12\delta^2}.
\tag{CE3}
$$

This reuses the source result rather than reconstructing its proof.
The two nonnegative errors sum to the integrable entire function
$Q_\delta-P_\delta$. The standard real-line bound for an integrable
entire function of finite exponential type makes that difference
bounded; hence both power extremals are $O_\delta(1+|x|)$ on the real
line. The usual polynomial-growth version of the Paley–Wiener bound
then gives $O_{K,\delta}(1+|u|)$ for their translates $z-u$, uniformly
for $z$ in a fixed compact subset $K$ of the complex plane. This bound
and the first moment in (CE1) justify locally uniform integration below,
including differentiation on compact subsets.

Define

$$
\begin{aligned}
\ell_{A,\delta}(z)
 &=\frac12\left[\int P_\delta(z-u)\,d\mu_A^+(u)
                  -\int Q_\delta(z-u)\,d\mu_A^-(u)\right],\\
u_{A,\delta}(z)
 &=\frac12\left[\int Q_\delta(z-u)\,d\mu_A^+(u)
                  -\int P_\delta(z-u)\,d\mu_A^-(u)\right].
\end{aligned}
\tag{CE4}
$$

They are even real entire functions of exponential type at most
$2\pi\delta$, and the signs in (CE4) give

$$
\boxed{\ell_{A,\delta}(x)\le H_A(x)\le u_{A,\delta}(x)
\qquad(x\in\mathbb R).}
\tag{CE5}
$$

Tonelli applies to the nonnegative differences from (CE2). Using the
actual two masses in (CE1), rather than treating the signed measure as
positive, gives the exact errors

$$
\int_{\mathbb R}(H_A-\ell_{A,\delta})\,dx
=\int_{\mathbb R}(u_{A,\delta}-H_A)\,dx
=\frac{\kappa_A}{4\delta^2}.
\tag{CE6}
$$

Evenness therefore yields

$$
\boxed{\int_0^\infty(H_A-\ell_{A,\delta})\,dt
       =\frac{\kappa_A}{8\delta^2}.}
\tag{CE7}
$$

These are explicit envelopes for the unchanged cutoff weight. They do
not assert extremality for $H_A$, arithmetic sampling convergence, a
compact zero-height cutoff, or a sign estimate on the original complete
zero response. Fourier support on the additive real variable is not
spectral truncation at the actual complex zeta zeros.

### A finite centered prime comparison

The lower envelope (CE5) gives a finite arithmetic consumer without
assuming that an unweighted $L^1$ error controls an infinite
von-Mangoldt weighted sum. Keep $R\ge A\ge e^2$, $V=\log R$,
$D(t)=\psi(t)-t$, and the existing unconditional constant $C_\psi$ in
(GR3). Define the finite centered response

$$
\mathcal J_{A,\delta}(R)
=\int_0^R\ell_{A,\delta}(t)\,dt
 -\sum_{2\le n\le R}\Lambda(n)\ell_{A,\delta}(n).
\tag{CP1}
$$

Both terms are finite. No separately divergent pole or prime integral
has been taken. Set $e=H_A-\ell_{A,\delta}\ge0$. For this same $R$,
nonnegative von Mangoldt weights and (CE7) give

$$
\begin{aligned}
\int_0^R H_A(t)\,dt-\sum_{2\le n\le R}\Lambda(n)H_A(n)
&=\mathcal J_{A,\delta}(R)+\int_0^R e(t)\,dt
                -\sum_{2\le n\le R}\Lambda(n)e(n)\\
&\le\mathcal J_{A,\delta}(R)+\frac{\kappa_A}{8\delta^2}.
\end{aligned}
\tag{CP2}
$$

An atom at $n=A$ satisfies the same pointwise order. No zero real part,
multiplicity, or height is altered in the original response.

Partial summation, with the right endpoint included in $\psi(R)$,
keeps the full original integral:

$$
-I_\psi(A)
=\left[\int_0^R H_A(t)\,dt
       -\sum_{2\le n\le R}\Lambda(n)H_A(n)\right]
 +D(R)H_A(R)-\int_R^\infty D(t)k(t)\,dt.
\tag{CP3}
$$

The existing (GR3) implies $|D(t)|\le C_\psi t/\log^2t$ for $t>1$.
Its boundary allowance is $C_\psi/V^3$, and direct integration pays
all of the remaining tail by

$$
\int_R^\infty |D(t)|k(t)\,dt
\le C_\psi\left(\frac1{2V^2}+\frac1{3V^3}\right).
$$

Consequently the finite directed upper bound is

$$
\boxed{\begin{aligned}
-\sqrt A L I_\psi(A)\le{}&\sqrt A L\mathcal J_{A,\delta}(R)
 +\frac{1+L}{8A^{3/2}L\delta^2}\\
&+C_\psi\sqrt A L
   \left(\frac1{2V^2}+\frac4{3V^3}\right).
\end{aligned}}
\tag{CP4}
$$

This pays the approximation and the entire omitted arithmetic tail for
any displayed parameters. It neither requires nor proves convergence
of an infinite prime sample of the envelope error. For instance,
$\delta=1$ and $R=\exp(A^{1/4}\log A)$ make both displayed added
allowances tend to zero as $A\to\infty$; this is asymptotic, since
$C_\psi$ has not been numerically certified. It gives no starting clock
and no claim that evaluating this finite prime sum is inexpensive.

At the unchanged conditional least global Robin-ratio maximizing
integer, a sufficiently strong upper estimate on the actual
$\mathcal J_{A,\delta}(R)$ would still be needed to pay the strict
core after (CP4). No such main estimate is supplied. The original
$F_A$, actual zero multiset, complete elementary contributions and
unbounded Robin/RH goal remain unchanged; no compact spectral
truncation or RH inference follows from additive exponential type.
This is a paper-level comparison, not a Lean-verified result.

## Joint short-interval cancellation in the Gamma comparison

The allowance in (GP6) discards the cancellation between the two sides
of the original cutoff. The uniform short-interval input already
recorded in the [Guth–Maynard note](../Analytic/guthmaynard2024largevalues.md),
Corollary 1.3 of [arXiv:2405.20552v2](https://arxiv.org/abs/2405.20552v2),
supplies a two-sided comparison with a smaller admissible Gamma shape.
The global PNT input is the Fiori–Jaskari theorem quoted above. These
source theorems, the absolute centering in (GP4)–(GP5), and the full
combined remainder (GR1) are reused. The following is a paper-level
application, without mathematical-priority or Lean-verification claims.

Retain $A\to\infty$, $L=\log A$, $D(t)=\psi(t)-t$, $h_A,w_c,J_\alpha$
and the Gamma law from (GP1)–(GP5). Define

$$
\begin{aligned}
\eta_0(A)&=\sup_{t\ge A}\frac{|D(t)|}{t},\\
\eta_{\rm si}(A)&=
\sup_{\substack{A/2\le u<v\le3A/2\\v-u\ge A^{2/3}}}
\frac{|D(v)-D(u)|}{v-u}.
\end{aligned}
\tag{GS1}
$$

There are absolute constants $K,c>0$ such that, for all sufficiently
large $A$ and every noninteger $\alpha\ge4$,

$$
\boxed{\begin{aligned}
\sqrt A L|J_1(A)-J_\alpha(A)|\le K\bigg\{&
\frac{\sqrt A}{\alpha}
 [\eta_0(A)+\eta_{\rm si}(A)+A^{-1/30}]\\
&+\sqrt{A\alpha}\,A^{-9/10}
 +\sqrt A e^{-c\alpha}\bigg\}.
\end{aligned}}
\tag{GS2}
$$

The starting value and constants are not numerically certified. This
is an asymptotic comparison, not an additional finite Robin clock.

### The local prime input and its uniform range

The retained global PNT theorem gives, for some fixed $c_0>0$,

$$
\eta_0(A)\ll
\exp\left[-c_0\frac{L^{3/5}}{(\log L)^{1/5}}\right].
\tag{GS3}
$$

Use Guth–Maynard Corollary 1.3 with the fixed parameter $\epsilon=1/20$.
For $u\in[A/2,3A/2]$ and $A^{2/3}\le h\le A^{9/10}$, its required
range $u^{37/60}\le h\le u^{0.99}$ holds uniformly for sufficiently
large $A$. Multiplying the prime count by $\log u$ introduces an error
$O(h^2/(A L))$ from the variation of $\log p$. Thus

$$
\vartheta(u+h)-\vartheta(u)
=h+O\bigl(h[L e^{-L^{1/4}}+A^{-1/10}]\bigr).
$$

Here $(\log u)^{1/4}=L^{1/4}+O(L^{-3/4})$ uniformly. If
$A^{9/10}<h\le A$, with $u+h\le3A/2$, partition into equal pieces of lengths between
$A^{9/10}/2$ and $A^{9/10}$ and add the same estimates. The classical
Chebyshev bound and prime-power identity give
$\psi(t)-\vartheta(t)=O(\sqrt t)$; paying this at the two endpoints,
with $h\ge A^{2/3}$, proves

$$
\boxed{\eta_{\rm si}(A)\ll
 L e^{-L^{1/4}}+A^{-1/10}+A^{-1/6}.}
\tag{GS4}
$$

This uses the uniform corollary, not the separate almost-all theorem.
It neither assumes a short-interval relative error from global PNT
nor substitutes $\pi$ or $\vartheta$ for $\psi$ without paying prime
powers.

### Remove only the exactly centered linear dilation

Choose the following endpoint convention and retain it in the prime
sum:

$$
a_A(t)=
\begin{cases}
-1/(AL),&0<t\le A,\\
1/(t\log^2t),&t>A.
\end{cases}
\qquad
B_c(t)=w_c(t)-h_A(t)-(c-1)a_A(t).
\tag{GS5}
$$

Both $a_A$ and $w_c-h_A$ are absolutely integrable against $dt$ and
$d\psi(t)$; for the latter use (GP4). Moreover
$\int_0^\infty a_A(t)\,dt=-1/L+1/L=0$ and
$\int_0^\infty(w_c-h_A)\,dt=0$. The absolute $d\psi+dt$ norm of
$a_A$ is $O(1/L)$ by Chebyshev and partial summation. Consequently
(GP5), Fubini, and $\mathbb E(C-1)=0$ give the unchanged arithmetic
difference

$$
\boxed{J_1-J_\alpha
 =\mathbb E\int_0^\infty B_C(t)\,dD(t).}
\tag{GS6}
$$

No divergent pole and prime quantities are separated in this identity.

For $1/2\le c\le3/2$, put $e=c-1$ and split $B_c=b_c+v_c$, where

$$
b_c(t)=
\begin{cases}
e^2/(cAL),&0<t\le A,\\[2pt]
\displaystyle\frac1{t(\log t-\log c)}-
 \frac1{t\log t}-\frac e{t\log^2t},&t>A.
\end{cases}
\tag{GS7}
$$

This regular part agrees with $B_c$ outside the interval between $A$
and $cA$. Taylor's theorem in $c$, uniformly on $[1/2,3/2]$, gives

$$
|b_c(t)|\ll\frac{e^2}{t\log^2t},\qquad
|b_c'(t)|\ll\frac{e^2}{t^2\log^2t}\qquad(t>A).
$$

Partial summation on $(A,\infty)$, together with the constant part on
$(0,A]$, therefore yields

$$
\left|\int_0^\infty b_c(t)\,dD(t)\right|
\ll\eta_0(A)e^2/L.
\tag{GS8}
$$

In particular, the boundary contribution is paid using $D(A)$; the
change of formula at $A$ has not been ignored.

The local residual $v_c$ is zero outside the closed interval with
endpoints $A,cA$. Inside that interval its nonzero formula is

| Dilation | Interval | *v*<sub>*c*</sub>(*t*) |
| --- | --- | --- |
| *c* &gt; 1 | *A* &lt; *t* &lt; *c* · *A* | 1 / (*c* · *A* · *L*) − 1 / (*t* · log(*t* / *c*)) |
| *c* &lt; 1 | *c* · *A* &lt; *t* &lt; *A* | 1 / (*t* · log(*t* / *c*)) − 1 / (*c* · *A* · *L*) |

The actual endpoint values are those of $B_c-b_c$ in (GS5)–(GS7).
The first derivative of $1/[t\log(t/c)]$ is $O(1/(A^2L))$ in this
interval. Including the possible jump at $A$ gives

$$
\|v_c\|_\infty+\operatorname{Var}(v_c)
\ll |e|/(AL).
\tag{GS9}
$$

### Pay the shrinking cutoff interval, including its atoms

Set $H_0=A^{2/3}$, $H_1=A^{7/10}$ and $h=A|e|$. For
$h\ge H_1$, (GS1) bounds $|D(t)-D(A)|$ by
$\eta_{\rm si}(A)h$ whenever $|t-A|\ge H_0$. For smaller distances,
monotonicity of $\psi$ and (GS4) applied to
$[A-H_0,A+H_0]$ give the bound $O(H_0)$. Since
$H_0/H_1=A^{-1/30}$, it follows uniformly on the support of $v_c$ that

$$
|D(t)-D(A)|\ll
[\eta_{\rm si}(A)+A^{-1/30}]h.
$$

The same bound holds for one-sided limits after paying a possible
endpoint prime-power atom of size at most $\log(2A)=O(\log A)$,
absorbed in $H_0$. Integration of a bounded-variation function against
these increments, using (GS9), gives

$$
\left|\int v_c(t)\,dD(t)\right|
\ll [\eta_{\rm si}(A)+A^{-1/30}]e^2/L
\qquad(H_1\le h\le A/2).
\tag{GS10}
$$

For $h<H_1$, the support lies in $[A-H_1,A+H_1]$. Its total
$d\psi+dt$ mass is $O(H_1)$ by (GS4), with the endpoint atom included.
Therefore
$|\int v_c\,dD|\ll |e|H_1/(AL)$. The maximum of the Gamma density
is $O(\sqrt\alpha)$ uniformly for $\alpha\ge4$, by the standard
Stirling bound at its mode. Hence

$$
\begin{aligned}
\mathbb E[|C-1|\mathbf1_{\{|C-1|<H_1/A\}}]
 &\ll\sqrt\alpha(H_1/A)^2,\\
\sqrt A L\,
\mathbb E\left[\left|\int v_C\,dD\right|
                  \mathbf1_{\{|C-1|<H_1/A\}}\right]
 &\ll\sqrt{A\alpha}\,A^{-9/10}.
\end{aligned}
\tag{GS11}
$$

For the remaining event $C\notin[1/2,3/2]$, (GP4) and the absolute
norm of $a_A$ give
$|\int B_c\,dD|\ll(1+c+c^{-1})/L$ for every $c>0$.
The Gamma moment-generating function and Chernoff's inequality give
$\Pr(C\notin[1/2,3/2])\le2e^{-c_1\alpha}$ for an absolute
$c_1>0$. The second moment of $1+C+C^{-1}$ is bounded uniformly for
$\alpha\ge4$, using
$\mathbb EC^2=1+1/\alpha$ and
$\mathbb EC^{-2}=\alpha^2/[(\alpha-1)(\alpha-2)]$.
Cauchy–Schwarz thus pays the entire event by
$O(\sqrt A e^{-c_1\alpha/2})$ after normalization. In particular no
scales with $cA<1$ have been discarded.

Finally average (GS8) and (GS10), use
$\mathbb E(C-1)^2=1/\alpha$, and add (GS11) and this Gamma tail.
This proves (GS2) uniformly over its stated shapes.

### A smaller shape family with vanishing full comparison error

Fix $0<b_-\le b_+<\infty$, and take any noninteger shape satisfying

$$
b_-a_*(A)\le\alpha\le b_+a_*(A),
\qquad a_*(A)=\sqrt A\,e^{-L^{1/4}/2}.
\tag{GS12}
$$

For $b_-=1/2$ and $b_+=2$, for example,
$\alpha=\lfloor a_*(A)\rfloor+1/2$ is lawful eventually.
The first term of (GS2), using (GS3)–(GS4), is
$O_{b_-,b_+}(L e^{-L^{1/4}/2})$. The small-interval term is
$O_{b_-,b_+}(A^{-3/20}e^{-L^{1/4}/4})$, and the Gamma tail is smaller.
Reusing the complete elementary remainder in (GR1) gives

$$
\boxed{-\sqrt A L I_\psi(A)
 =\sqrt A L Z_\alpha(A)
  +O_{b_-,b_+}(L e^{-L^{1/4}/2}) .}
\tag{GS13}
$$

Every zero in $Z_\alpha$ still has its actual real part,
multiplicity and height, and the coefficient remains
$H_\alpha(\rho)F_A(\rho)$. No main spectral response has been bounded.
In (GS12) the old allowance $\sqrt A/\alpha$ diverges, whereas the
joint arithmetic comparison tends to zero. This is the gained
transport regime; it supplies neither a sign nor a finite numerical
threshold for the remaining main response.

At the same conditional least integer $N>5040$ attaining the global
Robin-ratio maximum, this estimate uses $A=\log N$ without changing
the selected source, the strict core, or the existing conclusion
$A>10^{45}$. The asymptotic starting point in (GS2) has not been
numerically compared with this finite exclusion. A full signed upper
bound for $Z_\alpha(A)$ with enough strict slack remains required.
Robin's criterion and RH remain
unproved by these applications.

## Reusing the coefficient remainder on a larger finite clock

Keep the same conditional least integer $N>5040$ attaining the global
Robin-ratio maximum under the Robin-violation hypothesis. The preceding
finite-clock application already gives $A=\log N>10^{45}$; put
$L=\log A$. The following application uses the existing coefficient
remainder (H1), directed comparison (GE5), Gamma damping (GH1), verified
height and complete zero-count bound. It does not construct a new
smoothing transform or repeat their proofs.

### Use the full coefficient remainder separately on the two height ranges

The existing (H1) and its numerator estimate give, throughout the actual
critical strip $0<\beta<1$,

$$
\sqrt A L|F_A(\beta+it)|
\le(1+1/L)\frac{A^{\beta-1/2}}{|\beta+it||1-\beta-it|}
\left(1+\frac{2(L+2)}{L(L+1)|1-\beta-it|}\right).
\tag{GJ1}
$$

This retains the complete original coefficient, including its remainder;
it sharpens the coarser factor two in (GH2) by direct use of the already
available estimate. No zero coefficient is replaced by only its leading
term. For $L>78$, the verified critical head has
$|1-\rho|\ge1/2$, so its parenthesized factor is less than $1.054$:

$$
\frac{4(L+2)}{L(L+1)}
<\frac{4\cdot80}{78\cdot79}<0.054.
$$

For the actual unverified tail $|t|>H=3\cdot10^{12}$,
$|1-\rho|\ge|t|>H$ instead bounds that factor by $1.0001$.
Criticality is used only on the verified head. The original real parts
and the complete infinite multiset of tail zeros are retained.

Using the same positive $c_0$ identity, both ordinate signs and (GH1),
(GJ1) gives the finite bound

$$
\sqrt A L|Z_\alpha(A)|
<M_1(\alpha)(1+1/L)
\left[1.054c_0+2(1.0001)\sqrt A S_2(H)
 \exp\left(-\frac{H^2}{2(\alpha+H)}\right)\right].
\tag{GJ2}
$$

Here $M_1(\alpha)=\alpha/(\alpha-1)$, $c_0<0.05$ and
$S_2(H)<1.48\cdot10^{-12}$ are the same previously paid quantities.
In particular, this argument does not need a new verified height or a
new zero enumeration.

### Pay the complete response on the added interval

Take the exact noninteger shape and additional interval

$$
\alpha=\frac{29}{20}10^{23}+\frac12,
\qquad 10^{45}<A\le10^{46}.
$$

Then $L>78$, $\sqrt A\le10^{23}$,
$M_1(\alpha)<1.0001$, and

$$
\frac{H^2}{2(\alpha+H)}>31,
\qquad e^{31}>10^{13}.
$$

For the exponential inequality, $e>8/3$ and
$8^{31}>10^{13}3^{31}$ suffice. The head and complete tail in (GJ2)
therefore obey the exact rational budgets

$$
(1.0001)(1.02)(1.054)(0.05)<0.054,
$$

$$
2(1.0001)^2(1.02)(10^{23})
 (1.48\cdot10^{-12})10^{-13}<0.031.
\tag{GJ3}
$$

For the arithmetic comparison term, reuse
[Dusart's Theorem 5.2 and Proposition 3.2](../Weil/dusart2010estimates.md).
The original v1 theorem's $k=2$, $\eta_2=3.965$, $x_2=2$ row and the
complete prime-power correction give

$$
\frac{\psi(A)}A
<1+\frac{3.965}{L^2}+1.00007A^{-1/2}+1.78A^{-2/3}
<1.001.
$$

The final inequality follows from $3.965/78^2<0.0007$ and
$1.00007\cdot10^{-22}+1.78\cdot10^{-30}<0.0003$.
The source row applies throughout the added interval; no asymptotic
starting threshold is substituted for its explicit $x_2=2$.
Since $\alpha-1>1.4499\cdot10^{23}$, the two remaining terms of (GE5)
satisfy

$$
\frac{\psi(A)}{(\alpha-1)\sqrt A}
<\frac{1.001}{1.4499}<0.691,
\qquad
\frac{5M_1(\alpha)}{\sqrt A}<6\cdot10^{-22}.
\tag{GJ4}
$$

Combining (GE5) with (GJ2)–(GJ4) pays the original full signed response:

$$
\boxed{-\sqrt A L I_\psi(A)
<0.054+0.031+0.691+6\cdot10^{-22}<0.777,
\qquad 10^{45}<A\le10^{46}.}
\tag{GJ5}
$$

All elementary and trivial contributions, including Gamma scales below
the unit cutoff, are retained through the already proved (GE5).
The strict core for this same selected source still gives
$\sqrt A L D^*(A)>\mathcal E(L)>0.778$. Hence

$$
\boxed{\sqrt A L\Delta(N)>0.001,
\qquad 10^{45}<A\le10^{46}.}
\tag{GJ6}
$$

Together with the preceding $A>10^{45}$ restriction, this forces
$\log N>10^{46}$ for the same hypothetical least global maximizer.
It is a paper-level enlargement of the excluded selected-source window,
with no new classical theorem, priority claim, Lean certification or
all-integer finite Robin verification. The fixed verified height and
shape still provide no uniform main bound as $A\to\infty$; the complete
unbounded signed Robin target and RH remain unproved.

## An effective directed Gamma comparison retaining the cutoff sign

Retain the original $h_A,w_c,J_1,J_\alpha,D=\psi-\mathrm{id}$ and
the endpoint convention in (GS5). Reuse the absolutely convergent
centering (GP4)–(GP5), (GS6), and the decomposition (GS7)–(GS9).
The following explicit upper comparison preserves the sign of the local
residual against the actual nonnegative prime-power measure. No new
short-interval theorem or smoothing transform is required.

For $A\ge e^{78}$, $L=\log A$, and every noninteger $\alpha\ge4$, put
$\eta_0(A)=\sup_{t\ge A}|\psi(t)-t|/t$ as in (GS1). Then

$$
\boxed{\sqrt A L[J_1(A)-J_\alpha(A)]
\le [0.52+2\eta_0(A)]\frac{\sqrt A}{\alpha}
 +400\sqrt A\,e^{-\alpha/60000}.}
\tag{GK1}
$$

This is a directed inequality. The absolute asymptotic comparison
(GS2) retains its stated scope; (GK1) supplies explicit constants without
assigning a numerical starting point to that asymptotic result.

### Pay the regular part using only the global error

Fix $99/100\le c\le101/100$ and write $e=c-1$. For $t>A$, put
$v=\log t$ and $u(c,t)=1/[t(v-\log c)]$. Its derivatives are

$$
\partial_c^2u=
\frac{2-(v-\log c)}{t c^2(v-\log c)^3},\qquad
\partial_t\partial_c^2u=
\frac{(v-\log c)^2-6}{t^2c^2(v-\log c)^4}.
$$

Throughout the segment joining $1$ to $c$, one has
$v-\log c\ge v-1/100\ge(999/1000)v$ and $c\ge99/100$.
Taylor's formula and
$[(99/100)^2(999/1000)^2]^{-1}<1.024$ therefore give

$$
|b_c(t)|\le\frac{0.512e^2}{t\log^2t},\qquad
|b_c'(t)|\le\frac{0.512e^2}{t^2\log^2t}\quad(t>A).
\tag{GK2}
$$

On $(0,A]$, the same existing regular part equals
$e^2/(cAL)$. Partial summation against $D$, including its actual value
at $A$ and the change of formula there, gives

$$
\int b_c\,dD=
\left[\frac{e^2}{cAL}-b_c(A+)\right]D(A)
 -\int_A^\infty D(t)b_c'(t)\,dt.
$$

The upper boundary vanishes by the global PNT input already used in
(GS3). Applying (GK2), $|D(t)|\le\eta_0(A)t$ for all $t\ge A$, and
$\int_A^\infty dt/(t\log^2t)=1/L$ yields

$$
\left|\int b_c\,dD\right|
\le\frac{\eta_0(A)e^2}{L}
 \left[\frac{100}{99}+0.512+\frac{0.512}{L}\right]
 \le\frac{2\eta_0(A)e^2}{L}.
\tag{GK3}
$$

This uses a bound on the regular part against the global error; no
short-interval bound has been inferred from global PNT.

### Retain the negative local residual, including the endpoint atoms

The actual local residual $v_c=B_c-b_c$ from (GS5)–(GS7) is
nonpositive. For $c>1$ its formula on $A<t<cA$ is
$1/(cAL)-1/[t\log(t/c)]$, and $v_c(A)=v_c(cA)=0$.
For $c<1$ its formula on $cA<t\le A$ is
$1/[t\log(t/c)]-1/(cAL)$, with $v_c(cA)=0$.
It is zero elsewhere. Since $1/[t\log(t/c)]$ decreases with $t$ on
these intervals, both displayed formulas are nonpositive. These values
also fix the sign at a possible prime-power atom at $A$ or $cA$.

Consequently the actual measure $d\psi\ge0$ gives

$$
\int v_c\,dD=\int v_c\,d\psi-\int v_c\,dt
\le-\int v_c\,dt.
$$

On the entire interval with endpoints $A,cA$,
$t\ge(99/100)A$ and $\log(t/c)\ge L-1/100$. Thus

$$
\left|\frac{d}{dt}\frac1{t\log(t/c)}\right|
\le\frac{1.034}{A^2L}.
$$

Indeed, the ratio to $1/(A^2L)$ is at most
$[(99/100)^2]^{-1}[L/(L-1/100)][1+1/(L-1/100)]<1.034$
for $L\ge78$. The local residual vanishes at $cA$, so integrating
the resulting triangular upper bound gives

$$
\boxed{\int v_c\,dD
\le\frac{1.034(A|e|)^2}{2A^2L}
 \le\frac{0.52e^2}{L}.}
\tag{GK4}
$$

An atom contributes to the nonpositive prime term; it is not replaced
by a Lebesgue density or discarded with an unknown sign.

### Pay all Gamma scales outside the narrow interval

An explicit global bound needed only for this tail follows directly
from the existing Dusart Theorem 5.2 $k=0$ row and Proposition 3.2:
$\psi(t)\le4t$ for $t>0$. For $t<2$, $\psi(t)=0$; for $t\ge2$ use
$\vartheta(t)<2t$ and
$1.00007t^{-1/2}+1.78t^{-2/3}<2$.
Applying the already established (GP4) estimates with this constant
gives, for every $c>0$,

$$
\int|w_c-h_A|\,d\psi\le\frac{16(c+c^{-1})}{L},\qquad
\int|w_c-h_A|\,dt\le\frac{4(c+c^{-1})}{L}.
$$

For clarity, below $A\max(1,c)$ the corresponding bound with
$\psi(t)\le Bt$ is $2B(c+c^{-1})/L$. Above that point it is also
$2B(c+c^{-1})/L$: use the logarithmic difference and
$|\log c|+\tfrac12(\log c)^2\le c+c^{-1}$, since $L\ge2$.
This is a numerical use of the existing all-scale convergence argument.
The affine derivative in (GS5) satisfies
$\int|a_A|\,(d\psi+dt)\le14/L$ by the same partial summation.
Since $|c-1|\le c+c^{-1}$, these estimates pay the complete centered
kernel, with room in the constant:

$$
\left|\int B_c\,dD\right|
\le\frac{100(c+c^{-1})}{L}\qquad(c>0).
\tag{GK5}
$$

This includes every scale with $cA<1$. Only absolutely convergent
differences are integrated, as in (GP4)–(GP5).

Let $C$ have the same mean-one Gamma law with shape and rate $\alpha$.
Use its existing moment-generating function and Chernoff bound with
$\delta=1/100$. The two exponents satisfy
$\delta-\log(1+\delta)\ge\delta^2/[2(1+\delta)]>1/30000$ and
$-\delta-\log(1-\delta)\ge\delta^2/2>1/30000$. Therefore

$$
\Pr(C\notin[99/100,101/100])\le2e^{-\alpha/30000},\qquad
\mathbb E(C+C^{-1})^2
\le\frac54+2+\frac83<6.
$$

Cauchy–Schwarz and (GK5) bound the normalized contribution from that
whole event by $400\sqrt A e^{-\alpha/60000}$. On its complement,
(GK3)–(GK4) apply. Averaging with
$\mathbb E(C-1)^2=1/\alpha$ proves (GK1) using the globally centered
identity (GS6). No conditional mean-one assertion has been used.

### Preserve the complete original zero response

Reusing $J_1=-I_\psi$, $J_\alpha=Z_\alpha+\overline R_\alpha$ and
the full elementary upper bound (GE4) gives

$$
\boxed{\begin{aligned}
-\sqrt A L I_\psi(A)\le{}&\sqrt A L Z_\alpha(A)
 +[0.52+2\eta_0(A)]\frac{\sqrt A}{\alpha}\\
&+400\sqrt A e^{-\alpha/60000}
 +\frac{5M_1(\alpha)}{\sqrt A}.
\end{aligned}}
\tag{GK6}
$$

Here $Z_\alpha$ retains the original $H_\alpha(\rho)F_A(\rho)$,
every actual real part, multiplicity and height. The improvement is an
effective directed arithmetic payment obtained from the retained local
sign, not a new bound on the main response. The unbounded signed Robin
estimate and RH remain unproved. This is a paper-level application of
the existing prime bounds and kernel identities, without a mathematical
priority or Lean-certification claim.

## A further finite clock from the effective cutoff-sign payment

Keep the same conditional least integer $N>5040$ attaining the global
Robin-ratio maximum under the Robin-violation hypothesis. The preceding
application already excludes $A=\log N\le10^{46}$; put $L=\log A$.
Apply (GK6) on the additional interval

$$
10^{46}<A\le\frac72\,10^{46},\qquad
\alpha=\frac75\,10^{23}+\frac12.
$$

This uses the effective directed comparison, the full original
coefficient bound (GJ1), Gamma damping (GH1), and the existing complete
elementary remainder. No primes, arithmetic profiles or zero ordinates
are newly enumerated.

### Pay the actual global arithmetic error

Dusart's original Theorem 5.2 $k=2$, $\eta_2=3.965$, $x_2=2$ row and
Proposition 3.2, already used in (GJ4), give for every $t\ge A$

$$
\frac{|\psi(t)-t|}{t}
\le\frac{3.965}{\log^2t}+1.00007t^{-1/2}+1.78t^{-2/3}
<0.001.
$$

Hence $\eta_0(A)<0.001$. Moreover $L>78$,
$\sqrt A<1.871\cdot10^{23}$ and $\alpha\ge1.4\cdot10^{23}$.
The normalized central comparison term in (GK6) is therefore

$$
[0.52+2\eta_0(A)]\frac{\sqrt A}{\alpha}
<\frac{0.522(1.871)}{1.4}<0.698.
\tag{GL1}
$$

The Gamma tail is explicit: $\alpha/60000>10^{18}$ and
$e^x>x^3/6$ for $x>0$ imply $e^{\alpha/60000}>10^{53}$.
Thus $400\sqrt A e^{-\alpha/60000}<8\cdot10^{-28}$.
The entire elementary contribution is less than $6\cdot10^{-23}$ by
(GE4). This includes Gamma scales below the unit cutoff.

### Pay every original zero above the verified height

The existing (GJ2) gives, with $H=3\cdot10^{12}$,

$$
\sqrt A L|Z_\alpha(A)|
<M_1(\alpha)(1+1/L)
\left[1.054c_0+2(1.0001)\sqrt A S_2(H)
 e^{-H^2/[2(\alpha+H)]}\right].
$$

Here $c_0<0.05$, $S_2(H)<1.48\cdot10^{-12}$ and
$M_1(\alpha)<1.0001$ are unchanged. For the selected shape,
$H^2/[2(\alpha+H)]>32$ and $e^{32}>4\cdot10^{13}$;
the latter follows from $e>8/3$ and
$8^{32}>4\cdot10^{13}3^{32}$. Both ordinate signs, the actual tail
real parts and all heights to infinity remain included. The head and
tail satisfy the exact rational budgets

$$
(1.0001)(1.02)(1.054)(0.05)<0.054,
$$

$$
2(1.0001)^2(1.02)(1.871\cdot10^{23})
 (1.48\cdot10^{-12})(4\cdot10^{13})^{-1}<0.015.
\tag{GL2}
$$

Combining (GK6), (GL1) and (GL2) pays the original full signed response:

$$
\boxed{-\sqrt A L I_\psi(A)
<0.054+0.015+0.698+8\cdot10^{-28}+6\cdot10^{-23}
<0.768.}
\tag{GL3}
$$

The same selected source obeys the strict core
$\sqrt A L D^*(A)>\mathcal E(L)>0.778$ and
$\Delta(N)=I_\psi(A)+D^*(A)$. Therefore

$$
\boxed{\sqrt A L\Delta(N)>0.01,
\qquad10^{46}<A\le\frac72\,10^{46}.}
\tag{GL4}
$$

Together with the preceding exclusion, this forces
$\log N>(7/2)10^{46}$ for the same hypothetical least global maximizer.
It is a selected-source finite exclusion with a normalized margin,
not an all-integer finite Robin verification or an unbounded main
estimate. The full RH objective remains unproved. All classical prime,
zero-count and verified-height inputs are reused; this paper-level
application carries no mathematical-priority or Lean-certification claim.

## Absolute full-weight cost at a fixed negative heat time

Keep the same conditional least global Robin-ratio maximizer $N$, the
arithmetic clock $A=\log N>(7/2)10^{46}$, and $L=\log A$. The result
below also holds for every fixed $A>1$. It concerns a particular
absolute transport through negatively deformed zeros; it supplies no
upper bound for the original signed response $-\sqrt A L I_\psi(A)$.

The inputs are Alexander Dobner, *A proof of Newman's conjecture for
the extended Selberg class*, [Acta Arithmetica 201 (2021), 29–62](https://doi.org/10.4064/aa200603-23-7), inspected in
[arXiv:2005.05142v2](https://arxiv.org/html/2005.05142v2), Theorems 4–5,
Lemma 3 and §3.1, and the NIST DLMF
[principal exponential integral](https://dlmf.nist.gov/6.2#E1) and
[sector asymptotic expansion](https://dlmf.nist.gov/8.20#E2).
These published results are reused as `literature-attested` inputs.
The combined full-weight convergence restriction is a `repo-derived`
paper-level source application; no
mathematical-priority or Lean-certification claim is made.

### Continue the complete coefficient, keeping its cancellation

For $0<\Re s<1$, put $v=\log u$ in the unchanged coefficient (M1).
The DLMF principal $E_1$ definition and one integration by parts give

$$
\begin{aligned}
F_A(s)
&=\frac1s\int_L^\infty e^{(s-1)v}
                 \left(\frac1v+\frac1{v^2}\right)\,dv\\
&=\frac{A^{s-1}}{sL}+E_1((1-s)L).
\end{aligned}
\tag{NH1}
$$

Thus the right side defines the natural principal continuation
$\widehat F_A$ on $\mathbb C\setminus(\{0\}\cup[1,\infty))$.
Continuation defines these individual terms beyond the integral's
half-plane of convergence; it does not itself establish a spectral
transport identity.

Let $s=x+iy$, $y\to+\infty$, with $|x|\le B\log y$ for a fixed $B$.
Then $z=(1-s)L$ lies, eventually, in $|\arg z|\le3\pi/4$.
DLMF (8.20.2), with its parameter $p=1$, supplies uniformly there

$$
E_1(z)=e^{-z}\left(z^{-1}-z^{-2}+O(|z|^{-3})\right).
$$

Substitution into the **full** (NH1) yields

$$
\begin{aligned}
\widehat F_A(s)
&=A^{s-1}\left(
 \frac1{Ls(1-s)}-\frac1{L^2(1-s)^2}+O_{A,B}(y^{-3})\right)\\
&=\frac{1+L}{L^2}\frac{A^{s-1}}{y^2}
       \left(1+O_{A,B}\!\left(\frac{\log y}{y}\right)\right).
\end{aligned}
\tag{NH2}
$$

The terms $1/(sL)$ and $1/((1-s)L)$ cancel at order $y^{-1}$.
The $-z^{-2}$ term supplies the additional $1/L^2$ in the nonzero
leading coefficient. Neither part of the original weight has been
discarded. All asymptotics here fix $A$ before taking the height limit.

### Obtain enough distinct actual zeros from the source's shifts

Fix one $\epsilon>0$ throughout and use Dobner's heat parameter
$t=-\epsilon$. In the Riemann specialization his equations (11)–(12)
give

$$
D_\epsilon(s)=\sum_{n\ge1}
 e^{-\epsilon\log^2 n/4}n^{-s},\qquad
J_\epsilon(s)=s+\frac\epsilon4\operatorname{Log}\frac{s}{2\pi}.
\tag{NH3}
$$

The completion has the normalization
$\xi_t((1+iz)/2)=8H_t(z)$, with the same heat time $t$.
These are deformed $\xi_{-\epsilon}$ zeros, not original zeta zeros.

Dobner's Lemma 3 supplies a zero of $D_\epsilon$. His §3.1 proof,
using Theorems 4–5, supplies actual zeros of
$\xi_{-\epsilon}(J_\epsilon(s))$ in sufficiently high translates
of one fixed zero-isolating circle of radius $r$. The same shift
sequence satisfies

$$
\liminf_{m\to\infty}(\tau_{m+1}-\tau_m)>0,
\qquad \limsup_{m\to\infty}\frac{\tau_m}{m}<\infty.
$$

In particular $\tau_m\asymp_\epsilon m$. Choose $d>0$ such that
the consecutive gaps are eventually at least $d$, and retain every
$q$-th shift, where $qd>2r+\epsilon\pi/4$. On the upper half-plane,
$J_\epsilon$ adds an imaginary offset in $(0,\epsilon\pi/4)$.
Consequently the images of the retained circles have disjoint height
intervals. Choosing one actual zero in each produces **distinct**
zeros $w_m$ of the same $\xi_{-\epsilon}$ with

$$
\Im w_m\asymp_\epsilon m,\qquad
\Re w_m=\frac\epsilon4\log(\Im w_m)+O_\epsilon(1).
\tag{NH4}
$$

This uses the source's shift-density information, not merely the
existence of infinitely many zeros. The selected preimages stay in
one fixed bounded real strip, and $\Im J_\epsilon(s)=\Im s+O_\epsilon(1)$,
which proves the real-part statement in (NH4).

### A necessary absolute-budget condition, including equality

Write $\kappa=\epsilon L/4$. Equations (NH2) and (NH4) imply, for
all sufficiently large $m$,

$$
|\widehat F_A(w_m)|\asymp_{A,\epsilon}m^{\kappa-2}.
\tag{NH5}
$$

The constants are positive because $(1+L)/L^2>0$ and
$A^{\Re w_m-1}\asymp_{A,\epsilon}(\Im w_m)^\kappa$.
Hence, counting the actual deformed zeros with multiplicities,

$$
\boxed{
\epsilon\log A\ge4
\quad\Longrightarrow\quad
\sum_{\substack{\xi_{-\epsilon}(w)=0\\\Im w>0}}
 |\widehat F_A(w)|=\infty.}
\tag{NH6}
$$

At equality the selected subseries dominates the harmonic series;
for larger $\epsilon L$ it dominates a divergent power series.
Thus $\epsilon\log A<4$ is a **necessary** condition for this
principal-continued, complete-weight, absolute full-spectrum
transport. For $\epsilon\log A<4$, (NH5) makes this particular
selected subseries converge, but establishes no convergence or
uniform bound for the rest of the deformed spectrum.

The conclusion is about absolute cost at one fixed negative heat
time. It proves neither signed divergence nor a failure of Robin or
RH, and does not exclude transports that retain cancellation or use
additional comparison terms. Such a route still needs an all-height
identity and a paid signed error returning to the original zeros,
their real parts and multiplicities, the original elementary
correction and the strict core at the same $N$. No changing heat time
per zero, finite-spectrum truncation or unproved positive-time
certificate is used to discharge that obligation.

## The subcritical full-spectrum absolute boundary

The necessary condition (NH6) has a converse for every fixed $A>1$
and fixed $\epsilon>0$. The additional step is a uniform right-half-plane
comparison, not a use of Dobner's Theorem 4 outside its stated
$|\Re s|\le C(\Im s)^{1/4}$ range. Reuse his exact negative-heat
convolution (9), the Riemann completion, and the already retained
(NH1)–(NH6). The [DLMF digamma expansion (5.11.2)](https://dlmf.nist.gov/5.11#E2)
is used in its fixed sector $|\arg z|\le\pi/2$.
These are `literature-attested` inputs; the uniform comparison and
combined convergence boundary below are `repo-derived` paper-level
applications, with no mathematical-priority or Lean-certification claim.

### A uniform comparison on the entire right half-plane

Write

$$
\gamma(s)=\tfrac12s(s-1)\pi^{-s/2}\Gamma(s/2),\qquad
c=\epsilon/4,\qquad
J_\epsilon(s)=s+c\operatorname{Log}(s/(2\pi)),
$$

$$
\gamma_{-\epsilon}(s)=\gamma(s)
 \exp((s-J_\epsilon(s))^2/\epsilon).
$$

For fixed $\epsilon>0$, the comparison is

$$
\boxed{\frac{\xi_{-\epsilon}(J_\epsilon(s))}
 {\gamma_{-\epsilon}(s)}
 =D_\epsilon(s)+O_\epsilon(|s|^{-1}),
 \qquad \Re s\ge2,\quad |s|\longrightarrow\infty.}
\tag{NH7}
$$

Uniformity includes arbitrarily large $\Re s$, both ordinate signs,
and the real axis. It is not uniform in $\epsilon$ as $\epsilon\to0$.

Here is the required interface proof. The DLMF expansion gives uniformly
in this half-plane

$$
\frac{\gamma'}{\gamma}(s)
=\frac1s+\frac1{s-1}-\frac12\log\pi
 +\frac12\frac{\Gamma'}{\Gamma}(s/2)
=\frac12\operatorname{Log}(s/(2\pi))+O(|s|^{-1}).
$$

Its imaginary part is bounded on the whole half-plane: the principal
argument is bounded, and the remaining bounded part is covered by
continuity on a compact set. Consequently, for an absolute $M$ and
all real $v$,

$$
\left|\frac{\gamma(s+iv)}{\gamma(s)}\right|\le e^{M|v|}.
$$

Set

$$
R_s(v)=\frac{\gamma(s+iv)}{\gamma(s)}
 \exp\!\left(-\frac{iv}{2}\operatorname{Log}(s/(2\pi))\right),
\qquad r=|s|.
$$

Then $|R_s(v)|\le e^{(M+\pi/4)|v|}$ for all $v$. Integrating the
logarithmic derivative along the vertical segment, for
$|v|\le r^{1/4}$ and large $r$, gives

$$
|R_s(v)-1|\ll\frac{|v|+v^2}{r}.
$$

Indeed, $|s+iu|\ge r/2$ on that segment and
$|\operatorname{Log}(s+iu)-\operatorname{Log}s|\le2|u|/r$.
The integrated exponent is $O((|v|+v^2)/r)=o(1)$ uniformly on this
range. No bounded-real-part Stirling estimate is used at an unbounded
real part.

In Dobner's (9), shift the vertical contour to $\Re z=\Re s$ and
write $z=s+iv$. For each fixed $s$ this is a finite contour shift;
the Gaussian and the usual vertical decay kill the horizontal ends.
After division by $\gamma_{-\epsilon}(s)$ the exact identity is

$$
\frac{\xi_{-\epsilon}(J_\epsilon(s))}{\gamma_{-\epsilon}(s)}
=\frac1{\sqrt{\pi\epsilon}}\int_{\mathbb R}
 e^{-v^2/\epsilon}R_s(v)\zeta(s+iv)\,dv.
\tag{NH8}
$$

Replacing $R_s$ by $1$ gives exactly $D_\epsilon(s)$ by the Gaussian
Fourier integral and the absolutely convergent Dirichlet series.
On $\Re s\ge2$, $|\zeta(s+iv)|\le\zeta(2)$. The local difference
therefore has integral $O_\epsilon(r^{-1})$. On $|v|>r^{1/4}$ the
uniform exponential bound for $R_s$ gives
$O_\epsilon(\exp(-r^{1/2}/(2\epsilon)))=o_\epsilon(r^{-1})$.
This proves (NH7), without estimating every Dirichlet term separately.

### Every sufficiently high zero lies in a logarithmic region

On $\Re s\ge2$,
$|D_\epsilon(s)-1|\le\zeta(2)-1<1$.
The completion $\gamma_{-\epsilon}$ is nonzero there, so (NH7) shows
that $\xi_{-\epsilon}(J_\epsilon(s))\ne0$ for all sufficiently large
$|s|$ in this entire half-plane.

To cover the rightmost region, let $w$ have sufficiently large modulus
and satisfy
$\Re w\ge c\log(|w|/(2\pi))+3$.
Put $s_0=w-c\operatorname{Log}(w/(2\pi))$.
On $|s-s_0|=1/2$ one has $\Re s\ge5/2$ and

$$
J_\epsilon(s)-w=(s-s_0)
 +c[\operatorname{Log}(s/(2\pi))-
       \operatorname{Log}(w/(2\pi))].
$$

The second term is $O_\epsilon(\log|w|/|w|)<1/2$.
The logarithms and the intervening segments stay in the right
half-plane. Rouché's theorem gives a preimage $s$ inside the circle;
it satisfies $\Re s\ge2$ and $|s|\asymp|w|$.
Thus there is no such zero $w$. Apply the same argument to $1-w$ using
$\xi_{-\epsilon}(1-w)=\xi_{-\epsilon}(w)$.
Together these bounds imply, for every zero of sufficiently large
modulus,
$|\Re w|\le c\log|w|+O_\epsilon(1)$.
This forces $|\Im w|\to\infty$ with $|w|$ and then gives

$$
\boxed{1-c\log y-O_\epsilon(1)
 \le\Re w\le c\log y+O_\epsilon(1),
 \qquad y=\Im w\longrightarrow+\infty.}
\tag{NH9}
$$

All actual zeros are covered; this is not the lower-density subsequence
in (NH4). To replace $|w|$ by $y$, note that the bound on $|\Re w|$
precludes $|\Re w|\ge|\Im w|$ at arbitrarily large modulus, and hence
$|w|\le\sqrt2\,|\Im w|$ eventually.

### Count the whole spectrum and use the complete original coefficient

The original Fourier kernel $\Phi$ in Dobner's (2) is positive for
$u\ge0$: each summand has the positive factor
$2\pi n^2e^{4u}-3$. Evenness gives positivity on the whole real line.
For $|s-1/2|\le R$, its exact Fourier representation implies

$$
|\xi_{-\epsilon}(s)|
\le\int_{\mathbb R}\Phi(u)e^{2R|u|}\,du
\le2\xi_0(1/2+R),
\qquad \xi_{-\epsilon}(1/2)>0.
$$

Classical real Stirling growth gives a logarithm
$O(R\log(R+2))$ for the upper bound. Jensen's zero-count theorem,
applied at $1/2$ with radii $R$ and $2R$, therefore gives
$O_\epsilon(R\log(R+2))$ zeros in the disk, counted with multiplicities.
Together with (NH9), this gives the complete height count

$$
N_\epsilon(T)=\#\{w:\xi_{-\epsilon}(w)=0,\ 0<\Im w\le T\}
\ll_\epsilon T\log(T+2).
\tag{NH10}
$$

The bounded-height exceptions are finite by (NH9) and analyticity.
This step reuses the standard Jensen theorem, not an original-zeta
zero count applied to a different function.

Fix $A>1$ as well, write $L=\log A$ and $\kappa=\epsilon L/4$.
The retained complete-weight asymptotic (NH2), with (NH9), now gives
for every sufficiently high actual zero

$$
|\widehat F_A(w)|\ll_{A,\epsilon} (\Im w)^{\kappa-2}.
$$

For $\kappa<1$, the mass in a dyadic height band is at most
$O_{A,\epsilon}(j2^{j(\kappa-1)})$ by (NH10), and these bounds sum.
Thus the converse to (NH6) is

$$
\boxed{\sum_{\substack{\xi_{-\epsilon}(w)=0\\\Im w>0}}
 |\widehat F_A(w)|<\infty
 \quad\Longleftrightarrow\quad \epsilon\log A<4,
 \qquad A>1,\quad\epsilon>0.}
\tag{NH11}
$$

Every zero has its actual real part and multiplicity, and all positive
heights are retained. (NH6) supplies divergence at and above the
boundary; (NH7)–(NH10) supply full-spectrum convergence below it.
The tail below the boundary is
$O_{A,\epsilon}(T^{\kappa-1}\log(T+2))$ as $T\to\infty$,
with fixed parameters. No uniform allowance as $\epsilon\to0$ or
$\epsilon\log A\to4$ is asserted.

This determines the absolute convergence domain of the particular
continued complete-weight deformation. It provides no numerical
Robin budget, signed transport identity, or comparison error returning
to the original zero multiset. The same selected integer $N$,
$A=\log N>(7/2)10^{46}$, the original $F_A$, positive elementary
correction and strict core remain in the unproved target (G9).
In particular, absolute convergence of the deformed trace does not
prove its signed upper bound or RH.

## A joint small-negative-time comparison of the complete signed trace

The fixed-parameter convergence in (NH11) can be supplemented with a
quantitative comparison to the original trace. Reuse (NH8), its global
vertical ratio bound, the principal continuation (NH1), and the
all-spectrum count and convergence (NH9)–(NH11). The new interface is
uniform in the arithmetic clock and in small negative heat time; no
individual zero trajectories or zero-gap bounds are required.

Write $H_\epsilon=\xi_{-\epsilon}'/\xi_{-\epsilon}$, with $H_0$ for
the original completion. Define the full real trace

$$
Z_\epsilon(A)=\sum_{\xi_{-\epsilon}(w)=0}\widehat F_A(w).
$$

All zeros here are nonreal: positivity of the original Fourier kernel
makes $\xi_{-\epsilon}(x)>0$ for every real $x$. The trace includes both
ordinate signs and every multiplicity. At $\epsilon=0$ it is precisely
$Z_{\rm orig}(A)$ from (G9). The branch continuation is used for deformed
zeros with real part beyond $1$; their coefficients are not replaced
by convergent original integrals there.

There are absolute constants $\epsilon_0>0$ and $C<\infty$ such that

$$
\boxed{|Z_\epsilon(A)-Z_{\rm orig}(A)|\le C\epsilon A^2,
\quad A\ge e^2,\quad 0<\epsilon\le\epsilon_0,
\quad \epsilon\log A\le1.}
\tag{NH12}
$$

This is a `repo-derived` paper-level application of the retained
convolution and spectral interfaces, together with the standard Cauchy,
Hadamard and argument-principle theorems. It does not assert mathematical
priority, Lean certification, a numerical value of $C$ or
$\epsilon_0$, or a signed Robin upper bound.

### Center the small-time error before taking a logarithmic derivative

Keep $J_\epsilon,\gamma_{-\epsilon},R_s$ from (NH7)–(NH8), and set

$$
U_\epsilon(s)=
 \frac{\xi_{-\epsilon}(J_\epsilon(s))}{\gamma_{-\epsilon}(s)}.
$$

For $\Re s\ge2$, (NH8) gives the exact Gaussian average of
$R_s(v)\zeta(s+iv)$. The retained log-Gamma estimates imply that the
first two $v$ derivatives of this product are bounded uniformly for
$|v|\le1$ and $\Re s\ge2$. To see the needed uniformity, use

$$
\partial_v\log R_s(v)
=i\left[\frac{\gamma'}\gamma(s+iv)
 -\tfrac12\operatorname{Log}(s/(2\pi))\right].
$$

The bracket and its $v$ derivative are bounded there. The DLMF
sector estimate supplies the large-$|s|$ bound, Cauchy's derivative
estimate supplies its derivative, and the remaining compact region
has no Gamma pole or zero. The series for $\zeta,\zeta',\zeta''$ are
uniformly absolutely convergent in $\Re s\ge2$.

Taylor-expand the product at $v=0$ and subtract its linear term.
The centered Gaussian integrates that linear term to zero, while its
second moment is $\epsilon/2$. On $|v|>1$, the retained
$e^{(M+\pi/4)|v|}$ envelope pays the whole tail by $O(\epsilon)$ for
$0<\epsilon\le1/2$, including the subtracted affine term. Hence

$$
U_\epsilon(s)=\zeta(s)+O(\epsilon)
\quad(\Re s\ge2),
\tag{NH13}
$$

with an absolute constant. This improves the parameter dependence
needed here; (NH7)'s fixed-$\epsilon$ height estimate is not assigned
a uniform constant without proof.

Since $|\zeta(s)|\ge2-\zeta(2)>0$, choose an absolute
$\epsilon_0\le1/2$ small enough that $U_\epsilon$ is bounded away
from zero on the entire half-plane. On $\Re s=3$, Cauchy's estimate
on radius-$1/2$ disks also gives $U_\epsilon'-\zeta'=O(\epsilon)$.
The denominators are now paid, so
$U_\epsilon'/U_\epsilon-\zeta'/\zeta=O(\epsilon)$.

The exact normalization obeys

$$
\frac{\gamma_{-\epsilon}'}{\gamma_{-\epsilon}}(s)
=\frac{\gamma'}\gamma(s)
 +\frac\epsilon8\frac{\operatorname{Log}(s/(2\pi))}{s}.
$$

Consequently, on the whole line $\Re s=3$,

$$
K_\epsilon(s):=H_\epsilon(J_\epsilon(s))J_\epsilon'(s)
=H_0(s)+O(\epsilon),
\qquad |H_0(s)|\ll\log(|s|+2).
\tag{NH14}
$$

Both bounds have absolute constants. No function-value estimate is
substituted for a logarithmic-derivative estimate without this step.

### Transport the complete coefficient on these curves

Differentiating the exact (NH1), including its exponential-integral
part, gives

$$
\widehat F_A'(z)=A^{z-1}
 \left[\frac1{z(1-z)}-\frac1{Lz^2}\right],\qquad L=\log A.
\tag{NH15}
$$

This derivative is single-valued away from $0,1$; the original weight
itself still has its branch cut. Put $s=3+iy$, $r=|s|$,
$\kappa=\epsilon L/4\le1/4$, and

$$
Q_\epsilon(s)=\widehat F_A(J_\epsilon(s))
             +\widehat F_A(1-J_\epsilon(s)).
$$

On the segments from $s$ to $J_\epsilon(s)$ and their reflections,
$|z|,|1-z|\asymp r$. They remain respectively in the right and left
half-planes, and the first segment has the same ordinate sign at both
ends. Its real part is at most $3+(\epsilon/4)\max(\log(r/(2\pi)),0)$.
For bounded $r$, any analogous reflected increase is bounded by
$\epsilon L\le1$. Thus (NH15) gives

$$
|Q_\epsilon(s)-Q_0(s)|
 \ll\epsilon A^2\log(r+2)r^{\kappa-2}.
$$

One also has $|Q_0(s)|\ll A^2r^{-2}$ uniformly for $A\ge e^2$.
This full-coefficient bound can be obtained from (NH15) without losing
its cancellation: integrate from $3+iy$ to the corresponding imaginary
infinity, where (NH2) gives zero, and integrate $e^{iLt}$ once by
parts. The rational bracket is $O((1+t^2)^{-1})$ and its derivative
is $O((1+|t|^3)^{-1})$; $L\ge2$ pays the integration factor.
Use the same calculation on $-2-iy$, whose exponential factor is
$A^{-3}$. Each ordinate sign is treated on its own branch; at $y=0$
take the one-sided limits. It follows that

$$
\begin{aligned}
|Q_0(s)|&\ll A^2r^{-2},\\
|Q_\epsilon(s)|&\ll A^2\log(r+2)r^{\kappa-2},\\
|Q_\epsilon(s)-Q_0(s)|
 &\ll\epsilon A^2\log(r+2)r^{\kappa-2}.
\end{aligned}
\tag{NH16}
$$

No leading-term replacement of $\widehat F_A$ is used.

### The whole trace has an exact contour, cut and pole balance

Let $\Gamma_\epsilon$ be $J_\epsilon(3+i\mathbb R)$, oriented upward,
and put $b_\epsilon=J_\epsilon(3)$. The curve and its reflection enclose
all zeros. For completeness, $J_\epsilon$ is injective on $\Re s>2$:
the real part of

$$
\frac{J_\epsilon(s_1)-J_\epsilon(s_2)}{s_1-s_2}
=1+\frac\epsilon4\int_0^1
 \frac{dt}{s_2+t(s_1-s_2)}
$$

is positive. Its boundary line maps to a graph, since
$\Im J_\epsilon(b+iy)=y+(\epsilon/4)\arctan(y/b)$ is strictly
increasing and onto. Properness at infinity then identifies the
half-plane image with the region to the right of that graph.
By (NH13) there are no zeros in this image. The reflected exterior
is zero-free by the functional equation. In particular all zeros lie
between $\Gamma_\epsilon$ and $1-\Gamma_\epsilon$.

Use the argument principle in this intervening region, slit along
$[1,b_\epsilon]$ and with the pole at $0$ accounted for. The already
cited [DLMF (6.2.4)](https://dlmf.nist.gov/6.2#E4),
$E_1(z)=\operatorname{Ein}(z)-\operatorname{Log}z-\gamma$, shows

$$
\widehat F_A(x+i0)-\widehat F_A(x-i0)=2\pi i\quad(x>1),
\qquad \operatorname{Res}_{z=0}\widehat F_A(z)=\frac1{AL}.
$$

The upper side of the slit is traversed from $1$ to $b_\epsilon$;
its contribution is therefore
$\log(\xi_{-\epsilon}(b_\epsilon)/\xi_{-\epsilon}(1))$.
The logarithms here are real logarithms of positive values.
The circle at the logarithmic branch point $1$ tends to zero.
Reflection changes $H_\epsilon(1-z)$ to $-H_\epsilon(z)$,
so the two exterior curves combine into the exact balance

$$
\boxed{
Z_\epsilon(A)=\frac1{2\pi i}
 \int_{3-i\infty}^{3+i\infty}Q_\epsilon(s)K_\epsilon(s)\,ds
 +\log\frac{\xi_{-\epsilon}(b_\epsilon)}{\xi_{-\epsilon}(1)}
 -\frac{H_\epsilon(0)}{AL}.}
\tag{NH17}
$$

The two integral halves use the corresponding principal boundary
values at the real crossing; the integral is absolutely convergent
by (NH14)–(NH16). Both ordinate signs and all multiplicities remain.
At $\epsilon=0$ this is the identical contour balance for
$Z_{\rm orig}$, not a different kernel or another maximizing integer.

The infinite-contour limit also needs its horizontal ends paid.
The retained Fourier growth and a positive lower bound at $1/2$
give the (NH10) disk/height counts uniformly for
$0\le\epsilon\le\epsilon_0$; the lower bound may use
$\xi_{-\epsilon_0}(1/2)>0$. In each large dyadic interval choose
heights whose unit neighborhoods contain $O(\log T)$ zeros and whose
distance from every zero ordinate is at least $c/\log T$.
These heights exist by averaging the complete count and removing
intervals of that radius with sufficiently small $c$.

The standard genus-one Hadamard logarithmic derivative is

$$
H_\epsilon(z)=B_\epsilon+
 \sum_w\left(\frac1{z-w}+\frac1w\right).
$$

Its finite part at these heights is $O(T\log T)$: only
$O(\log T)$ zeros have ordinate distance below $1$, their reciprocals
cost $O(\log^2T)$, and the other $O(T\log T)$ terms have distance
at least $1$. The $1/w$ terms cost $O(\log^2T)$, and the
$|w|>4T$ tail costs $O(\log T)$ by the complete count.
Here $|z|\asymp T$ on the horizontal ends, and the endpoints' real
width is $O(\log T)$. The complete-coefficient estimate (NH2) therefore
pays these ends by $O_{A,\epsilon}(T^{\kappa-1}\log^2T)\to0$.
The Hadamard theorem is used for the deformed entire function itself;
no original-zeta count or simple-zero assumption is imported.
This justifies (NH17) over the full spectrum, including collisions.

### Pay the signed trace difference on the same arithmetic clock

Subtract (NH17) at zero heat time. Equations (NH14)–(NH16) give

$$
\left|\frac1{2\pi i}\int
 [Q_\epsilon K_\epsilon-Q_0H_0],ds\right|
\ll\epsilon A^2\int_{\mathbb R}
 |3+iy|^{\kappa-2}\log^2(|3+iy|+2)\,dy
\ll\epsilon A^2,
$$

uniformly for $\kappa\le1/4$. The exact slit and pole differences
are $O(\epsilon)$ as well. Indeed, $b_\epsilon-3=O(\epsilon)$,
and the Fourier representation has uniformly bounded $x$ and
$\epsilon$ derivatives on the fixed real compact set $0\le x\le3$,
$0\le\epsilon\le\epsilon_0$. Positivity bounds its denominators away
from zero there. The required moments are finite by the original
super-exponential kernel decay. Hence the real logarithm difference
and $H_\epsilon(0)-H_0(0)$ are $O(\epsilon)$; $1/(AL)\le1$.
This proves (NH12), with every contour correction retained.

For one common heat time at each $A$, choose

$$
\epsilon(A)=\min(\epsilon_0/2,A^{-3}).
$$

It satisfies all the preceding hypotheses for $A\ge e^2$. Using the
unchanged positive elementary term $r_A$ from (G9), (NH12) gives

$$
\boxed{-\sqrt A L I_\psi(A)
=\sqrt A L Z_{\epsilon(A)}(A)+r_A
 +O\!\left(LA^{-1/2}\right).}
\tag{NH18}
$$

The implicit constant is independent of $A$. The same selected
$N$ and $A=\log N>(7/2)10^{46}$ remain the source, and the original
zero real parts, multiplicities and infinite height range are paid
through the complete comparison. The time depends on the one
arithmetic clock, never on individual zeros. No uniform fixed negative
time is used as $A\to\infty$.

The comparison provides no upper bound for the signed main trace
$\sqrt A L Z_{\epsilon(A)}(A)$. In particular its absolute convergence
and its zero-free exterior do not establish the Robin budget
$\mathcal E(L)$. The constants have not been numerically certified
against the selected finite clock, so an $o(1)$ comparison alone is
not an exact finite Robin certificate. The original strict core and
positive $r_A$ still require enough signed slack. RH remains unproved.
