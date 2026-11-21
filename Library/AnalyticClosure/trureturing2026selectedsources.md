---
bibkey: trureturing2026selectedsources
authors: trureturing research
year: 2026
title: Selected source bounds
doi: null
url: https://github.com/the-omega-institute/trureturing/blob/727e10f660466a6dc69ea491c8f334969b9c9d87/Library/ArithSums/nicolas2025comparison.md#project-application-full-signed-shorter-q-drift-and-preloaded-ga2-successors
claim: Project calculations on the extremal envelopes studied in the Nicolas comparison note, under the hypotheses given in each section.
strata_touched: []
license: citation-only
triage: anchor
---

# Selected source bounds

These sections continue the project’s calculations on Nicolas’s comparison of the two extremal envelopes. [Source and section index](../ArithSums/nicolas2025comparison.md)

## Project application: full signed shorter Q drift and preloaded GA2 successors

This is a complete **ordinary mathematical derivation relative to the
published Guth–Maynard short-interval input**. Its additional analytic
content is the integrated full signed difference of actual and reference
layers at the fixed length \(H=A^{4/5}\), including a bound uniform in
the growing layer index. It then applies the already audited finite lcm
accounting to the same actual GA2 integer. No selfmatching hypothesis is
needed for that application.

The preceding MS0–MS9/MSP section is reused at the immutable project
commit `963847e45dc06ddb633295b84b2bd36d4c231eae`, NC file blob
`14f2f364318cf8f02e8b58d50ab9f61802f4764e`. In particular, MS3–MS6
supply the smooth actual second-cutoff calculation and its whole weighted
increment; MS0–MS2 and MS9 retain the actual integer, endpoint convention
and signed first-layer accounting. The original
[FIB §§85, 87, 98 and 111](../../docs/develop/theory/FIBONACCI_ATOMIC_RELATION_GENERATION.md),
[ZE/5040 actual layers and own-price defect](../../docs/develop/theory/ZECKENDORF_EULER_5040.md),
and [Mantovanelli workload and proper prime-local bridge](../Analytic/mantovanelli2026primeworkload.md)
remain the underlying project interfaces.

The declared completed design inputs are
`actual-higher-layer-gm-shorter-Q-candidate.md`, SHA-256
`5a967ecdb296bf5c7c64413cf9c00ddc0f7ed3868c69a7ef8375386eef39ac6f`,
and its complete ordinary proof `audit-proof.md`, SHA-256
`9f18c0fe96eafb4fe61aa2da8b6370055912c961833fe5248ce4c191aec416a3`;
and `ga2-preloaded-layer-successor-candidate.md`, SHA-256
`f99946147a279237a5515659ce73334a3ccdadd7dab1be0297d8a2806314cdc5`,
with `ordinary-audit.md`, SHA-256
`307be4ca1430efc5843323b2189fcff07ad2f3ee669db59ed1f3faa0c81c4a41`.
Their preserved results and collection receipts report ordinary approval
within those stated scopes. Those prior audits are design evidence here,
not independent current validation of this source draft. No complete
independent audit of the primary GM theorem, new compilation, Lean/kernel
verification, official acceptance or priority claim is made.

### Actual and reference inventories on one common finite support

All logarithms are natural. For real \(x>1\), set

\[
f(x)=\log\log x,\qquad
\lambda(x)=f'(x)=\frac1{x\log x},\qquad
w(x)=-\lambda'(x)=\frac{\log x+1}{x^2(\log x)^2}>0.
\]

For \(q>1\) and an integer \(k\ge1\), put

\[
S_k(q)=\sum_{j=1}^k q^j,\qquad
\ell_k(q)=\log(1+1/S_k(q)),\qquad
r_k(q)=\frac{\ell_k(q)}{\log q}.
\]

For a prime \(p\), write \(r_{p,k}=r_k(p)\) and
\(h_p=\log p\). The existing Euler stack identity is

\[
\frac{\sum_{j=0}^k p^{-j}}{\sum_{j=0}^{k-1}p^{-j}}
=1+\frac1{p+\cdots+p^k},\qquad
W(n):=\log\frac{\sigma(n)}n
=\sum_p\sum_{k=1}^{v_p(n)}r_{p,k}h_p.
\]

Each \(r_k\) is smooth and strictly decreasing from infinity to zero:
\(\ell_k>0\) decreases strictly, \(\log q>0\) increases strictly,
and their endpoint limits give the stated range. Thus there is a unique
smooth increasing \(q_k(x)>1\) with
\(r_k(q_k(x))=\lambda(x)\). Define the **strict actual** inventory by

\[
K_k(x)=\sum_{p<q_k(x)}\log p
=\sum_{r_{p,k}>\lambda(x)}\log p,\qquad
N_x=\prod_p p^{\#\{k:r_{p,k}>\lambda(x)\}},\qquad
K(x)=\sum_{k\ge1}K_k(x)=\log N_x.
\]

The reference convention is weak:

\[
\theta(y)=\sum_{p\le y}\log p,\qquad
\psi(x)=\sum_{p^k\le x}\log p
=\sum_{k\ge1}\theta(x^{1/k}),\qquad Q(x)=K(x)-\psi(x).
\]

This \(Q\) is specifically the actual-minus-reference log inventory;
it is not any other quantity called \(Q\) earlier in this source.
All prime-power pairs are counted, with their individual \(\log p\)
weights.

The exact marginal bound

\[
0<r_{p,k}<\frac1{p^k\log p}
\]

shows that every possibly active or tied actual layer on \([A,B]\)
lies in the finite set
\(L_B=\{(p,k):r_{p,k}\ge\lambda(B)\}\), since membership implies
\(p^k\log p<B\log B\) and \(p<B\). The reference support
\(\{(p,k):p^k\le B\}\) is also finite. These two fixed sets give
common support for every \(x\in[A,B]\), so all subsequent sum/integral
interchanges are finite. Equal-price actual layers are excluded from
\(N_x\). Different primes may activate simultaneously; every layer of
such an event is retained separately in the accounting.

### Exact derivative control uniform in the growing layer index

The audited candidate's H1–H5 are written QH1–QH5 here to avoid the
earlier H1–H7 labels in this file. These inequalities hold uniformly
for **every** integer \(k\ge1\), rather than for each fixed \(k\)
with unspecified dependent constants.

Writing \(z=1/S_k(q)\), exact differentiation gives

\[
\ell_k'(q)=-\frac{S_k'(q)}{S_k(q)(S_k(q)+1)},\qquad
-\frac{q\ell_k'(q)}{\ell_k(q)}
=\frac{qS_k'(q)}{S_k(q)}
\frac{z}{(1+z)\log(1+z)}. \tag{QH1}
\]

Let \(m=(k+1)/2\). Pair the terms \(j<m\) and \(k+1-j>m\)
in \(\sum_{j=1}^k(j-m)q^j\). Each pair contributes

\[
(m-j)(q^{k+1-j}-q^j)\ge0;
\]

the middle term, when present, is zero. Thus
\(qS_k'(q)/S_k(q)\ge(k+1)/2\). Also \(S_k(q)\ge k\),
so \(z\le1/k\), and \(\log(1+z)\le z\) gives

\[
\frac{z}{(1+z)\log(1+z)}\ge\frac1{1+z}\ge\frac{k}{k+1}.
\]

Consequently

\[
-\frac{qr_k'(q)}{r_k(q)}
=-\frac{q\ell_k'(q)}{\ell_k(q)}+\frac1{\log q}
\ge\frac k2. \tag{QH2}
\]

Implicit logarithmic differentiation uses
\(-\lambda'(x)/\lambda(x)=(1+1/\log x)/x\), and proves

\[
0<\frac{q_k'(x)}{q_k(x)}
\le\frac{2(1+1/\log x)}{kx}\le\frac4{kx}
\qquad(x\ge e). \tag{QH3}
\]

For \(A\ge e\), \(0\le u\le H\), \(H/A\le1/4\), integrate:

\[
0\le\log\frac{q_k(A+u)}{q_k(A)}
\le\frac4k\log(1+u/A)\le\frac{4u}{kA}\le1.
\]

Using \(e^t-1\le2t\) on \([0,1]\) therefore gives

\[
0\le q_k(A+u)-q_k(A)\le\frac{8u\,q_k(A)}{kA}. \tag{QH4}
\]

At the cutoff, \(\log(1+1/S_k)<1/S_k\le q^{-k}\), hence
\(q_k(A)^k\log q_k(A)<A\log A\). In particular, **provided
\(q_k(A)\ge2\)**,

\[
q_k(A)<R_A^{1/k},\qquad R_A=\frac{A\log A}{\log2}. \tag{QH5}
\]

No large-\(q\) expansion uniform in growing \(k\) has been assumed.
A nonempty actual layer at \(B\), or even a tie at \(B\), requires
\(2^k<R_B\); a nonempty reference layer requires \(2^k\le B\).
For sufficiently large \(A\) and \(B\le2A\), both families lie in

\[
1\le k\le D_A:=\left\lceil\frac{\log R_B}{\log2}\right\rceil
\le7\log A.
\]

This is one common \(O(\log A)\) index support, including layers
empty at \(A\) but active before \(B\). The actual layer with
\(q_k(B)=2\) is empty under the strict convention and causes no
omission. The same bounds cover all equality events in \(L_B\).

### One GM threshold, length enclosure and the logarithmic weight

Use the primary **uniform Corollary 1.3** of
[Guth–Maynard, arXiv:2405.20552v2](https://arxiv.org/html/2405.20552v2),
as recorded in the [project GM source](../Analytic/guthmaynard2024largevalues.md).
Its entire primary theorem proof is not independently audited here.
Fix, once and for all,

\[
\epsilon_{\rm GM}=1/60,\qquad
\beta=17/30+\epsilon_{\rm GM}=7/12.
\]

The published input gives constants \(C_{\rm GM},Y_0>0\) such that
for **every real** \(y\ge Y_0\) and every real length
\(y^\beta\le v\le y^{99/100}\),

\[
\left|\pi(y+v)-\pi(y)-\frac v{\log y}\right|
\le C_{\rm GM}v e^{-(\log y)^{1/4}}. \tag{QGM}
\]

Increase this single unknown start to \(Y\ge e\), so that
\(C_{\rm GM}\log y\,e^{-(\log y)^{1/4}}\le1\) for every
\(y\ge Y\). Neither \(Y_0\) nor \(Y\) is assigned a numerical
value. For a permitted length, let \(P=\pi(y+v)-\pi(y)\). Then
\(P\le2v/\log y\), and

\[
0\le\theta(y+v)-\theta(y)-(\log y)P
\le\log(1+v/y)P\le\frac{2v^2}{y\log y}.
\]

Thus the required two-sided conversion is

\[
\theta(y+v)-\theta(y)
=v+O\left(v\log y\,e^{-(\log y)^{1/4}}
+\frac{v^2}{y\log y}\right). \tag{QTC}
\]

The factor \(\log y\) multiplying the absolute \(\pi\) error
is retained. Since \(v\le y^{99/100}\le y\), the same argument
also gives \(\theta(y+v)-\theta(y)\le4v\). If
\(0\le v<y^\beta\), use monotonicity and apply GM only to the
enclosing length \(y^\beta\), which lies inside its allowed range.
Consequently, with this same \(Y\),

\[
0\le\theta(y+v)-\theta(y)\le4(v+y^\beta)
\quad(y\ge Y,\ 0\le v\le y^{99/100}). \tag{QH6}
\]

This enclosure does not extend GM below its minimum length. Small
cutoffs \(y<Y\) will instead use the fixed finite bound
\(\theta(2Y)\); they do not acquire a layer-dependent GM start.

### All higher actual and reference increments, including endpoint atoms

From now on fix exactly

\[
H=A^{4/5},\qquad B=A+H,\qquad
\rho_A(u)=\frac{w(A+u)}{w(A)},\qquad
S_A=\frac{H^2}{\sqrt A}=A^{11/10}.
\]

For \(k\ge3\), \(y=q_k(A)\ge Y\), and
\(v=q_k(A+u)-q_k(A)\), QH4–QH5 give, uniformly in \(k,u\),

\[
v\le\frac{8Hy}{kA},\qquad
\frac v{y^{99/100}}
\le\frac83 A^{-1/5}R_A^{1/300}\longrightarrow0. \tag{QH7}
\]

The last power is \(A^{-59/300}\) times a fixed logarithmic
factor. Thus one common eventual \(A\)-threshold verifies the GM
**maximum** length for every such growing-index cutoff at once.

Let \(a(z)=\log z\) if \(z\) itself is an integer prime, and zero
otherwise. The exact strict-to-weak conversion, valid also at events, is

\[
K_k(A+u)-K_k(A)
=\theta(y+v)-\theta(y)+a(y)-a(y+v).
\]

The initial strict atom has a plus sign; the final one has a minus sign.
At \(u=0\) they cancel. Because \(\log y=O(y^\beta)\), QH6
and monotonicity of the actual cutoff give

\[
0\le K_k(A+u)-K_k(A)\le C(v+y^\beta).
\]

If \(q_k(A)<Y\), QH4 instead gives \(q_k(B)\le2Y\) once
\(A\) exceeds one common threshold. Its increment is then at most
\(\theta(2Y)\), even when \(q_k(A)<2\) and the initial layer is
empty. Simultaneous activations do not change these per-layer bounds.

For the reference cutoff \(y=A^{1/k}\), exact differentiation gives
\(y'(x)/y(x)=1/(kx)\). It satisfies QH4 with a smaller constant
and \(y\le R_A^{1/k}\). Apply exactly the same large-/small-cutoff
split, the same upper-length check and the same GM \(Y\). Its weak
increment already excludes the initial prime and includes the terminal
prime, and needs no strict-atom correction.

For a large higher cutoff, \(v\le C(H/A)R_A^{1/3}\) and
\(y^\beta\le R_A^{\beta/3}\). Sum both nonnegative inventories
over their common support \(3\le k\le D_A\), absorbing
\(\theta(2Y)\) into one constant. For every sufficiently large real
\(A\), simultaneously for every \(0\le u\le H\),

\[
\begin{aligned}
&\sum_{k\ge3}[K_k(A+u)-K_k(A)]\\
&\quad+\sum_{k\ge3}
 [\theta((A+u)^{1/k})-\theta(A^{1/k})]\\
&\le C\log A\left[\frac HA R_A^{1/3}+R_A^{\beta/3}+1\right].
\end{aligned} \tag{QH8}
\]

Both sums on the left are literally nonnegative. Their signed difference
is therefore bounded in absolute value by this same right side.

The exact derivative

\[
w'(x)=-x^{-3}\left(\frac2{\log x}
+\frac3{(\log x)^2}+\frac2{(\log x)^3}\right)<0
\]

gives \(0<\rho_A(u)\le1\). Integrating on the **entire** interval
with common finite support proves

\[
\begin{aligned}
&\left|\int_0^H\rho_A(u)\sum_{k\ge3}
 \bigl[K_k(A+u)-K_k(A)
 -\theta((A+u)^{1/k})+\theta(A^{1/k})\bigr]\,du\right|\\
&\le CH\log A
 \left[\frac HA R_A^{1/3}+R_A^{\beta/3}+1\right].
\end{aligned} \tag{QH9}
\]

After division by \(S_A\), the three errors are bounded by

\[
C\left[A^{-1/6}(\log A)^{4/3}
+A^{-19/180}(\log A)^{43/36}
+A^{-3/10}\log A\right]\longrightarrow0. \tag{QH10}
\]

For example, \(1/2-4/5+\beta/3=-19/180\) and
\(1+\beta/3=43/36\). This controls short **increments**, rather
than subtracting two old pointwise
\(O(A^{1/3}(\log A)^{7/3})\) errors. Integrating the latter would
give the nonvanishing relative allowance
\(O(A^{1/30}(\log A)^{7/3})\).

### Whole second-layer integration and the reference square subtraction

Reuse MS2's actual first-cutoff enclosure \(x-1<q_1(x)<x\).
It gives

\[
0\le d_1(x):=\theta(x)-K_1(x)\le\log x,
\]

including a prime at either endpoint of \([q_1(x),x]\). The
first-layer actual-minus-reference increment is
\(d_1(A)-d_1(A+u)\), so its absolute weighted integral is at most
\(H\log B\). Its normalized cost is
\(O(A^{-3/10}\log A)\), with no assumed favorable sign.

For the fixed actual second layer, MS3–MS4 derive from the **smooth
implicit equation**, not from differentiating an asymptotic remainder,

\[
q_2(x)=\sqrt{2x}\,[1+O(1/\log x)],\qquad
q_2'(x)=\frac1{\sqrt{2x}}[1+O(1/\log x)],
\]

\[
v_2(u):=q_2(A+u)-q_2(A)
=\frac{u}{\sqrt{2A}}
+O\left(\frac{u}{\sqrt A\log A}+\frac{uH}{A^{3/2}}\right).
\]

Here the fixed-layer calculation uses exactly
\(\ell_2'(q)=-(2q+1)/[(q^2+q)(q^2+q+1)]\) and
\(q^2\log q=x\log x[1+O(1/q)]\). Comparison at
\(\sqrt x\) and \(2\sqrt x\) first traps the cutoff, and implicit
differentiation then supplies the derivative. This fixed-layer expansion
is not substituted for QH1–QH5 at growing \(k\).

The reference square has the different exact derivative and increment

\[
(\sqrt x)'=\frac1{2\sqrt x},\qquad
v_{\rm sq}(u):=\sqrt{A+u}-\sqrt A
=\frac{u}{2\sqrt A}+O\left(\frac{uH}{A^{3/2}}\right).
\]

For both starts \(y=q_2(A)\) and \(y=\sqrt A\), use the same
\(Y\) as above and the common enclosing length

\[
h_0=(2\sqrt A)^\beta=2^{7/12}A^{7/24}.
\]

Eventually \(\sqrt A\le q_2(A)\le2\sqrt A\), both starts
exceed \(Y\), and

\[
y^\beta\le h_0\le y^{99/100},\qquad
0\le v_2(u),v_{\rm sq}(u)\le CA^{3/10}
\le y^{99/100}.
\]

Also \(h_0\le v_2(H),v_{\rm sq}(H)\) eventually, since
\(3/10-7/24=1/120>0\). The maximum-length comparison has
\(3/10<99/200\). Thus the enclosing interval itself respects both
GM length restrictions, for both actual and reference starts.

For \(v\ge h_0\), use QTC; for \(v<h_0\), use monotonicity
and GM at the permitted length \(h_0\). Uniformly across the whole
range of either increment this gives

\[
\theta(y+v)-\theta(y)=v+O(\eta_Av+h_0),\qquad
\eta_A=C\left[\log A\,e^{-(c\log A)^{1/4}}+H/A\right]\to0,
\]

where a fixed \(c=1/3\) is admissible after increasing the common
\(A\)-start. The \(\log A\) factor from QTC remains. For the
actual second layer add the exact atoms \(a(y)-a(y+v)\), with
absolute cost \(O(\log A)\). The reference square uses weak
endpoints directly. Events at \(u=0,H\), and simultaneous events
of other layers, require no exceptions.

The exact logarithmic derivative

\[
\frac{w'(x)}{w(x)}
=\frac1x\left[-2-\frac2{\log x}+\frac1{\log x+1}\right]
\]

has absolute value at most \(4/x\) for \(x\ge e\); hence
\(\rho_A(u)=1+O(H/A)\) uniformly. Integrate from \(0\) to \(H\),
paying the lower-length enclosure, atoms and weight variation:

\[
\begin{aligned}
U_2&:=\int_0^H\rho_A(u)[K_2(A+u)-K_2(A)]\,du\\
&=\frac{\sqrt2}{4}S_A
+O\left(\frac{H^2}{\sqrt A\log A}+\frac{H^3}{A^{3/2}}
+\eta_AS_A+Hh_0+H\log A\right).
\end{aligned} \tag{QH11}
\]

This is MS6, with the same fixed \(4/5,1/60\) parameters. In contrast,

\[
\begin{aligned}
U_{\rm sq}&:=\int_0^H\rho_A(u)
 [\theta(\sqrt{A+u})-\theta(\sqrt A)]\,du\\
&=\frac14S_A
+O\left(\frac{H^3}{A^{3/2}}+\eta_AS_A+Hh_0\right).
\end{aligned} \tag{QH12}
\]

The factors come from \(\int_0^Hu\,du=H^2/2\): the actual
derivative \(1/\sqrt{2A}\) yields \(\sqrt2/4\), whereas the
reference derivative \(1/(2\sqrt A)\) yields \(1/4\).
The enclosing and atom costs, paid before normalization, are

\[
\frac{Hh_0}{S_A}=2^{7/12}A^{-1/120},\qquad
\frac{H\log A}{S_A}=A^{-3/10}\log A.
\]

### Precise full signed Q statement and quantified error

Define the complete signed drift

\[
S_Q(A,H)=\int_0^H[Q(A+u)-Q(A)]\rho_A(u)\,du.
\]

Its finite exact decomposition is the first-layer correction, plus
\(U_2-U_{\rm sq}\), plus the signed higher-layer integral in QH9.
Combining the preceding estimates proves

\[
S_Q(A,A^{4/5})
=\left(\frac{\sqrt2-1}{4}+o(1)\right)A^{11/10}. \tag{QH13}
\]

More precisely, there exist constants \(C>0\) and \(A_*>2\)
such that **for every real \(A\ge A_*\)**, with exactly
\(H=A^{4/5}\),

\[
\left|\frac{S_Q(A,H)}{S_A}-c_Q\right|
\le\mathcal E_Q(A):=C\mathcal F_Q(A),\qquad
c_Q=\frac{\sqrt2-1}{4}, \tag{QQE}
\]

\[
\begin{aligned}
\mathcal F_Q(A)={}&\frac1{\log A}+A^{-1/5}
+\log A\,e^{-((\log A)/3)^{1/4}}+A^{-1/120}\\
&+A^{-3/10}\log A
+A^{-1/6}(\log A)^{4/3}
+A^{-19/180}(\log A)^{43/36}.
\end{aligned}
\]

All seven terms tend to zero. Constants may depend on the fixed primary
GM input and elementary estimates, but not on \(A,u,k\), selfmatching
or GA2 status. The single \(A_*\) pays the GM \(Y\), both square
cutoffs, all growing-index upper-length checks, the small-cutoff bound,
finite support and derivative estimates simultaneously. It is unknown
and no numerical start is supplied.

Equivalently, the precise tolerance formulation is

\[
\forall\delta>0\ \exists A_\delta\ge A_*,
\ \forall A\in\mathbb R,
\quad A\ge A_\delta\Longrightarrow
\left|S_Q(A,A^{4/5})-c_QA^{11/10}\right|
\le\delta A^{11/10}. \tag{QQD}
\]

The GM epsilon stays fixed at \(1/60\); \(\delta\) is the final
normalized-error tolerance. This is an ordinary GM-relative proof for
all sufficiently large real centers, not a selected-subsequence estimate.
This appended result makes no broader-\(\alpha\) assertion. It does
not supply a numerical start, a finite Robin interval, a formal/kernel
supplier, or an RH conclusion.

### Exact connection at an arbitrary actual GA2 integer

Let \(N>e^2\) be an integer, \(A=\log N\), \(a_p=v_p(N)\),
and assume GA2 in its literal sense:

\[
G(Nm)\le G(N)\quad(m\in\mathbb N_{>0}),\qquad
G(n)=\frac{\sigma(n)/n}{\log\log n}.
\]

No deletion comparison, global maximality or equation \(K(A)=A\)
is assumed. The audited occupancy argument uses the actual next layer:

\[
r_{p,a_p+1}\log p=W(Np)-W(N)
\le f(A+\log p)-f(A)<\lambda(A)\log p.
\]

The last inequality is strict concavity of \(f\). Stack monotonicity
therefore puts **every** layer with \(r_{p,k}\ge\lambda(A)\)
in \(N\), including equality layers. Thus \(N_A\mid N\), and
the finite occupied extra inventory is

\[
E_N=\{(p,k):1\le k\le a_p,\ r_{p,k}\le\lambda(A)\},\qquad
\delta_N=A-K(A)=\log(N/N_A)=\sum_{e\in E_N}h_e\ge0.
\]

For a layer \(e=(p,k)\), write \(r_e=r_{p,k}\) and \(h_e=h_p\).

For \(x\in[A,B]\), take the literal integer and clock

\[
M_x=\operatorname{lcm}(N,N_x),\qquad Y_N(x)=\log M_x,
\qquad P_N(x)=\sum_{e\in E_N:\ r_e>\lambda(x)}h_e.
\]

The generic maximizing-multiple construction already exists in
[`GoldenFutureExtensionMaximum.lean`](../../D5/S3/Arith/GoldenFutureExtensionMaximum.lean),
especially `golden_future_extension_maximum_attained`, with the
max(base exponent, new prefix exponent) witness. The corresponding
construction also appears in
[`GoldenColossalClosure.lean`](../../D5/S3/Arith/GoldenResource/GoldenColossalClosure.lean).
We reuse it; no new generic optimizer theorem or duplicate implementation
is claimed. The relevant exact application of the audited finite layer
inventory is

\[
Y_N(x)=A+K(x)-K(A)-P_N(x),\qquad
0\le P_N(x)\le\delta_N,
\quad M_A=N,\quad Y_N(A)=A. \tag{QG1}
\]

Indeed, an activated layer already in \(E_N\) must be subtracted
from the unrestricted increment: it is not a new reward of \(M_x/N\).

The audited finite lcm identity, valid for any \(H>0\), is

\[
\log\frac{G(M_B)}{G(N)}
=\int_A^B[Y_N(t)-t]w(t)\,dt+C_B(Y_N(B)),\qquad
C_B(y)=f(B)+\lambda(B)(y-B)-f(y)\ge0. \tag{QG2}
\]

Strict concavity gives \(C_B(y)=0\) exactly when \(y=B\).

For completeness, its finite event accounting is as follows. Every
genuinely missing layer has \(r_e<\lambda(A)\), a unique
activation \(t_e>A\) with \(\lambda(t_e)=r_e\), and is added
to \(M_B/N\) precisely when \(t_e<B\). If its total mass and
Euler reward are \(L=Y_N(B)-A\) and
\(R=W(M_B)-W(N)\), finite integration gives

\[
\int_A^B[Y_N(t)-t]w(t)\,dt
=R-\lambda(B)L-[f(B)-f(A)-H\lambda(B)].
\]

Adding \(C_B(A+L)\) gives \(R+f(A)-f(A+L)\), exactly the
left side of QG2. Strict terminal ties are excluded and contribute zero
interval pressure. If a permitted subset of terminal tied layers of mass
\(J\) is deliberately added, its reward is \(\lambda(B)J\);
the integral is unchanged and the defect becomes \(C_B(Y_N(B)+J)\).
Simultaneous events keep all their separate masses. The displayed
successor is consistently the strict \(M_B\), with its **actual**
terminal clock \(Y_N(B)\), which need not equal \(B\).

Define at this same \(A\)

\[
T_\psi(A,H)=\int_0^H
 [\psi(A+u)-\psi(A)-u]\rho_A(u)\,du,\qquad
V_N(A,H)=\int_0^HP_N(A+u)\rho_A(u)\,du\ge0.
\]

Using QG1 and the exact identity \(K=\psi+Q\), the integrand is

\[
\begin{aligned}
Y_N(A+u)-(A+u)
={}&K(A+u)-K(A)-u-P_N(A+u)\\
={}&\psi(A+u)-\psi(A)-u
+Q(A+u)-Q(A)-P_N(A+u).
\end{aligned}
\]

The **complete initial \(K(A)\) cancels**. There is no selfmatch
substitution. Thus the exact desired connection is

\[
\boxed{\displaystyle
\log\frac{G(M_B)}{G(N)}
=w(A)[T_\psi(A,H)+S_Q(A,H)-V_N(A,H)]
+C_B(Y_N(B)).} \tag{QG3}
\]

Neither the preoccupied loss nor the actual terminal concavity defect
has been discarded. The identity is finite and exact independently of
GM; only the subsequent estimate for \(S_Q\) requires \(H=A^{4/5}\)
and the common sufficiently-large-real start.

### Own-price defect and below-terminal-price extra layers

Reuse the unrestricted finite pressure

\[
\mathscr S(\lambda)=\max_{n\ge1}[W(n)-\lambda\log n]
=\sum_{p,k}(r_{p,k}-\lambda)_+h_p.
\]

Because all positive own-price layers are already in \(N\), its
**own** price defect is exactly

\[
d_A(N)=\mathscr S(\lambda(A))-[W(N)-\lambda(A)A]
=\sum_{e\in E_N}(\lambda(A)-r_e)h_e\ge0. \tag{QG4}
\]

Finite integration of the preoccupied indicators gives

\[
w(A)V_N=\sum_{e\in E_N}(r_e-\lambda(B))_+h_e,
\qquad
0\le V_N\le\delta_NJ_H,\qquad
J_H=\frac{\lambda(A)-\lambda(B)}{w(A)}=\int_0^H\rho_A(u)\,du.
\tag{QG5}
\]

Here \(0<J_H<H\), and \(J_H=H[1+O(H/A)]\) when \(H=o(A)\).
An extra layer tied at \(A\) has zero initial defect but contributes
its whole price drop to \(w(A)V_N\); a tie at \(B\) contributes
zero to this latter sum.

For \(a=\lambda(A)>b=\lambda(B)\) and \(r\le a\), the exact
identity \((a-r)+(r-b)_+=(a-b)+(b-r)_+\), including equality
cases, yields

\[
\boxed{\displaystyle
d_A(N)+w(A)V_N
=(\lambda(A)-\lambda(B))\delta_N
+\sum_{e\in E_N}(\lambda(B)-r_e)_+h_e.} \tag{QG6}
\]

The residual sum is the mass-weighted price defect of occupied extras
that remain below the terminal price. It is required. Arbitrary GA2
does not imply \(\delta_N=0\), \(V_N=0\), \(d_A(N)=0\), or
vanishing of this residual. In particular the zero defect of \(N_A\)
cannot be transported to the different actual integer \(N\).

### The additional signed condition remains unproved

The exact weak-reference Lambda form of the prime-power term is

\[
w(A)T_\psi(A,H)
=\sum_{A<n\le B}\Lambda(n)[\lambda(n)-\lambda(B)]
-[f(B)-f(A)-H\lambda(B)]. \tag{QG7}
\]

This follows by finite integration of
\(\psi(t)-\psi(A)=\sum_{A<n\le t}\Lambda(n)\).
A prime-power atom at \(A\) is excluded, one at \(B\) has zero
weight, and every prime power in between has its full \(\Lambda\)
weight. QG7 is the full signed prime-power budget, not a prime-only sum.

Fix a real \(\kappa<c_Q=(\sqrt2-1)/4\). There is an unknown
common \(A_\kappa\ge A_*\) for which
\(\mathcal E_Q(A)\le(c_Q-\kappa)/2\) for all real
\(A\ge A_\kappa\). The sufficient **additional unproved**
condition, at the **same actual sources** and their same shorter interval,
is

\[
T_\psi(A,A^{4/5})-V_N(A,A^{4/5})
\ge-\kappa\frac{H^2}{\sqrt A}. \tag{QGP}
\]

If this condition held at such a source, QG3 and QQE would give

\[
\log\frac{G(M_B)}{G(N)}
\ge\frac{c_Q-\kappa}{2}\,w(A)S_A+C_B(Y_N(B))>0,
\]

for the literal integer multiple \(M_B\) of this same \(N\).
This would contradict GA2; it also forces \(M_B>N\), rather than
merely producing a scalar witness. Equivalently GA2 and the proved
supplier give only the necessary upper bound

\[
T_\psi-V_N
\le-[c_Q-\mathcal E_Q(A)]S_A-\frac{C_B(Y_N(B))}{w(A)}
\quad(A\ge A_*). \tag{QG8}
\]

This is an ordinary conditional deduction, **not** a new formal theorem
assuming its desired conclusion. QGP is not proved here, in the prior
ordinary audits, or by the imported GM estimate. At the main \(A\)
scale, GM permits an integrated relative error allowance of order
\(\eta_AH^2\); after division by \(S_A\) this is of order
\(\eta_A\sqrt A\), which is not made small by the cited
subexponential error. This diagnoses an unpaid estimate, not a failure
of the proposed actual signed condition. Actual higher-layer positivity,
almost-all centers or averaged correlations do not establish QGP or
remove \(V_N\).

### Selected global maximum, unknown start and the 5040 boundary

There is a separate zero-extra case under the original **actual proper
deletion plus insertion bridge**. The archived Mantovanelli
`thm:direct-bridge` starts with the same integer \(N>e\) satisfying

\[
N/p>e,\quad G(N)\ge G(N/p)\ (p\mid N),\qquad
G(N)\ge G(Np)\ (p\text{ prime}).
\]

It gives the strict, event-free own-price state
\(N=N_A\), \(K(A)=A\) at \(A=\log N\). Under the full
unchanged selection and properness premises in this source, it applies
to the selected least global maximizer over \(n>5040\). Consequently,
for that same properly bridged source,

\[
E_N=\varnothing,\quad\delta_N=V_N=d_A(N)=0,\quad
M_B=N_B,\quad Y_N(B)=K(B),
\]

and QG3 reduces to

\[
\log\frac{G(N_B)}{G(N_A)}
=w(A)[T_\psi+S_Q]+C_B(K(B)). \tag{QG9}
\]

Only in this separate case does QGP reduce to
\(T_\psi\ge-\kappa S_A\). The terminal defect is still retained;
neither \(K(B)=B\) nor a zero terminal own-price defect is assumed.
GA2 alone supplies insertion comparisons and **does not** supply the
proper deletion bridge or these zero-extra conclusions.

The selected hypothetical global maximizer is a **single source**.
Its existence does not ensure \(A\ge A_*\) or \(A_\kappa\).
Unbounded stable roots are not an unbounded family of global maxima.
The separately documented unbounded GA2 family does not automatically
selfmatch, satisfy QGP, or eliminate its extra inventory. An eventual
argument on that family would require QGP to cover its same members;
no such coverage is established here.

The earlier conditional \(\log N>7.2\cdot10^{46}\) concerns the
same selected least **global maximizer**, under its full previously
declared chain of suppliers. It is **not a least-counterexample bound**
and cannot pay the unknown GM or shorter-drift starts. This appended
argument neither extends that finite interval nor furnishes a numerical
replacement for the common start.

For a useful finite boundary illustration, the declared completed
ordinary 5040 audit reproduced **26 rational/integer checks**: logarithm
enclosures, strict power comparisons and exact Euler ratios. At the own
clock \(A=\log5040\), it gives

\[
N_A=2^3 3^2 5\cdot7=2520,\qquad
E_{5040}=\{(2,4)\},\qquad\delta_{5040}=\log2.
\]

One exact enclosure uses
\(z_x=(x-1)/(x+1)\),
\(L_x=2\sum_{j=0}^{23}z_x^{2j+1}/(2j+1)\) and
\(U_x=L_x+2z_x^{49}/[49(1-z_x^2)]\), for
\(x\in\{2,3,5,7\}\). The positive logarithm series gives
\(L_x<\log x<U_x\). These rational endpoints establish
\(8<A<9\), \(\log8>2\), \(\log9<20/9\), hence
\(15<A\log A<20\) and \(1/20<\lambda(A)<1/15\).
The included terminal layers and excluded next layers are certified by
the following exact integer inequalities:

| Layer | Strict power comparison | Consequence |
|---|---|---|
| \((2,3)\) | \(15^{15}>2\,14^{15}\) | \(r_{2,3}>1/15\) |
| \((3,2)\) | \(13^{15}>3\,12^{15}\) | \(r_{3,2}>1/15\) |
| \((5,1)\) | \(6^{15}>5\,5^{15}\) | \(r_{5,1}>1/15\) |
| \((7,1)\) | \(8^{15}>7\,7^{15}\) | \(r_{7,1}>1/15\) |
| \((2,4)\) | \(31^{20}<2\,30^{20}\) | \(r_{2,4}<1/20\) |
| \((3,3)\) | \(40^{20}<3\,39^{20}\) | \(r_{3,3}<1/20\) |
| \((5,2)\) | \(31^{20}<5\,30^{20}\) | \(r_{5,2}<1/20\) |
| \((7,2)\) | \(57^{20}<7\,56^{20}\) | \(r_{7,2}<1/20\) |
| \((11,1)\) | \(12^{20}<11\,11^{20}\) | \(r_{11,1}<1/20\) |

Stack monotonicity covers preceding and later layers, and strict
antitonicity of \(r_1(q)\) covers every prime \(p\ge11\).
The exact Euler values are
\(Z(2520)=26/7\), \(Z(5040)=403/105\), with ratio \(31/30\).
Therefore, without requiring a GA2 classification of 5040,

\[
d_A(5040)=\lambda(A)\log2-\log(31/30)>0,\qquad
w(A)V_{5040}=(r_{2,4}-\lambda(B))_+\log2,
\]

\[
d_A(5040)+w(A)V_{5040}
=(\lambda(A)-\lambda(B))\log2
+(\lambda(B)-r_{2,4})_+\log2.
\]

The existing
[`GoldenResource5040PriceInterval.lean`](../../D5/S3/Arith/GoldenResource5040PriceInterval.lean)
and
[`GoldenResource5040EndpointComparison.lean`](../../D5/S3/Arith/GoldenResource/GoldenResource5040EndpointComparison.lean)
already give supporting-price and single-layer comparisons. A supporting
price for 5040 is different from its own clock price. This illustration
explains why a preoccupied \((2,4)\) layer cannot be paid again in a
successor; it is boundary bookkeeping, not a new prime-sign theorem,
GA2 classification, kernel claim or use of the asymptotic GM supplier at
5040.

### Reuse and remaining mathematical work

MS0–MS9/MSP are preserved. In particular their prime-only unpaid MSP
condition is not retrospectively declared proved; QGP is the stated
full-prime-power sufficient condition with the actual preoccupied loss.
The additional ordinary analytic estimate here is QH13/QQE/QQD, obtained
by controlling the signed higher increments and subtracting the paid
reference square term. QG1–QG6 apply the completed finite accounting;
the generic future optimizer, Euler layer factorization, pressure and
proper prime-local bridge are existing mathematics.

The prior pinned-library source observations identify reusable finite
support, factorization, lcm, logarithm and integration interfaces. They
do not certify a new build or a formal GM theorem. This source flight
introduces no Lean wrapper, axiom, compilation, required-check result,
formal or official acceptance. A substantive future formal implementation
must consume the uniform actual cutoff derivative, common support,
GM input or an explicitly retained analytic premise, all endpoint atoms,
whole weighted errors and the same-source finite lcm identity.

QGP, coverage of the unknown common start at the required actual sources,
and the formal analytic implementation remain open. There is no numerical
start, broader exponent claim, new finite interval, priority assertion or
RH completion. The full RH/Robin/5040 research goal remains **ACTIVE**.

## Project application: a tighter sinc allowance reaches 8

This `repo-derived` application retains the complete signed response,
positive law, deterministic transport and unrestricted reserve of the
GAK application above. Its additional estimate is a tighter sine cutoff,
consumed with different law parameters. Under the same primary analytic
premises stated in GAK section 1, it gives a strict Robin margin for
**every** integer in the larger clock interval
\[
 \frac72 10^{46}<A=\log n\le8\cdot10^{46}.
\tag{GAK40}
\]
The original margin \(3/1000\) on the original interval through
\(7.2\cdot10^{46}\) remains valid; the margin for (GAK40) is
\(2/1000\). No primary analytic proof audit, Lean/kernel certification,
least-counterexample bound or unbounded RH estimate is asserted.

### Tighter cutoff using the existing sine tools

For all real \(v\) with \(|v|\ge51/20\),
\[
 \frac{|\sin v|}{|v|}\le\frac7{32}.
\tag{GAK41}
\]
The monotonicity of sinc on \((0,\pi)\), the alternating sine remainder,
the concavity tangent bound and \(|\sin v|\le1\) are standard tools.
Here is their parameter-specific application, without a new general
sinc theorem.

Put \(b=51/20\), \(q_0=7/32\), and
\[
 P_{13}(b)=\sum_{j=0}^{6}\frac{(-1)^jb^{2j+1}}{(2j+1)!}.
\]
The omitted sine tail starts with the negative degree-fifteen term;
successive omitted absolute terms decrease, since already
\(b^2/(16\cdot17)<1\). Thus \(\sin b\le P_{13}(b)\).
Exact rational comparison gives
\[
 q_0b-P_{13}(b)>\frac1{10000}.
\tag{GAK42}
\]
Since sinc decreases on \([b,\pi]\), this pays the first band.

On \([\pi,32/7]\), use the classical bound \(\pi>157/50\) and put
\(t=v-\pi\). Then \(0\le t<501/350\) and \(v<2\pi\), so
\(|\sin v|=\sin t\). The degree-five upper prefix
\[
 P_5(t)=t-t^3/6+t^5/120
\]
has a negative first omitted term and decreasing omitted terms on this
band, and hence \(\sin t\le P_5(t)\). It is concave on
\([0,501/350]\), because \(P_5''(t)=-t+t^3/6\le0\).
With \(t_0=34/25\), exact comparisons give
\[
 \begin{split}
 q_0-P_5'(t_0)&>\frac1{1000},\\
 q_0\frac{157}{50}
   -\bigl(P_5(t_0)-t_0P_5'(t_0)\bigr)&>\frac3{1000}.
 \end{split}
\tag{GAK43}
\]
The tangent upper bound therefore satisfies
\[
 \sin t\le P_5(t)
 \le P_5(t_0)+(t-t_0)P_5'(t_0)
 <q_0(t+157/50)<q_0v.
\]
For \(v\ge32/7\), use \(|\sin v|/v\le1/v\le7/32\).
Reflection supplies the negative axis and proves (GAK41).

### Change the law parameters and retain actual zero real parts

Use the **same whole-law construction** (GAK3)–(GAK6), now with
\[
 H=3\cdot10^{12},\qquad k=21,\qquad
 a=\frac{51}{20H},\qquad x=a^2,\qquad q=\frac{219}{1000}.
\tag{GAK44}
\]
Its mean is exactly one. The parameter-dependent bounds are
\[
 M_*=\frac1{1-2kx},\qquad
 V_*=\frac{kx}{3-(k+3)x},\qquad
 \epsilon=ka+\frac{kx}{1-x}.
\tag{GAK45}
\]
Both denominators are positive, and exact substitution gives
\[
 \epsilon<1/1000,\qquad
 \frac{99}{100}<1-\epsilon\le C
 \le(1-\epsilon)^{-1}<\frac{101}{100}.
\tag{GAK46}
\]
These are full-support bounds, with no discarded scales or conditional
mean. All moment and centered transport hypotheses in GAK therefore
remain available.

For an actual tail zero \(\rho=\beta+i\gamma\), put
\(u=\beta-1\in(-1,0)\), retaining \(|\gamma|\ge H\).
The complex normalization argument of (GAK8), using (GAK41), gives
\[
 |S(a(u+i\gamma))|
 \le\frac7{32}+\frac{20}{51}\frac{a}{1-x},
\]
and consequently
\[
 |H_C(\rho)|\le q_*^{21}<q^{21},\qquad
 q_*:=\frac{7/32+(20/51)a/(1-x)}{1-x}
       <\frac{219}{1000}.
\tag{GAK47}
\]
In particular the normalization \((1-x)^{-1}\) is not omitted.
This bounds **all actual** \(0<\beta<1\), both ordinate signs, and
all tail heights. Critical-line verification is used only on the
original finite head. The head estimate (GAK9) still uses \(M_*\).

### Pay the complete response on the enlarged interval

Retain \(L=\log A\), \(T=\sqrt A L\), the full coefficient
\(F_A\) in (GAK10), all actual multiplicities and endpoint conventions.
The parameter-dependent derivations (GAK18)–(GAK24) apply to the law
(GAK44): replace their original tail damping by \(q^{21}\), and use
the new \(M_*,V_*\). No leading-term replacement or new zero
population is introduced. The signed elementary correction remains in
the complete deterministic response and its allowance.

The lower-clock bounds \(L>107\), \(\sqrt A>10^{23}\) and
\(\eta_0(A)<10^{-6}\) in (GAK25)–(GAK26) are independent of the
upper endpoint. Put
\[
 r=\frac{2829}{1000}10^{23},\qquad
 r^2=8.003241\cdot10^{46}>8\cdot10^{46}.
\tag{GAK48}
\]
Thus \(\sqrt A<r\) throughout (GAK40), including its upper endpoint.
Define exact positive rational allowances
\[
 \begin{split}
 U_h&=\frac{108}{107}\frac{527}{500}\frac1{20}M_*,\\
 U_t&=2\frac{108}{107}\frac{10001}{10000}r
        \frac{37}{25\cdot10^{12}}\left(\frac{219}{1000}\right)^{21},\\
 U_v&=\frac{260001}{500000}rV_*,\qquad
 U_e=\frac{5M_*}{10^{23}},\qquad U=U_h+U_t+U_v+U_e.
 \end{split}
\tag{GAK49}
\]
These increase each positive cost in (GAK23)–(GAK24). They pay the
entire head, infinite tail, centered transport and elementary correction,
respectively. In particular \(A^{\beta-1/2}\le\sqrt A\) is applied
only after retaining the actual tail \(\beta\) in (GAK47).
The reused estimates therefore give \(-T I_\psi(A)<U\).

For the original reserve constant
\[
 Q_R=\frac{67838284064811}{83593750000000},
\]
exact rational substitution in (GAK49) yields
\[
 0.002407<Q_R-U<0.002408,\qquad Q_R-U>\frac2{1000}.
\tag{GAK50}
\]
For orientation only, the rounded contributions are
\(U_h\approx0.0531925234\), \(U_t\approx0.0119215981\),
\(U_v\approx0.7440015715\); the comparison (GAK50) uses the exact
fractions, including \(U_e\).

Reuse (GAK37) and **each integer's actual defect** in (GAK39), at
\(A=\log n\) and \(\lambda=1/(AL)\). It follows that
\[
 \sqrt A\log A\,\Delta(n)
 >\frac2{1000}+\frac{\log A}{(\log A+2)^3}
   +\sqrt A\log A\,d_A(n)>0.
\tag{GAK51}
\]
This proves the stated conditional Robin conclusion on (GAK40), with
no CA hypothesis and without setting \(d_A(n)=0\).

For the separate **same least global maximizer** corollary, retain every
selection, own-price CA, properness, SevenSmooth, Kalyabin,
Axler/Nicolas lower-clock and finite signed-response supplier listed in
GAK section 10. That complete extra chain places the same selected
\(A\) above \((7/2)10^{46}\); (GAK51) then excludes
\(A\le8\cdot10^{46}\). Only under that unchanged extra chain does
the same selected least global maximizer satisfy
\(\log N>8\cdot10^{46}\). This is not a bound for the least Robin
counterexample, or a transfer to an unbounded selected family.

### Reuse, certificates and the remaining unbounded gap

The positive law, full-response exchange, deterministic transport,
reserve and integer-defect identity are reused from GAK. Standard sine
tools supply the cutoff calculation; no new general theorem or global
originality claim is made. The actual gain over the original GAK
parameters is quantitative: at (GAK48), their same rational allowance
exceeds \(Q_R\), while (GAK49) pays it with margin (GAK50).

The parameter-specific
[exact rational program and results](https://github.com/the-omega-institute/trureturing-experiments/tree/0f4e4f1e8c1f1923dfbccc1903257d698d6db49f/experiments/robin-sinc-clock-8e46)
check the sine-prefix and tangent comparisons, denominator positivity,
whole support, actual-real-part normalization, square-root endpoint and
complete allowance. Their 20 comparisons use rational arithmetic;
decimal displays are not evidence. They do not certify the named
external analytic inputs or the full analytic inference in Lean.

For this fixed law \(V_*>0\) and \(q^{21}>0\). Its positive
transport and unverified-tail allowances still grow with \(\sqrt A\).
Thus (GAK51) supplies a finite interval improvement only. The original
unbounded same-source signed-tail estimate and RH remain open.

## Project application: terminal values and all-branch actual-source error budgets

This section uses the actual objective and the unrestricted pressure of
[FIB §§85, 87 and 98](../../docs/develop/theory/FIBONACCI_ATOMIC_RELATION_GENERATION.md),
the finite-tail formula in [ZE, “定理 1.1：尾积分的有限算式” and
“定理 1.2：压力余量的精确二分解”](../../docs/develop/theory/ZECKENDORF_EULER_5040.md),
and the complete shorter-successor result (QH13), (QQE), (QQD) and
(QG1)–(QG8) above. In particular, the proof of the full signed shorter
$Q$ drift is reused. The additional estimate is a uniform all-branch
quadrature and literal-competitor error budget at the last prime label of
the same actual integer. Its consumers below are an exact terminal
$\Xi$ identity and a finite comparison with a legal integer competitor.

All arithmetic values $G(n)$ and $F(n)$ below have $n\ge3$; every use
of $f(x)$, $\lambda(x)$ or $w(x)$ has $x>1$. Write
\[
Z(n)=\frac{\sigma(n)}n,\qquad W(n)=\log Z(n),\qquad
G(n)=\frac{Z(n)}{\log\log n},\qquad
F(n)=\log G(n)=W(n)-f(\log n),
\]
\[
f(x)=\log\log x,\qquad \lambda(x)=\frac1{x\log x},\qquad
w(x)=-\lambda'(x)=\frac{\log x+1}{x^2(\log x)^2}.
\tag{AVB01}
\]
Thus $f(\log n)=\log\log\log n$. Direct differentiation gives
$f''=-w<0$ and
\[
w'(x)=-x^{-3}\left(\frac2{\log x}+
 \frac3{(\log x)^2}+\frac2{(\log x)^3}\right)<0.
\]
The constant $\gamma$ throughout is the original Euler constant. The full
signed target remains
\[
\boxed{\quad
\forall n\in\mathbb N,\quad n>5040\Longrightarrow
 I_\psi(\log n)+R(\log n)+d_{\log n}(n)>0.
\quad}
\tag{AVB02}
\]
It is active and unproved. This section proves ordinary mathematical
estimates relative to the stated analytic source inputs.

### Actual attainment, strict inventories and the terminal value

For a prime $p$ and $k\ge1$, retain the Euler layer notation \[ h_p=\log p,\qquad \ell_{p,k}=\log\left(1+\frac1{p+\cdots+p^k}\right),\qquad r_{p,k}=\frac{\ell_{p,k}}{h_p},\qquad c_p=\ell_{p,1}. \] Finite Euler telescoping gives $W(n)=\sum_{(p,k)\text{ occupied}}\ell_{p,k}$. The prices decrease strictly with $k$, first prices decrease strictly with $p$, and $0<r_{p,k}<1/(p^k\log p)$. Use the strict inventory \[ N_x=\prod_p p^{\#\{k\ge1:r_{p,k}>\lambda(x)\}},\qquad K(x)=\log N_x,\qquad \psi(x)=\sum_{p^k\le x}\log p,\qquad Q(x)=K(x)-\psi(x). \tag{AVB03} \] The actual inventory is strict, whereas $\psi$ is weak and right-continuous. For each $x>1$ the inventory is finite, and $N_x$ increases by divisibility. These are the existing FIB §98.1–98.2 and (QG1) conventions, with the actual layer cutoffs of ZE Definition 7.1, equation (20), and the [existing actual-state definition](trureturing2026finiteclocks.md#same-actual-state-finite-support-and-endpoint-correction) above.

An actual GA2 integer $q\ge3$ satisfies $G(qm)\le G(q)$ for every positive
integer $m$. Let $\mathcal D_m$ be all positive multiples of $m\ge3$.
The ordinary source input used to supply actual attainment is
\[
(U)\qquad \forall X>0\ \exists q\ge3\text{ actual GA2},\quad \log q\ge X.
\tag{AVB04}
\]
Caveney–Nicolas–Sondow, *On SA, CA, and GA numbers*,
[arXiv:1112.6010v2, Theorem 5(iii)](https://arxiv.org/abs/1112.6010v2),
supplies this input under RH failure. The family used here is conditional
on that source supply.

For clarity, the reused attainment argument concerns actual $G$, rather
than the fixed-price objective. If $m\mid q$ and $q$ is actual GA2, then
for any $n\ge3$, the legal multiple $L=\operatorname{lcm}(q,n)$ satisfies
$Z(n)\le Z(L)$ and $L\le qn$. Since all log-log denominators are positive,
\[
G(n)\le G(q)\frac{\log\log(qn)}{\log\log n}
 \le G(q)\left(1+\frac{\log q}{\log n\,\log\log n}\right).
\tag{AVB05}
\]
If some member of $\mathcal D_m$ has value strictly above $G(q)$, this
vanishing tail bound puts all sufficiently late class members strictly
below that value, and a nonempty finite initial piece attains the full
class maximum. Otherwise $q$ already attains it. Input $U$ supplies a
divisible witness for each $m$: choose a price below every occupied price
of $m$ and use GA2 insertion at a sufficiently large $q$.
Indeed insertion implies
\[
r_{p,v_p(q)+1}h_p
 \le f(\log q+h_p)-f(\log q)<\lambda(\log q)h_p,
\]
so every layer with $r_{p,k}\ge\lambda(\log q)$ is occupied.

For every attaining $N\in\mathcal D_m$, including all ties, insertion
and deletion above a forced exponent give, at $A=\log N$,
\[
r_{p,v_p(N)+1}<\lambda(A),\qquad
v_p(N)>v_p(m)\Longrightarrow r_{p,v_p(N)}>\lambda(A).
\]
Deletion is legal because $m\mid N/p$ and $N/p\ge m\ge3$. Its clock
$A-h_p$ is consequently greater than $1$, and strict concavity gives the
second strict inequality. Stack monotonicity yields the characterization
\[
N=\operatorname{lcm}(m,N_A).
\tag{AVB06}
\]
Every such attaining integer is actual GA2.

For prime $p\ge29$, define $N_p$ as the least attaining natural number
on $\mathcal D_{5040p}$, and put $A_p=\log N_p$, $v(p)=F(N_p)$.
Here $N_p\ge5040p$ gives $A_p>11$. The forced 5040 core is strictly
active at every $x>11$: its terminal prices satisfy
$r_{2,4}>1/22$, $r_{3,2}>2/39$, $r_{5,1}>1/12$ and
$r_{7,1}>1/16$, while $\lambda(x)<1/22$.
These inequalities follow respectively from
$(31/30)^{22}>1+22/30+231/900+1540/27000>2$,
$\log(13/12)>1/13$, $\log3<3/2$, and
$\log5,\log7<2$. Earlier layers have larger prices. Thus (AVB06)
at $m=5040p$ becomes, for every maximizer in that class,
\[
N=\operatorname{lcm}(p,N_A),\qquad
E_N:=\{(q,k)\text{ occupied in }N:r_{q,k}\le\lambda(A)\}
 \subseteq\{(p,1)\}.
\tag{AVB07}
\]
The extra is either empty or precisely the forced first $p$-layer.
The lower bound $A_p>11$ follows, for example, from
$5040>2^{12}$, $\log2>2/3$, $p\ge29>3^3$ and $\log3>1$.

Use Gronwall in its original normalization: the limiting upper and
lower envelopes concern $G(n)/e^\gamma$. This is the
$\mathrm{robinRatio}$ normalization in
[PaddingRatio](../../D5/S3/Arith/Robin/PaddingRatio.lean);
the interfaces are
[gronwall_lower_envelope](../../D5/S3/Weil/GronwallLowerEnvelope.lean)
and [gronwall_upper_envelope](../../D5/S3/Weil/GronwallUpperEnvelope.lean).
The ordinary lower envelope at arbitrarily large $n$, combined with
(AVB05), gives $G(q)\ge e^\gamma$ for every actual GA2 $q\ge3$.
Since $N_p\ge5040p\to\infty$, the upper envelope now implies
\[
G(N_p)\longrightarrow e^\gamma,\qquad
v(p)\ge\gamma,\qquad v(p)\longrightarrow\gamma.
\tag{AVB08}
\]
The final limit uses positivity and continuity of the real logarithm.
Neither zero nor $1$ is the terminal $F$ value.

Strict excess uses the additional ordinary input
\[
(U^+)\qquad
\forall X>0\ \exists q\ge3\text{ actual GA2},\quad
 \log q\ge X,\quad G(q)>e^\gamma.
\tag{AVB09}
\]
It follows under RH failure from the positive oscillation on CA integers
and tail-maximizer construction in CNS, pp.15–16: for every integer
$T\ge5041$, choose $n_0\ge T$ with $G(n_0)>e^\gamma$.
Gronwall's upper envelope makes all sufficiently late values strictly
smaller than $G(n_0)$, so the full tail $n\ge T$ attains a maximum
strictly above $e^\gamma$ in a finite initial piece. Its maximizer is
GA2 because every positive multiple stays in that tail.
Taking $T\ge e^X$ proves $U^+$.

For fixed $p\ge29$, use $U^+$ with $\log q\ge p+1$ and
\[
r_{p,1}>\frac1{(p+1)\log p}>\lambda(p+1).
\]
GA2 insertion and the active 5040 core give $5040p\mid q$.
Actual maximality in $\mathcal D_{5040p}$ then gives $v(p)>\gamma$.
This is the only use of $U^+$ here. The error budgets below need
$v(p)-\gamma\ge0$ and the terminal limit in (AVB08), and do not use
strict excess or transport a signed estimate from this witness $q$.

### Canonical order and legal brackets on every branch

The finite Euler identity for $g=\gcd(X,Y)\ge3$ and
$l=\operatorname{lcm}(X,Y)$ is $W(g)+W(l)=W(X)+W(Y)$.
With $z=\log g>1$, $u=\log(X/g)$ and $v=\log(Y/g)$,
\[
F(g)+F(l)-F(X)-F(Y)
 =\int_0^u\int_0^v w(z+s+t)\,dt\,ds\ge0.
\tag{AVB10}
\]
Equality holds exactly when $u=0$ or $v=0$, that is, when the integers
are nested by divisibility. This is finite Euler min/max modularity and
strict concavity on the displayed positive-log rectangle.

For nested imposed classes $m\mid d$, the meet of an $m$-maximizer
and a $d$-maximizer is a legal $m$-competitor, and their join a legal
$d$-competitor. Summed maximality and (AVB10) force nesting and equality
of both value comparisons. If the $m$-maximizer is least, its meet is
itself. Hence it divides every attaining $d$-maximizer. Least attainment
is essential for this canonical conclusion.

Fix primes $29\le p<r$, set $\delta=\log(r/p)>0$,
$A=A_p$ and $C=A_r$. If $p\mid N_r$, their meet is a legal
$\mathcal D_{5040p}$ competitor and their join a legal
$\mathcal D_{5040r}$ competitor. Applying the same argument gives
$N_p\mid N_r$, $A\le C$ and $v(p)\ge v(r)$.
The fact that a meet contains 5040 alone would not justify the
$p$-class comparison.

If $p\nmid N_r$, (AVB07) and first-price antitonicity give
$N_r=rV$, $V=N_C$, with $p,r$ absent from $V$ and $5040\mid V$.
The completed integer $pV$ is legal in $\mathcal D_{5040p}$, and
\[
F(pV)-F(rV)=c_p-c_r+f(C)-f(C-\delta)>0.
\]
Thus $v(p)>v(r)$, and $r\nmid N_p$, since otherwise $N_p$ would be
a legal $r$-class competitor. Put $k=v_p(N_p)\ge1$. The two completed
replacements $rN_p/p$ and $pN_r/r$ are legal in their opposite classes;
both retain the full 5040 core, and their clocks $A+\delta,C-\delta$
exceed $1$. Their combined Euler increment is exactly
$c_p-\ell_{p,k}\ge0$, not a first-layer removal when $k>1$.
If $A+\delta>C$, these two replacement clocks are strictly more
spread with the same sum than $A,C$. Strict concavity decreases the
summed $f$ values, so the summed $F$ values strictly increase, contradicting
the two actual maximality comparisons. Consequently $C-A\ge\delta$.
Only now can one deduce $N_A\mid N_C$, $p\nmid N_A$, and $k=1$.
Thus on this nonnested branch
\[
N_p=pU,\quad N_r=rV,\quad U=N_A\mid V=N_C,\quad
p,r\nmid V,\quad D=\log(V/U)=C-A-\delta\ge0.
\tag{AVB11}
\]
The literal legal competitors $pV$ and $rU$ give
\[
c_p-c_r+f(C)-f(C-\delta)
 \le v(p)-v(r)
 \le c_p-c_r+f(A+\delta)-f(A).
\tag{AVB12}
\]
The lower bracket is used only on this branch.

The upper bracket holds on every branch. When $r\nmid N_p$, comparison
with $rN_p/p$ gives
\[
v(p)-v(r)
 \le\ell_{p,k}-c_r+f(A+\delta)-f(A)
 \le c_p-c_r+f(A+\delta)-f(A).
\tag{AVB13}
\]
When $r\mid N_p$, value order and feasibility give equality of values.
The preceding nonnested argument excludes $p\nmid N_r$, so
$N_p\mid N_r$. Least attainment in the $r$-class gives $N_r\le N_p$,
and therefore $N_r=N_p$. The zero drop obeys (AVB13).
This proves both canonical clock order and
\[
A_p\le A_r,\quad v(p)\ge v(r),\qquad
N_p=N_r\ \Longleftrightarrow\ r\mid N_p.
\tag{AVB14}
\]

A repeated-source plateau has $E_N=\varnothing$, since (AVB07)
puts that same extra set in each of two distinct singleton labels.
A distinct-clock equal-value transition is nested, but is retained.
Its arriving source also has empty extra: otherwise $N_r=rV$ with
$p\mid V$, $5040p\mid V$, and $c_r\le\lambda(C)\log r$.
The legal $p$-competitor $V$ has clock $C-\log r>1$, and strict
concavity gives
\[
F(V)-F(N_r)=f(C)-f(C-\log r)-c_r>0,
\]
contradicting $F(N_r)=v(p)$. No existence of such transitions is assumed.

On every nested edge $p\mid N_r$, the distinct labels and (AVB07)
put $p$ in $N_C$. Thus
$\lambda(C)<r_{p,1}<\lambda(p)$, whence
\[
C>p.
\tag{AVB15}
\]
In particular the active price at a nested arrival is
$\lambda(C)<\lambda(p)$. This includes plateaus and will pay their
toll without applying the nonnested lower bracket.

### Convergence before subtraction and the actual competitor deficiencies

Let $p_0=29<p_1<\cdots$ be consecutive ordinary primes.
Write $N_i=N_{p_i}$, $A_i=\log N_i$, $v_i=v(p_i)$,
$c_i=c_{p_i}$, $\delta_i=\log(p_{i+1}/p_i)$ and
$\Delta v_i=v_i-v_{i+1}\ge0$.
For a starting index $j$ set $e_j=v_j-\gamma\ge0$.
By (AVB08), $\sum_{i\ge j}\Delta v_i=e_j$.
Initially define the nonnegative extended sum
\[
L_j=\sum_{i\ge j}\delta_i\lambda(A_{i+1}).
\tag{AVB16}
\]
On nonnested edges, the lower bracket (AVB12) implies
$\delta_i\lambda(A_{i+1})\le\Delta v_i$.
On every other edge (AVB15) bounds the summand by
$\delta_i\lambda(p_i)$.

Bertrand gives $p_{i+1}<2p_i$ and $\delta_i\le\log2$.
On $u\in[\log p_i,\log p_{i+1}]$,
\[
\frac{e^{-\log p_i}/\log p_i}{e^{-u}/u}
 \le2\left(1+\frac{\log2}{\log29}\right)<3.
\]
These consecutive intervals cover the entire logarithmic prime tail.
Therefore
\[
\sum_{i\ge j}\delta_i\lambda(p_i)
 \le3\int_{\log p_j}^\infty\frac{e^{-u}}u\,du
 \le\frac3{p_j\log p_j}.
\tag{AVB17}
\]
It follows first that $L_j\le e_j+3/(p_j\log p_j)<\infty$.
Monotonicity and cofinality of $A_i$ then give
\[
0\le\sum_{i\ge j}\delta_i
 [\lambda(A_i)-\lambda(A_{i+1})]
 \le(\log2)\lambda(A_j).
\tag{AVB18}
\]
This is a full nonnegative telescope, including zero plateau increments.
In particular $\sum_{i\ge j}\delta_i\lambda(A_i)$ is finite.
Only with these convergences established do we sum (AVB13), using
$c_i\to0$ and $v_i\to\gamma$, to obtain
\[
-\frac3{p_j\log p_j}\le e_j-L_j
 \le c_j+(\log2)\lambda(A_j).
\tag{AVB19}
\]

Define the actual upper-bracket allowance and slack by
\[
b_i=f(A_i+\delta_i)-f(A_i)
 =\int_0^{\delta_i}\lambda(A_i+t)\,dt,\qquad
\tau_i=c_i-c_{i+1}+b_i-\Delta v_i\ge0.
\tag{AVB20}
\]
Here $0\le b_i\le\delta_i\lambda(A_i)$, so its sum converges.
At a finite endpoint $m$ the exact identity is
\[
\sum_{i=j}^m\tau_i
 =c_j-c_{m+1}+\sum_{i=j}^m b_i-e_j+e_{m+1}.
\]
Passing to infinity in these convergent terms gives
\[
e_j=c_j+\sum_{i\ge j}b_i-\sum_{i\ge j}\tau_i,\qquad
0\le\sum_{i\ge j}\tau_i
 \le c_j+\frac3{p_j\log p_j}+(\log2)\lambda(A_j).
\tag{AVB21}
\]
For the inequality, use $\sum b_i\le L_j+(\log2)\lambda(A_j)$ and
$L_j-e_j\le3/(p_j\log p_j)$. There is no subtraction of divergent
positive series.

Choose a literal legal successor-class competitor on every edge:
\[
X_i=
 \begin{cases}
 N_i,&p_{i+1}\mid N_i,\\
 p_{i+1}N_i/p_i,&p_{i+1}\nmid N_i,
 \end{cases}
\qquad
\eta_i=v_{i+1}-F(X_i)\ge0.
\tag{AVB22}
\]
The first case is precisely a plateau by (AVB14), with $\eta_i=0$
and $\tau_i=c_i-c_{i+1}+b_i$.
In the second case let $k_i=v_{p_i}(N_i)$.
Finite Euler subtraction, removing the actual terminal $k_i$-layer,
gives exactly
\[
\tau_i=\eta_i+c_i-\ell_{p_i,k_i}.
\tag{AVB23}
\]
Thus $0\le\eta_i\le\tau_i$ on every edge, including distinct nested
arrivals. The kth-layer correction and the plateau allowance are
retained; $\eta_i$ is a deficiency of a legal completed integer.

### Last label, uniform constants and the actual Stieltjes representation

Fix a source $N=N_p$, put $A=\log N$ and $s=P^+(N)$.
Since $s\ge p\ge29$ and $5040s\mid N$, feasibility gives
$v(s)\ge F(N)=v(p)$; value order gives equality.
Least attainment gives $N_s\le N$, while canonical clock order gives
$A_s\ge A_p$. Hence $N_s=N$.
More generally, the labels whose clocks are at most $A$ are exactly
the primes $29\le r\le s$. For $r\le p$ use clock order.
For $p<r\le s$, either this case is empty because the extra is nonempty
and $s=p$, or $N=N_A$ and the first-layer prime prefix gives $r\mid N$.
The legal meet comparison gives $N_r\mid N$, hence $A_r\le A$.
If $r>s$, clock order gives $A_r\ge A$, and equality would give
$N_r=N$, contradicting $r\mid N_r$ and $r\nmid N$.
Thus $s$ is the last label producing this integer. Plateau labels form
a consecutive finite block, whose last label is $s$; a nonempty extra
has only its own label.

The real first-layer cutoff $q_1(A)$ solves
$r_{q_1(A),1}=\lambda(A)$ as in ZE Definition 7.1.
The elementary strict bounds
$r_{A-1,1}>1/[A\log(A-1)]>\lambda(A)$ and
$r_{A,1}<\lambda(A)$ give
\[
A-1<q_1(A)<A.
\]
If the extra is nonempty, $s=p$ and $r_{p,1}\le\lambda(A)$.
The inequality $r_{p,1}>1/[(p+1)\log p]$ excludes $p\le A-1$,
so $s>A-1$.
If it is empty, $N=N_A$. Put $m=\lfloor(A-1)/2\rfloor\ge5$.
Bertrand gives a prime $m<q<2m\le A-1<q_1(A)$, so $q\mid N_A$.
In both cases,
\[
s>\frac A3;
\qquad
\text{in the empty-extra case }
s\ge q>m\ge\frac{A-3}2>\frac A3,\quad s<A.
\tag{AVB24}
\]
The comparison $(A-3)/2>A/3$ uses $A>11$, and $s<A$ uses
$\lambda(A)<r_{s,1}<\lambda(s)$.
An extra prime is not bounded above by $A$.

Relabel the same tail by choosing $j$ with $p_j=s$ and write
$e_s=e_j$, $L_s=L_j$, $u_s=e_s-L_s$.
Since $c_s<1/s<3/A$, $3/(s\log s)\le9/A$, and
$(\log2)\lambda(A)<1/A$, (AVB19)–(AVB23) imply
\[
\boxed{\quad |v(s)-\gamma-L_s|=|u_s|\le\frac9A,\qquad
 \sum_{i\ge j}\eta_i\le\sum_{i\ge j}\tau_i\le\frac{13}A.\quad}
\tag{AVB25}
\]
The upper side of (AVB19) is already less than $4/A$.
With $S_A=A^{11/10}$,
\[
\frac{1/A}{w(A)S_A}
 =A^{-1/10}\frac{(\log A)^2}{1+\log A}\longrightarrow0.
\tag{AVB26}
\]
The bound depends only on $A$, so its supremum over all actual sources
with clocks at least a real $T$ tends to zero as $T\to\infty$.
These are paid errors at the consumed scale. Neither $e_s$ nor $L_s$
is asserted individually small at that scale.

For this terminal tail, denote its cumulative logarithmic label mass by
\[
J_s(t)=\sum_{\substack{i\ge j\\A_{i+1}\le t}}\delta_i
 \quad(t\ge A).
\tag{AVB27}
\]
This local $J_s(t)$ has a real clock argument; the divisor deficit
$J_s(d)$ near the beginning of this note is a different function.
Last-label characterization proves $A_{i+1}>A$ for every $i\ge j$,
so $J_s(A)=0$. The function is right-continuous and locally finite:
$A_{i+1}\le t$ implies $p_{i+1}\le e^t/5040$, leaving only finitely
many labels on every compact interval. Simultaneous future clocks,
including repeated future plateaus, have one aggregated atom of mass
$\sum_{A_{i+1}=t}\delta_i$.

If $p_k$ is the last included successor label, telescoping gives
$J_s(t)=\log(p_k/s)$; if there are no included labels the mass is zero.
Since $5040p_k\le e^t$ and $5040s\le e^A$,
\[
0\le J_s(t)\le t-\log5040-\log s,\qquad
\lambda(t)J_s(t)\longrightarrow0.
\tag{AVB28}
\]
Finite Stieltjes integration by parts, with atoms in $(A,T]$, gives
\[
\int_{(A,T]}\lambda(t)\,dJ_s(t)
 =\lambda(T)J_s(T)+\int_A^T J_s(t)w(t)\,dt.
\]
The left side increases to the already proved convergent $L_s$ in
(AVB16)–(AVB18). Equation (AVB28) removes the boundary at infinity.
Consequently the actual representation is
\[
\boxed{\quad
L_s=\int_{(A,\infty)}\lambda(t)\,dJ_s(t)
    =\int_A^\infty J_s(t)w(t)\,dt<\infty.
\quad}
\tag{AVB29}
\]
This convergence follows from the all-branch value bound before the
integration-by-parts limit. The crude estimate $J_s(t)\le t$ would
not establish it, since $\int^\infty t\,w(t)\,dt$ diverges.

### Weighted nonnested jump width and its limitation

On a nonnested consecutive edge retain (AVB11), with
$N_i=p_iU_i$, $N_{i+1}=p_{i+1}V_i$,
$D_i=\log(V_i/U_i)$, $A=A_i$, $\delta=\delta_i$ and
$C=A_{i+1}=A+D_i+\delta$.
The two literal competitors define distinct nonnegative deficiencies
\[
\alpha_i=v_i-F(p_iV_i),\qquad
\beta_i=v_{i+1}-F(p_{i+1}U_i)=\eta_i.
\]
The equality with $\eta_i$ uses $k_i=1$ on this branch.
The exact comparisons are
\[
\begin{aligned}
\Delta v_i&=c_i-c_{i+1}+f(C)-f(C-\delta)+\alpha_i,\\
\Delta v_i&=c_i-c_{i+1}+f(A+\delta)-f(A)-\beta_i.
\end{aligned}
\]
Subtracting gives the complete bracket width
\[
\alpha_i+\beta_i
 =\int_0^\delta\int_0^{D_i}w(A+x+t)\,dt\,dx
 =\int_0^\delta[\lambda(A+x)-\lambda(A+D_i+x)]\,dx.
\tag{AVB30}
\]
Decrease of $w$ yields the lower bound $w(C)\delta D_i$.
Also $f(C)-f(C-\delta)\ge\delta\lambda(C)$ and
$f(A+\delta)-f(A)\le\delta\lambda(A)$, so the width is at most
$\delta[\lambda(A)-\lambda(C)]$. Enlarging the nonnegative subset sum
to the full telescope (AVB18) proves
\[
\sum_{\substack{i\ge j\\\text{nonnested}}}
 w(A_{i+1})\delta_iD_i
 \le\sum_{\substack{i\ge j\\\text{nonnested}}}(\alpha_i+\beta_i)
 \le(\log2)\lambda(A_j).
\tag{AVB31}
\]
This does not telescope over only the selected edges.

If $D_i=0$, the width forces $\alpha_i=\beta_i=0$.
If $D_i>0$, the legal integer $p_{i+1}U_i$ is strictly smaller than
the least attaining $N_{i+1}$, so $\beta_i>0$.
Least attainment provides no quantitative lower separation of their
real values. The distinction between $\alpha_i$, $\beta_i$ and the
all-branch $\eta_i$ matters: the $13/A$ budget controls replacement
deficiencies $\eta_i$, whereas $\alpha_i$ is controlled here by the
width, and is not that replacement deficiency.

For fixed $A,\delta$, the width in (AVB30) increases with $D$ to the
finite value $f(A+\delta)-f(A)$ as $D\to\infty$, whereas
$w(A+D+\delta)\delta D\to0$.
Thus (AVB31) weights remote jumps weakly and provides no clock mesh.
Nested branches, including distinct equal-value arrivals, remain outside
the nonnested width identity and are still included in (AVB25).

### Correct centered coupling with the original complement

Retain every prime-power reference weight and the unrestricted pressure:
\[
P(x)=\sum_{q^k\le x}\frac1{kq^k},\qquad
\mathscr S(c)=\sum_{q,k}(r_{q,k}-c)_+\log q,\qquad
R(x)=P(x)-\lambda(x)\psi(x)-\mathscr S(\lambda(x)).
\tag{AVB32}
\]
The pressure argument has $c>0$. Here $(z)_+=\max(z,0)$; a positive
part is multiplied by $\log q$.
The sums defining $P$ and the positive pressure are finite at each
admitted point. This is FIB §87.3 and §98.1, with the same pressure
as (QG4) and the original $R$ in (GAK39). The reference coefficient is
$1/(kq^k)$, whereas a $\psi$ or $\Lambda$ atom has mass $\log q$.
They have different roles.

On every compact interval $[a_0,b_0]\subset(1,\infty)$, a positive
minimum price and $r_{q,k}<1/(q^k\log q)$ give one common finite support
for all possible pressure terms and activation ties. There are also
only finitely many reference prime-power atoms.
At $x=q^k$ the jump of $P$ is exactly
$1/(kq^k)=\lambda(q^k)\log q$, so the jump of $\lambda\psi$
cancels it. Between atoms $(P-\lambda\psi)'=\psi w$.
The finite positive-part pressure is continuous at activation ties,
locally absolutely continuous, and has derivative $Kw$ almost
everywhere. Strict choices at the events do not change that derivative.
Thus $R$ is locally absolutely continuous and, for arbitrary endpoint
events and $B>A>1$,
\[
R(B)-R(A)=-\int_A^B Q(t)w(t)\,dt.
\tag{AVB33}
\]
No differentiation of an untruncated infinite pressure series is involved.

Let $H=B-A$, $a=\lambda(A)$, $b=\lambda(B)$ and
$\rho_A(u)=w(A+u)/w(A)$. Keep the original centered definitions
\[
T_\psi(A,H)=\int_0^H[\psi(A+u)-\psi(A)-u]\rho_A(u)\,du,
\quad
S_Q(A,H)=\int_0^H[Q(A+u)-Q(A)]\rho_A(u)\,du.
\]
The original effective-PNT/Mertens normalization of (GAK38) and FIB
§87.3 gives
\[
I_\psi(x)=\int_x^\infty(\psi(t)-t)w(t)\,dt
 =\gamma+f(x)-P(x)+\lambda(x)(\psi(x)-x).
\tag{AVB34}
\]
The convergent tail and its original Euler constant are retained.
Subtracting its tails over $[A,B]$ and then its initial centered value
gives the required identity with the full price-drop factor:
\[
\boxed{\quad
w(A)T_\psi(A,H)
 =I_\psi(A)-I_\psi(B)-(\psi(A)-A)(a-b).
\quad}
\tag{AVB35}
\]
Indeed the centered integrand is
$(\psi(t)-t)-(\psi(A)-A)$ and $\int_A^B w=a-b$.
Similarly (AVB33) yields
\[
w(A)S_Q(A,H)=R(A)-R(B)-Q(A)(a-b).
\tag{AVB36}
\]
These finite centered subtractions preserve the weak-reference initial
atom convention and do not assume an additional infinite-tail limit.

For the same actual source $N=N_s$ at $A=\log N$, write
\[
\delta_N=A-K(A)=\sum_{e\in E_N}h_e,\qquad
d_A(N)=\mathscr S(a)-W(N)+aA
       =\sum_{e\in E_N}(a-r_e)h_e.
\]
Use exactly the (QG1), (QG5) preoccupied inventory and loss:
\[
P_N(x)=\sum_{\substack{e\in E_N\\r_e>\lambda(x)}}h_e,\qquad
V_N(A,H)=\int_0^H P_N(A+u)\rho_A(u)\,du,
\]
\[
w(A)V_N=\sum_{e\in E_N}(r_e-b)_+h_e,\qquad
R_{\rm term}(N,B)=\sum_{e\in E_N}(b-r_e)_+h_e.
\tag{AVB37}
\]
Since every $r_e\le a$, scalar positive-part algebra gives, including
own-price and terminal ties,
\[
d_A(N)+w(A)V_N=(a-b)\delta_N+R_{\rm term}(N,B).
\tag{AVB38}
\]
This is exactly (QG6); the terminal residual is retained.

At its own clock, the unrestricted finite identity (GAK39), also
(OCQ13), gives
\[
I_\psi(A)+R(A)+d_A(N)=\gamma-F(N)=-e_s.
\tag{AVB39}
\]
It concerns this actual integer $N$, not just its subinventory $N_A$.
Adding (AVB35) and (AVB36), using
$\psi(A)-A+Q(A)=K(A)-A=-\delta_N$, and subtracting $w(A)V_N$,
then gives
\[
\begin{aligned}
w(A)(T_\psi+S_Q-V_N)
 &=I_\psi(A)+R(A)-I_\psi(B)-R(B)+(a-b)\delta_N-w(A)V_N\\
 &=-e_s-I_\psi(B)-R(B)-R_{\rm term}(N,B).
\end{aligned}
\tag{AVB40}
\]
Immediately consume (AVB25) and (AVB29), at the same last label
$s=P^+(N)$, by defining
\[
\Xi_s(B)=L_s+I_\psi(B)+R(B)+R_{\rm term}(N,B).
\]
The exact result is
\[
\boxed{\quad w(A)(T_\psi+S_Q-V_N)=-\Xi_s(B)-u_s,\qquad
 |u_s|\le9/A,\quad u_s=o(w(A)S_A)\text{ uniformly}.\quad}
\tag{AVB41}
\]
This pays the replacement of the actual terminal excess by its
actual Stieltjes integral. It does not pay $L_s$, $e_s$, the original
tail, $R(B)$ or the terminal residual separately.

For explicit singleton bookkeeping let $r=r_{s,1}$ and $h=\log s$.
The literal strict successor and clock are
$M_B=\operatorname{lcm}(N,N_B)$ and $Y=Y_N(B)=\log M_B$.
In both extra branches the exact formulas are
\[
\begin{aligned}
Y&=K(B)+\mathbf1_{r\le b}h, &
d_A(N)&=(a-r)_+h,\\
w(A)V_N&=\mathbf1_{r\le a}(r-b)_+h,&
R_{\rm term}(N,B)&=(b-r)_+h.
\end{aligned}
\tag{AVB42}
\]
The indicator in $V_N$ excludes an already active first layer.
When the extra is empty $r>a$ and all the displayed extra terms vanish.
At $r=a$ the forced extra has zero own-price defect but its full
$w(A)V_N=(a-b)h$. At $r=b$ it remains in $Y$ although both its
$V_N$ contribution and terminal residual vanish. At $r<b$ it remains
in $Y$ and has positive terminal residual. Missing neutral terminal
layers are excluded by $N_B$; deliberately adding them would change
the literal $Y$ and its terminal cost.

### A finite actual competitor consumes the jump budget at the same cost

Reuse the exact (QG3) finite identity for the same $N$:
\[
F(M_B)-F(N)=w(A)(T_\psi+S_Q-V_N)+C_B(Y),\qquad
C_B(y)=f(B)+b(y-B)-f(y)\ge0\quad(y>1).
\tag{AVB43}
\]
Here $Y=\log\operatorname{lcm}(N,N_B)$ is literal and need not equal $B$;
strict concavity gives $C_B(y)=0$ exactly when $y=B$.
The existing maximizing-multiple construction
[GoldenFutureExtensionMaximum](../../D5/S3/Arith/GoldenFutureExtensionMaximum.lean),
in particular golden_future_extension_maximum_attained, and
[GoldenColossalClosure](../../D5/S3/Arith/GoldenResource/GoldenColossalClosure.lean),
maximizes $W-b\log n$ over multiples of $N$ by installing all missing
positive-price layers. It is the fixed-price construction used in
(QG1)–(QG3), not an actual-$G$ optimization assertion.

Take a nonnested consecutive edge starting at $N=N_i=p_iU_i$.
Here the departing extra is nonempty, so its last label is $s=p_i$.
Let the literal integer $Z=p_iV_i$ have clock $z=A+D_i$.
Since $U_i\mid V_i$, $Z$ is a multiple of the same $N$, and
$F(Z)=F(N)-\alpha_i$. Fixed-price maximality gives
$W(M_B)-bY\ge W(Z)-bz$.
The identity
$W(X)-b\log X=F(X)+f(B)-bB-C_B(\log X)$
then gives
\[
F(M_B)-F(N)\ge-\alpha_i+C_B(Y)-C_B(A+D_i).
\tag{AVB44}
\]
The $C_B(Y)$ here is exactly the one in (AVB43). Cancelling that
same cost yields the finite, original-objective comparison
\[
T_\psi(A,H)\ge-S_Q(A,H)+V_N(A,H)
 -\frac{\alpha_i+C_B(A+D_i)}{w(A)}.
\tag{AVB45}
\]
From (AVB31) at $j=i$, $\alpha_i\le(\log2)\lambda(A)$, and
$\lambda(A)/w(A)=A\log A/(1+\log A)<A$. Therefore
\[
\boxed{\quad
T_\psi(A,H)\ge-S_Q(A,H)+V_N(A,H)
 -(\log2)A-\frac{C_B(A+D_i)}{w(A)}.
\quad}
\tag{AVB46}
\]
This is a real finite consumer of the weighted nonnested jump estimate.
To consume the actual competitor budget as well, let $\Omega_i$ denote
the width in (AVB30). On this edge $\alpha_i=\Omega_i-\eta_i$, so
(AVB45) is equivalently the bound
\[
T_\psi\ge-S_Q+V_N-\frac{\Omega_i+C_B(A+D_i)}{w(A)}
 +\frac{\eta_i}{w(A)},\qquad
0\le\frac{\eta_i}{w(A)}\le\frac{13}{A\,w(A)}=o(S_A).
\tag{AVB46C}
\]
The last estimate is uniform by (AVB25)–(AVB26). Thus the finite
comparison retains the actual replacement correction, and its omission
costs at most the paid $13/[A\,w(A)]$ allowance.
This uses $\beta_i=\eta_i$ only on the nonnested branch, and does not
replace $\alpha_i$ by $\eta_i$.
The nonnegative cost $C_B(A+D_i)/w(A)$ is still unpaid, and cofinality
does not provide nonnested departures beyond every required common
start. Even if that source supply and an $o(w(A)S_A)$ cost were supplied,
the $O(A)=o(S_A)$ error in (AVB46) would leave only the critical
coefficient $c_Q$, not any fixed $\kappa<c_Q$.
The strict $\beta_i>0$ at $D_i>0$ supplies no such uniform margin.

### Full shorter-Q quantifiers and the unpaid actual-source sign

For the remaining comparison specialize to the existing shorter scale
$H=A^{4/5}$, $B=A+H$ and $S_A=A^{11/10}=H^2/\sqrt A$.
Retain the ordinary GM input exactly as in (QGM): fixed
$\epsilon_{\rm GM}=1/60$, $\beta_{\rm GM}=7/12$, and constants
$C_{\rm GM},Y_0$ for which
\[
|\pi(y+v)-\pi(y)-v/\log y|
 \le C_{\rm GM}v e^{-(\log y)^{1/4}},\qquad
y\ge Y_0,\quad y^{7/12}\le v\le y^{99/100}.
\]
It is an absolute prime-counting error uniform in that range.
The conversion to $\theta$ retains
$O(v\log y\,e^{-(\log y)^{1/4}}+v^2/(y\log y))$, including its logarithmic
factor. The common finite support and growing-index derivative controls
of (QH1)–(QH10), the strict atom correction
$+\operatorname{atom}(y)-\operatorname{atom}(y+v)$, all higher actual
and reference layers, and the actual/reference square coefficients
$\sqrt2/4$ and $1/4$ are those already paid in (QH11)–(QH13).
They give (QQE), with one unknown common all-real start $A_*$:
\[
\left|\frac{S_Q(A,A^{4/5})}{S_A}-c_Q\right|
 \le C\mathcal F_Q(A),\qquad c_Q=\frac{\sqrt2-1}{4},
 \qquad A\ge A_*,
\]
\[
\begin{aligned}
\mathcal F_Q(A)={}&\frac1{\log A}+A^{-1/5}
 +\log A\,e^{-((\log A)/3)^{1/4}}+A^{-1/120}\\
 &+A^{-3/10}\log A+A^{-1/6}(\log A)^{4/3}
 +A^{-19/180}(\log A)^{43/36}.
\end{aligned}
\tag{AVB47}
\]
All seven terms tend to zero. One common start pays the GM threshold,
both square cutoffs, support, all growing-index length tests and the
error tolerance for every sufficiently large real $A$.
No numerical common start is supplied by this estimate.
Its control of $S_Q$ does not supply the main-scale signed $T_\psi$ input:
an absolute GM allowance there, divided by $S_A$, has size
$\sqrt A\log A\,e^{-c(\log A)^{1/4}}$ for a fixed $c>0$,
which is not $o(1)$. The exponent
$(\log A)/2-c(\log A)^{1/4}+\log\log A$ tends to $+\infty$.
This diagnoses an unpaid allowance, not the size or sign of the true
arithmetic error.

The singleton loss is uniform even when the forced prime is much larger
than $A$. If $V_N>0$, its sole extra has $b<r_{s,1}\le a$.
Since $r_{s,1}<\lambda(s)$ and $\lambda$ decreases, $s<B$.
Equation (AVB37) gives
$w(A)V_N\le(a-b)\log s<(a-b)\log B$.
Also $(a-b)/w(A)=\int_0^H\rho_A(u)\,du<H$, since $w$ decreases.
The zero-loss case is immediate. Thus, without a bound $\log s\le\log A$,
\[
0\le V_N(A,A^{4/5})<A^{4/5}\log(2A)
 =g(A)S_A,\qquad
g(A)=A^{-3/10}\log(2A)\longrightarrow0.
\tag{AVB48}
\]
This pays a uniform preoccupied loss. It does not pay a signed
$T_\psi$ allowance.

Combining (AVB41) and (AVB43) exposes the exact GA2 orientation:
\[
\boxed{\quad
\Xi_s(B)+u_s=F(N)-F(M_B)+C_B(Y)
 \ge C_B(Y)\ge0.
\quad}
\tag{AVB49}
\]
The inequality is actual GA2 at the same literal multiple $M_B$.
Reversing it would introduce the missing favorable sign.
In particular the paid $9/A$ and $13/A$ errors do not make
$\Xi_s(B)$ favorably negative.

The exact (QG7) finite Lambda kernel, at that same real $A$, is
\[
k_A(n)=\mathbf1_{A<n\le B}
       \frac{\lambda(n)-\lambda(B)}{w(A)},\qquad
D_0(A)=\frac{f(B)-f(A)-H\lambda(B)}{w(A)},\qquad
T_\psi=\sum_{n\ge1}\Lambda(n)k_A(n)-D_0(A).
\tag{AVB50}
\]
Its initial atom is excluded and its terminal atom has zero weight.
Every prime power $n=q^k$ has its full $\Lambda(n)=\log q$ mass.
Finite integration of
$\psi(t)-\psi(A)=\sum_{A<n\le t}\Lambda(n)$ proves the displayed
formula, including
$D_0(A)=\int_0^H u\rho_A(u)\,du$.
For any real $\kappa$ the exact same-source equivalence is
\[
T_\psi(A,A^{4/5})\ge-\kappa S_A
\ \Longleftrightarrow\
\Xi_s(B)+u_s\le w(A)[\kappa S_A-S_Q(A,H)+V_N(A,H)].
\tag{AVB51}
\]
When $\kappa<c_Q$ is fixed, the right side is
$-(c_Q-\kappa+o(1))w(A)S_A$, a strictly negative margin eventually.
Equation (AVB49) exhibits the opposite GA2 orientation. The desired
contradiction therefore still requires the following actual arithmetic
source-and-sign input:
\[
\boxed{\quad
\exists\text{ fixed }\kappa<c_Q\ \forall\text{ required real }T_0\
 \exists p\ge29\text{ prime}:\quad
 A_p\ge T_0,\qquad
 \sum_{n\ge1}\Lambda(n)k_{A_p}(n)
 \ge D_0(A_p)-\kappa A_p^{11/10}.
\quad}
\tag{AVB52}
\]
This input is unproved. The required start includes a common (QQD)
tolerance start, the uniform (AVB48) tolerance start and every additional
analytic transfer start. Clock cofinality from $N_p\ge5040p$ can pass
each unknown finite start, but it does not supply the favorable sign
in (AVB52).

For its precise consumer let $\varepsilon=(c_Q-\kappa)/4$.
Beyond the common starts, (AVB47)–(AVB48) give
$S_Q\ge(c_Q-\varepsilon)S_A$ and $V_N\le\varepsilon S_A$.
If (AVB52) supplied the additional $T_\psi\ge-\kappa S_A$ there,
then
\[
T_\psi+S_Q-V_N\ge\frac{c_Q-\kappa}{2}S_A,\qquad
F(M_B)-F(N)\ge\frac{c_Q-\kappa}{2}w(A)S_A+C_B(Y)>0.
\tag{AVB53}
\]
The contradiction is at a literal integer multiple of the selected
actual $N$; it uses no standalone theorem with the missing sign
silently assumed as a proved conclusion.

A finite positive average is an equivalent selection interface only
with the same source coverage. Precisely, for every required $T_0$,
take a finite set of actual labels with $A_p\ge T_0$ and nonnegative
weights $a_p$ of positive total weight. A proved inequality
\[
\sum_p a_p\sum_n\Lambda(n)k_{A_p}(n)
 \ge\sum_p a_p[D_0(A_p)-\kappa A_p^{11/10}]
\tag{AVB54}
\]
forces at least one positive-weight label to satisfy (AVB52), since
otherwise the finite sum of its strict failures is negative.
Conversely a single qualifying source gives this finite interface.
Neither inequality is supplied by cofinality or scalar means.
Duplicate plateau labels aggregate weight at one integer and create
no independent samples.

For clarity about an alternative transfer route, the actual weak-$\psi$
stability estimate for $X\ge1024$, $A,C\in[X,2X]$ and
$d=|C-A|\le X^{4/5}/2$ is
\[
|T_\psi(A,A^{4/5})-T_\psi(C,C^{4/5})|
 \le120X^{4/5}(d+1)\log X.
\tag{AVB55}
\]
One direct derivation writes
$Q_a(t)=\psi(t)-\psi(a)-(t-a)$ and $R_a(t)=w(t)/w(a)$ on
$I_a=[a,a+a^{4/5}]$. Put $L=X^{4/5}$ and $\ell_0=\log(3X)$.
The full prime-power count gives
$0\le\psi(v)-\psi(u)\le(v-u+1)\ell_0$ for $X\le u\le v\le3X$,
so $|Q_a(t)|\le5L\ell_0$.
For $C\ge A$, the symmetric-difference length of $I_A,I_C$ is at most
$3d$, including the full upper-endpoint motion. Its cost is at most
$15Ld\ell_0$. On their intersection,
$Q_C-Q_A=d-[\psi(C)-\psi(A)]$, costing at most $4L(d+1)\ell_0$.
Finally $|w'/w|\le4/X$ gives
$0\le R_C-R_A\le4d/X$, costing at most
$40dL^2\ell_0/X\le40dL\ell_0$.
Adding and using $\ell_0\le2\log X$ proves (AVB55).
The $+1$ retains an initial prime-power jump and cannot be removed
merely by continuity of the remaining weights.

Dividing (AVB55) by $X^{11/10}$ shows that
$d=o(X^{3/10}/\log X)$ would suffice for vanishing normalized transfer
error. A fixed-margin favorable center at cofinally many scales together
with paired actual clocks at that distance and all common starts would
therefore suffice. The favorable centers and their paired actual-source
coverage are both unpaid. This sufficient pairing is not inserted as a
premise of (AVB25), (AVB41), (AVB46) or (AVB52).
Bertrand label gaps, the weighted width and monotone cofinal clocks give
no such mesh; no stronger uniform mesh is asserted or required here.

### Source scope and the remaining full target

Euler factorization, positive-price prefix optimization, scalar strict
concavity, Bertrand, Gronwall and finite Stieltjes integration by parts
are standard inputs. The original pressure, $I_\psi$, $R$, same-integer
defect and finite lcm consumer are the existing FIB/ZE/NC interfaces
cited above. The project-derived addition is (AVB19)–(AVB25), the
all-branch actual-value and accumulated literal-competitor error package,
with (AVB29) and (AVB31) making its actual measure and weighted jump
content explicit. Its immediate substantive uses are (AVB41) and
(AVB45)–(AVB46). No global novelty or primary-proof claim is made.

The own-clock event sampling (OCQ1)–(OCQ14) above retains its own
post-event source $N_p=C_{b_p}$ and its separate unproved continuous
signed-head condition (OCQ10). Its (OCQ13) all-integer defect identity
is reused in (AVB39); its sample choice, seven-eighths zero ceiling
and conditional (OCQ14) consumer do not supply (AVB52).
The $N_p$ of this section instead denotes the least actual maximizer
on $\mathcal D_{5040p}$, as explicitly defined above.
No identification of those two source families is used.
Seven-eighths nonvanishing, almost-all centers and bounded multiplicative
correlations likewise supply no stated same-actual-source Lambda sign.

The conditional finite real-clock interval (GAK40)–(GAK51), through
$A=8\cdot10^{46}$, retains its original source/material premises and
each integer's defect in (GAK39). It is a finite interval and source
corollary. Neither it nor the earlier $7.2\cdot10^{46}$ interval is an
unbounded family start, a least-counterexample bound, or payment of
the unknown GM/QQE starts. A separately selected least global maximizer,
a least counterexample, and the cofinal forced-prime family are not
interchangeable sources.

All separate deletion comparisons here occur above the forced exponent
and stay in their stated multiple class with integer at least $3$.
Completed prime replacements are compared only after insertion and
in their legal opposite forced class; no bare forced-prime deletion
comparison is used. The proper-deletion bridge used for a global $n>5040$ source has its own full hypotheses:
a deletion that merely remains above $e$ need not remain above $5040$.
Restricted comparisons cannot replace that bridge, and no integer
replacement is imported from the wrong domain.

The paid errors are $u_s$ and the sum of actual $\eta_i$, at uniform
$o(w(A)S_A)$ precision. The unpaid estimates are the signed cancellation
in (AVB51)–(AVB52), its every-start source coverage, and, for the
nonnested finite-competitor route, source supply, the literal cost
$C_B(A+D_i)$ and a strict coefficient gain beyond the critical $c_Q$.
Formal analytic suppliers and their dependency verification are separate
from this ordinary exposition. No estimate here proves the full
every-$n>5040$ signed target (AVB02), which remains active and unproved.
## Project application: forced windows and exact pairing of actual maximizing multiples

Use the strict inventories, Euler layers, \(f,\lambda,w,K,\psi,Q\),
\(T_\psi,S_Q,V_N\) and concavity cost \(C_t\) of QH1–QH13 and
QG1–QG8. Write \(N_t^{\rm str}\) for that section's strict actual
integer \(N_t\), to distinguish it from a maximizing multiple. Thus
\(K(t)=\log N_t^{\rm str}\), actual equality layers are excluded, and
the reference \(\psi(t)=\sum_{q^k\le t}\log q\) is weak and includes
every prime power. All compact positive-price intervals have one common
finite layer support, including actual ties and reference atoms.

For \(n\ge3\), put \(F(n)=\log G(n)=W(n)-f(\log n)\). For an ordinary
prime \(p\ge29\), let
\[
\mathscr M_p=\mathop{\rm argmax}_{5040p\mid n,\ n\in\mathbb N_{>0}}F(n),
\quad v(p)=\max_{5040p\mid n}F(n),\quad
N_p^{\rm mult}=\min\mathscr M_p,\quad A_p^{\rm mult}=\log N_p^{\rm mult}.
\]
These are maxima of the **actual Robin ratio over the entire multiples
class**. They are distinct from the earlier event-indexed fixed-price
integers \(N_p=C_{b_p}\).

The completed all-branch deductions supply the following intermediate inputs: actual attainment under RH failure; for every maximizing tie over multiples of \(m\ge3\), with clock \(A\), \[ N=\operatorname{lcm}(m,N_A^{\rm str}); \] the strict activation of all 5040 layers when \(m=5040p,\ p\ge29\); and consequently \[ N=\operatorname{lcm}(p,N_A^{\rm str}),\qquad E_N\subseteq\{(p,1)\}. \] They also supply the global clock/value ordering of the **least** sources, their finite constant-integer blocks, and the last-label bounds used below. These all-branch and E1–E8 inputs are reused as recorded in the [completed forced-window proof, §§2, 8–9](../ArithSums/trureturing2026extrawindowpairing.md). Global least-source ordering does not assert global ordering of arbitrary ties. The finite positive-prefix optimizer at an arbitrary positive price is the existing [golden_future_extension_maximum_attained](../../D5/S3/Arith/GoldenFutureExtensionMaximum.lean); its private prefix construction realizes \(\operatorname{lcm}(N,N_t^{\rm str})\) at price \(\lambda(t)\). [GoldenColossalClosure](../../D5/S3/Arith/GoldenResource/GoldenColossalClosure.lean) also has the exponent-max construction, at its base threshold. Neither fixed-price result is substituted for actual-\(G\) attainment.

### Fixed ordinary suppliers and the forced window

Assume RH is false. The CNS oscillation input on CA integers, with
\(\Theta=\sup_{\rho\text{ a nontrivial zero of }\zeta}\Re\rho\),
supplies **one fixed**
\[
1-\Theta<b<\tfrac12,\qquad d>0,
\]
and arbitrarily large actual integer witnesses \(m\), with \(X=\log m\),
such that \(F(m)\ge\gamma+dX^{-b}\). Here \(0<b<1/2\), since
\(\Theta\le1\). This is the log-converted form of CNS
[arXiv:1112.6010v2](https://arxiv.org/abs/1112.6010v2), printed p.15,
whose underlying oscillation citation is **Robin 1983, [15], p.241**,
not the separate Robin 1984 criterion.

CNS equation (2), printed p.2, supplies the positive upper envelope.
Using the upper rounding \(0.6483\) also printed on p.15, let
\(K_R=0.6483e^{-\gamma}>0\). For every \(n\ge3\), \(A=\log n>1\),
\[
F(n)-\gamma\le\frac{K_R}{(\log A)^2}.
\]
This is an upper envelope with a positive error. Both published inputs
are ordinary suppliers; their underlying analytic proofs are not
reproved here.

Use QGM with its fixed \(\epsilon_{\rm GM}=1/60\) and
\(\beta=7/12\), for all real starts and only lengths
\(y^\beta\le h\le y^{99/100}\). Enlarge its unknown common start so
that its relative counting error is at most \(1/2\). Then every permitted
interval contains a prime, and eventually the next ordinary prime after
\(p\) is at most \(p+p^\beta\). This remains a label-spacing input.

For each qualifying witness \(X\), define
\[
\ell_X=\frac d8X^{1-b}\log X,\qquad
R_X=\exp\!\left(\sqrt{\frac{2K_R}{d}}X^{b/2}\right),\qquad
\mathcal P_X=\{p\text{ prime}:e^{\ell_X}\le p\le e^{2\ell_X}\}.
\tag{FW0}
\]
\(R_X\) is the **window clock ceiling**, distinct from the original
Robin residual \(R(t)\). In the local proofs abbreviate
\(\ell=\ell_X,\ R=R_X\).

**Theorem N1 (uniform full-domain confinement and label uniqueness).**
There is an unknown witness start \(X_0\) such that for every qualifying
\(X\ge X_0\), every \(p\in\mathcal P_X\), and **every**
\(N\in\mathscr M_p\), with \(A=\log N\),
\[
v(p)\ge\gamma+\frac d2X^{-b},\qquad
\ell\le A\le R,\qquad
N=pN_A^{\rm str},\qquad E_N=\{(p,1)\},\qquad P^+(N)=p.
\tag{FW1}
\]
The same actual integer cannot be a maximizing tie for a different
ordinary label \(q\ge29\), including a label outside this window.
For each fixed \(M>0\),
\[
\frac{e^\ell}{R^M}\longrightarrow\infty
\tag{FW2}
\]
along the witnesses; its eventual start is independent of \(p\) and tie.

*Proof.* Set \(m_0=\operatorname{lcm}(5040,m)\),
\(d_0=\log(m_0/m)\in[0,\log5040]\), and take the literal integer
\(D_p=pm_0\). This is a legal multiple of \(5040p\), even when \(p\)
already divides \(m_0\). With \(k=v_p(m_0)\), exact Euler telescoping gives
\[
F(D_p)-F(m)=W(m_0)-W(m)+\ell_{k+1}(p)
 -[f(X+d_0+\log p)-f(X)].
\]
The two Euler increments are nonnegative. Since \(\lambda\) decreases,
the last cost is at most
\[
\frac{d_0+\log p}{X\log X}
\le\frac d4X^{-b}+\frac{\log5040}{X\log X}
\le\frac d2X^{-b}
\]
eventually, uniformly over the window. Thus \(F(D_p)\) has the required
floor. This uses the \((k+1)\)-st layer, not an absent-prime assumption.

For any integer with clock \(A>R\), the upper envelope is strictly below
that floor, since \(K_R/(\log R)^2=(d/2)X^{-b}\). In particular \(D_p\)
has clock at most \(R\). The nonempty finite set of multiples of
\(5040p\) with clock at most \(R\) therefore attains the entire
infinite-domain maximum, and contains all its ties. The lower clock
bound follows from \(N\ge5040p\); equality at the upper bound is retained.

Write \(a_R=\sqrt{2K_R/d}\). Then
\[
\frac{\ell}{\log R}
=\frac d{8a_R}X^{1-3b/2}\log X\longrightarrow\infty.
\]
Hence \(\ell-M\log R\to\infty\) for every fixed \(M\), proving FW2.
In particular \(p>2R\) eventually. For any tie, \(A\le R<p\), so
\(r_1(p)<\lambda(p)<\lambda(A)\). The reused strict 5040 activation
and all-branch characterization give \(N=pN_A^{\rm str}\), with exactly
one strictly inactive occupied extra. Every prime of \(N_A^{\rm str}\)
is \(<A\le R\), so \(P^+(N)=p\). If the same integer maximized another
label \(q\), its same own-clock nonempty extra set would be contained
in both \(\{(p,1)\}\) and \(\{(q,1)\}\), forcing \(q=p\). ∎

### One finite literal core and all choices of window ties

Define the common finite set and its real-parameter envelope by
\[
\mathcal C_X=\{u\in\mathbb N_{>0}:5040\mid u,\ \log u\le R,\
       \forall q\text{ prime},\ q\mid u\Rightarrow q\le R\},
\qquad
\mathcal V_X(h)=\max_{u\in\mathcal C_X}\{W(u)-f(\log u+h)\}
\quad(\ell\le h\le2\ell).
\tag{FW3}
\]
The set is nonempty eventually, since it contains 5040.

**Theorem N2 (exact envelope and all-choice ordering).**
For every sufficiently large qualifying witness and every
\(p\in\mathcal P_X\),
\[
v(p)=c_p+\mathcal V_X(\log p),\qquad c_p=\ell_1(p).
\tag{FW4}
\]
Multiplication by \(p\) is a bijection from **all** active cores at
\(\log p\) to \(\mathscr M_p\), preserving leastness.
The envelope is strictly decreasing and convex. If \(h_1<h_2\), every
active core clock at \(h_1\) is at most every active core clock at \(h_2\).
In particular, for any choices
\(N=pU\in\mathscr M_p,\ N'=rV\in\mathscr M_r\) at \(p<r\) in the window,
\[
A=\log N<C=\log N',\qquad U\mid V,\qquad
C-A=\log(V/U)+\log(r/p).
\tag{FW5}
\]
At a real \(h\), if active core clocks have extrema \(a_{\min},a_{\max}\),
the left/right derivatives and subgradient interval are
\[
\mathcal V'_{X,-}(h)=-\lambda(h+a_{\min}),\qquad
\mathcal V'_{X,+}(h)=-\lambda(h+a_{\max}),\qquad
\partial\mathcal V_X(h)=
[-\lambda(h+a_{\min}),-\lambda(h+a_{\max})].
\tag{FW6}
\]

*Proof.* FW1 puts every full-domain tie in the form
\(pN_A^{\rm str}\), whose core lies in \(\mathcal C_X\), including all
5040 layers. Conversely every \(u\in\mathcal C_X\) makes \(pu\) legal;
\(p>R\) makes \(p\) absent from that core, so its Euler factor is exactly
\(c_p\). Taking maxima proves both the identity and the full tie
bijection, rather than replacing the multiples domain by a restriction.

Each summand of FW3 has derivative \(-\lambda(\log u+h)<0\) and
second derivative \(w(\log u+h)>0\). Its finite maximum is convex and
strictly decreasing. If \(\log u>\log v\), the derivative of the
\(u\)-summand minus the \(v\)-summand is
\(\lambda(\log v+h)-\lambda(\log u+h)>0\). If \(u\) is active at
\(h_1\), that difference is strictly positive at \(h_2>h_1\);
\(v\) cannot be active there. This proves the all-choice order.
At actual labels, \(C>A\) follows after adding the strictly larger
label clock. Since \(U=N_A^{\rm str}\) and \(V=N_C^{\rm str}\),
monotonicity of strict inventories gives \(U\mid V\) and FW5.

The one-sided derivatives of a finite convex maximum are respectively
the minimum and maximum active derivatives, giving FW6. Actual active
cores remain a finite set of literal integers; intermediate subgradients
need not be clocks of integer cores. No assertion identifying different
ties at one parameter is used. ∎

### Literal replacements and their arriving-scale deficiencies

Let \(p<r\) be consecutive ordinary primes, both in \(\mathcal P_X\),
and choose any of their maximizing ties. Use
\[
N=pU,\quad N'=rV,\quad A=\log N,\quad C=\log N',\quad
\delta=\log(r/p)>0,\quad D=\log(V/U)\ge0,
\]
\[
Z=pV,\quad z=\log Z=A+D=C-\delta,\quad
\varepsilon=F(N)-F(Z),\quad
\varepsilon_r=F(N')-F(rU).
\tag{FW7}
\]
\(Z\) is a literal multiple of the **same original** \(N\).

**Theorem N3 (rectangle identity and uniform arrival errors).**
The sources \(N,N'\) are distinct and neither divides the other.
Both deficiencies in FW7 are nonnegative, and
\[
\varepsilon+\varepsilon_r
=\int_0^\delta\int_0^D w(A+s+t)\,dt\,ds
\le\delta\lambda(A).
\tag{FW8}
\]
Their cross-label value drop satisfies
\[
0<v(p)-v(r)\le\delta[1/p+\lambda(A)].
\tag{FW9}
\]
Put \(E_X=e^{-5\ell/12}\). Uniformly over these pairs and all tie choices,
\[
0<\delta\le E_X,\qquad
0\le\varepsilon\le\frac{E_X}{\ell\log\ell},
\tag{FW10}
\]
\[
\frac{\varepsilon}{w(C)},\ \frac{\varepsilon}{w(z)}
\le\frac{E_XR^2\log R}{\ell\log\ell}\longrightarrow0,
\qquad
\frac{\varepsilon}{w(C)C^{11/10}},\
\frac{\varepsilon}{w(z)z^{11/10}}
\le\frac{E_XR^{9/10}\log R}{\ell\log\ell}\longrightarrow0.
\tag{FW11}
\]
For each fixed \(M>0\), \(\delta R^M\) and \(\varepsilon R^M\)
tend uniformly to zero. No hypothesis controlling \(C/A\) is needed.

*Proof.* Both cores have primes at most \(R<p<r\), so each source
lacks the other's label prime. FW5 gives \(U\mid V\), making \(Z=pV\)
legal in \(N\)'s multiples class, and \(rU\) legal in the \(r\)-class.
Actual maximality gives the nonnegative deficiencies. The two label Euler
factors cancel in their sum, leaving
\[
f(A+D)-f(A)-f(A+D+\delta)+f(A+\delta).
\]
Twice integrating \(f''=-w\) gives FW8; integrating the inner curvature
over its full half-line bounds it by
\(\int_0^\delta\lambda(A+s)\,ds\le\delta\lambda(A)\).
Also
\[
F(pV)-F(rV)=c_p-c_r+f(C)-f(C-\delta)>0.
\]
Comparing with the legal \(rU\) bounds the drop by
\(c_p-c_r+f(A+\delta)-f(A)\).
The exact identity
\[
c_p-c_r=\int_{\log p}^{\log r}\frac{du}{e^u+1}\le\delta/p
\]
proves FW9.

GM is applied at length \(p^\beta\), inside its permitted range; thus
\(r\le p+p^\beta\) and
\(\delta\le p^{-5/12}\le E_X\). This gives FW10. For every
\(t\in[\ell,R]\),
\[
w(t)\ge\frac1{R^2\log R},\qquad
w(t)t^{11/10}\ge\frac1{R^{9/10}\log R}.
\]
Together with \(A\le z<C\le R\), these give the explicitly expanded
arrival estimates FW11. All their ceilings vanish because
\(\log R=o(\ell)\), as do the fixed-\(M\) bounds. The cross-label
drop itself has normalized bound
\[
\frac{v(p)-v(r)}{w(C)C^{11/10}}
\le E_XR^{9/10}\log R
       \left[e^{-\ell}+\frac1{\ell\log\ell}\right]\longrightarrow0.
\]
Thus its strictness supplies no fixed normalized gain. If \(D=0\),
\(Z=N\) and both deficiencies vanish. When \(D>0\),
\(\varepsilon=0\) may still be a same-domain tie; choosing the least
arrival gives \(\varepsilon_r>0\), without a quantitative margin. ∎

### Exact integer rigidity and the signed compensated contact

**Theorem N4 (literal pairing without clock-ratio control).**
For every sufficiently large qualifying window and every FW7 pair,
\[
M_z=\operatorname{lcm}(N,N_z^{\rm str})=Z,\qquad
\log M_z=z,\qquad
N_t^{\rm str}=V\quad(z\le t\le C).
\tag{FW12}
\]
In particular the original arriving clock \(C\) is exactly
\(\delta\) after this optimizer clock. \(Z\) need not be GA2 or a
canonical maximizing source.

For the **canonical least sources**, let \(p=p_j\) be the departure's
last label and reuse the E1–E8 right-continuous arriving-clock sum
\[
J_p(t)=\sum_{\substack{i\ge j\\ A_{p_{i+1}}^{\rm mult}\le t}}
             \log(p_{i+1}/p_i),
\]
where \(p_i\) run through successive ordinary prime labels. Then
\[
J_p(t)=0\quad(A\le t<C),\qquad J_p(C)=\delta.
\tag{FW13}
\]
With \(Y_N(t)=\log\operatorname{lcm}(N,N_t^{\rm str})\), the compensated
endpoint and the preceding integral are exactly
\[
Y_N(C)-C+J_p(C)=0,\qquad
\int_z^C[Y_N(t)-t+J_p(t)]w(t)\,dt=-C_C(z)<0.
\tag{FW14}
\]

*Proof.* Monotonicity and FW5 give
\(U\mid N_z^{\rm str}\mid V\). The label \(p>C\) is absent from these
cores. Thus \(M_z=pN_z^{\rm str}\mid Z=pV\), and its clock \(y\)
satisfies \(A\le y\le z\).

Reuse the literal finite positive-prefix optimizer at price \(\lambda(z)\).
Its deficiency against this same \(Z\) is
\[
\Delta_z=[W(M_z)-\lambda(z)y]-[W(Z)-\lambda(z)z]\ge0.
\]
Directly at these integers, with
\(C_z(y)=f(z)+\lambda(z)(y-z)-f(y)\), one obtains
\[
\varepsilon=[F(N)-F(M_z)]+C_z(y)+\Delta_z.
\tag{FW15}
\]
All three terms are nonnegative: \(M_z\) is an actual multiple of the
actual-GA2 integer \(N\), the cost is concave-tangent cost, and the last
term is fixed-price deficiency. For \(y\le z\),
\[
C_z(y)=\int_y^z(t-y)w(t)\,dt\ge\tfrac12w(z)(z-y)^2.
\]
Consequently the *actual common ceiling* in FW11 gives
\[
(z-y)^2\le
\frac{2E_XR^2\log R}{\ell\log\ell}\longrightarrow0.
\tag{FW16}
\]
Eventually \(z-y<\log2\), uniformly. Since \(Z/M_z\) is a positive
integer, any failure of equality would give \(Z/M_z\ge2\), contradicting
FW16. Therefore \(M_z=Z\) exactly. Cancelling the literal common factor
\(p\) gives \(N_z^{\rm str}=N_C^{\rm str}=V\).
Monotonicity gives equality on the **closed** interval \([z,C]\).
A missing equality layer at \(z\) would become strictly active before
\(C\), contradicting it. A missing tie at \(C\) remains excluded and has
zero terminal pressure.

For canonical sources, FW1 makes both label blocks singletons, including
possible labels outside the window. Their global least-source clock
order, and consecutiveness of \(p,r\), give no arriving-clock atom in
\([A,C)\) and exactly the mass \(\delta\) at \(C\). A later label at
the same clock would produce the same integer as \(N'\), contradicting
FW1's label uniqueness. This proves FW13 with weak arrival indexing;
no general plateau masses are omitted.

On \([z,C]\), \(Y_N(t)=z\). Before \(C\) the compensated integrand is
\(z-t\), and at \(C\) it jumps to \(z-C+\delta=0\). Its integral is
\(-\int_z^C(t-z)w(t)\,dt=-C_C(z)<0\).
The single endpoint atom has zero ordinary integration measure.
The uncorrected envelope integrals from \(A\) to \(z\) and to \(C\),
using the existing finite lcm identity, are respectively
\(-\varepsilon\) and \(-\varepsilon-C_C(z)\).
No divergent tail integrals are subtracted.

The small retained cost also satisfies
\[
0<C_C(z)\le\tfrac12w(z)\delta^2,\qquad
\frac{w(z)}{w(C)}\le e^{4\delta/z}\longrightarrow1.
\]
Here the bound \(|w'/w|\le4/t\) applies once \(t\ge e\). Hence eventually
\[
\frac{C_C(z)}{w(C)C^{11/10}}
\le\frac{\delta^2}{C^{11/10}}\longrightarrow0,
\qquad C_C(z)\le\tfrac12w(\ell)E_X^2.
\]
These uniform estimates retain the negative sign in FW14. ∎

### Cofinal literal forward successors and real-base transport

**Theorem N5 (cofinal exact pairing and a nontrivial forward integer).**
For every finite common start \(T\), and every finite collection of
supplier or tolerance starts, there is a sufficiently large qualifying
window and a canonical FW7 pair with \(A,z,C\) beyond all these starts.
For each such pair put
\[
h=z^{4/5},\quad B_z=z+h,\quad
L=pN_{B_z}^{\rm str},\quad Y=\log L.
\]
Then, eventually and uniformly,
\[
N\mid Z\mid L,\qquad L>Z\ge N,\qquad
V_Z(z,z^{4/5})=0,\qquad V_{N'}(C,C^{4/5})=0.
\tag{FW17}
\]
Applying the existing exact QG accounting at this same \(Z\), and then
subtracting its deficiency against this same original \(N\), gives
\[
F(L)-F(N)
=w(z)[T_\psi(z,z^{4/5})+S_Q(z,z^{4/5})]
       +C_{B_z}(Y)-\varepsilon.
\tag{FW18}
\]
The actual terminal clock \(Y\) and its full nonnegative cost are retained.
At the arriving original source \(N'\), its own literal successor is
\(rN_{C+C^{4/5}}^{\rm str}\).

*Proof.* GM at the real start \(e^\ell\), length \(e^{\beta\ell}\),
gives a prime \(p\) just above \(e^\ell\); GM at \(p\) gives its next
prime \(r\). Eventually \(r<4e^\ell<e^{2\ell}\), so both belong to
\(\mathcal P_X\). Since \(A,z,C\ge\ell\to\infty\), the unbounded
actual witness clocks pass any finite collection of starts together.
These are the original canonical maximizing integers, not the oscillation
seed \(m\) or its padded comparator \(D_p\). FW1 supplies cofinal
extra-bearing canonical source blocks.

FW12 gives \(N_z^{\rm str}=V\), so \(Z=pV\) divides \(L\).
Since \(p>2R\) and \(B_z<2z\le2R\), its unique occupied extra remains
strictly below the price throughout \([z,B_z]\). Thus its entire
preoccupied loss is exactly zero. The same argument with \(r,C\) proves
the arriving source's zero loss. The finite QG2–QG3 accounting only
requires \(N_z^{\rm str}\mid Z\), the strict initial core and the actual
literal successors; GA2 of \(Z\) is not needed. It therefore gives FW18.
All initial \(K(z)\) terms cancel as in QG3; \(K(z)=z\) is not assumed.

For strict nontriviality apply GM at the real start \(z+h/3\) with length
\(h/3\). Its permitted-length inequalities hold eventually because
\(7/12<4/5<99/100\). There is a prime
\[
z+h/3<q\le z+2h/3.
\]
Its first layer is absent from \(N_z^{\rm str}\), since \(q>z\).
Eventually \(q<B_z-1<q_1(B_z)\), by MS2's strict first cutoff enclosure,
so that layer belongs to \(N_{B_z}^{\rm str}\). Also \(q<p\).
Thus \(q\mid L/Z\), proving \(L>Z\) independently of any favorable sign.
This does not imply \(Z>N\), a positive \(D\), or GA2 of either forward
integer.

The Lambda term in FW18 is precisely QG7 evaluated at \((z,h)\):
it sums **every** prime power in \((z,B_z]\), with weight
\(\Lambda(n)[\lambda(n)-\lambda(B_z)]\), and subtracts
\(f(B_z)-f(z)-h\lambda(B_z)\). Its initial atom is excluded and its
terminal atom has zero weight. No prime-only or balanced-tent replacement
is made. If terminal equality layers of mass \(J\) are deliberately
installed, their Euler reward is \(\lambda(B_z)J\), the pressure integral
is unchanged, and the cost becomes \(C_{B_z}(Y+J)\). FW18 consistently
uses the strict successor with its original \(Y\). ∎

The completed real-base \(C_0=120\) estimate applies to **every real**
\(x\ge1024\), centers \(a,c\in[x,2x]\), and
\(|c-a|\le x^{4/5}/2\):
\[
|T_\psi(c,c^{4/5})-T_\psi(a,a^{4/5})|
\le120x^{4/5}(|c-a|+1)\log x.
\]
Reuse this estimate with the **actual real base** \(x=z\), \(a=z\),
\(c=C=z+\delta\). Eventually all its comparable-base hypotheses hold,
since \(\delta\le E_X\le1\). It yields the new uniform partner transfer
\[
\frac{|T_\psi(C,C^{4/5})-T_\psi(z,z^{4/5})|}{C^{11/10}}
\le240z^{-3/10}\log z
\le240\ell^{-3/10}\log\ell\longrightarrow0,\qquad
\frac{C^{11/10}}{z^{11/10}}\longrightarrow1.
\tag{FW19}
\]
The moving upper endpoint, weight normalization and initial prime-power
jumps are included in the reused estimate. Its indispensable \(+1\)
is retained even when \(\delta\) is tiny; \(\log Z\) is not assumed to
be a power of two. This applies to the full discontinuous \(\psi\),
not a Lipschitz surrogate.

### Consuming the cofinal extras at every fixed ratio

Enumerate the distinct canonical source blocks in label order as
\(\mathcal N_j\), with clocks \(\mathcal A_j\), last labels
\(p_j=P^+(\mathcal N_j)\), and next ordinary primes \(r_j\).
Let \(\mathcal C_j=A_{r_j}^{\rm mult}=\mathcal A_{j+1}\).
The reused all-branch replacement is the same-source literal integer
\[
\mathcal Z_j=\operatorname{lcm}(\mathcal N_j,N_{\mathcal C_j}^{\rm str}),
\qquad
\mathcal A_j\le\mathcal z_j=\log\mathcal Z_j\le\mathcal C_j.
\]
This definition preserves all branches, including zero-extra blocks.
Finite blocks and unbounded labels give
\(\mathcal A_j,p_j\to\infty\). The reused **departure last-label**
bounds are
\[
\mathcal A_j<3p_j,\qquad
E_{\mathcal N_j}=\varnothing\ \Longrightarrow\ p_j<\mathcal A_j.
\]
They are not applied at a small arrival label inside a zero-extra plateau.

**Theorem (cofinal geometry consumed from N1 and N5).**
Under the same ordinary RH-false suppliers,
\[
\forall q>1\ \forall T\
\exists j:\quad
T\le\mathcal A_j<\mathcal C_j\le q\mathcal A_j,\qquad
\mathcal A_j\le\mathcal z_j\le\mathcal C_j.
\tag{FW20}
\]
Here \(q\) is fixed first; starts may depend on it. Moreover every
sufficiently large qualifying witness window contains a canonical FW7
pair with \(C\le qA\).

*Proof.* Fix \(q>1\), and choose \(\rho=(1+q)/2\in(1,q)\).
If a zero-extra departure is followed by an extra arrival, that arrival
has the unique label \(r_j\). Its extra first layer cannot have
\(r_j\le\mathcal C_j-1\), by the strict first cutoff enclosure.
Consequently \(\mathcal C_j<r_j+1\). Label spacing and the zero-extra
departure's **last** label give
\[
\mathcal C_j<r_j+1\le p_j+p_j^\beta+1
 <\mathcal A_j+\mathcal A_j^\beta+1<q\mathcal A_j
\]
eventually.

Suppose the edges in FW20 were not cofinal. In a tail every
\(\mathcal C_j>q\mathcal A_j\), so no zero-extra block there can be
followed by an extra block. A zero-extra block would therefore force all
subsequent blocks to have zero extra, contrary to N5's cofinal extras.
This tail must consist wholly of extra blocks. Each arrival then has a
unique label, so \(p_{j+1}=r_j\) are consecutive ordinary primes.
Enlarge the tail until \(p_{j+1}\le\rho p_j\).
For all \(k\ge1\), iteration and the last-label bound would give
\[
q^k\mathcal A_j<\mathcal A_{j+k}<3p_{j+k}\le3\rho^kp_j,
\]
impossible since \(q/\rho>1\). This proves the cofinal assertion.

For the window assertion take
\[
k_X=\left\lfloor\frac{\log(R/\ell)}{\log q}\right\rfloor+1,
\qquad q^{k_X}\ell>R.
\]
The initial \(p_0\) constructed in N5 has
\(\log p_0\le\ell+\log2\). Its actual successive primes satisfy
\[
\log p_i\le\ell+\log2+iE_X<2\ell
\qquad(0\le i\le k_X)
\]
by induction using GM at each permitted label and \(k_XE_X\to0\).
The inequality simultaneously justifies their window membership.
FW1 gives \(k_X+1\) distinct canonical clocks in \([\ell,R]\).
If all their consecutive edges had \(C>qA\), the last clock would exceed
\(q^{k_X}\ell>R\). At least one edge has \(C\le qA\), and \(A\ge\ell\)
makes these edges cofinal. N4's ratio-free rigidity did not require this
additional geometry. ∎

In particular FW20 with \(q=2\) pays the premise of the completed
two-price cofinal geometry consumer recorded in the ordinary proof §8.
Its existing all-branch projection
\(\mathcal y_j=\log\operatorname{lcm}(\mathcal N_j,N_{\mathcal z_j}^{\rm str})\)
therefore obeys, cofinally,
\[
0\le\mathcal C_j-\mathcal y_j
\le8\,3^{5/24}\mathcal A_j^{7/24}\sqrt{\log\mathcal A_j}
      +\log(8\mathcal A_j)
=o\!\left(\frac{\mathcal A_j^{3/10}}{\log\mathcal A_j}\right).
\tag{FW21}
\]
Here \(\mathcal A_j\le\mathcal y_j\le\mathcal z_j\le\mathcal C_j
\le2\mathcal A_j\), so its real comparable base is
\(x=\mathcal y_j\). The same \(C_0=120\) estimate gives transfer
\(o(\mathcal C_j^{11/10})\). This consumes the existing conditional
consumer; its projection estimate is not reproved as a new theorem.
It is separate from the exact, ratio-free window pairing FW12.
FW20 is a fixed-ratio cofinal statement, not convergence on every edge
or a shrinking-rate mesh.

### The remaining full signed obligation

QQE/QQD, with all seven errors and their one unknown all-real tolerance
start, apply at the cofinal clocks just constructed:
\[
S_Q(z,z^{4/5})=(c_Q+o(1))z^{11/10},\qquad
c_Q=(\sqrt2-1)/4.
\]
This is reused FullQ, with both actual and reference higher powers and
the reference square subtraction intact. FW11 pays the same original
source's deficiency at the **arriving** scale, FW17 pays the occupied
loss exactly, and FW19 pays transport without discarding its atom cost.
Actual GA2 of \(N\), however, makes FW18 only the necessary **upper**
comparison
\[
w(z)[T_\psi(z,z^{4/5})+S_Q(z,z^{4/5})]
\le\varepsilon-C_{B_z}(Y).
\tag{FW22}
\]
No favorable lower coefficient follows.

The unchanged selected-source debt is one fixed \(\kappa<c_Q\) such that,
beyond **every** required common start \(T\), some original canonical
\(N_p^{\rm mult}\) has \(A_p^{\rm mult}\ge T\) and
\(T_\psi(A_p^{\rm mult},(A_p^{\rm mult})^{4/5})
\ge-\kappa(A_p^{\rm mult})^{11/10}\).
For this route its support may be confined to the proved cofinal window
sources; that favorable estimate on them is still unpaid. Alternatively
one owes a fixed positive normalized lower margin for the complete
\(w(z)(T_\psi+S_Q)-\varepsilon\) on cofinal proved partners.
FW19 would transport a supplied fixed favorable partner coefficient with
strict slack to the arriving original source; it supplies no such sign.

The existing E1–E8 last-label error budgets \(9/A\) and \(13/A\),
their already proved convergence, and the complete compensation are
unchanged. In particular the corrected E7 identity is reused:
\[
w(A)T_\psi=I_\psi(A)-I_\psi(B)
-(\psi(A)-A)[\lambda(A)-\lambda(B)].
\]
Its necessary comparison and the compensation do not make FW14's
negative local integral positive. No favorable finite nonzero
same-family weighted Lambda/tent average or positive localized
Tauberian estimate is obtained. Neither cofinal \(D>0\) or \(Z>N\),
nor the balanced-left placement \(z-z^{4/5}\ge A\), is supplied.
When a tent extends left of \(A\), its whole occupied crossing sum
remains; FW18 uses the valid forward interval instead.

All analytic starts here remain unknown; the source's separate
conditional finite interval through \(8\cdot10^{46}\) cannot pay them.
The literal sources, endpoint costs and full Lambda sign have not been
replaced by relaxed cores or different integers. The deductions above
are ordinary supplier-relative mathematics and carry no priority claim.
The full signed target
\[
\forall n\in\mathbb N,\quad n>5040\ \Longrightarrow\
I_\psi(\log n)+R(\log n)+d_{\log n}(n)>0
\]
remains **ACTIVE_UNPROVED**.
