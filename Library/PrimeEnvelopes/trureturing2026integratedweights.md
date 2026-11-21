---
bibkey: trureturing2026integratedweights
authors: trureturing research
year: 2026
title: Integrated prime weights
doi: null
url: https://github.com/the-omega-institute/trureturing/blob/727e10f660466a6dc69ea491c8f334969b9c9d87/Library/ArithSums/nicolas2025comparison.md#project-application-cofinal-additive-edges-and-the-exact-constant-core
claim: Project calculations on the extremal envelopes studied in the Nicolas comparison note, under the hypotheses given in each section.
strata_touched: []
license: citation-only
triage: anchor
---

# Integrated prime weights

These sections continue the project’s calculations on Nicolas’s comparison of the two extremal envelopes. [Source and section index](../ArithSums/nicolas2025comparison.md)

## Project application: cofinal additive edges and the exact constant core

Under RH failure, the CNS positive-oscillation and Robin upper-envelope suppliers, the uniform Guth--Maynard Corollary 1.3 input, and the [FW0--FW22/N1--N5 suppliers](../ArithSums/trureturing2026extrawindowpairing.md), this appendix proves cofinal additive edges, exact constant cores, and their finite forward consumer. It follows that full forced-window section and uses the same original integer family, the factor \(5040\), and the same Robin objective. These are project deductions relative to those ordinary mathematical suppliers; they are not attributed to Nicolas or to the cited analytic authors.

### Definitions and the supplier interface

For \(x>1\) put

\[
 f(x)=\log\log x,\qquad \lambda(x)=f'(x)=\frac1{x\log x},
 \qquad w(x)=-\lambda'(x)=\frac{\log x+1}{x^2(\log x)^2}.
\]

Thus \(f''=-w<0\), and \(w\) is positive and decreasing.  For an integer
\(n\ge3\), write

\[
 W(n)=\log\frac{\sigma(n)}n,\qquad F(n)=W(n)-f(\log n),
 \qquad G(n)=e^{F(n)}.
\]

For a prime \(q\) and \(k\ge1\), define the Euler-layer data

\[
 h_q=\log q,\quad
 \ell_{q,k}=\log\left(1+\frac1{q+\cdots+q^k}\right),\quad
 r_{q,k}=\frac{\ell_{q,k}}{h_q}.
\]

Finite Euler telescoping gives

\[
 W(n)=\sum_{(q,k)\,\mathrm{occupied\ in}\,n}\ell_{q,k}.
\]

The \(r_{q,k}\) decrease strictly in \(k\), and

\[
 0<r_{q,k}<\frac1{q^k\log q},\qquad r_{q,1}<\lambda(q).
\]

The strict actual inventory and its clock are

\[
 N_t^{\rm str}=\prod_q q^{\#\{k:r_{q,k}>\lambda(t)\}},
 \qquad K(t)=\log N_t^{\rm str},
\]

whereas the reference Chebyshev--von Mangoldt clock is weak:

\[
 \psi(t)=\sum_{q^k\le t}\log q,
 \qquad Q(t)=K(t)-\psi(t).
\]

Every compact interval in \((1,\infty)\) has a common finite support of actual layers,
actual equality layers, and reference prime powers.  These conventions are
the finite inventory and endpoint conventions of [FIB §§85, 87, 98](../../docs/develop/theory/FIBONACCI_ATOMIC_RELATION_GENERATION.md) and [ZE/5040, Definition 7.1, “各指数层的素数截止值”](../../docs/develop/theory/ZECKENDORF_EULER_5040.md).  Equality layers are
excluded from \(N_t^{\rm str}\); reference atoms at their endpoint are
kept with their weak convention.

The analytic suppliers used here are the following.  Under RH failure,
put \(\Theta=\sup_{\rho\text{ a nontrivial zero of }\zeta}\Re\rho\), and
fix one \(1-\Theta<b<1/2\) and one \(d>0\) supplied by the positive
oscillation on CA integers of Caveney--Nicolas--Sondow. Since
\(1/2<\Theta\le1\), this gives \(0<b<1/2\). The primary is
[arXiv:1112.6010v2, printed p.15](https://arxiv.org/abs/1112.6010v2),
whose cited oscillation input is Robin 1983, [15], p.241.  The stable project source is the [CNS source note](../Arith/caveney2012sacaga.md).  There are arbitrarily large
actual witness integers \(m\), with \(X=\log m\), for which
\[
 F(m)\ge\gamma+dX^{-b}.
\]
The same original Robin upper envelope, in the normalization used by the
comparison file, supplies a constant \(K_R=0.6483e^{-\gamma}\) with
\[
 F(n)-\gamma\le\frac{K_R}{(\log\log n)^2}
 =\frac{K_R}{(\log(\log n))^2}
 \qquad(n\ge3).
\]
Writing \(A=\log n\), the denominator in the last display is
\((\log A)^2\).  No proof of either published analytic input is repeated.

We also use the uniform Corollary 1.3 of Guth--Maynard, as recorded in the [project GM source note](../Analytic/guthmaynard2024largevalues.md),
[arXiv:2405.20552v2](https://arxiv.org/html/2405.20552v2), with
\(\epsilon=1/60\) and \(\beta=7/12\): for every sufficiently large real
\(y\) and every \(y^\beta\le v\le y^{99/100}\),
\[
 \left|\pi(y+v)-\pi(y)-\frac v{\log y}\right|
 \le C_{\rm GM}v\exp\!\bigl(- (\log y)^{1/4}\bigr).
\]
Increase its one unknown common start until
\(C_{\rm GM}\log y\exp(- (\log y)^{1/4})\le1/2\) for every later real
\(y\). Then every permitted interval contains a prime.  That is the only use of this supplier in the counting
argument.

For a qualifying witness define
\[
 \ell=\frac d8X^{1-b}\log X,
 \qquad
 R=\exp(a_RX^{b/2}),\quad a_R=\sqrt{2K_R/d},
 \qquad
 \mathcal P_X=\{p\text{ prime}:e^\ell\le p\le e^{2\ell}\}.
\]
Here \(R\) is a window clock ceiling, not the original signed residual
\(R(t)\).  The accepted FW/N1 supplier says that, after one common
unknown start, every \(p\in\mathcal P_X\) and every maximizing tie in
the full class of positive multiples of \(5040p\) has
\[
 \ell\le A=\log N\le R,\qquad N=pN_A^{\rm str},\qquad
 E_N=\{(p,1)\},\qquad P^+(N)=p,
\]
and that no such integer is a maximizing tie for a different ordinary
label.  The accepted N2 supplier gives, for \(p<r\) in the same window
and any choices of maximizing ties,
\[
 N=pU,\quad N'=rV,\quad A=\log N<C=\log N',\quad U\mid V,
 \quad C-A=\log(V/U)+\log(r/p).
\]
For \(p\ge29\), denote the full multiples class and its canonical source by
\[
 \mathscr M_p=\mathop{\rm argmax}_{5040p\mid n,\ n\in\mathbb N_{>0}}F(n),
 \qquad N_p^{\rm mult}=\min\mathscr M_p,
 \qquad A_p^{\rm mult}=\log N_p^{\rm mult}.
\]
All cofinal and global source conclusions below use these **least
full-domain maximizers**. The N2 all-choice ordering inside a qualifying
window applies, in particular, to these canonical choices; it is not a
global order assertion for arbitrary ties. Each source is actual GA2,
because every positive integer multiple remains in its full \(5040p\)
class. The reused global least-source order and the N1 label uniqueness
make each window source a singleton label block, with last label
\(P^+(N_p^{\rm mult})=p\). Thus consecutive ordinary primes in a window
produce genuine consecutive last-label blocks of the original canonical
family. These are actual maximizers, not fixed-price optimizers or
oscillation padding integers.

The elementary padding behind the window statement is recalled for
source clarity.  Let \(m_0=\operatorname{lcm}(5040,m)\),
\(d_0=\log(m_0/m)\le\log5040\), and \(D_p=pm_0\).  If
\(k=v_p(m_0)\), then
\[
 F(D_p)-F(m)=W(m_0)-W(m)+\ell_{p,k+1}
 -[f(X+d_0+\log p)-f(X)].
\]
The Euler increments are nonnegative and the last term is at most
\((d_0+\log p)/(X\log X)\).  Since \(\log p\le2\ell\), this is at most
\(dX^{-b}/2\) for all sufficiently large witnesses.  Hence every
\(p\)-class has a member above the floor
\(\gamma+dX^{-b}/2\).  The Robin envelope is below that floor once
\(A>R\), because \(K_R/(\log R)^2=dX^{-b}/2\).  The finite part
\(A\le R\) therefore contains every full-domain maximizing tie.  Finally
\[
 \frac{\ell}{\log R}=\frac d{8a_R}X^{1-3b/2}\log X\longrightarrow\infty,
\]
so \(e^\ell/R^M\to\infty\) for every fixed \(M>0\), uniformly over the
window.  In particular \(p>2R\) eventually.

Under these same RH-false suppliers, the finite arithmetic conclusions
to be proved are

\[
\boxed{\begin{gathered}
 \text{for every fixed }\alpha>0\text{ there are cofinally many canonical}\\
 \text{original-source edges }0<C-A\le A^\alpha,\\
 \text{and cofinally many such edges }0<C-A<\log2\text{ with }U=V.
\end{gathered}}
\tag{CW0}
\]

The rest of the appendix proves this box and its exact consumer.

### Membership before counting

The next lemma is the point at which the prime count is used.  It is
proved before either the fixed-\(\alpha\) or the \(\log2\) pigeonhole
count, so no prime is counted merely because it was presumed to lie in
the window.

At \(y=e^\ell\) and \(v=e^{\beta\ell}\), the uniform GM estimate gives a
prime \(p_0\) with
\[
 e^\ell<p_0\le e^\ell+e^{\beta\ell},
 \qquad \log p_0\le\ell+\log2
\]
for large \(\ell\).  Let \(p_{i+1}\) be the actual next ordinary prime
after \(p_i\).  Whenever \(p_i\ge e^\ell\), apply GM at \(y=p_i\) with
\(v=p_i^\beta\).  This interval is permitted and contains a prime, so
\[
 0<\delta_i:=\log\frac{p_{i+1}}{p_i}
 \le\log(1+p_i^{\beta-1})
 \le p_i^{-5/12}\le E,
 \qquad E=e^{-5\ell/12}.
\]
For every specified finite \(k\), induction gives
\[
 \log p_i\le\ell+\log2+iE\qquad(0\le i\le k).
\]
Indeed the successor remains at least \(e^\ell\), and the displayed
bound is precisely the logarithm of the multiplicative successor
estimate.  If \(kE\to0\), choose the witness after the supplier starts
and with \(\ell>\log2+kE\).  Then all \(p_0,\ldots,p_k\) lie in
\([e^\ell,e^{2\ell})\), before any counting conclusion is drawn.  This
finite induction does not assert that an infinite sequence remains in one
fixed window.

For later use, the estimate \(ER^M\to0\) follows directly from
\(\log R=o(\ell)\).  It is uniform for each fixed \(M\), but no uniformity
in a moving \(M\) is claimed.

### The fixed-\(\alpha\) cofinal edge

Fix \(\alpha>0\) before choosing the witness.  Put
\[
 k_\alpha=\left\lceil\frac R{\ell^\alpha}\right\rceil+1.
\]
Then
\[
 k_\alpha E\le E\left(\frac R{\ell^\alpha}+2\right)\longrightarrow0.
\]
The preceding finite induction therefore puts \(p_0,\ldots,p_{k_\alpha}\)
inside \(\mathcal P_X\). Let \(N_i=N_{p_i}^{\rm mult}=p_iU_i\) and
\(A_i=\log N_i\) be the corresponding canonical least maximizers.  By the accepted N2
ordering, \(A_i<A_{i+1}\le R\), \(U_i\mid U_{i+1}\), and
\[
 A_{i+1}-A_i=\log(U_{i+1}/U_i)+\log(p_{i+1}/p_i)>0.
\]
If all \(k_\alpha\) edges had \(A_{i+1}-A_i>A_i^\alpha\), then, since
\(A_i\ge\ell\),
\[
 A_{k_\alpha}>A_0+k_\alpha\ell^\alpha>R,
\]
contradicting \(A_{k_\alpha}\le R\).  Thus one of these distinct
consecutive-label edges satisfies the claimed upper bound.  Since
\(\ell\to\infty\) along the CNS witnesses, choosing \(\ell\ge T\) gives
one with \(A\ge T\) for every finite \(T\).  This proves
\[
\begin{gathered}
 \forall\alpha>0\ \forall T\in\mathbb R\ \exists\text{ a consecutive}\\
 \text{canonical original-source edge with }A\ge T
 \text{ and }0<C-A\le A^\alpha.
\end{gathered}
\tag{CW1}
\]

The quantifiers in this statement are fixed-alpha quantifiers: the start
may depend on \(\alpha\) and on the supplier constants.  It does not say
that every edge has this spacing, that all \(\alpha\)'s work at one common
start, or that any long window has a mesh estimate.

### Exact \(\log 2\) rigidity

Now put
\[
 k_2=\left\lceil\frac{2R}{\log2}\right\rceil+1.
\]
The same membership induction applies because

\[
 k_2E\le\left(\frac{2R}{\log2}+2\right)E\longrightarrow0.
\]

Thus the \(k_2+1\) actual sources associated with
\(p_0,\ldots,p_{k_2}\) are all in the same admitted window.  If each of
the \(k_2\) edges had \(C_i-A_i\ge\log2\), telescoping would give
\[
 A_{k_2}\ge A_0+k_2\log2>2R,
\]
which contradicts \(A_{k_2}\le R\).  Select an edge with
\[
 0<C-A<\log2.
\]
For this edge \(U\mid V\), so \(j=V/U\) is a positive integer.  If
\(j\ge2\), then
\[
 C-A=\log j+\log(r/p)\ge\log2+\log(r/p)>\log2,
\]
which is impossible.  Consequently \(j=1\), and the exact arithmetic
identities are
\[
 U=V,\qquad D:=\log(V/U)=0,\qquad Z:=pV=pU=N,
 \qquad z:=\log Z=A,
\qquad \varepsilon:=F(N)-F(Z)=0.
\tag{CW2}
\]

The same choice can be made beyond every finite collection of analytic
or tolerance starts: choose a sufficiently large qualifying witness with
\(\ell\) above their maximum and satisfying the membership inequalities.
Thus the unchanged-core edges are cofinal in the original canonical
least-source family. Their sources remain distinct: \(N=pU\) and
\(N'=rU\), with \(p<r\). In fact \(C-A=\log(r/p)\le E\) on each
selected edge.  This proves a cofinal exact constant core, not a whole-window
common core, an every-edge equality, a long constant-core run, or a
cofinal assertion that \(D>0\) or \(Z>N\).

For reference, the counting argument is robust under a genuinely supplied
tolerance \(E_c=e^{-c\ell}\), \(c>0\): if the actual prime recurrence
gives \(\delta_i\le E_c\) and \(\log R=o(\ell)\), then
\(k_2E_c\to0\) and, for every fixed \(\alpha>0\),
\(k_\alpha E_c\to0\), so the same membership and both counting proofs
apply. This conditional observation
does not improve the supplied GM exponent and is not used as an input.

### The exact forward successor on the same original integer

Take one of the selected canonical constant-core edges. Its distinct
original integers are \(N=pU\) and \(N'=rU\), with \(p<r\); they share
only the core \(U=N_A^{\rm str}=N_C^{\rm str}\). Put
\[
 h=A^{4/5},\qquad B=A+h,\qquad
 L=pN_B^{\rm str},\qquad Y=\log L.
\]
Since \(B<2A\le2R<p\), the forced layer \((p,1)\) is absent from
\(N_t^{\rm str}\) throughout \([A,B]\).  Since \(U=N_A^{\rm str}\)
and strict inventories are divisibility-monotone,
\[
 N\mid L,\qquad 5040\mid L,
 \qquad L=\operatorname{lcm}(N,N_B^{\rm str}).
\]

The successor is genuinely larger.  Apply GM at the real point
\(A+h/3\) with length \(h/3\).  Eventually
\((A+h/3)^\beta\le h/3\le(A+h/3)^{99/100}\), so there is a prime

\[
 A+h/3<q\le A+2h/3.
\]

The first actual cutoff satisfies \(B-1<q_1(B)<B\).  Hence, for large
\(A\), \(q<B-1<q_1(B)\), so \((q,1)\) is absent from \(N_A^{\rm str}\)
and present in \(N_B^{\rm str}\).  Also \(q<p\), because \(q<B<2R<p\).
Therefore \(q\mid L/N\), and
\[
 L>N=Z.
\]
This is a literal integer successor retaining the full \(5040\) factor;
it is not a scalar relaxed competitor and is not asserted to be GA2.

The unique occupied extra of \(N\) is \((p,1)\), and

\[
 d_A(N)=(\lambda(A)-r_{p,1})\log p>0,
 \qquad
 R_{\rm term}(N,B)=(\lambda(B)-r_{p,1})\log p>0.
\]

Its occupied pressure loss is nevertheless exactly zero:
\[
 P_N(t)=0\ (A\le t\le B),
 \qquad V_N(A,h)=\int_0^hP_N(A+u)\frac{w(A+u)}{w(A)}\,du=0.
\]
The zero loss is caused by strict inactivity of the extra, while the own
defect remains positive.  These are different terms in the exact identity.

More generally, let \(N\ge3\) be an integer, \(A=\log N>1\),
\(h>0\), \(B=A+h\), and \(N_A^{\rm str}\mid N\). Let \(E_N\) be
its finite set of occupied layers excluded from \(N_A^{\rm str}\), and put
\[
 P_N(t)=\sum_{e\in E_N:\ r_e>\lambda(t)}h_e,
 \qquad
 Y_N(t)=\log\operatorname{lcm}(N,N_t^{\rm str}).
\]
The literal lcm clock is
\[
 Y_N(t)=A+K(t)-K(A)-P_N(t).
\]
With \(\rho_A(u)=w(A+u)/w(A)\), define
\[
 T_\psi(A,h)=\int_0^h[\psi(A+u)-\psi(A)-u]\rho_A(u)\,du,
 \quad
 S_Q(A,h)=\int_0^h[Q(A+u)-Q(A)]\rho_A(u)\,du,
 \quad V_N(A,h)=\int_0^hP_N(A+u)\rho_A(u)\,du.
\]
With \(Y=Y_N(B)>1\), the finite strict-lcm identity is
\[
 F(\operatorname{lcm}(N,N_B^{\rm str}))-F(N)
 =w(A)[T_\psi(A,h)+S_Q(A,h)-V_N(A,h)]+C_B(Y),
\]
where
\[
 C_B(Y)=f(B)+\lambda(B)(Y-B)-f(Y)\ge0.
\tag{CW3}
\]

Here \(C_B\) is the actual terminal concavity cost, not a fixed-price
objective term.  The selected branch has \(\operatorname{lcm}(N,N_B^{\rm str})=L\)
and \(V_N=0\).

For completeness, the proof is finite. On \([A,B]\), take one common
support containing all actual layers, equality layers, and reference
atoms. A missing actual layer has \(r_e\le\lambda(A)\) and an activation
\(t_e\ge A\) with \(\lambda(t_e)=r_e\). It is added to the strict
terminal lcm exactly when \(t_e<B\). Its integrated pressure is
\[
 \int_A^B\mathbf1_{t_e<t}h_ew(t)\,dt
 =(r_e-\lambda(B))_+h_e.
\]
A missing tie at \(A\) activates immediately to the right and has this
same weight; a missing tie at \(B\) is excluded and has zero weight.
Write \(\Delta=Y-A\) and
\(\mathcal W=W(\operatorname{lcm}(N,N_B^{\rm str}))-W(N)\). Finite
layer summation and one integration by parts give
\[
 \int_A^B[Y_N(t)-t]w(t)\,dt
 =\mathcal W-\lambda(B)\Delta-[f(B)-f(A)-h\lambda(B)].
\]
Adding \(C_B(A+\Delta)\) gives
\(\mathcal W+f(A)-f(A+\Delta)\), precisely the left side of CW3.
The clock formula and \(K=\psi+Q\) give, pointwise,
\[
 Y_N(A+u)-(A+u)
 =\psi(A+u)-\psi(A)-u+Q(A+u)-Q(A)-P_N(A+u),
\]
which yields its right side. The initial \(K(A)\) cancels without
assuming \(K(A)=A\). Reference atoms retain their weak convention:
\(\psi(t)-\psi(A)=\sum_{A<n\le t}\Lambda(n)\), with the initial
reference atom excluded and the terminal atom carrying zero pressure
weight. Simultaneous actual events retain every separate layer mass.
If missing terminal equality layers of total mass \(J\) are deliberately
installed, their reward is \(\lambda(B)J\); the pressure integral is
unchanged, but the clock and cost become \(Y+J\) and \(C_B(Y+J)\).
CW3 uses the strict successor and its actual \(Y\). No infinite-tail
subtraction is used.

The complete reference term, including every prime power, is
\[
 w(A)T_\psi(A,h)
 =\sum_{A<n\le B}\Lambda(n)[\lambda(n)-\lambda(B)]
 -[f(B)-f(A)-h\lambda(B)].
\tag{CW4}
\]
Indeed integrate each step function \(\mathbf1_{n\le t}\) over
\([A,B]\): its weight is
\(\int_n^B w(t)\,dt=\lambda(n)-\lambda(B)\), while the linear term has
integral \(f(B)-f(A)-h\lambda(B)\).  A prime power \(n=q^k\) carries
the full \(\Lambda(n)=\log q\) weight.  A reference atom at \(A\) is
excluded by the open lower endpoint and one at \(B\) has zero weight.
All simultaneous actual events retain their separate layer masses.

Because \(N\) is an actual GA2 integer and \(L\) is a positive multiple, \(F(L)-F(N)\le0\).  On the selected edge the exact identity therefore gives the necessary upper comparison \[ w(A)[T_\psi(A,A^{4/5})+S_Q(A,A^{4/5})] \le -C_B(Y)\le0. \tag{CW5} \] The [full-Q supplier QH1--QH13/QQE/QQD](trureturing2026selectedsources.md#precise-full-signed-q-statement-and-quantified-error) gives, for every sufficiently large real center, \(S_Q(A,A^{4/5})=(c_Q+o(1))A^{11/10}\), where \[ c_Q=\frac{\sqrt2-1}{4}>0. \] More precisely, there are \(C_Q>0\) and one unknown \(A_*>2\) such that for every real \(A\ge A_*\), \[ \left|\frac{S_Q(A,A^{4/5})}{A^{11/10}}-c_Q\right| \le C_Q\mathcal F_Q(A), \] \[ \begin{aligned} \mathcal F_Q(A)={}&\frac1{\log A}+A^{-1/5} +\log A\,e^{-((\log A)/3)^{1/4}}+A^{-1/120}\\ &+A^{-3/10}\log A+A^{-1/6}(\log A)^{4/3} +A^{-19/180}(\log A)^{43/36}. \end{aligned} \] All seven errors tend to zero. The actual square coefficient \(\sqrt2/4\), the subtracted reference square coefficient \(1/4\), both higher-layer inventories, and the strict endpoint correction \(+\operatorname{atom}(y)-\operatorname{atom}(y+v)\) remain in this supplier. Equivalently, for every fixed tolerance \(\eta>0\), there is one unknown \(A_\eta\ge A_*\) such that \(\left|S_Q(A,A^{4/5})-c_QA^{11/10}\right|\le\eta A^{11/10}\) for **every real** \(A\ge A_\eta\). The cofinal canonical sources pass each such start; no numerical start is supplied. The displayed direction is an upper direction forced by GA2.  It is not a favorable lower bound for \(T_\psi\).

### Scope of the project deductions

Under the same RH-false CNS/Robin, uniform GM, and full FW/N1--N5
suppliers, the results proved here are the cofinal additive edge for every
fixed \(\alpha>0\), the cofinal exact unchanged-core edge with
\(0<C-A<\log2\), the conditional tolerance generalization when an actual
\(E_c\) recurrence is supplied, and the exact same-original full-\(\Lambda\)
consumer with its necessary GA2 upper direction. The cofinal sources
are canonical least full-domain maximizers with their original last
labels and clocks. The generalization supplies no new prime estimate.

The mathematical dependencies and remaining obligations are:

| input or result | hypotheses and mathematical use |
|---|---|
| CNS positive oscillation and Robin envelope | RH failure supplies fixed \(1-\Theta<b<1/2\), \(d>0\), unbounded actual witnesses; the unconditional envelope gives the upper clock ceiling |
| Guth--Maynard Corollary 1.3 | one unknown all-real start, fixed \(\beta=7/12\), admitted lengths through \(y^{99/100}\); used for actual successor primes and the nontrivial forward integer |
| [FW0--FW22/N1--N5](../ArithSums/trureturing2026extrawindowpairing.md) | full-domain attainment and label uniqueness for all ties, finite-window all-choice ordering, and global ordering of canonical least sources |
| membership, cofinality, rigidity, and CW3--CW5 | proved above on that same source family; strict inventories, full \(\Lambda\), occupied loss, and actual terminal cost are retained |
| [QH1--QH13/QQE/QQD](trureturing2026selectedsources.md#precise-full-signed-q-statement-and-quantified-error) | full signed \(Q\)-drift for every sufficiently large real center, with all seven errors and endpoint/higher-layer terms |
| [finite_signed_response_identity](../../D5/S3/Arith/Robin/ActualVonMangoldtBandCompensation.lean) | distinct finite centered-dilation identity; its kernel, theta premise, and finite boundary require a bridge to this forward consumer |
| [OpenAI/math](../Analytic/openai2026quasirh.md), [Mantovanelli/rough-shift](../Analytic/mantovanelli2026primeworkload.md), and [short-uniformity](../Analytic/shortuniformity2026robininterfaces.md) interfaces | their distinct zero-free, shift, weight, model, or testing hypotheses have not been instantiated for these selected full-\(\Lambda\) weights |
| full RH/Robin/5040 statement | \(I_\psi(\log n)+R(\log n)+d_{\log n}(n)>0\) for every actual integer \(n>5040\); remains ACTIVE_UNPROVED |

The formal-source consumer just named is
`D5.S3.Arith.Robin.ActualVonMangoldtBandCompensation.finite_signed_response_identity`,
under its actual real-parameter hypotheses \(A\ge e^{78}\),
\(99/100\le c\le101/100\), \(A<R_{\rm cut}\), and
\(cA\le R_{\rm cut}\). Here \(R_{\rm cut}\) denotes that theorem's
finite cutoff parameter, distinct from both the window ceiling and the
original residual.
Its conclusion has the form
\[
 \mathrm{finiteResponse}
 =\mathrm{smoothBoundary}+\mathrm{bandVolume}
 -\mathrm{actualCompensation}.
\]
Its companion `finite_signed_response_upper_of_theta_increment_lower`
additionally requires \(H>0\), \(0\le\epsilon<1\), and
\(\mathrm{ThetaIncrementLower}(99A/100,H,\epsilon)\): for every
\(99A/100\le u<v\le198A/100\) with \(H\le v-u\),
\[
 (1-\epsilon)(v-u)\le\theta(v)-\theta(u).
\]
Its conclusion retains
\(\mathrm{smoothBoundary}+\epsilon\,\mathrm{bandVolume}
+(1-\epsilon)\,\mathrm{shortAllowance}\).
This kernel has a different finite boundary normalization from the
\(T_\psi\) kernel above; the required theta premise and the bridge to
the displayed full-\(\Lambda\) forward consumer remain unpaid.

The selected-source signed obligation for this route remains **one fixed**
\(\kappa<c_Q\) such that, beyond **every** required common unknown finite
start \(T\), there is an original canonical least source
\(N_p^{\rm mult}\) in the proved cofinal window family, with
\(A=A_p^{\rm mult}\ge T\), satisfying
\[
 T_\psi(A,A^{4/5})\ge-\kappa A^{11/10},
\]
or an equivalent fixed positive lower margin for the complete same-source
quantity.  Neither cofinality, zero occupied loss, exact \(Z=N\), positive
\(Q\)-drift, nor least attainment supplies that sign.  In particular, no
finite interval through \(8\cdot10^{46}\) pays an unknown asymptotic start,
and no finite common-start substitution is made.

No every-edge convergence and no every-edge \(A^{4/5}\)-scale spacing is
claimed.  Cofinal original-source \(A^\alpha\)-scale edges are proved for
each fixed \(\alpha>0\), and cofinal exact unchanged-core edges are proved
with \(0<C-A<\log2\), all under the same RH-false suppliers and on
canonical least full-domain sources. The original full signed lower input
remains unpaid. The unchanged all-integer target is
\[
 \forall n\in\mathbb N,\quad n>5040\ \Longrightarrow
 I_\psi(\log n)+R(\log n)+d_{\log n}(n)>0,
\]
and remains **ACTIVE_UNPROVED**. Here \(R(t)\) is the original signed
residual, not the window clock ceiling.

# Integrated weights of the original selected family

Let \(3\le\ell\le\mathcal R\), and let \(S\subset[\ell,\mathcal R]\)
be measurable, of mass \(M=|S|>0\). In the original source application,
\(S\) is the **complete** union of unchanged-core intervals of consecutive
window labels belonging to the canonical least full-domain maximizers
\[
 N_p=\min\operatorname*{argmax}_{5040p\mid n} \left[
 \log(\sigma(n)/n)-\log\log\log n\right].
\]
Nothing in the following weight construction changes these integers.
Put
\[
 f(x)=\log\log x,\quad\lambda(x)=1/(x\log x),\quad
 w(x)=-\lambda'(x),\quad H_t=t^{4/5},\quad B_t=t+H_t.
\]
Define the real kernel by
\[
 k_t(x)=\begin{cases}
 [\lambda(x)-\lambda(B_t)]/[w(t)t^{11/10}],&t<x\le B_t,\\
 0,&\text{otherwise}.
 \end{cases}
\]
Thus no price is evaluated at \(x\le1\). Set
\[
 \mathcal W(x)=\int_S k_t(x)\,dt,\qquad
 a(t)=\frac{f(B_t)-f(t)-H_t\lambda(B_t)}{w(t)t^{11/10}},
 \quad \mathcal D=\int_S a(t)\,dt,
\]
\[
 b(t)=\frac{\lambda(t)-\lambda(B_t)}{w(t)t^{11/10}},
 \qquad\mathcal B=\int_S b(t)\,dt.
\]

For the source geometry, the strict inventory means
\[
 r_{q,k}=\frac{\log(1+1/(q+\cdots+q^k))}{\log q},\quad
 \mathcal N(t)=\prod_{q\ \mathrm{prime}}
 q^{\#\{k\ge1:r_{q,k}>\lambda(t)\}},\quad K(t)=\log\mathcal N(t).
\]
Every compact clock interval has one finite set of potentially active or
tied actual layers, since \(r_{q,k}<1/(q^k\log q)\). Equal-price
layers are excluded from the strict inventory.

**Proposition.** The weight \(\mathcal W\) is nonnegative, compactly
supported, and absolutely continuous. Its derivative is, almost everywhere,
\[
 \mathcal W'(x)=\mathbf1_S(x)b(x)
 -w(x)\int_{\substack{t\in S\\t<x<B_t}}
           \frac{dt}{w(t)t^{11/10}}.
\tag{A1}
\]
In (A1) the two nonnegative densities are defined on \(x>1\) and
are extended by zero on \(x\le1\), without evaluating a price there.
Both densities have integral \(\mathcal B\), and
\[
 \mathcal B\le M\ell^{-3/10},\quad
 \operatorname{Var}(\mathcal W)\le2\mathcal B,\quad
 0\le\mathcal W\le\mathcal B,\quad
 \int_0^\infty\mathcal W(x)\,dx=\mathcal D.
\tag{A2}
\]

*Proof.* Since \(w\) decreases,
\(b(t)\le H_t/t^{11/10}=t^{-3/10}\). For every real \(x\),
\[
 k_t(x)=b(t)\mathbf1_{x>t}
 -\frac1{w(t)t^{11/10}}\int_t^{B_t}\mathbf1_{s<x}w(s)\,ds.
\]
This representation also holds at both endpoints. Integrating in \(t\)
and applying Tonelli expresses \(\mathcal W\) as the difference of the
indefinite integrals of the two integrable densities in (A1). Each has
integral \(\mathcal B\). Absolute continuity and the variation bound
follow. Also \(0\le k_t\le b(t)\), and all kernels vanish outside
\([\ell,2\mathcal R]\). Finally direct integration gives
\(\int k_t=a(t)\); Tonelli proves the last identity. No estimate for
the number of connected components of \(S\) is used. \(\square\)

Let \(\psi(x)=\sum_{n\le x}\Lambda(n)\) use the full von Mangoldt
function, and put
\[
 \Phi(t)=t^{-11/10}\int_0^{H_t}
  [\psi(t+u)-\psi(t)-u]\frac{w(t+u)}{w(t)}\,du,
 \quad\mathcal I=\int_S\Phi(t)\,dt,
 \quad J=\lfloor2\mathcal R\rfloor.
\]

**Corollary (discrete centering with absolute small error).**
With \(\Lambda(1)=0\),
\[
 \mathcal I=\sum_{n=1}^J(\Lambda(n)-1)\mathcal W(n)+e_S,
\quad
 e_S=\int_0^\infty(\{x\}-1/2)\mathcal W'(x)\,dx,
\quad |e_S|\le M\ell^{-3/10}.
\tag{A3}
\]
Equivalently,
\[
 \mathcal I=\sum_{d=1}^J\mu(d)
       \sum_{m=1}^{\lfloor J/d\rfloor}\log m\,\mathcal W(dm)
       -\mathcal D.
\tag{A4}
\]
Every reference power \(q^k\) is present with mass \(\log q\).

*Proof.* The finite step identity for \(\psi\) gives
\(\Phi(t)=\sum_{n=2}^J\Lambda(n)k_t(n)-a(t)\).
An initial atom \(n=t\) is excluded, and an included terminal atom
\(n=B_t\) has zero weight. Finite interchange gives
\(\mathcal I=\sum\Lambda(n)\mathcal W(n)-\mathcal D\).
Integration by parts against \(\lfloor x\rfloor\) and against \(x\)
gives
\[
 \sum_n\mathcal W(n)-\int\mathcal W
 =\int\{x\}\mathcal W'(x)\,dx
 =\int(\{x\}-1/2)\mathcal W'(x)\,dx.
\]
The boundary terms vanish, and (A2) bounds its absolute value by
\(\operatorname{Var}(\mathcal W)/2\le\mathcal B\). This proves (A3).
For (A4), use \(\Lambda=\mu*\log\) and regroup only pairs with
\(dm\le J\). Indeed the coefficient of \(\log p\) in
\(\sum_{d\mid n}\mu(d)\log(n/d)\) is
\((1-1)^{\omega(n)-1}\) for each prime dividing \(n>1\): it is
one for a prime power and zero otherwise. At \(n=1\) the logarithm
vanishes. Thus this regrouping retains every power and every divisor
scale. \(\square\)

For any real or complex sequence indexed by positive integers, \(a_n\), let \(A_a(x)=\sum_{n\le x}a_n\).
The exact testing interface is
\[
 \sum_{n=1}^J a_n\mathcal W(n)
 =-\int_0^\infty A_a(x)\mathcal W'(x)\,dx
 =\int_S\frac1{w(t)t^{11/10}}
     \int_t^{B_t}[A_a(x)-A_a(t)]w(x)\,dx\,dt.
\tag{A5}
\]
The first identity is finite Abel summation. The second uses (A1) and
\(b(t)=\int_t^{B_t}w(x)\,dx/[w(t)t^{11/10}]\); it cancels the
same initial prefix, without changing any integer endpoint.

In particular, if \(C\ge0\), \(c\ge0\), and a supplied ordinary
prefix estimate is
\(|A_a(x)|\le Cx/(\log x)^c\) for every real \(x\ge3\), then
\[
 \left|\sum_n a_n\mathcal W(n)\right|
 \le3C\int_S\frac{t^{7/10}}{(\log t)^c}\,dt.
\tag{A6}
\]
To prove this, bound the jump part of (A1) by
\(b(t)Ct/(\log t)^c\), and its descending part by
\(b(t)2Ct/(\log t)^c\), since \(t\le x\le B_t<2t\).
When \(|a_n|\le1\), positivity and (A3) also give the elementary
bound \(\mathcal D+\mathcal B\); one may take the minimum of the two
allowances.

The pinned OpenAI/math ordinary affine Liouville supplier, at
`adc7f1241b42e322a6451854ab7e4b4c146bf78a`, gives precisely the prefix
premise of (A6) for
\(a_n=\lambda_L(a_1n+b_1)\lambda_L(a_2n+b_2)\), with fixed
\(a_1,a_2\ge1\), \(b_1,b_2\ge0\), and
\(a_1b_2-a_2b_1\ne0\). Here \(\lambda_L\) is Liouville, not the
price \(\lambda\). The exponent is absolute and the constant depends
on these fixed forms. Thus (A6) is a genuine ordinary, supplier-relative
application to the original selection weight, even though that weight is
not multiplicative. The source is the ordinary preprint's quantitative
affine theorem and the actual `OAI/NumberTheory/TwoPointCorrelations/FinalMain.lean`
entry, not the `sorry` comparator interface. No external formal validation
is asserted. Neither this large allowance nor its minimum with the
elementary bound gives the required absolute \(O(M)\) signed estimate.

For every cofactor \(m\), including moving ones, (A5) applied to the
dilated weight gives
\[
 \sum_{d\le\lfloor J/m\rfloor}\mu(d)\mathcal W(md)
 =-\int_0^\infty M_\mu(x/m)\mathcal W'(x)\,dx
 =\int_S\frac1{w(t)t^{11/10}}
       \int_t^{B_t}[M_\mu(x/m)-M_\mu(t/m)]w(x)\,dx\,dt.
\tag{A7}
\]
No factor \(m\) remains: the derivative of the dilated weight cancels
the change-of-variable Jacobian. Its elementary bound is
\(\mathcal D/m+\mathcal B\). A qualitative Mertens supplier gives,
for each fixed \(m\), the alternative bound
\[
 \frac{3\eta_\mu(\ell/m)}m\int_S t^{7/10}\,dt,
 \quad\eta_\mu(s)=\sup_{y\ge s}|M_\mu(y)|/y\longrightarrow0.
\]
This does not provide a uniform small allowance when \(m\) grows up
to \(J\). The full sum in (A4) still needs all its logarithms and rows.

The original good-edge geometry also has an exact continuous comparison.
Let its endpoint sources be \(pU,rU\), with clocks \(A<C\), both
GA2 against all positive multiples, and suppose the strict inventory
\(\mathcal N(t)\) equals \(U\) on the closed interval \([A,C]\).
For sufficiently late original witnesses, both labels exceed
\(2\mathcal R\), whereas all primes in \(V_t=\mathcal N(B_t)\)
are below \(B_t<2\mathcal R\). Also \(U\mid V_t\) and
\(5040\mid U\); hence \(rV_t\) is a legal integer multiple
of \(rU\) retaining 5040. Put
\(D_t=\log(V_t/U)\), \(Y_t=t+D_t\), and
\[
 C_B(Y)=f(B)+\lambda(B)(Y-B)-f(Y)\ge0.
\]
Then, with \(Q=\log\mathcal N-\psi\) and the full signed
\(S_Q(t,H)=\int_0^H[Q(t+u)-Q(t)]w(t+u)/w(t)\,du\),
\[
 w(t)[t^{11/10}\Phi(t)+S_Q(t,H_t)]+C_{B_t}(Y_t)
 \le-\int_t^C[\lambda(s)-\lambda(s+D_t)]\,ds\le0.
\tag{A8}
\]
To prove it, freeze \(V_t\) and differentiate
\[
 W(V_t)-W(U)-f(s+D_t)+f(s),\qquad W(n)=\log(\sigma(n)/n).
\]
Here \(V_t\) and \(D_t\) are frozen while \(s\) varies. Its
derivative is \(\lambda(s)-\lambda(s+D_t)\ge0\), and its value
at \(C\) is \(F(rV_t)-F(rU)\le0\). Finite layer integration between
\(U\) and \(V_t\) identifies its value at \(t\) with the left side
of (A8): an activation at \(t\) is initially absent and integrated on
its right, and an activation tied at \(B_t\) is excluded with zero
integrated weight. Adding the displayed terminal cost cancels the linear
terms. At \(t=A\), \(Y_t\) is the actual original lcm-successor
clock; other real centers are scalar interpolations of that legal
endpoint comparison, not newly claimed integer maximizers.

For the complete original family, the full-Q supplier gives
\(S_Q(t,H_t)/t^{11/10}\to c_Q=(\sqrt2-1)/4\), uniformly beyond
an unknown every-real tolerance start. Integrating (A8) preserves the
interpolated cost and nonnegative comparison slack. Independently, the
actual departures retain their discrete terminal costs. Thus (A3)
provides an absolute \(o(M)\) bridge to the same weighted
\(\Lambda-1\) lower obligation. A fixed lower coefficient
\(\kappa<c_Q\), available on cofinally many complete original
families after every common start, is still **unproved**. All-integer
RH/Robin/5040 remains **ACTIVE_UNPROVED**.


## Full-family quantifiers, reference powers and finite source maps

These additions are ordinary project deductions relative to the same
completed source-localization, corrected CW and FW suppliers and the
immutable sources named below. They preserve the same original integers,
the complete original selected set, and every reference and divisor row.

In the original RH-false application, one fixes the CNS/Robin constants
\(1-\Theta<b<1/2\), \(d>0\) before the unbounded witness clocks
\(X\). The suppliers give
\[
 \ell=(d/8)X^{1-b}\log X,\quad
 \mathcal R=\exp(\sqrt{2K_R/d}X^{b/2}),\quad
 E=e^{-5\ell/12},\quad K_R=0.6483e^{-\gamma},
\]
\[
 \ell-(2+\mathcal R/\log2)E\le M_X\le\ell,
 \quad M_X\sim\ell,\quad \log\mathcal R=o(\ell).
\]
The source-window all-choice ordering applies to the canonical least
full-domain maximizers; no global arbitrary-tie assertion is substituted.
The ordinary window labels are exactly primes
\(p\in[e^\ell,e^{2\ell}]\), and consecutive good edges have
\(N_i=p_iU_i\), \(U_i=U_{i+1}\),
\(C_i-A_i=\delta_i=\log(p_{i+1}/p_i)\in(0,E]\).
Here every sum indexed by \(i\) is over all these good edges.
Every full selected interval has closed strict inventory \(U\), with
its half-open version used only for disjoint integration. The unknown
uniform GM and full-Q starts are retained.

For an actual departure \(A_i\), put
\(L_i=p_i\mathcal N(B_{A_i})\), \(Y_i=\log L_i\), and retain
the actual discrete cost
\[
 \mathcal C_X=\sum_i
 \frac{\delta_i C_{B_{A_i}}(Y_i)}{w(A_i)A_i^{11/10}}\ge0.
\]
The finite lcm identity and actual GA2 yield, for every fixed tolerance
\(\eta>0\) beyond the common starts,
\[
 \mathcal I_X\le-(c_Q-\eta)M_X-\mathcal C_X+\varepsilon_X,
 \quad\varepsilon_X=30E\mathcal R^{7/10}\log(2\mathcal R)=o(1).
\tag{A9}
\]
The whole-interval comparison (A8) independently yields
\[
 \mathcal I_X\le-(c_Q-\eta)M_X-
 \widetilde{\mathcal C}_X-\mathcal H_X,
\]
\[
 \widetilde{\mathcal C}_X=\sum_i\int_{A_i}^{C_i}
 \frac{C_{B_t}(t+D_t)}{w(t)t^{11/10}}dt,\quad
 \mathcal H_X=\sum_i\int_{A_i}^{C_i}
 \frac{\int_t^{C_i}[\lambda(s)-\lambda(s+D_t)]ds}
 {w(t)t^{11/10}}dt.
\tag{A10}
\]
Both costs are retained; they are not identified with one another.
GM at real \(t+H_t/3\), length \(H_t/3\), supplies a prime
between \(t+H_t/3\) and \(t+2H_t/3\) once the permitted relative
counting error is below \(1/2\). The admitted length ratios follow from
\(7/12<4/5<99/100\). Using \(x-1<q_1(x)<x\), its first layer
is absent at \(t\) and strictly present at \(B_t\), uniformly for
\(t\ge\ell\). Thus \(D_t>0\) eventually. The explicit slack
satisfies
\[
 0<\mathcal H_X\le EM_X\ell^{-1/10}=o(1),
\tag{A11}
\]
because \(C_i-t\le E\), the inner integral is at most
\(E\lambda(t)\), and \(\lambda(t)/w(t)<t\). This is an upper
bound for that specific slack; it gives no fixed favorable margin.
Pointwise (A8) also gives
\(\int_S\Phi^2\ge(c_Q-\eta)^2M_X\) for \(0<\eta<c_Q\).

The exact sufficient lower obligation is
\[
 \exists\text{ one fixed }\kappa<c_Q\quad
 \forall\text{ finite common starts }T\quad
 \exists\text{ qualifying original witness with }\ell\ge T:
 \quad\mathcal I_X\ge-\kappa M_X.
\tag{A12}
\]
The selected set is the **complete** original family for that witness.
Fix \(\eta=(c_Q-\kappa)/2\) first. Then (A9) contradicts (A12)
for a sufficiently late such witness, since it would require
\((c_Q-\kappa)M_X/2+\mathcal C_X\le\varepsilon_X\).
This proves the implication, not the lower bound.
The discrete departure mean differs by \(\varepsilon_X/M_X=o(1)\).
A favorable full mean gives a favorable departure atom after fixing
slack; a single favorable atom does not imply the full family mean.
An original cofinal atom would separately suffice for the GA2
contradiction, but has not been obtained.

The exact baseline in (A2) has the quantitative size
\[
 \frac12(1+\ell^{-1/5})^{-4}\int_S\sqrt t\,dt
 \le\mathcal D\le\frac12\int_S\sqrt t\,dt.
\tag{A13}
\]
This uses \(|w'/w|\le4/t\) and direct integration of
\(u\,w(t+u)/(w(t)t^{11/10})\). Replacing \(\mathcal D\) by its
leading term need not have absolute \(o(M)\) error. The \(d=1\)
row in (A4), by itself, is at least
\((\log\ell)(\mathcal D-\mathcal B)\); divided by \(M\) it
diverges by (A13). It cannot be deleted and paid by its own absolute
\(O(M)\) mass. No sign for a regrouped nonrough remainder is inferred.

### Reference powers at the exact first-moment scale

With \(\theta(x)=\sum_{q\le x}\log q\), define the analogous
\(\Phi_\theta\) by replacing \(\psi\) in \(\Phi\) with
\(\theta\). Finite step integration gives exactly
\[
 \Phi(t)-\Phi_\theta(t)
 =\sum_{q^k,\ k\ge2}\log q\,k_t(q^k)\ge0.
\tag{A14}
\]
At project pin `fe5fd5fbd2ef0072806ad77b3d10fcd8f2e46fa2`,
`Library/ArithSums/nicolas2025comparison.md` QH12 integrates the full
reference-square increment and gives its normalized value
\(1/4+o(1)\) for every sufficiently large real center. Its exact
derivative is \(1/(2\sqrt t)\), whereas the actual second-cutoff
derivative is \(q_2'(t)=(1/\sqrt{2t})[1+O(1/\log t)]\), giving the
distinct leading coefficient \(\sqrt2/4\). The lower-length enclosure
\(h_0=(2\sqrt t)^{7/12}\) costs
\(H_th_0/t^{11/10}=2^{7/12}t^{-1/120}\).

QH8 bounds the **sum of the two nonnegative** actual and reference
higher-increment inventories, on a common growing support
\(k\le7\log t\); hence it also bounds the reference increments
alone. QH9–QH10 give their integrated normalized allowance
\[
 C[t^{-1/6}(\log t)^{4/3}
 +t^{-19/180}(\log t)^{43/36}+t^{-3/10}\log t].
\]
This uses one common GM threshold, permitted enclosing intervals for
increments shorter than the GM minimum, and a finite small-cutoff bound;
GM is never applied below its minimum. The complete QQE error function is
\[
\begin{aligned}
 \mathcal F_Q(t)={}&1/\log t+t^{-1/5}
 +\log t\,e^{-((\log t)/3)^{1/4}}+t^{-1/120}\\
 &+t^{-3/10}\log t+t^{-1/6}(\log t)^{4/3}
 +t^{-19/180}(\log t)^{43/36}.
\end{aligned}
\]
Both square calculations, every growing higher layer, strict initial
actual atoms, excluded strict terminal atoms and weak reference endpoints
remain in that supplier. It has one unknown every-real tolerance start.
Consequently
\[
 \mathcal I_X=\int_S\Phi_\theta(t)dt+\tfrac14M_X+o(M_X).
\tag{A15}
\]
With fixed slack, an equivalent theta formulation of the open lower
obligation has coefficient strictly below
\(c_Q+1/4=\sqrt2/4\). This equivalence concerns existence of a fixed
strict coefficient, not equality at the unbuffered boundary. Under the
same RH-false suppliers the necessary upper bound is instead
\(\int_S\Phi_\theta\le-\sqrt2 M_X/4+o(M_X)\).
No favorable theta estimate replaces the all-power target.

### Full centered covariance and a genuine rough-block application

For each selected center put
\[
 Z_t(d)=\sum_{m\le J/d}\log m\,k_t(dm),\quad
 \Gamma(d,e)=\int_SZ_t(d)Z_t(e)dt,\quad
 b_1(d)=\int_Sa(t)Z_t(d)dt,\quad c_1=\int_Sa(t)^2dt.
\]
The exact finite convolution gives the complete centered expansion
\[
\begin{aligned}
 \int_S\Phi^2={}&\sum_d\mu(d)^2\Gamma(d,d)
 +2\sum_{z=1}^{J-1}\sum_{r=1}^{J-z}
 \mu(r)\mu(r+z)\Gamma(r,r+z)\\
 &-2\sum_d\mu(d)b_1(d)+c_1.
\end{aligned}
\tag{A16}
\]
This keeps the diagonal, all logarithmic cofactor rows, shifts, linear
term and baseline. For \(\Gamma_z(r)=\Gamma(r,r+z)\), extended by
zero past its support, and
\(S_r(z)=\sum_{d=1}^r\mu(d)\mu(d+z)\), exact Abel telescoping is
\[
 \sum_r\mu(r)\mu(r+z)\Gamma_z(r)
 =\sum_{r=1}^JS_r(z)[\Gamma_z(r)-\Gamma_z(r+1)],
 \quad\Gamma_z(J+1)=0.
\tag{A17}
\]
The actual qualitative source gives \(S_r(z)=o_z(r)\) for fixed
positive \(z\); it gives no uniform conclusion for all growing shifts.

Fix \(C_0\ge1\), \(1<\tau<2\), \(\epsilon=10^{-4}\) and a
large \(B\) beyond the named common supplier start. Let
\[
 P_0=e^{B^{1-\epsilon}},\quad
 P_0/\tau\le M_0\le e^{C_0B},\quad D=\lceil M_0\rceil,
\]
and let \(Z\subset(M_0,\tau M_0]\) be a finite set of positive
\(P_0\)-rough integers. Set
\[
 \omega_r=\max_{z\in Z}z|\Gamma_z(r)-\Gamma_z(r+1)|,\quad
 c_r(z)=z[\Gamma_z(r)-\Gamma_z(r+1)]/\omega_r
\]
when the row is nonzero, and set zero for empty sets or zero rows.
Then \(|c_r(z)|\le1\), and these coefficients are fixed before
the dummy sum over \(d\le r\). Thus
\[
 O_Z=\sum_{z\in Z}\sum_d\mu(d)\mu(d+z)\Gamma_z(d)
 =\sum_{r=1}^J\omega_r\sum_{z\in Z}c_r(z)S_r(z)/z.
\tag{A18}
\]

The actual ordinary preprint `build/qualitative/analytic-transfer.tex`,
lemma `lem:rough-multiplier`, at external pin
`adc7f1241b42e322a6451854ab7e4b4c146bf78a`, permits arbitrary fixed
bounded coefficients on this exact support. Its fixed multiplier integer
is \(h=1\) here. It gives
\[
 \|Q\|_\infty\ll B^{-1+\epsilon}\log B,\quad
 \int_{\mathbb T}|Q|^4\ll
 M_0^{-1}B^{-4+4\epsilon}(\log B)^6,
 \quad Q(\alpha)=\sum_Zc(z)e(z\alpha)/z.
\]
The source proof depends only on the rough support; no dependence of
coefficients on the averaging integer is permitted. Dependence on the
fixed row and original selected family is permitted.

The finite FQ/MRT derivation in the project pin's
`Library/Analytic/mantovanelli2026primeworkload.md` combines this premise
with named MRT Theorem 1.7 and the quantitative Möbius distance bound.
It retains exactly
\[
 \mathcal M_\mu(r,Q)=\inf_{|u|\le r,q\le Q,\chi\bmod q}
 \sum_{p\le r}\frac{1-\Re(\mu(p)\overline{\chi(p)p^{iu}})}p,
 \quad Q_H(r)=\min((\log r)^{1/125},(\log H)^5),
\]
and the frequency supremum outside the short-interval average.
For windows \(D,3D\), the exact early and late overlap triangles
have total absolute mass \(D(D-1)\), costing \((D-1)h_Z\) after
division by \(D\), where \(h_Z=\sum_Z1/z\le1\).
The complete finite allowance is
\[
 F_B(0)=0,\quad F_B(r)=rh_Z\quad(1\le r<3D),
\]
\[
\begin{aligned}
 F_B(r)={}&C_{20}r[B^{-1-\epsilon}
 +B^{-2+10\epsilon}(\log B)^8\\
 &+B^{-1+9\epsilon}(\log B)^7(\log r)^{-1/700}]
 +(D-1)h_Z\quad(r\ge3D).
\end{aligned}
\]
Here \(C_{20}\) is fixed, and the common supplier start is unknown.
The eventual simpler range is
\(r\ge\lceil\max(e^B,DB^2)\rceil\), with the actual rounded
\(D\). Applying this finite estimate to every fixed row of (A18)
proves the valid ordinary supplier-relative bound
\[
 |O_Z|\le\sum_{r=1}^J\omega_rF_B(r).
\tag{A19}
\]
The full exact budget, all small rows, nonrough shifts, diagonal, linear
term and baseline in (A16) remain necessary. Neither a small centered
energy bound nor a favorable first-moment sign follows. The covariance
of the different largest-optimizer sample in Mantovanelli is not
identified with this \(\Gamma\).

### Precise remaining analytic input and other source boundaries

The actual affine source permits \(\mu\): it is 1-bounded and
multiplicative, and its prime values, hence pretentious distances, equal
Liouville's. Its full growing-height nonpretentiousness is supplied by
the source's MRT Appendix C and fixed-modulus PNT argument. Applying the
qualitative binary result to \(\mu(n)\cdot1(n+1)\) gives the
classical \(M_\mu(x)=o(x)\), used in (A7). In all rows (A7), the
prefix is evaluated at \(x/m\), not at \(x\) or \(e^t\).
Qualitative decay for fixed \(m\) supplies neither a uniform small
bound for \(m\le J\) nor a paid sum with every \(\log m\).

Actual `DirichletL/Nonvanishing.lean` retains only strict
\(\Re s>7/8\), positive moduli and the principal-pole exception;
it is not RH. Its detector has ideal-character, modulus, width and
capacity hypotheses distinct from (A4). Ideal Möbius on the Eisenstein
ring does not become integer Möbius under norm: the inert prime ideal
\((2)\) has norm 4 and Möbius \(-1\), whereas \(\mu(4)=0\).
No ideal/detector transport to (A4) is claimed.

The separate D5 `finite_signed_response_identity` retains
\(A\ge e^{78}\), \(99/100\le c\le101/100\),
\(A<R_{\rm cut}\), \(cA\le R_{\rm cut}\). Its upper companion
also needs \(H>0\), \(0\le\epsilon<1\) and every admitted theta
increment on \([99A/100,198A/100]\) of length at least \(H\).
Its smooth boundary, volume and short allowance are not this kernel's
forward baseline. The short-uniformity sources likewise retain their
models, fixed testing complexity or well-factorable hypotheses and total
prime baseline. None has been silently instantiated as the missing sign.

The remaining input is (A12), or equivalently (A4)'s complete double sum
at least \(\mathcal D_X-\kappa M_X\), with one fixed
\(\kappa<c_Q\), after every common unknown start. By (A3), a proved
lower coefficient strictly below \(c_Q\) for the **same** weighted
\(\Lambda-1\) sum transfers using fixed slack. The negative selected
initial excursion does not bound its coupled forward tail; tiny future
Stieltjes errors do not bound the whole terminal comparison. No fixed
\(\kappa\), source sign, RH, stronger external formal closure or
all-integer Robin/5040 proof is supplied. The original signed target for
every \(n>5040\) remains **ACTIVE_UNPROVED**.

## Project application: density-weighted order-nine transport reaches 3e47

This `repo-derived` quantitative application consumes the complete zero-mass
bound already established in [Polak (W5), (X1)–(X2)](../Analytic/polak2026finiterobinca.md#keep-the-coupled-logarithmic-exponent-in-the-complete-density-tail)
inside the existing GAK positive-law transport. The density theorem,
whole-law construction, coefficient remainder and unrestricted reserve
are reused. Their proofs and finite zero computations are not repeated.
The additional step is to retain the density-weighted mass before choosing
the smoothing order. Under the five primary analytic premises listed in
GAK section 1, together with Chourasiya–Simonič's
[arXiv:2507.15184v2](https://arxiv.org/pdf/2507.15184v2), Corollary 1 and
Table 1, the resulting signed allowance applies uniformly on

$$
8\cdot10^{46}<A\le3\cdot10^{47},\qquad
L=\log A,\quad T_A=\sqrt A L.
\tag{GAD1}
$$

The cited density rows and finite-height verification remain external
premises. This is an ordinary analytic application, without a full
primary-proof audit, a Lean/kernel proof or a worldwide priority claim.

### Retain the actual real-part layers in the complete zero mass

Keep $H=3\cdot10^{12}$, $h=\log H$ and $s=\log(Hh)$. Reuse Polak's
positive-ordinate mass, including every actual zero with analytic
multiplicity,

$$
B_2(A)=\sum_{\gamma>H}m_\rho
 \frac{A^{\beta-1/2}+A^{1/2-\beta}}{\gamma^2},\qquad
\alpha(\sigma)=\frac{1+\sigma}{2-\sigma}.
$$

Its already established (X2) consequence is

$$
B_2(A)<2A^{1/4}S_2(H)
 +144Lh^4\int_{3/4}^1
    A^{\sigma-1/2}(Hh)^{-\alpha(\sigma)}\,d\sigma
 +30000H^{-2}(\sqrt A-A^{1/4}).
\tag{GAD2}
$$

This integrates the actual reflected population through every height
above $H$. In particular it does not substitute a finite-height ceiling
for a full-tail count. Its density source and parameter correspondence
are those of Polak (W1), (W2), (W5), (X1).

GAK25 gives $L>107$ on (GAD1). The same rational logarithm enclosure
gives $\log3<1.099$ and $\log10<2.303$, hence $h<28.74<29$.
The positive exponential prefix
$\sum_{j=0}^{10}(84/25)^j/j!>1437/50$ gives
$\log28.74<3.36$. Therefore $s<32.1$.

For $f_A(\sigma)=L(\sigma-1/2)-s\alpha(\sigma)$,

$$
f_A'(\sigma)=L-\frac{3s}{(2-\sigma)^2}\ge L-3s>0
\qquad(3/4\le\sigma\le1).
$$

Integrating this derivative lower bound from $\sigma$ to $1$ yields
$f_A(\sigma)\le f_A(1)-(L-3s)(1-\sigma)$. Thus

$$
\int_{3/4}^1e^{f_A(\sigma)}\,d\sigma
 <\frac{e^{L/2-2s}}{L-3s}.
$$

Since $h^4e^{-2s}=h^2/H^2$, (GAD2) gives the useful uniform envelope

$$
B_2(A)<2A^{1/4}S_2(H)
 +\frac{144h^2\sqrt A}{H^2}\frac{L}{L-3s}
 +\frac{30000\sqrt A}{H^2}.
\tag{GAD3}
$$

Set $r=5478\cdot10^{20}$. Then
$r^2=3.0008484\cdot10^{47}>3\cdot10^{47}$, so $\sqrt A<r$
and $A^{1/4}<10^{12}$. Also $L/(L-3s)<10$, because $L>107$,
$3s<96.3$ and $107/(107-96.3)=10$. Reuse
$S_2(H)<37/(25\cdot10^{12})$ to obtain

$$
B_2(A)<2(10^{12})\frac{37}{25\cdot10^{12}}
 +\frac{144(29)^2r}{H^2}\,10+\frac{30000r}{H^2}
 =\frac{9442616}{125}<76000.
\tag{GAD4}
$$

Reflection at fixed positive ordinate preserves multiplicity, and
conjugation supplies negative ordinates. Consequently

$$
B_2(A)=\sum_{|\gamma|>H}
       \frac{m_\rho A^{\beta-1/2}}{\gamma^2}.
\tag{GAD5}
$$

No further factor of two belongs in the complete high-zero response.

### Consume the complete mass with a lower-variance whole law

Use GAK3–GAK6 with the changed order $k=9$, leaving
$\delta=51/(20H)$ and $q=219/1000$. Put $x=\delta^2$ and reuse

$$
M_*=(1-2kx)^{-1},\qquad V_*=\frac{kx}{3-(k+3)x}.
$$

All denominators are positive; the whole support lies in $(.99,1.01)$
and the mean is exactly one. GAK41 and GAK47's actual-real-part
normalization give $|H_C(\rho)|<q^9$ for every $|\gamma|>H$;
the head bound remains $M_*$. The scalar normalization base in GAK47
is independent of $k$, so only its power changes.

Retain the original complete coefficient $F_A$ of GAK10, including
GAK12's remainder, in $Z_C(A)=\sum_\rho m_\rho H_C(\rho)F_A(\rho)$.
GAK24's head and tail remainder factors $527/500$ and $10001/10000$,
together with (GAD4)–(GAD5), imply

$$
T_A|Z_C(A)|<U_h+U_t,
$$

$$
\begin{aligned}
U_h&=\frac{108}{107}\frac{527}{500}\frac1{20}M_*,\\
U_t&=\frac{108}{107}\frac{10001}{10000}q^9(76000),\\
U_v&=\frac{260001}{500000}rV_*,\qquad
U_e=\frac{5M_*}{10^{23}}.
\end{aligned}
\tag{GAD6}
$$

GAK26's bound $\eta_0(A)<10^{-6}$ is independent of the upper
endpoint, and $\sqrt A>10^{23}$ still holds. GAK23 therefore gives
the original uncentered signed integral, retaining its cutoff atoms and
full elementary response,

$$
-T_AI_\psi(A)<U_h+U_t+U_v+U_e<\frac{19}{25}.
\tag{GAD7}
$$

The sufficient exact rational comparisons are
$U_h<.0532$, $U_t<.0889$, $U_v<.6175$ and
$U_e<6\cdot10^{-23}$. Their sum is less than $.76$.
No class average, favorable class selection or zero-phase sign is used.

### Keep the actual integer defect and the selected-source distinction

For each integer $n$ whose own clock $A=\log n$ satisfies (GAD1),
reuse its own nonnegative $d_A(n)$ and the exact identity GAK39.
GAK37's same unrestricted reserve obeys
$T_AR(A)>Q_R+L/(L+2)^3$, with the unchanged
$Q_R=67838284064811/83593750000000$ and $Q_R-19/25>1/20$.
Consequently, under the stated analytic premises,

$$
T_A\Delta(n)>
\frac1{20}+\frac{L}{(L+2)^3}+T_A d_A(n)>0.
\tag{GAD8}
$$

This bounded all-integer clock conclusion sets no defect to zero and
requires no CA or maximizer condition. It does not establish Robin
for every smaller integer up to this upper endpoint.

For the separate least-global-maximizer corollary, retain every extra
selection and lower-clock supplier in GAK section 10 and the corollary
following GAK51. That full existing chain already puts the same
selected $N$ above $\log N=8\cdot10^{46}$. Equation (GAD8) then
excludes $\log N\le3\cdot10^{47}$ for that same selected source.
This conditional consequence is not a bound for the least counterexample.

The parameter-specific
[rational program and results](https://github.com/the-omega-institute/trureturing-experiments/tree/fbe2ee18cadc21f30afc368a29a5604fdb44e8b5/experiments/robin-density-transport-3e47)
check the changed logarithm,
exponential prefix, density mass, support, normalization and complete
allowances. It does not certify the external analytic suppliers or the
full inference in Lean. For this fixed $H$ and order-nine law,
$V_*>0$ and the positive transport allowance grows with $\sqrt A$.
The original unbounded signed estimate and RH remain open.


## Complete higher-prime-power transport on an unlimited clock range

This application retains the GAK kernel, actual prime-power counting
functions and a single whole probability law. The inputs are the existing
GAK36–GAK39 pressure reserve and identity, and
[Dusart arXiv:1002.0442v1](https://arxiv.org/pdf/1002.0442v1),
Lemma 3.3 and Theorem 5.2. The square-root main term, convexity and
prime-counting estimates are published suppliers. The application below
pays the complete $k\ge2$ transport for this kernel; the first-power
prime transport and full smoothed signed response remain unpaid.
No additional all-integer Robin interval or global RH conclusion follows.

### The same whole law and complete counting function

Write $L=\log A$, $T_A=\sqrt A L$ and retain

$$
K(u)=\frac{1+\log u}{u^2\log^2u},\qquad
P_{\ge2}(t)=\psi(t)-\vartheta(t)
=\sum_{k\ge2}\vartheta(t^{1/k}).
$$

Let $\mu$ be any whole probability law satisfying
$99/100\le C\le101/100$ almost surely and $\mathbb EC=1$.
This includes the original GAK and GAD laws; no conditioning or
separate choice of law for different components is made. Define

$$
\begin{aligned}
J_c^{\ge2}(A)&=-\frac1c\int_A^\infty P_{\ge2}(cu)K(u)\,du,\\
\mathcal T_{\ge2}(A,\mu)&=J_1^{\ge2}(A)-\mathbb E J_C^{\ge2}(A),\\
m_\mu&=\mathbb EC^{-1/2},\qquad
V_\mu=\mathbb E(C-1)^2,\\
B(A)&=T_A\int_A^\infty\sqrt u K(u)\,du.
\end{aligned}
\tag{GPP1}
$$

The counting function retains every actual atom $p^k$, $k\ge2$, of
mass $\log p$, with $p^k\le t$ at endpoints. It is not replaced by a
density in the definition of either response.

### Uniform full-tail comparison

Put

$$
s=\frac{99A}{100}>(3594641)^2,\qquad
\epsilon(s)=\frac4{5\log^2s}+\frac{89}{50}s^{-1/6}.
$$

Dusart Lemma 3.3 gives
$0\le P_{\ge2}(t)-\vartheta(\sqrt t)<1.777745t^{1/3}$ for every
$t>0$. Theorem 5.2's row $(k,\eta_k,x_k)=(2,1/5,3594641)$ gives
$|\vartheta(y)-y|<y/(5\log^2y)$ for $y\ge3594641$.
Consequently, for $t\ge s$,

$$
|P_{\ge2}(t)-\sqrt t|
\le\sqrt t\left[\frac4{5\log^2t}+\frac{89}{50}t^{-1/6}\right]
\le\epsilon(s)\sqrt t.
\tag{GPP2}
$$

These are applications of the fixed primary statements; their underlying
finite computations and analytic proofs are external inputs.
Since every $cu\ge s$ for $u\ge A$, the same bound controls all scales
and the whole infinite tail. Positivity of $K$ and the integrable
square-root majorant justify exchanging expectation and integration.
Subtracting the two responses gives

$$
\mathcal T_{\ge2}
=\int_A^\infty
\left[\mathbb E\frac{P_{\ge2}(Cu)}C-P_{\ge2}(u)\right]K(u)\,du.
$$

The square-root main term is $(m_\mu-1)\sqrt u$; the error is at most
$(m_\mu+1)\epsilon(s)\sqrt u$. Thus

$$
\left|T_A\mathcal T_{\ge2}-B(A)(m_\mu-1)\right|
\le B(A)(m_\mu+1)\epsilon(s).
\tag{GPP3}
$$

Integration by parts, with the upper boundary zero, gives

$$
B(A)=2-T_A\int_A^\infty\frac{du}{u^{3/2}\log^2u},\qquad
2-\frac2L\le B(A)<2.
\tag{GPP4}
$$

For $f(c)=c^{-1/2}$, $0<f''(c)=3c^{-5/2}/4<1$ throughout the support.
Convexity and Taylor's bound, using the exact whole-law mean, imply

$$
0\le m_\mu-1\le\frac{V_\mu}{2}\le\frac1{20000}.
$$

If $A>e^{107}$, then $s>e^{106}$, so
$4/(5\log^2s)<1/14000$ and $(89/50)s^{-1/6}<1/70000$.
The second comparison follows from $e>2$ and $106/6>17$.
Hence $\epsilon(s)<3/35000<1/10000$ and $m_\mu+1<201/100$.
Combining these bounds with GPP3–GPP4 proves

$$
\left|T_A\mathcal T_{\ge2}(A,\mu)\right|
<2\left[\frac1{20000}+\frac{201}{100}\frac1{10000}\right]
=\frac{251}{500000}<\frac1{1000}
\qquad(A>e^{107}).
\tag{GPP5}
$$

This is uniform for all such real clocks, with no upper endpoint,
and allows the whole law to vary with $A$ within the stated conditions.

### Fixed-law sign and the original reserve consumer

For a fixed law, GPP3–GPP4 and $\epsilon(.99A)\to0$ give

$$
T_A\mathcal T_{\ge2}(A,\mu)\longrightarrow2(m_\mu-1).
\tag{GPP6}
$$

For a fixed nondegenerate mean-one law, strict convexity makes this
limit strictly positive. This is eventual positivity; GPP5 does not
assert positivity for every $A>e^{107}$, or for a varying law.
In particular, the negative local square atoms from GAK21 cannot
be recorded as extra reserve without their regular companions:
the complete higher-power contribution eventually has the opposite sign.

Let $J_c^\vartheta$ retain the GAK definition with
$\vartheta(cu)-cu$ in place of $\psi(cu)-cu$, and set
$\mathcal T_\vartheta=J_1^\vartheta-\mathbb E J_C^\vartheta$.
Then $J_c^\psi-J_c^\vartheta=J_c^{\ge2}$ exactly.
For each integer's own clock $A=\log n>e^{107}$, GAK39 therefore gives

$$
\Delta(n)=R(A)+d_A(n)-J_\mu^\psi(A)
-\mathcal T_\vartheta(A,\mu)-\mathcal T_{\ge2}(A,\mu).
$$

Retain every analytic premise and event convention of GAK36–GAK39.
The original unrestricted reserve bound GAK37 requires only its lower
clock, so it still applies on this unlimited range. Using GPP5 yields

$$
\begin{aligned}
T_A\Delta(n)>&\ Q_R-\frac1{1000}
+\frac{L}{(L+2)^3}+T_A d_A(n)\\
&-T_AJ_\mu^\psi(A)-T_A\mathcal T_\vartheta(A,\mu),\\
Q_R={}&\frac{67838284064811}{83593750000000}.
\end{aligned}
\tag{GPP7}
$$

The actual nonnegative defect of this same integer is retained; it is
not replaced by zero or by the defect of a selected optimizer.
GPP7 pays the complete higher-prime-power transport with an explicit
small budget on an unlimited range. It supplies no upper bound for
the remaining combined $J_\mu^\psi+\mathcal T_\vartheta$ at the same
source. The full signed response still includes all actual zeros,
real parts, coefficients and elementary terms. These ordinary
applications are not new prime-counting theorems or Lean-certified
results; the all-integer Robin inequality and RH remain open.


## A classical positive xi law pays the smoothed response on an unlimited range

This application directly reuses the distribution in
[Biane–Pitman–Yor, arXiv:math/9912170v1](https://arxiv.org/pdf/math/9912170v1),
§2.2, Proposition 1(i) and equation (20). The positive xi law and its
functional equation are classical results, not new constructions here.
The xi null-vector mechanism is also already used in the
[Weil comparison application](../Weil/frankliebseiringer2006hardy.md);
its vanishing at actual zeros is not a new result. The present consumer
is the original Robin response, whose integrability, broad-law transport
and reserve must be paid separately.
The other inputs are this note's all-scale remainder estimate GE2,
integrated coefficient bound GAK13, complete higher-power comparison
GPP2–GPP4, and same-integer identity and reserve GAK37–GAK39. Their
analytic premises, finite-verification inputs and endpoint conventions
are retained. No new zero computation or prime-counting theorem is used.

The law below has unbounded support. It does not satisfy GPP1's narrow
support hypothesis, so that section's uniform transport budget cannot
be applied to it. The estimates below instead pay both small scales and
the whole higher-power tail for this one law. They leave the original
first-prime transport unbounded and do not prove RH or the strict Robin
inequality for every integer greater than 5040.

### Reuse the published law with the consumer's mean normalization

Use the usual completed function
$\xi(s)=s(s-1)\pi^{-s/2}\Gamma(s/2)\zeta(s)/2$.
The cited proposition supplies a positive random variable $Y$ with

$$
\mathbb EY^s=2\xi(s)\qquad(s\in\mathbb C).
$$

In particular all real moments exist and $\mathbb EY=1$. Equation (20)
identifies $Y^{-1}$ with the size-biased law of $Y$.
Put

$$
m=2\xi(2)=\frac\pi3,\qquad C=\frac1{mY},\qquad
\mu=\operatorname{Law}(C).
$$

The published functional equation $\xi(s)=\xi(1-s)$ gives exactly

$$
\mathbb EC=1,\qquad
H_C(s):=\mathbb EC^{s-1}=2m^{1-s}\xi(s).
\tag{XLR1}
$$

Thus $H_C(\rho)=0$ for every actual nontrivial zero, with no assumption
about its real part. This uses a fixed positive probability law, not a
choice of signs or a deletion of a zero tail. The moments needed below
are

$$
\begin{aligned}
\mathbb EC^{-1}&=m,\\
M_4:=\mathbb EC^{-4}&=\frac{2\pi^2}{15}m^4<2,\\
1\le m_{1/2}:=\mathbb EC^{-1/2}
&=\sqrt m\,\mathbb E\sqrt Y\le\sqrt m<\frac{128}{125}.
\end{aligned}
\tag{XLR2}
$$

For the last line use convexity with $\mathbb EC=1$, then Cauchy–Schwarz
with $\mathbb EY=1$. The rational bounds follow from $\pi<22/7$:
$m<22/21$, $(22/21)^4<5/4$, $\pi^2<10$, and
$22/21<(128/125)^2$.

### Average the actual full response, including scales below the cutoff

Keep $L=\log A$, $T_A=\sqrt A L$, the GPP kernel $K$ and the actual
$J_c^\psi$ of GAK14. In this section $A>e^{107}$.
The expectation of its infinite integral is absolutely justified as
follows. At each $u\ge A$, divide the law into
$G_u=\{C\ge u^{-1/2}\}$ and its complement.
On $G_u$, $Cu\ge\sqrt u$ and the existing unconditional logarithmic PNT
input gives

$$
\frac{|\psi(Cu)-Cu|}{C}
\le\frac{4C_\psi u}{\log^2u}.
$$

On the complement, $\psi(t)\le t\log t$ for $t\ge1$, and $\psi(t)=0$
for $t<1$. Markov's inequality and XLR2 give

$$
\begin{aligned}
\mathbb P(C<u^{-1/2})&\le M_4u^{-2},\\
\mathbb E\left[\frac{\psi(Cu)}C;\ C<u^{-1/2}\right]
&\le\tfrac12M_4u^{-1}\log u<u^{-1}\log u,\\
\mathbb E\left[\frac{|\psi(Cu)-Cu|}C;\ C<u^{-1/2}\right]
&<u^{-1}(\log u+2).
\end{aligned}
\tag{XLR3}
$$

Both bounds become integrable after multiplication by $K(u)$.
Consequently $\mathbb E|J_C^\psi|<\infty$, and absolute Fubini permits
expectation inside its full infinite integral. No portion with $Cu<1$
is discarded.

The integrated zero series can likewise be averaged absolutely.
For $0<\beta<1$,
$\mathbb EC^{\beta-1}\le1+\mathbb EC^{-1}=1+m$.
Taking the endpoint limit in GAK13, and using $A^{\beta-1}\le1$, yields

$$
\sum_\rho m_\rho\mathbb E
 \left|C^{\rho-1}F_A(\rho)\right|
\le 2w(A)(1+m)\mathcal C_\zeta<\infty.
$$

Here $w(A)=(1+\log A)/\log^2 A$, and $\mathcal C_\zeta$ is the same
complete absolute zero weight used in GE1. This is an exchange of the
integrated coefficient series, not of the unsmoothed explicit formula.
XLR1 and GAK14–GAK15 therefore give

$$
Z_\mu(A)=\sum_\rho m_\rho H_C(\rho)F_A(\rho)=0,
\qquad J_\mu^\psi(A)=\mathbb Er_C(A).
$$

GE2 applies to every positive $c$, including $cA<1$. Averaging its
one-sided bound gives the actual signed estimate

$$
T_AJ_\mu^\psi(A)<\frac{5m}{\sqrt A}<\frac1{1000}
\qquad(A>e^{107}).
\tag{XLR4}
$$

Integrability of $r_C=J_C-Z_C$ follows from the two preceding absolute
bounds. XLR4 is an upper bound, not an absolute estimate. All pole,
constant and trivial-zero corrections are still included in $r_C$.

### Pay the complete higher-prime-power transport for this same law

Use the actual $P_{\ge2}=\psi-\vartheta$ and
$\mathcal T_{\ge2}$ of GPP1, now with this unbounded $\mu$.
On $G_u$, use GPP2 with $s=\sqrt A$; it applies because $Cu\ge\sqrt u$.
On its complement, XLR3 also bounds $P_{\ge2}(Cu)/C$, and

$$
\sqrt u\,\mathbb E[C^{-1/2};\ C<u^{-1/2}]
\le M_4u^{-5/4}<2u^{-5/4}.
$$

The good-scale square-root comparison, these two small-scale tails,
and GPP2 for $P_{\ge2}(u)$ give

$$
\begin{split}
\left|\mathbb E\frac{P_{\ge2}(Cu)}C-P_{\ge2}(u)
 -(m_{1/2}-1)\sqrt u\right|
\le{}&(m_{1/2}+1)\epsilon(\sqrt A)\sqrt u\\
&+u^{-1}\log u+2u^{-5/4}.
\end{split}
\tag{XLR5}
$$

These same bounds justify the nonnegative Tonelli exchange and its
finiteness. With the unchanged $B(A)$ of GPP4, integration gives

$$
\begin{split}
\left|T_A\mathcal T_{\ge2}
 -B(A)(m_{1/2}-1)\right|
\le{}&B(A)(m_{1/2}+1)\epsilon(\sqrt A)\\
&+L A^{-3/2}+2A^{-7/4}.
\end{split}
\tag{XLR6}
$$

Indeed $T_A\int_A^\infty u^{-1}\log u K(u)du\le L A^{-3/2}$,
and $T_A\int_A^\infty2u^{-5/4}K(u)du<2A^{-7/4}$, by
$(1+\log u)/\log u\le2$ and $\log u\ge L$.

For the constants, $\sqrt A>e^{48}$ and $e>8/3$ give $e^8>2500$ and

$$
\epsilon(\sqrt A)
<\frac1{2500}+\frac{89}{125000}<\frac1{500}.
$$

Also $L A^{-3/2}+2A^{-7/4}<1/1000$: both terms decrease with $L>107$,
and $e^L>2^L$ with $L<e^{L/2}$ bounds their sum by
$e^{-L}+2e^{-7L/4}<3\cdot2^{-107}<1/1000$.
Using GPP4's $B(A)<2$ and XLR2 now gives

$$
\left|T_A\mathcal T_{\ge2}(A,\mu)\right|
<\frac6{125}+\frac{506}{62500}+\frac1{1000}
<\frac3{50}.
\tag{XLR7}
$$

This covers all actual powers $k\ge2$, their endpoints, the entire
positive law and the whole infinite integral. Together with XLR4 it pays
one combined actual quantity on the unlimited range:

$$
T_A\bigl[J_\mu^\psi(A)+\mathcal T_{\ge2}(A,\mu)\bigr]
<\frac{61}{1000}\qquad(A>e^{107}).
\tag{XLR8}
$$

### Consume the bound at the original integer and state the unpaid term

Define $\mathcal T_\vartheta=J_1^\vartheta-\mathbb EJ_C^\vartheta$
using this same $\mu$. The preceding integrability bounds also pay this
expectation. For each integer's own clock $A=\log n>e^{107}$, the
unchanged exact GAK39 identity reads

$$
\Delta(n)=R(A)+d_A(n)-J_\mu^\psi(A)
 -\mathcal T_\vartheta(A,\mu)-\mathcal T_{\ge2}(A,\mu).
$$

Combining XLR8 with the original reserve GAK37 gives

$$
\begin{aligned}
T_A\Delta(n)>{}&Q_R-\frac{61}{1000}
 +\frac{L}{(L+2)^3}+T_A d_A(n)-T_A\mathcal T_\vartheta(A,\mu)\\
>{}&\frac34+\frac{L}{(L+2)^3}
 +T_A d_A(n)-T_A\mathcal T_\vartheta(A,\mu),
\end{aligned}
\tag{XLR9}
$$

where the last strict inequality uses the existing exact
$Q_R=67838284064811/83593750000000>811/1000$.
The nonnegative defect belongs to this same integer and the original
unrestricted pressure; no optimizer substitution is made.

XLR8 is an estimate for the actual combined smoothed response and
higher-power transport. XLR9 has only the first-prime transport left
unbounded. No sufficient upper bound for that term is established here.
Indeed $J_\mu^\psi+\mathcal T_\vartheta+\mathcal T_{\ge2}=J_1^\psi$
exactly: annihilating the smoothed zero series does not annihilate the
unsmoothed arithmetic error. The first-prime transport keeps the
remaining oscillation, and its wide-scale cancellations have not been
bounded at this reserve. This application is paper mathematics using
published and existing inputs, with no Lean certification or literature
priority claim. RH and strict Robin for every integer $n>5040$ remain
unproved.

## A full-response budget for logarithmically growing signed xi clocks

This application reuses XLR1's published Biane–Pitman–Yor law, the
integrated explicit formula GAK10–GAK16, GPP2–GPP4 and the original
same-integer account GAK37–GAK39. It is a repo-derived application controlling a changing family of
signed clocks; the fixed positive-law allowance XLR8 is not applied
to that family. The interpolation algebra is standard, and no
literature priority or Lean certification is claimed.

The additional classical inputs are
[Johnston–Yang, arXiv:2204.01980v2](https://arxiv.org/pdf/2204.01980v2),
Lemma 2.7, already recorded as
[PK (Z1)](../Analytic/polak2026finiterobinca.md#the-additional-published-input),
and [DLMF 5.11.9](https://dlmf.nist.gov/5.11.E9) and
[25.2.10](https://dlmf.nist.gov/25.2.E10).
The latter formula with $n=1$ gives
$\zeta(\sigma+it)=O((1+|t|)^3)$ uniformly for $0\le\sigma\le1/2$:
the periodic-Bernoulli integral is uniformly absolutely bounded
there, and its coefficient is a cubic polynomial. Vertical-strip
Stirling and the entire continuation of $\xi$ consequently give
rapid vertical decay for XLR1's
$h(s)=2m^{1-s}\xi(s)$ on this strip. These are published inputs and
their parameter correspondence, rather than new zeta estimates.

### One signed family and a common degree cap

Put $m=\pi/3$ and retain the whole law $\mu$ of XLR1, with
$h(s)=\int c^{s-1}\,d\mu(c)$. For an integer $k\ge1$ define

$$
Q(z)=(1-z)(1-z/m),\qquad
P_k(z)=1-Q(z)^k=\sum_{j=1}^{2k}p_{k,j}z^j,
$$

$$
\nu_k=\sum_{j=1}^{2k}p_{k,j}\mu^{*j},\qquad
H_k(s)=\int c^{s-1}\,d\nu_k(c)=P_k(h(s)).
\tag{GPC1}
$$

Here convolution is multiplicative. The signed mass, first moment
and inverse first moment are all one, since
$h(0)=m$ and $h(1)=h(2)=1$. Also $H_k(\rho)=0$ at every actual
nontrivial zero, with no critical-line assumption. The usual
polynomial interpolation gives vanishing derivatives of $H_k-1$
through order $k-1$ at $s=0,1$. These algebraic identities provide
neither positivity of $\nu_k$ nor Jensen's inequality.

For real $t$ let $b_t=\int c^t\,d\mu(c)$ and
$R_t=(1+b_t)(1+b_t/m)$. All these moments are finite. The
coefficient absolute-value envelope gives

$$
M_t(k):=\int c^t\,d|\nu_k|(c)\le1+R_t^k.
\tag{GPC2}
$$

Fix $\eta=1/24$. Choose one $\kappa>0$ so that
$\kappa\log R_t\le\eta$ for every
$t\in\{0,-1,-4,-2/3,1/3\}$. For $1\le k\le\kappa\log A$,

$$
M_t(k)\le2A^\eta
\qquad(t\in\{0,-1,-4,-2/3,1/3\},\ A\ge1).
\tag{GPC3}
$$

The same $\kappa$ is decreased below to control the complete zero
spectrum. No bounded-total-variation or fixed-degree limit is assumed.

Write $\rho=\beta+i\gamma$, $\delta_\rho=1-\beta$. The classical
zero-free region, together with the existing finite verification for
$|\gamma|<2$, gives

$$
\delta_\rho\ge\frac{a_0}{\log(2+|\gamma|)},\qquad
a_0=\min\{1/5.5666305,\ (\log2)/2\}>0.
$$

Only this finite head uses verified criticality. Rapid vertical
decay supplies $B_0<\infty$ with
$|h(\rho/2)|\le B_0/(1+|\gamma|)^2$. Since

$$
\log_+|Q(z)|
\le(1+1/m)|z|,
$$

there is a fixed $B>0$ with
$\log_+|Q(h(\rho/2))|\le(B/a_0)\delta_\rho$.
Reduce $\kappa$ so that $\kappa B/a_0\le1/4$. Then, simultaneously
for all actual zeros and all $k\le\kappa\log A$,

$$
A^{\beta/2-1/2}|H_k(\rho/2)|
\le2\exp\!\left(-\frac{\delta_\rho\log A}{4}\right).
\tag{GPC4}
$$

Indeed $|H_k|\le1+|Q(h)|^k\le2A^{\delta_\rho/4}$.
This bounds filter growth and the zero-free gap on the same zero.
No numerical value of $\kappa$ or common starting point is supplied.

### Uniform full smoothed response

Keep $L=\log A$, $T_A=\sqrt A L$, and the unchanged $K,F_A,J_c^\psi$.
In particular $J_1^\psi=-I_\psi$; the integrated zero coefficient in
$J_c^\psi$ has the positive sign $c^{\rho-1}F_A(\rho)$.
The following assertions hold uniformly through the common degree cap:

$$
\begin{aligned}
\sup_{1\le k\le\kappa L}T_A|J_{\nu_k}^\psi(A)|&\longrightarrow0,\\
\sup_{1\le k\le\kappa L}
\left|T_A\mathcal T_{\ge2}(A,\nu_k)
 -B(A)(H_k(1/2)-1)\right|&\longrightarrow0.
\end{aligned}
\tag{GPC5}
$$

Here $J_\nu^\psi=\int J_c^\psi\,d\nu(c)$ and the actual transport is

$$
\mathcal T_{\ge2}(A,\nu)
=\int_A^\infty
 \left[\int\frac{P_{\ge2}(cu)}c\,d\nu(c)-P_{\ge2}(u)\right]K(u)\,du.
$$

All powers, all positive clocks and the entire infinite tail remain.
We establish absolute integrability against $|\nu_k|$ before using
any signed cancellation.

Put $E_A=\{c<A^{-1/2}\}$ and abbreviate $M_t=M_t(k)$. The absolute
measure satisfies

$$
\begin{aligned}
|\nu_k|(E_A)&\le A^{-2}M_{-4},\\
\int_{E_A}c^{-1}\,d|\nu_k|&\le A^{-3/2}M_{-4},\\
\int_{E_A}c^{-1/2}\,d|\nu_k|&\le A^{-7/4}M_{-4}.
\end{aligned}
\tag{GPC6}
$$

For absolute integrability of $J_\nu^\psi$, apply XLR3 to
$|\nu_k|$, splitting at $c=u^{-1/2}$ for each $u$.
Above that cut the logarithmic PNT gives
$O(M_0u/\log^2u)$; below it the trivial
$\psi(t)\le t\log_+t$ gives $O(M_{-4}u^{-1}(1+\log u))$.
Both are $K$-integrable. For the actual contribution of the fixed
$E_A$, split again at $u^{-1/2}$. The upper part costs
$O(M_{-4}A^{-3/2}/L)$ after multiplication by $T_A$, and the lower
part costs $O(M_{-4}L A^{-3/2})$.

On $E_A^c$ one has $cu\ge\sqrt A$. The finite-endpoint integrated
explicit formula and GAK13 therefore apply. The zero count makes
$\mathcal S_1=\sum_\rho m_\rho/(|\rho||1-\rho|)$ finite.
Replacing the complementary Mellin integral by the full
$H_k(\rho)=0$ leaves only $E_A$; GPC6 bounds its normalized cost
by $O(M_{-4}\mathcal S_1/A)$. The constant and trivial-zero terms
have absolute normalized cost $O(M_{-1}/\sqrt A)$:
their integral is $O(M_{-1}/(AL))$, using
$|\log(1-(cu)^{-2})|\le2(cu)^{-2}$ on the good set.

All constants here are independent of $k$. GPC3 makes each allowance
vanish, proving the first line of GPC5. This uses absolute elementary
remainders, not a one-sided positive-law estimate for signed $\nu_k$.

### The square term with every zero retained

Define

$$
S_\nu(A)=\int_A^\infty\int
 \frac{\psi(\sqrt{cu})-\sqrt{cu}}c\,d\nu(c)K(u)\,du.
$$

On $E_A$, $c<1$ and the absolute integrand before multiplication
by $K$ is at most
$\sqrt u\,c^{-1/2}(1+\log u)$. GPC6 bounds its normalized tail
by $O(M_{-4}L^2 A^{-7/4})$.

For the whole square integral,
$c^{-1/2}(1+\log_+c)\le C(1+c^{-1})$ supplies an absolute
large-clock majorant; its small-clock part is covered by GPC6.
On $E_A^c$, $\sqrt{cu}\ge A^{1/4}$. The same finite-endpoint
explicit-formula argument, now with $s=\rho/2$, has zero coefficient

$$
-\frac12c^{\rho/2-1}F_A(\rho/2).
$$

The factor $1/2$ follows from the original $1/\rho$ coefficient;
it is not absorbed into the zero multiplicity. GAK13 gives a
summable finite-endpoint majorant. The constant and trivial-zero
terms again cost $O(M_{-1}/\sqrt A)$ after normalization, using
$|\log(1-(cu)^{-1})|\le2/(cu)$.
Completing the complementary Mellin moment to $H_k(\rho/2)$ costs
$O(M_{-4}A^{-3/2}\mathcal S_2)$, where

$$
\mathcal S_2=\sum_\rho\frac{m_\rho}{|\rho||1-\rho/2|}<\infty.
$$

For the complete full-law sum, GAK13 and GPC4 give the common
normalized majorant

$$
C\sum_\rho
 \frac{m_\rho}{|\rho||1-\rho/2|}
 \exp\!\left(-\frac{\delta_\rho\log A}{4}\right)
 \longrightarrow0.
\tag{GPC7}
$$

Both ordinate signs and actual multiplicities occur in these sums.
The convergence follows from the summable $\mathcal S_2$ majorant
and $\delta_\rho>0$ at each actual zero; GPC4 makes it independent
of the changing $k$. This proves
$\sup_{k\le\kappa L}T_A|S_{\nu_k}(A)|\to0$.
It does not exchange an unsmoothed zero series absolutely.

### Every remaining prime power

For every $t>0$ there is the exact finite-sum identity

$$
\begin{aligned}
P_{\ge2}(t)&=\psi(\sqrt t)+R_3(t),\\
R_3(t)&=\sum_{j\ge3}\vartheta(t^{1/j})-P_{\ge2}(\sqrt t).
\end{aligned}
$$

The global Chebyshev bound and the number of admissible exponents
give $|R_3(t)|\le C t^{1/3}(1+\log_+t)^2$. Below the first prime
power both sides vanish; no small-$t$ singularity is introduced.
For $u\ge A\ge e$,

$$
\int\frac{|R_3(cu)|}{c}\,d|\nu_k|(c)
\le C u^{1/3}(1+\log u)^2(M_{-2/3}+M_{1/3}).
$$

Here $(1+\log_+(cu))^2\le C(1+\log u)^2(1+c)$.
The full normalized $K$-tail is
$O(A^{\eta-1/6}L^2)\to0$, uniformly in $k$.
This also supplies absolute Fubini for the complete remainder.
Separately GPP2 pays the reference
$P_{\ge2}(u)-\sqrt u=o(\sqrt u)$ on the entire $u\ge A$ tail,
with no growing total-variation multiplier on that reference.
The square main term is
$\sqrt u\int c^{-1/2}\,d\nu_k=\sqrt u\,H_k(1/2)$.
Combining these facts proves the second line of GPC5.

### The original integer's account and the unpaid estimate

XLR2 gives $b=h(1/2)\in[1,\sqrt m]$ and
$-1<Q(b)\le0$. For even $k$,
$H_k(1/2)-1=-Q(b)^k\le0$. Thus GPC5 supplies one
$\epsilon_*(A)\to0$, independent of even $k$ in the cap, such that

$$
T_A[J_{\nu_k}^\psi(A)+\mathcal T_{\ge2}(A,\nu_k)]
\le\epsilon_*(A).
\tag{GPC8}
$$

For any integer-valued $k(A)\to\infty$ within the cap, this combined
expression tends to zero in absolute value; parity is unnecessary
for that limit. No convergence to a positive law or to $\delta_1$
is asserted.

Use the centered response
$J_c^\vartheta=-c^{-1}\int_A^\infty[\vartheta(cu)-cu]K(u)\,du$
and $\mathcal T_\vartheta=J_1^\vartheta-\int J_c^\vartheta\,d\nu_k$.
Their integrability follows from the preceding $\psi$ and
proper-power bounds. For each integer's own $A=\log n>e^{107}$,
mass one preserves the exact account

$$
\Delta(n)=R(A)+d_A(n)-J_{\nu_k}^\psi
 -\mathcal T_\vartheta(A,\nu_k)-\mathcal T_{\ge2}(A,\nu_k).
$$

GAK37 and GPC8 therefore imply, eventually and uniformly for even
$2\le k\le\kappa L$,

$$
T_A\Delta(n)>
 Q_R+\frac{L}{(L+2)^3}+T_A d_A(n)
 -T_A\mathcal T_\vartheta(A,\nu_k)-\epsilon_*(A).
\tag{GPC9}
$$

The nonnegative defect and unrestricted pressure still belong to
this same integer. GPC5–GPC9 admit clocks with an increasing number
of exact logarithmic moment cancellations while paying the full
smoothed and higher-power response. They do not bound the
remaining first-prime transport against that defect. In particular,
$J_{\nu_k}^\psi+\mathcal T_\vartheta+\mathcal T_{\ge2}=J_1^\psi$
still holds exactly. No mean-one price normalization, signed Jensen
inequality, new finite verification interval or RH/Robin proof follows.

## Exact nonlinear price calibration with adjacent growing xi clocks

This repo-derived application reuses GPC1–GPC9 and XLR1, including
the published BPY law, all real moments and the complete growing-family
response budget. Adjacent-error extrapolation, polynomial
interpolation and Gamma integrals are standard tools. The additional
calculation concerns their full-law, moving-degree price error and
the actual small-clock cutoff. No literature priority, Lean
certification or signed Jensen inequality is claimed.

### The same source and the actual price observation

Retain $m=\pi/3$, $h$, $Q$, $\nu_j$ and $H_j$ of GPC1.
Write $L=\log A$, $T_A=\sqrt A L$, and choose

$$
k=k(A)=\lfloor L^{1/3}\rfloor,\qquad
\chi_A(c)=\max(c,e/A),\qquad
\lambda(x)=\frac1{x\log x}\quad(x\ge e).
$$

The normalized price observation is

$$
y_A(c)=\frac{\lambda(A\chi_A(c))}{\lambda(A)}
 =\frac{AL}{A\chi_A(c)\log(A\chi_A(c))}.
\tag{APC1}
$$

For all $c>0$, $y_A(c)\le L/c$. Thus its integral against each
$|\nu_j|$ is finite. Define

$$
Y_{A,j}=\int y_A(c)\,d\nu_j(c),\qquad
E_{A,j}=1-Y_{A,j}\qquad(j=k,k+1).
$$

The original source and its image under $\chi_A$ remain distinct.
The effect of this cutoff on the prime responses is estimated below.

All real moments justify differentiating $h$ near zero. The elementary
$\log c\le c-1$ gives
$h'(0)=\int c^{-1}\log c\,d\mu\le1-m<0$. Consequently

$$
\alpha=-\frac{m-1}{m}h'(0)>0,\qquad
g(u)=Q(h(-u))=\alpha u\exp(O(u)).
\tag{APC2}
$$

Here $Q'(m)=(m-1)/m$. Choose a fixed $u_0\in(0,1)$ and $D<\infty$
so that $g(u)>0$ and
$|\log(g(u)/(\alpha u))|\le Du$ for $0<u\le u_0$.
Neither constant depends on $A$ or $j$.

### The complete price error from a finite Laplace interval

Use only the truncated function

$$
f_A(c)=Lc^{-1}\int_0^{u_0}e^{-u(L+\log c)}\,du.
$$

This integral also defines the value when $L+\log c=0$.
No full half-line Laplace integral is interchanged with the clock law.
Put $\tau=e/A$. For $c\ge\tau$,

$$
|y_A(c)-f_A(c)|
 =y_A(c)e^{-u_0(L+\log c)}
 \le L A^{-u_0}c^{-1-u_0}.
$$

For $c<\tau$,

$$
|f_A(c)|\le Lu_0[c^{-1}+A^{-u_0}c^{-1-u_0}],
\qquad y_A(c)=AL/e.
$$

Using GPC2's absolute moments
$M_t(j)=\int c^t\,d|\nu_j|$ and
$\int_{c<\tau}c^{-q}\,d|\nu_j|\le\tau^{4-q}M_{-4}(j)$
for $q=0,1,1+u_0$ proves the whole-law bound

$$
\left|Y_{A,j}-\int f_A\,d\nu_j\right|
 \le L A^{-u_0}M_{-1-u_0}(j)
       +C L A^{-3}M_{-4}(j).
\tag{APC3}
$$

All $c>0$, including $Ac\le1$, occur in this estimate.
Absolute Fubini on $[0,u_0]$ follows from
$M_{-1}(j)+M_{-1-u_0}(j)<\infty$. Therefore

$$
\int f_A\,d\nu_j
 =L\int_0^{u_0}e^{-Lu}H_j(-u)\,du
 =1-e^{-u_0L}-L\int_0^{u_0}e^{-Lu}g(u)^j\,du.
$$

For $j=k,k+1$, GPC2 gives $M_t(j)=\exp(O(j))$ at every fixed $t$.
Since $j=O(L^{1/3})$, APC3 implies, for one fixed $c_0>0$,

$$
E_{A,j}=I_{L,j}+O(e^{-c_0L}),\qquad
I_{L,j}=L\int_0^{u_0}e^{-Lu}g(u)^j\,du.
\tag{APC4}
$$

The cutoff and truncation have thus been controlled before taking a
relative asymptotic.

### Moving order and the separated adjacent errors

For $L>2Dj$, APC2 bounds $I_{L,j}$ between

$$
\alpha^jL\int_0^{u_0}e^{-(L+Dj)u}u^j\,du
\quad\hbox{and}\quad
\alpha^jL\int_0^{u_0}e^{-(L-Dj)u}u^j\,du.
$$

The corresponding full Gamma integrals are
$\alpha^jL j!/(L\pm Dj)^{j+1}$. The fraction beyond $u_0$ is at most
$(j+1)/[(L\pm Dj)u_0]$, by the first moment of the normalized positive
Gamma integral. As $j=k,k+1$, one has $j^2/L\to0$, so

$$
I_{L,j}=\frac{\alpha^j j!}{L^j}
       \left(1+O\!\left(\frac{j^2}{L}\right)\right).
$$

Moreover $\log(\alpha^j j!L^{-j})=-O(j\log L)=o(L)$.
The absolute error in APC4 is therefore negligible relative to this
main term. This proves the full-law, moving-order formula

$$
E_{A,j}=\frac{\alpha^j j!}{L^j}
       \left(1+O\!\left(\frac{j^2}{L}\right)\right),
\qquad j=k,k+1.
\tag{APC5}
$$

In particular the two errors are positive eventually, and their
actual ratio satisfies

$$
r_A=\frac{E_{A,k+1}}{E_{A,k}}
 =\frac{\alpha(k+1)}L
       \left(1+O\!\left(\frac{k^2}{L}\right)\right)\longrightarrow0.
\tag{APC6}
$$

Thus $0<r_A<1/2$ eventually. No numerical common starting point or
numerical error constant is supplied; no fixed-order expansion has
been applied to a changing order.

### Exact calibration and the source properties it preserves

Apply the standard adjacent-error extrapolation to the actual errors:

$$
\sigma_A=\frac{\nu_{k+1}-r_A\nu_k}{1-r_A},
\qquad
\bar\sigma_A=(\chi_A)_\#\sigma_A.
\tag{APC7}
$$

The first is the full source measure; the second is the actual
clamped clock measure. By definition of $r_A$,

$$
\int y_A\,d\sigma_A
 =\frac{Y_{A,k+1}-r_AY_{A,k}}{1-r_A}=1.
$$

For $\sigma_A$, mass, first clock moment and inverse clock moment
are all one. Its Mellin transform vanishes at every actual xi zero.
At $s=0,1$, all derivatives of $H_{\sigma_A}-1$ through order $k-1$
vanish, since both adjacent transforms have these properties.
For each fixed real $t$,

$$
N_t(A):=\int c^t\,d|\sigma_A|(c)
 \le\frac{M_t(k+1)+r_AM_t(k)}{1-r_A}
 =\exp(O(k))=A^{o(1)}.
\tag{APC8}
$$

These exact Mellin, jet and clock-moment properties refer to
$\sigma_A$ before the cutoff. They are not asserted for
$\bar\sigma_A$. The latter has mass one and exact nonlinear price
mean $\int\lambda(Ac)\,d\bar\sigma_A(c)=\lambda(A)$.
Neither measure is asserted positive or ordered by Jensen's inequality.

### Pay the complete original response after the cutoff

Since $k,k+1\to\infty$ and eventually $k+1\le\kappa L$,
GPC5 and its limit along growing orders give

$$
T_A|J_{\sigma_A}^\psi(A)|
 +T_A|\mathcal T_{\ge2}(A,\sigma_A)|\longrightarrow0.
$$

This uses linearity on mass-one signed measures and bounded mixing
coefficients. In particular
$H_j(1/2)-1=-Q(h(1/2))^j\to0$; no uniform absolute limit for all
fixed orders is assumed.

It remains to pay the actual cutoff, which need not preserve exact
Mellin zeros. Since $\tau=e/A<A^{-1/2}$ eventually, GPC's absolute
small-clock argument gives

$$
T_A\int_{c<\tau}|J_c^\psi(A)|\,d|\sigma_A|(c)
 =O(N_{-4}(A)L A^{-3/2}).
$$

Also $J_\tau^\psi(A)=O(L)$. On $A\le u\le A^2$, the trivial
$\psi(t)\le t\log_+t$ bounds its integrand before $K$ by $u(L+2)$,
and $\int_A^{A^2}uK(u)\,du=O(1)$. On $u\ge A^2$,
$\tau u\ge\sqrt u$, so the existing logarithmic PNT gives an
integrable $O(u/\log^2u)$ bound. Finally
$|\sigma_A|(\{c<\tau\})\le\tau^4N_{-4}(A)$. Hence

$$
T_A|J_{\bar\sigma_A}^\psi-J_{\sigma_A}^\psi|
 \le C N_{-4}(A)
       [L A^{-3/2}+L^2 A^{-7/2}]\longrightarrow0.
$$

GPP2 and its bounded initial interval give
$P_{\ge2}(t)\le C\sqrt t$ for all $t>0$. Both laws have mass one,
so the reference $P_{\ge2}(u)$ cancels in their transport difference.
The complete small-clock and cutoff terms consequently cost

$$
\begin{aligned}
T_A|\mathcal T_{\ge2}(A,\bar\sigma_A)
       -\mathcal T_{\ge2}(A,\sigma_A)|
&\le CB(A)\left[
 \int_{c<\tau}c^{-1/2}\,d|\sigma_A|
 +\tau^{-1/2}|\sigma_A|(\{c<\tau\})\right]\\
&\le C N_{-4}(A)A^{-7/2}\longrightarrow0.
\end{aligned}
$$

The error estimates include every original clock value, every prime
power and the entire $u\ge A$ tail. They also prove absolute integrability
of the modified responses. Thus the actual price-calibrated clock
law has the full component budget

$$
T_A|J_{\bar\sigma_A}^\psi(A)|
 +T_A|\mathcal T_{\ge2}(A,\bar\sigma_A)|\longrightarrow0.
\tag{APC9}
$$

No one-sided positive-law constant has been transferred to a signed law.

### Original pressure and the same integer

For each original integer's $A=\log n$, put
$\lambda_A=1/(AL)$ and
$\Lambda_A(c)=\lambda(A\chi_A(c))$.
The same source satisfies $\int\Lambda_A\,d\sigma_A=\lambda_A$
exactly. The actual unrestricted pressure is integrable:
its existing asymptotic
$M(\lambda(x))=\gamma+\log\log x-1/\log x+O(1/\log^2x)$,
together with the cutoff $x\ge e$, bounds it by $C_A(1+c)$ on this
source; APC8 supplies the required absolute moment.

Keep $d_\lambda(n)=M(\lambda)-W(n)+\lambda\log n$ and define
$G_A=\int M(\Lambda_A(c))\,d\sigma_A-M(\lambda_A)$.
Exact calibration gives the same-integer identity

$$
\int d_{\Lambda_A(c)}(n)\,d\sigma_A(c)=d_A(n)+G_A.
\tag{APC10}
$$

The nonnegativity of each individual defect does not supply a sign
for this signed integral or for $G_A$.

Define $\mathcal T_\vartheta$ using $\bar\sigma_A$ and the centered
response of GPC9. APC9 pays its integrability and leaves the original
exact account intact:

$$
\Delta(n)=R(A)+d_A(n)-J_{\bar\sigma_A}^\psi
 -\mathcal T_\vartheta(A,\bar\sigma_A)
 -\mathcal T_{\ge2}(A,\bar\sigma_A).
$$

The unchanged GAK37 reserve therefore gives, eventually, one
$\epsilon(A)\to0$ such that

$$
T_A\Delta(n)>
 Q_R+\frac{L}{(L+2)^3}+T_A d_A(n)
 -T_A\mathcal T_\vartheta(A,\bar\sigma_A)-\epsilon(A).
\tag{APC11}
$$

This instantiates the original account with an explicitly calibrated
price family, unbounded source moment-cancellation order and paid
cutoff error. The remaining comparison between first-prime transport
and this same integer's defect is unproved. Generic fixed-family
Jensen obstructions are not removed by the construction; no pressure
sign, new finite verification interval or RH/Robin proof follows.

## Actual pressure order of the calibrated growing family

Retain exactly the source, cutoff, degree and calibration of APC1–APC11.
The following repo-derived application estimates their actual unrestricted
pressure correction $G_A$. It reuses the BPY law, the complete pressure
identity, the published PNT input and standard Laplace/Gamma asymptotics.
The earlier fixed-family signed Jensen tests do not supply this
moving-degree relative estimate. No literature priority, numerical common
starting threshold, Lean certification or RH/Robin proof is claimed.

### The complete actual-pressure remainder

Put

$$
B(x)=\gamma+\log\log x-\frac1{\log x}\qquad(x\ge e).
$$

GAK29 and GAK38 already give
$M(\lambda(x))=B(x)-I_\psi(x)-R(x)$, with the unrestricted pressure
and every prime power retained. Reuse
[Johnston–Yang, arXiv:2204.01980v2](https://arxiv.org/pdf/2204.01980v2),
Theorem 1.1, equation (1.3), as recorded in the
[existing supplier note](../Weil/johnstonyang2022pnt.md):

$$
|\psi(u)-u|\le9.39u(\log u)^{1.515}
 e^{-0.8274\sqrt{\log u}}\qquad(u\ge2).
$$

After $v=\log u$, its contribution to $|I_\psi(x)|$ is bounded by a
constant times
$\int_{\log x}^\infty(1+v)v^{-0.485}e^{-0.8274\sqrt v}\,dv$.
Absorbing the polynomial into a smaller exponential, and using the
existing whole-reserve upper $R(x)=O(x^{-1/2})$, gives fixed $C,b>0$ with

$$
|M(\lambda(x))-B(x)|\le C e^{-b\sqrt{\log x}}
\qquad(x\ \text{sufficiently large}).
\tag{ACP1}
$$

This is an application of the published theorem, without rerunning its
computations or independently certifying its whole proof. The difference
on the left is continuous, bounded on compact subsets of $[e,\infty)$,
and tends to zero, so it is globally bounded there.

For $j=k,k+1$, split the whole source at $c=A^{-1/2}$. Above this cut,
$A\chi_A(c)\ge\sqrt A$; below it use the global bound and
$|\nu_j|(c<A^{-1/2})\le A^{-2}M_{-4}(j)$. GPC2 consequently gives

$$
\int|M(\lambda(A\chi_A(c)))-B(A\chi_A(c))|\,d|\nu_j|(c)
\le e^{-b_1\sqrt L+O(j)}+e^{-2L+O(j)}
\tag{ACP2}
$$

for a fixed $b_1>0$. Arbitrarily small and clamped clocks are included.
The same allowance applies to the value at $x=A$ and to the bounded
adjacent mixture.

### The other interpolation node and the finite Laplace calculation

Since $\mu$ is a probability law with $\int c\,d\mu=1$, the strict
inequality $\log c<c-1$ away from $c=1$ gives $h'(1)<0$.
The law is nontrivial because $h(0)=m>1$. Define

$$
\beta_1=-\frac{m-1}{m}h'(1)>0,\qquad
v(u)=Q(h(1-u))=-\beta_1u\exp(O(u)).
\tag{ACP3}
$$

Here $Q'(1)=-(m-1)/m$; $\beta_1$ belongs to node $1$, whereas
APC2's positive $\alpha$ belongs to node $0$. All real moments justify
the derivatives. Choose fixed $u_0\in(0,1)$ and $D<\infty$ so that
$v(u)<0$ and $|\log[-v(u)/(\beta_1u)]|\le Du$ for $0<u\le u_0$.

For one clamped clock put $z=\log(A\chi_A(c))\ge1$. The standard
logarithm and reciprocal-logarithm formula is

$$
B(A\chi_A(c))-B(A)
=\int_0^\infty(e^{-Lu}-e^{-zu})(1/u+1)\,du.
$$

Only $[0,u_0]$ is interchanged with the signed source. The absolute
remaining tail is at most $C(e^{-u_0L}+e^{-u_0z})$, whose source
integral is at most $CA^{-u_0}[M_0(j)+M_{-u_0}(j)]$.
Near zero, absolute Fubini uses the cancelling difference and

$$
\frac{|1-\chi_A(c)^{-u}|}{u}
\le|\log\chi_A(c)|[1+\chi_A(c)^{-u_0}].
$$

Its absolute integral is finite by neighboring fixed real moments;
clamping a clock below $e/A<1$ decreases its absolute logarithm.
No two divergent $1/u$ integrals are separated.

Write $\tau=e/A$. For $c<\tau$ and $0<u\le u_0$,

$$
\frac{|\tau^{-u}-c^{-u}|}{u}
\le\log(\tau/c)c^{-u_0}
\le C\tau^{4-u_0}c^{-4}.
$$

The last bound follows from
$\sup_{0<t<1}t^{4-u_0}\log(1/t)<\infty$. It pays the complete
replacement of the truncated clamped Mellin factor by $H_j(1-u)$.
Thus, for some fixed $c_0>0$,

$$
S_{A,j}:=\int[B(A\chi_A(c))-B(A)]\,d\nu_j(c)
=\int_0^{u_0}e^{-Lu}v(u)^j(1/u+1)\,du
 +O(e^{-c_0L+O(j)}).
\tag{ACP4}
$$

### Moving degree, actual pressure and exact calibration

The integral in ACP4 has sign $(-1)^j$. Its magnitude lies between

$$
\beta_1^j\int_0^{u_0}e^{-(L+Dj)u}(u^{j-1}+u^j)\,du
$$

and the same expression with $L-Dj$. The full Gamma integrals have
leading value $\beta_1^j(j-1)!/L^j$. The $u^j$ term and the removed
Gamma tails cost $O(j/L)$ relatively; changing $L$ to $L\pm Dj$
costs $O(j^2/L)$. Since $j=k,k+1$ and $k=\lfloor L^{1/3}\rfloor$,

$$
S_{A,j}=\frac{(-\beta_1)^j(j-1)!}{L^j}
 \left(1+O\!\left(\frac{j^2}{L}\right)\right).
\tag{ACP5}
$$

The logarithm of this main magnitude is $-O(j\log L)$, and
$j\log L=o(\sqrt L)$. Therefore the whole actual-pressure allowance
ACP2 and the cutoff remainder ACP4 are negligible relatively, including
the $\exp(O(j))$ variation cost. The actual individual gap satisfies

$$
F_{A,j}:=\int M(\lambda(A\chi_A(c)))\,d\nu_j(c)-M(\lambda(A))
=\frac{(-\beta_1)^j(j-1)!}{L^j}
 \left(1+O\!\left(\frac{j^2}{L}\right)\right).
\tag{ACP6}
$$

This transfers a moving-order calculation to the actual unrestricted
pressure; it is neither a fixed-order substitution nor a smooth-only
sign claim.

Use the unchanged actual ratio $r_A$ from APC6. In
$G_A=(F_{A,k+1}-r_AF_{A,k})/(1-r_A)$, the two numerator main terms
have the same sign, so their coefficients add. Equations APC6 and ACP6 give

$$
G_A=(-1)^{k+1}
 \frac{\beta_1^k(k-1)![\beta_1k+\alpha(k+1)]}{L^{k+1}}
 \left(1+O\!\left(\frac{k^2}{L}\right)\right).
\tag{ACP7}
$$

The denominator $1-r_A=1+O(k/L)$ is absorbed in this relative error.
Consequently $G_A>0$ for odd $k$ and $G_A<0$ for even $k$, eventually
in both parity sectors. Stirling at this actual degree gives

$$
\log|G_A|=-\left(\frac23+o(1)\right)L^{1/3}\log L,
\qquad G_A\to0,
\qquad \sqrt A\log A\,|G_A|\to\infty.
\tag{ACP8}
$$

These are the actual gap's sign and magnitude, rather than growth
inferred from an upper allowance.

### What the comparison supplies at the original integer

Put $V_A=\int M(\lambda(A\chi_A(c)))\,d\sigma_A(c)$.
The same mixture of ACP5 and ACP2 proves

$$
V_A-B(A)=G_A(1+o(1)),\qquad R(A)=o(|G_A|).
\tag{ACP9}
$$

The second assertion uses the valid whole-reserve upper
$R(A)=O(A^{-1/2})$. It does not treat a reserve lower constant as an
upper budget. For odd $k$ the actual pressure upper
$M(\lambda(A))<V_A$ holds eventually, but $V_A>B(A)$ with a shift
larger than the root scale. For even $k$, $V_A<B(A)$ but
$M(\lambda(A))>V_A$. Thus this single comparison does not give the
proposed sufficient pressure upper $M(\lambda(A))<B(A)$ on either
sector. It determines neither the sign of $M(\lambda(A))-B(A)$ nor
the outcome of a compensated argument.

For every original integer $n$ with its own $A=\log n$, the exact target is

$$
\Delta(n)=B(A)-M(\lambda(A))+d_A(n)>0
\quad\Longleftrightarrow\quad
 d_A(n)>M(\lambda(A))-B(A).
\tag{ACP10}
$$

The stronger pressure upper is sufficient, not necessary. Retain APC10's
same-integer identity unchanged:
$\int d_{\lambda(A\chi_A(c))}(n)\,d\sigma_A(c)=d_A(n)+G_A$.
ACP7 now estimates its previously unspecified correction. Pointwise
nonnegative defects do not imply a nonnegative signed average, and no
other optimizer replaces $n$. No existence of an own-price zero-defect
integer in a specified parity sector is asserted.

APC9–APC11 still pay the complete smoothed and proper-power responses.
The comparison of first-prime transport with this same integer's defect
remains unproved. Exact price calibration and a favorable pressure
comparison do not by themselves remove the larger averaged benchmark
shift; no RH or all-integer Robin conclusion follows.
