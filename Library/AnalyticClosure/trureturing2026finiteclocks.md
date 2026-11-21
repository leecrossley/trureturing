---
bibkey: trureturing2026finiteclocks
authors: trureturing research
year: 2026
title: Finite clock bounds
doi: null
url: https://github.com/the-omega-institute/trureturing/blob/727e10f660466a6dc69ea491c8f334969b9c9d87/Library/ArithSums/nicolas2025comparison.md#project-supplement-a-uniform-selected-source-interval-through-403e46
claim: Project calculations on the extremal envelopes studied in the Nicolas comparison note, under the hypotheses given in each section.
strata_touched: []
license: citation-only
triage: anchor
---

# Finite clock bounds

These sections continue the project’s calculations on Nicolas’s comparison of the two extremal envelopes. [Source and section index](../ArithSums/nicolas2025comparison.md)

## Project supplement: a uniform selected-source interval through 4.03e46

This is a project derivation from the named premises below, extending
(GL4) on one additional interval. The interval choice and rational
enclosures are project calculations, not results attributed to Nicolas's
manuscript or the other cited papers. This is a conditional ordinary
proof and application, without a literature-priority, Lean-certification,
or all-integer finite-verification claim.

### Keep the selected integer, exact clock and source premises

Suppose Robin's strict inequality fails at some integer above 5040.
By the [Caveney–Nicolas–Sondow reduction](../Arith/caveney2012sacaga.md#which-potentially-critical-robin-source-is-covered),
Theorems 4(ii) and 5(iii), select the **same least global maximizer**
$N>5040$ of $G(n)=\sigma(n)/(n\log\log n)$. Put

$$
A=\log N,\qquad L=\log A,\qquad T=\sqrt A L,\qquad
W(n)=\log\frac{\sigma(n)}n,\qquad \lambda=\frac1{AL}.
$$

The selected level is at least $e^\gamma$, so
$\Delta(N)=\gamma+\log L-W(N)\le0$. This $N$ is not the least
counterexample. Reuse the finite ladder ending in (GL4), with its
[Axler finite-stop premise](../notes/axler2023robin.md) and its cited
zero-free and density inputs, to obtain $A>(7/2)10^{46}$.

For comparison, at an arbitrary integer $n>5040$ use its own
$A=\log n$, $L=\log A$ and $\lambda=1/(AL)$, and define
$\Delta(n)=\gamma+\log L-W(n)$. Here primes and positive powers
are used in $P_{\rm pp}$, and the pressure maximum is over integers:

$$
\begin{aligned}
M(\lambda)&=\max_{m\in\mathbb Z_{\ge1}}\{W(m)-\lambda\log m\},&
d_n&=M(\lambda)-W(n)+\lambda A\ge0,\\
P_{\rm pp}(A)&=\sum_{p^j\le A}\frac1{jp^j},&
R(A)&=P_{\rm pp}(A)-\lambda\psi(A)-M(\lambda),\\
I_\psi(A)&=\int_A^\infty(\psi(t)-t)
                  \frac{1+\log t}{t^2\log^2t}\,dt.
\end{aligned}
$$

The existing pressure and tail identities give
$\Delta(n)=I_\psi(A)+R(A)+d_n$; $d_n$ remains in this all-integer
identity. At the selected $N$ alone, the
[same-source transport](../Analytic/polak2026finiterobinca.md#application-at-the-same-critical-source-and-clock)
gives $d_N=0$ and $R(A)=D^*(A)$, hence (G1). Its premises are explicit:
CNS Fact 1 and GA2 make $N$ proper, so $N/p\ge4>e$ for deletion;
[Mantovanelli's archived direct bridge](../Analytic/mantovanelli2026primeworkload.md#the-existing-prime-local-bridge)
at the exact price $\lambda$ gives the event-free CA optimizer;
the existing unrestricted-exponent
[SevenSmooth exclusion](../../Blueprint/D5/S3/Arith/Robin/SevenSmooth.md)
rules out support index $k\le4$; and
[Kalyabin's Theorem 2 endpoint conditions](../Analytic/kalyabin2026maximalgronwall.md)
give $P=P^+(N)<A<P^+$ and exponent one at $P$.
Thus primes $p\le A$ are exactly the actual support, every actual
exponent attains Polak's full-support minimum over $a\ge1$, and his
Proposition 6 has $z(N,A)=B_2(N,A)=0$. There is no transfer of this
zero defect to arbitrary integers.

Reuse (G6)–(G7), including Nicolas's effective Theorem 1.3 branch
$6.78$, whose exact $N^{(0)}$ threshold is paid above. The primorial
cutoff $x$, support endpoint $P$ and clock $A$ stay distinct: (G2)–(G5)
pay the absent-prime suffix by GA2 and use $\Sigma(N)=Z(N)$ from CA;
they do not assume common maximizers of $\Phi$ and $\Sigma$.

The analytic inputs are the full classical explicit formula and its
endpoint-inclusive Stieltjes identities, [Dusart v1](https://arxiv.org/pdf/1002.0442v1)
Theorem 5.2 and Proposition 3.2,
[Platt–Trudgian's verification through height $3000175332800$](https://arxiv.org/abs/2004.09765v1),
and the Hasanalizade–Shen–Wong full zero count used in
[(F3) and (Z4) of the Polak note](../Analytic/polak2026finiterobinca.md#reusing-the-complete-residual-envelope).
Keep $H=3\cdot10^{12}$, $c_0=2+\gamma-\log(4\pi)<0.05$ and
$S_2(H)=\sum_{\Im\rho>H}m_\rho/(\Im\rho)^2<1.48\cdot10^{-12}$.
The preceding project derivations (GE1)–(GE4), (GH1), (GJ1)–(GJ2)
and (GK1)–(GK6) are used with exactly these premises.
The cited finite Robin and zero-verification computations, analytic
proofs and density-table computations are not rerun here. The
Mantovanelli, Kalyabin, Polak and Nicolas inputs retain their stated
preprint/archive status; no complete independent primary-proof audit
or fresh SevenSmooth compilation is asserted. Polak's separate huge
finite sweep is not a premise of the added interval.

### Uniform arithmetic and Gamma enclosures

Assume, for contradiction, that the same selected clock satisfies

$$
\frac72\,10^{46}<A\le\frac{403}{100}\,10^{46},\qquad
\alpha=\frac{73}{50}\,10^{23}+\frac12
       =\frac{292000000000000000000001}{2}.
\tag{GM1}
$$

Use the whole law $C\sim\operatorname{Gamma}(\text{shape }\alpha,
\text{rate }\alpha)$, not scale $\alpha$. Its mean is one,
$\mathbb E(C-1)^2=1/\alpha$ and
$M_1=\mathbb EC^{-1}=\alpha/(\alpha-1)$. The shape is noninteger
and at least $4$, as required in (GK6). With the complete coefficient
$F_A(s)=s^{-1}\int_A^\infty u^{s-2}(1+\log u)/\log^2u\,du$, put

$$
H_\alpha(s)=\frac{\Gamma(\alpha+s-1)}
 {\Gamma(\alpha)\alpha^{s-1}},\qquad
Z_\alpha(A)=\sum_\rho m_\rho H_\alpha(\rho)F_A(\rho).
$$

Every actual nontrivial zero, both ordinate signs and all multiplicities
are included. The preceding absolute-convergence arguments justify this
sum; conjugate pairing makes it real. Criticality is used only for
$|\Im\rho|\le H$; the tail retains every actual $0<\Re\rho<1$.

On the **whole** interval (GM1),

$$
L>107,\qquad 10^{23}<\sqrt A<r:=\frac{251}{125}\,10^{23},\qquad
M_1<\frac{10001}{10000},\qquad
\frac{H^2}{2(\alpha+H)}>\frac{1541}{50}.
\tag{GM2}
$$

Indeed, $\log10>2.3$ and $\log(7/2)>1.25$ give $L>107$;
$r^2=4.032064\cdot10^{46}>4.03\cdot10^{46}$.
The moment and damping bounds are direct rational comparisons at
the fixed $\alpha$, with no sampling of $A$.

Dusart's stronger Theorem 5.2 row is exactly
$k=2$, $\eta_k=0.01$, $x_k=7713133853$. It applies to **every**
$t\ge A$ in (GM1). Proposition 3.2 includes all higher prime powers,
so the decreasing right side gives

$$
\begin{aligned}
\eta_0(A)&:=\sup_{t\ge A}\frac{|\psi(t)-t|}{t}\\
&\le\frac{0.01}{L^2}+1.00007A^{-1/2}+1.78A^{-2/3}\\
&<\frac{0.01}{107^2}+\frac{1.00007}{10^{23}}
                  +\frac{1.78}{10^{30}}<10^{-6}.
\end{aligned}
\tag{GM3}
$$

This stronger constant is used with its own effective threshold;
it is not assigned to the earlier $3.965$ row.

The directed (GK6) and the absolute (GJ2) now give

$$
\begin{aligned}
-T I_\psi(A)\le{}&T Z_\alpha(A)
 +(0.52+2\eta_0(A))\frac{\sqrt A}{\alpha}
 +400\sqrt A e^{-\alpha/60000}+\frac{5M_1}{\sqrt A},\\
T|Z_\alpha(A)|<{}&M_1(1+1/L)
 \left[1.054c_0+2(1.0001)\sqrt A S_2(H)
            e^{-H^2/[2(\alpha+H)]}\right].
\end{aligned}
$$

Centering in (GK6) occurs before splitting the whole Gamma law at
$[0.99,1.01]$. Its regular part uses (GM3) for all $t\ge A$;
its local residual is nonpositive against the positive prime-power
measure, including endpoint atoms. The $c<1$ local part below $A$
uses this sign, not an unprovided prime-error bound below $A$.
All outside scales are paid by (GK5). In particular, $cA<1$ and the
finite endpoint response in (GE3) are retained; (GE4) is used only
as a directed upper bound, not an absolute bound.

For $x>0$, $e^x>\sum_{j=0}^{149}x^j/j!$. Exact rational evaluation
at $x=1541/50$ gives $e^{1541/50}>(121/50)10^{13}$.
Also $\alpha/60000>10^{18}$ and $e^x>x^3/6$ give
$e^{\alpha/60000}>10^{53}$. Substituting these and (GM2)–(GM3)
gives the following complete rational allowances:

| Contribution | Rational upper allowance | Strict outward bound |
|---|---:|---:|
| Verified head with full coefficient remainder | $(10001/10000)(108/107)(1.054)(0.05)$ | $0.0532$ |
| All heights above $H$, both signs | $2(10001/10000)^2(108/107)r(1.48\cdot10^{-12})/[(121/50)10^{13}]$ | $0.0248$ |
| Centered regular and signed local payment | $(0.520002)r/\alpha$ | $0.7152$ |
| Every outside Gamma scale | $400r/10^{53}$ | $9\cdot10^{-28}$ |
| Complete elementary/trivial response, including $cA<1$ | $5(10001/10000)/10^{23}$ | $6\cdot10^{-23}$ |

For clarity, the first three rational allowances are respectively
$142304229/2675000000$,
$25079915230749/1011484375000000$, and
$208832803200000000000000/292000000000000000000001$.
Summing the rational allowances, or their strict outward bounds, yields

$$
\boxed{-T I_\psi(A)<0.79321\quad\text{throughout (GM1)}.}
\tag{GM4}
$$

The damping exponent $t^2/[2(\alpha+t)]$ increases for $t>0$;
the full $S_2(H)$ therefore pays every height above $H$ through infinity.
No tail real part is moved to $1/2$, and no sign or coefficient remainder
is omitted in passing from $T Z_\alpha$ to its absolute upper allowance.

### Transcendental enclosures and the strict core

All decimal constants here denote exact terminating rationals. The
load-bearing logarithms can be enclosed by the convergent positive
series, with $z=(y-1)/(y+1)$ and $1\le y\le2$,

$$
q_m(y)=2\sum_{j=0}^{m-1}\frac{z^{2j+1}}{2j+1},\qquad
0\le\log y-q_m(y)
\le\frac{2z^{2m+1}}{(2m+1)(1-z^2)}.
$$

This follows by integrating the geometric series for $1/(1-z^2)$;
each omitted denominator is at least $2m+1$.
Write any rational $y\ge1$ as $2^k v$, $1\le v<2$, and add
the brackets for $v$ and $k\log2$. With $m=64$ the resulting rational
comparisons give $\log2<0.6931472$, $\log10>2.3$ and
$\log(7/2)>1.25$, as used above. Squaring positive rational endpoints
gives $1.4142135<\sqrt2<1.4142136$.
Positive Taylor prefixes through degree 149 give
$e^{17}>2\cdot10^7$ and $e^{52}>10^{22}$, as well as the damping
comparison used in (GM4). These are analytic enclosures with explicit
remainders or one-sided positive prefixes, not floating-point values.

For the existing core function $\mathcal E$ in (G7), differentiation
gives

$$
\mathcal E'(L)=\frac{(2+\log2)\sqrt2}{L^2}
-\frac{13.56}{L^3}+\frac{2.67}{6}e^{-L/6}
 +\left(L-2+\frac5{2L}+\frac5{L^2}\right)e^{-L/2}>0
\qquad(L\ge26).
$$

The first two terms have sum greater than $(2L-13.56)/L^3>0$;
the other terms are positive. Thus $L>107$ gives
$\mathcal E(L)>\mathcal E(107)$ uniformly. Since $107/6>17$ and
$107/2>52$, the outward enclosures just proved yield

$$
\begin{aligned}
\mathcal E(107)>{}&2(1.4142135)
 -\frac{(2+0.6931472)(1.4142136)}{107}
 +\frac{6.78}{107^2}-2.00014\\
&-\frac{2.67}{2\cdot10^7}
 -\frac{214+5/107}{10^{22}}>0.79328.
\end{aligned}
\tag{GM5}
$$

The last comparison is exact rational arithmetic. Together with (G6),
this is a whole-interval strict lower bound for the core at the same $N$.

### Contradiction and remaining boundary

By (G1), (GM4) and (GM5),

$$
\boxed{T\Delta(N)=T I_\psi(A)+T D^*(A)
 >0.79328-0.79321=\frac7{100000}>0
 \quad\text{throughout (GM1)}.}
\tag{GM6}
$$

This contradicts the selected source's $\Delta(N)\le0$.
Together with (GL4), it proves the conditional restriction
$\log N>(403/100)10^{46}$ for the same least global maximizer.
The open lower endpoint is supplied by (GL4), and the upper endpoint
is included by the uniform enclosures; there is no uncovered clock.

This excludes a selected-source interval, not every integer below
$\exp((403/100)10^{46})$, and gives no least-counterexample bound.
For arbitrary $n$ the exact $d_n$ remains. At surviving selected clocks,
the full signed requirement (G9), with its positive elementary
correction, remains unpaid. A substantive formal frontier is the
directed centered-Gamma transport (GK6), including the endpoint atoms,
whole mean-one law and $cA<1$ branch; scalar wrappers of the rational
budget do not close it. No such formal theorem is supplied here.
The RH/Robin research target remains active and unproved.

## Project application: every integer on the same finite clock interval

The existing effective reserve supplies a stronger quantifier on (GM1).
This application combines (GM4) with
[FIB §§249–250, especially (250.6)](../../docs/develop/theory/FIBONACCI_ATOMIC_RELATION_GENERATION.md#250-无穷远锚定将有效导数预算变为点值间隔).
It is a conditional ordinary derivation from those project sources,
without a new numerical endpoint, literature-priority claim or Lean
certification. Keep the unrestricted pressure over **all** positive
integers, including one, and the actual $R(A)$ and $d_n$ defined above.

Let $n$ be **any integer** such that

$$
\frac72\,10^{46}<A=\log n\le\frac{403}{100}\,10^{46},\qquad
L=\log A,\qquad T=\sqrt A L.
\tag{GAI1}
$$

Retain the classical prime-power pressure and tail identities and all
the analytic suppliers used in (GE1)–(GE4), (GH1), (GJ1)–(GJ2) and
(GK1)–(GK6), with the explicit Dusart inputs, finite zero criticality
through $H=3\cdot10^{12}$, $c_0<0.05$ and the complete
$S_2(H)<1.48\cdot10^{-12}$ enclosure. These are the same full Gamma,
centering, dilation, convergence and actual-zero-multiset premises
stated above. The reserve also uses Dusart v1 Theorem 5.2's precise row
$(k,\eta_k,x_k)=(2,1/5,3594641)$ from FIB §249.
The source proofs and computations remain named external or
project-level analytic inputs; their complete primary verification is
not supplied by this application.

### The signed estimate does not require source selection

Although (GM1) was first introduced inside a selected-source
contradiction, its analytic estimate (GM4) holds for every real $A$
in that interval. Indeed, (GM2) is uniform arithmetic; the stronger
Dusart row $(2,0.01,7713133853)$ and Proposition 3.2 give (GM3)
for every $t\ge A$. The centered directed comparison (GK6), including
the endpoint atoms and all outside Gamma scales, and the complete
zero-response bound (GJ2) therefore give the displayed five allowances
for each such $A$. Their sum is strictly less than $0.79321$.
Neither comparison uses a CA optimizer, CNS selection, properness,
$d_n=0$ or (GM5). All actual zeros above $H$ retain their real parts,
both ordinate signs and multiplicities. Consequently

$$
-T I_\psi(A)<\frac{79321}{100000}
\quad\text{for every real }A\text{ in (GAI1)}.
\tag{GAI2}
$$

The open lower endpoint and included upper endpoint are exactly those
of (GM1); no extension below or above them has been made.

### The effective actual reserve pays this same clock

FIB (250.6) applies to the same unrestricted $R(x)$ for every
$x\ge e^{100}$. Its numerical start comes from the explicit Dusart
row and the event-safe derivative comparison in §249. The boundary
condition at infinity is paid by §93.2's finite reserve bound
$0\le R(x)\le5x^{-2/3}+2/x+1/[2(\sqrt x-1)]\to0$.
It does not require an unspecified start for the asymptotic reserve
expansion, or the sign of the common tail that cancels in (250.1).
At $x=A$, (GM2) gives $L>107>100$, hence

$$
T R(A)>2(\sqrt2-1)
 -\frac{2(\sqrt2-1)+\sqrt2\log2}{L}
 +\frac{L}{(L+2)^3}.
\tag{GAI3}
$$

The bracket being subtracted is positive. Thus replacing $L>107$
by $107$ gives a valid lower bound. Use the strict rational enclosures

$$
\rho_-:=\frac{2828427}{2000000}<\sqrt2
 <\rho_+:=\frac{1767767}{1250000},\qquad
\log2<\ell_+:=\frac{2166085}{3125000}.
$$

The root inequalities follow by exact squaring; the logarithm bound
follows by the positive series
$\log2=2\sum_{j\ge0}(1/3)^{2j+1}/(2j+1)$ with its explicit
geometric remainder. Taking the lower root in the positive term and
the upper root and logarithm in the subtracted bracket yields

$$
\begin{aligned}
T R(A)&>Q+\frac{L}{(L+2)^3},\\
Q&:=2(\rho_--1)
 -\frac{2(\rho_+-1)+\rho_+\ell_+}{107}
 =\frac{67838284064811}{83593750000000}
 >\frac{8115}{10000}.
\end{aligned}
\tag{GAI4}
$$

This preserves the additional positive barrier term. No equality
case at $L=107$ or asymptotic numerical start is being assumed.

### Retain the defect for every integer

Use the exact identity $\Delta(n)=I_\psi(A)+R(A)+d_n$ at this
integer's own clock. Since $T>0$ and $d_n\ge0$, (GAI2) and (GAI4) give

$$
\begin{aligned}
T\Delta(n)
&>\frac{1530885627311}{83593750000000}
  +\frac{L}{(L+2)^3}+T d_n\\
&>\frac{1829}{100000}+T d_n>0.
\end{aligned}
\tag{GAI5}
$$

Thus Robin's strict inequality holds for every integer in (GAI1),
under the stated analytic premises. The defect has not been set to
zero or transferred from a selected source. The known small-clock
case $n=5041$, where $I_\psi(\log5041)+R(\log5041)<-1/200$,
lies outside this interval and still requires its actual defect.

The CNS reduction, properness, exact-price CA bridge, SevenSmooth
exclusion, Kalyabin endpoint conditions, Nicolas's effective $6.78$
branch and absent-prime ladder are not premises of (GAI5).
They remain premises of the earlier argument selecting the least
global maximizer and placing its clock above $(7/2)10^{46}$.
That delivered conditional lower bound, ultimately
$\log N>(403/100)10^{46}$, retains its scope. This application proves
neither a least-counterexample bound nor an all-integer verification
below the interval; Polak's separate huge finite sweep is not used.
The full signed all-integer target beyond this finite interval, its
formal analytic suppliers and RH remain unproved.

## Project application: a seven-eighths ceiling lowers the actual-sample cut

The original full coefficient (M1), estimate (H5) and
“A smaller moving cut from joint density and zero-free support” can be
consumed on the actual first-prime event samples. With the additional
seven-eighths ceiling recorded in the
[OpenAI source interface](../Analytic/openai2026quasirh.md), this gives a
smaller complete remainder at the detector's sample-moment scale. It is a
conditional ordinary application of existing sources, with no new
zero-free theorem or Lean certification.

The extra premise is precisely

$$
\beta\le\frac78\quad\text{for every actual nontrivial zeta zero}.
\tag{ASC1}
$$

Equality remains allowed. The pinned upstream declaration is
[`OAI.riemannZeta_ne_zero_of_seven_eighths_lt_re`](https://github.com/openai/math/blob/adc7f1241b42e322a6451854ab7e4b4c146bf78a/lean/OAI/NumberTheory/DirichletL/Nonvanishing.lean).
Its conclusion is used as an external analytic input; its complete
transitive proof closure has not been compiled or independently certified
here. Project Lean 4.33.0 and upstream Lean 4.34.1 remain distinct. The
stronger conditional completed-probe ceiling in the linked project note
is not used.

### Every event retains its own clock and complete response

Let $\mathcal P_X$ consist of the first-prime events $p$ with
$X\le b_p<3X$, using the largest inclusive optimizer $C_{b_p}$.
Put $A_p=\log C_{b_p}$, $L=\log X$ and $T(x)=\sqrt x\log x$.
The original full-layer and PNT suppliers, as used in the
[event-state construction](../Analytic/mantovanelli2026primeworkload.md),
give, for sufficiently large $X$,

$$
A_p\in[X/2,4X],\qquad m=|\mathcal P_X|\ll X/L.
\tag{ASC2}
$$

All higher and simultaneous layers remain in $C_{b_p}$; $A_p$ is not
identified with the event price $b_p$. Keep the original complete formula
$U_p=-T(A_p)I_\psi(A_p)$ and its elementary correction $r_{A_p}$.
For $H=X^{3/10}$ use the exact split

$$
U_p=V_p(H)+e_p(H),\quad
V_p(H)=T(A_p)\sum_{|\gamma|\le H}m_\rho F_{A_p}(\rho)+r_{A_p},\quad
e_p(H)=T(A_p)\sum_{|\gamma|>H}m_\rho F_{A_p}(\rho).
\tag{ASC3}
$$

These sums range over distinct actual zeros with multiplicity $m_\rho$
exactly once. Both ordinate signs and all actual real parts are retained.
Every zero exactly at $H$ stays in the head. The full pole and trivial-zero
correction stays in $r_{A_p}$.

### Consume the existing density layer at its new endpoint

For $5/8\le\sigma\le7/8$, reuse the existing
Chourasiya–Simonič density supplier with
$d(\sigma)=3(1-\sigma)/(2-\sigma)$. Its inclusive count and exclusive
suffix give

$$
\sum_{\gamma>H,\,\beta\ge\sigma}\frac{m_\rho}{\gamma^2}
\ll H^{d(\sigma)-2}(\log H)^3,
\quad H\ge3\cdot10^{12}.
$$

Under (ASC1), the original layer decomposition, including the full-count
base layer, therefore gives, uniformly for $x\in[X/2,4X]$,

$$
\sum_{|\gamma|>H}\frac{m_\rho x^{\beta-1/2}}{\gamma^2}
\ll \frac{x^{1/8}\log H}{H}
+\log x(\log H)^3\int_{5/8}^{7/8}
 x^{\sigma-1/2}H^{d(\sigma)-2}\,d\sigma.
\tag{ASC4}
$$

Set $f(\sigma)=(\sigma-1/2)\log x+(d(\sigma)-2)\log H$.
Since $d'(\sigma)=-3/(2-\sigma)^2$, $H=X^{3/10}$ gives
$f'(\sigma)\ge(13/45)L+O(1)$ throughout this interval.
For sufficiently large $X$ it is at least $(13/90)L$.
The integral in (ASC4) is thus at most
$90e^{f(7/8)}/(13L)$. Here $d(7/8)=1/3$, so
$e^{f(7/8)}\ll X^{3/8}H^{-5/3}=X^{-1/8}$.
This cancels the displayed outer logarithm. The original complete
coefficient bound (H5), with its remainder retained, yields

$$
|e_p(H)|\ll X^{-7/40}L+X^{-1/8}L^3
\quad\text{for every actual sample }p\in\mathcal P_X.
\tag{ASC5}
$$

### The full sample remainder pays the detector scale

Using (ASC2) and $(a+b)^2\le2a^2+2b^2$ gives

$$
\sum_{p\in\mathcal P_X}|e_p(H)|^2
\ll X^{13/20}L+X^{3/4}L^5
=o\!\left(Q(X)\right),\qquad
Q(X)=\frac{X^{3/4}e^{L^{1/4}/2}}{L^2}.
\tag{ASC6}
$$

Indeed, the quotient is bounded by
$O(X^{-1/10}L^3e^{-L^{1/4}/2}+L^7e^{-L^{1/4}/2})\to0$.
For this exact split, the $1$-Lipschitz map $z\mapsto(z-1/2)_+$ gives

$$
\left|\|(U_p-1/2)_+\|_2-\|(V_p(H)-1/2)_+\|_2\right|
\le\|e(H)\|_2=o(\sqrt{Q(X)}).
\tag{ASC7}
$$

Thus all head-tail cross effects are paid at the norm level, without
decorrelation. Also $\#\{p:|e_p(H)|>\eta\}=o(Q(X))$ for each fixed
$\eta>0$. The new cut is smaller than $X^{5/16}$ by the factor
$X^{-1/80}\to0$, under the additional premise (ASC1).

The complete signed head and a sufficient one-sided actual-sample
occupancy or positive-excess bound remain unpaid. The original signed
Landau suffix (J4) is retained; its stated errors alone do not furnish
this sample-square estimate at $H=X^{3/10}$.
No growing event-dependent selector is inserted into a fixed-parameter
OpenAI correlation theorem. No numerical common starting $X$, transfer
of the $4.03\cdot10^{46}$ global-maximizer bound, least-counterexample
bound, full Robin/RH proof, or official acceptance is supplied.

## Project application: the same actual reserve extends the clock to 4.23

The global complete-response estimates (GK6) and (GJ2), together with
the actual effective reserve (GAI3)–(GAI4), extend the all-integer
interval (GAI1). This is a conditional ordinary application of the same
project sources, without a new zero computation, external zero ceiling,
numerical reserve-asymptotic start or Lean certification.

Let $n$ be any integer with its own clock

$$
\frac72\,10^{46}<A=\log n\le\frac{423}{100}\,10^{46},
\qquad L=\log A,\qquad T=\sqrt A L.
\tag{GAJ1}
$$

Retain all the analytic premises of the preceding effective-reserve
application: unrestricted pressure and tail identities, the full
classical explicit formula, endpoint-inclusive Stieltjes conventions,
convergence and PNT inputs, the complete Gamma product and whole-law
moments, and all elementary responses, including scales with $cA<1$.
The exact Dusart v1 Theorem 5.2 rows remain
$(2,0.01,7713133853)$ for the global error and
$(2,1/5,3594641)$ for the reserve, with Proposition 3.2's full
higher-prime-power correction and the coarse $k=0$ bound.
Keep criticality through $H=3\cdot10^{12}$, the positive reciprocal
identity $c_0<0.05$ and the complete $S_2(H)<1.48\cdot10^{-12}$.
The actual reserve remains the unrestricted one over all positive
integers, including one, from FIB §§249–250 and its finite §93.2
anchor. These source proofs and computations remain named analytic
premises; their complete primary certification is not supplied here.

### Evaluate the global formulas at the larger endpoint

Keep the identical noninteger shape and rate

$$
\alpha=\frac{292000000000000000000001}{2},\qquad
C\sim\operatorname{Gamma}(\text{shape }\alpha,\text{rate }\alpha).
$$

Set $r=(2057/1000)10^{23}$. Exact squaring gives
$r^2=4.231249\cdot10^{46}>4.23\cdot10^{46}$, so
$\sqrt A<r$ even at the included upper endpoint of (GAJ1).
The lower endpoint still gives $L>107$ and $\sqrt A>10^{23}$.
Thus the global domain $A\ge e^{78}$, noninteger $\alpha\ge4$ of
(GK6), and $L>78$ of the full-coefficient (GJ2), both apply.
The interval subsequently used to illustrate (GJ2) does not restrict
its global proof. In particular, the old interval estimate (GM4) is
not being extrapolated.

The unchanged shape, height and lower endpoint retain

$$
M_1<\frac{10001}{10000},\qquad
\frac{H^2}{2(\alpha+H)}>\frac{1541}{50},\qquad
\eta_0(A)<10^{-6}.
$$

Here (GM3)'s proof uses the stronger Dusart row for every $t\ge A$
and only the lower clock endpoint; it therefore remains uniform on
(GAJ1). Reuse the positive exponential-series enclosures
$e^{1541/50}>(121/50)10^{13}$ and
$e^{\alpha/60000}>10^{53}$. Inserting these into the actual global
formulas gives the complete five allowances:

| Contribution | Exact rational upper allowance |
|---|---:|
| Verified head, full coefficient | $(10001/10000)(108/107)(1.054)(0.05)$ |
| All tail heights, both signs | $2(10001/10000)^2(108/107)r(1.48\cdot10^{-12})/[(121/50)10^{13}]$ |
| Centered regular and signed local payment | $(0.520002)r/\alpha$ |
| Every outside Gamma scale | $400r/10^{53}$ |
| Full elementary response, including $cA<1$ | $5(10001/10000)/10^{23}$ |

Every terminating decimal denotes an exact rational. Let $U_{423}$
be their sum. All actual tail-zero real parts, multiplicities, heights
and ordinate signs remain, as do the coefficient remainder, endpoint
atoms and centering before the whole Gamma law is split. Consequently

$$
-T I_\psi(A)<U_{423}\quad\text{throughout (GAJ1)}.
\tag{GAJ2}
$$

### Pay the same integer with its actual reserve and defect

The unchanged (GAI4), anchored by the finite reserve bound and valid
for $L>107$, gives

$$
T R(A)>Q_R+\frac{L}{(L+2)^3},\qquad
Q_R=\frac{67838284064811}{83593750000000}.
$$

Exact subtraction of the complete five-row sum yields

$$
Q_R-U_{423}
=\frac{22837901643254399996290102708491463199999986623442401}
 {78110000000000000000000267500000000000000000000000000000}
>\frac1{4000}.
\tag{GAJ3}
$$

Use the same-clock identity
$\Delta(n)=I_\psi(A)+R(A)+d_A(n)$, with its actual
$d_A(n)\ge0$. Equations (GAJ2)–(GAJ3) therefore give

$$
\boxed{T\Delta(n)>\frac1{4000}
 +\frac{L}{(L+2)^3}+T d_A(n)>0}
\quad\text{for every integer in (GAJ1)}.
\tag{GAJ4}
$$

No CA selection, zero-defect transfer or finite sweep is needed for
this interval consequence. Under the additional unchanged original
source-selection and lower-clock chain that gives
$\log N>4.03\cdot10^{46}$ for the same least global maximizer of
$G(n)=\sigma(n)/(n\log\log n)$ over $n>5040$ under Robin failure,
(GAJ4) excludes its remaining interval up to $4.23\cdot10^{46}$.
Thus that same conditional selected restriction improves to

$$
\log N>4.23\cdot10^{46}.
\tag{GAJ5}
$$

The CNS/properness, exact-price CA, SevenSmooth, Kalyabin eligible
endpoint, Axler finite-stop, Nicolas $6.78$ and original lower-clock
ladder premises retain their original role in that preceding chain.
This is not a least-counterexample bound or all-integer verification
below the interval. The unbounded signed Robin/RH target remains unproved. This application
supplies no new Lean/kernel or complete formal analytic verification.

## Project application: bounded log-uniform smoothing reaches 7.2

This project derivation combines the original complete Robin response and
its deterministic centered kernels with a finite positive law built from
the existing uniform/sinc library. It extends the same all-integer clock
interval while preserving the actual unrestricted FIB reserve and each
integer's defect. It is a conditional ordinary proof, with the primary
analytic suppliers retained below; no Lean/kernel or full RH proof is
claimed. This supplement is project work, not an additional result
attributed to Nicolas's manuscript.

In this section **NC** denotes the preceding material in this source,
**FIB** denotes `docs/develop/theory/FIBONACCI_ATOMIC_RELATION_GENERATION.md`,
and **PK** denotes `Library/Analytic/polak2026finiterobinca.md`. The
original sources and cited Fourier declarations used for this derivation
were read at project revision
`7f52221f2e23da81475058d5b5b6620e68709401`; the present supplement
reuses their definitions and conventions.

### 1. Exact theorem and premises

Write `g` for Euler's constant, to distinguish it from zero ordinates. Put

\[
 A_-=\tfrac72 10^{46},\quad A_+=\tfrac{36}{5}10^{46},\quad
 H=3\cdot10^{12},\quad k=23,\quad a=\frac5{2H}=\frac1{1200000000000}.
\]

For every real \(A_-<A\le A_+\), put \(L=\log A\), \(T=\sqrt A L\).
Under the premises below the complete signed integral satisfies

\[
 -T I_\psi(A)<U<Q_R-\frac3{1000},\qquad
 Q_R=\frac{67838284064811}{83593750000000}.
\tag{GAK1}
\]

For **each** integer \(n\) whose own clock \(A=\log n\) lies in that
interval, at its own price \(\lambda=1/(AL)\),

\[
 T\left[g+\log L-\log\frac{\sigma(n)}n\right]
 >\frac3{1000}+\frac{L}{(L+2)^3}+T d_A(n)>0.
\tag{GAK2}
\]

The required primary analytic inputs remain conditional in this conditional derivation:

1. The classical zeta explicit formula, in its endpoint-inclusive
   Stieltjes/half-value convention, and the integration and limiting
   conventions used in NC (GR5)–(GR8). Its constant term is \(-\log(2\pi)\)
   and its trivial-zero term is \(-\tfrac12\log(1-x^{-2})\). The exponential
   integral has the horizontal-from-left-infinity convention described in
   NC's Akatsuka Proposition 4.4 application. No lateral \(i\pi\) is added.
2. Effective unconditional PNT/Mertens convergence supplying the exact
   tail identity and an absolute constant \(C_\psi\) with
   \(|\psi(x)-x|\le C_\psi x/\log^2(2+x)\) for all \(x>0\), as in NC (GR3).
   These are logarithmic-error inputs, not a square-root error or an
   inferred short-interval theorem.
3. The actual nontrivial zero multiset \(\rho=\beta+i\gamma\),
   \(0<\beta<1\), with multiplicities \(m_\rho\), conjugation symmetry,
   the classical convergent zero count and identity
   \(\sum_\rho m_\rho/[\rho(1-\rho)]=c_0=2+g-\log(4\pi)<1/20\).
4. Platt–Trudgian's finite verification (through height 3000175332800)
   supplying \(\beta=1/2\) only for \(|\gamma|\le H\), and the full positive-
   ordinate bound
   \(S_2(H)=\sum_{\gamma>H}m_\rho/\gamma^2<1.48\cdot10^{-12}\).
   PK (F3), (Z4) identify the Hasanalizade–Shen–Wong zero-count supplier.
   Neither computation nor the complete primary proof is rerun here.
5. Dusart arXiv:1002.0442v1, Theorem 5.2, the exact rows
   \((2,0.01,7713133853)\) and \((2,1/5,3594641)\), and Proposition 3.2
   \(0\le\psi(t)-\vartheta(t)<1.00007\sqrt t+1.78t^{1/3}\).
   The classical Chebyshev estimate \(\vartheta(y)\le2y\) is also used;
   NC supplies it from the same source's \(k=0\) row. Finite computations
   underlying these sources remain external premises.

The complete coefficient bounds and the deterministic transport below are
derived, rather than assumed as law-general versions of Gamma results.
The reserve's numerical start and infinity anchor are also traced and
derived below. The all-integer theorem needs no CA, CNS, properness,
SevenSmooth, Kalyabin, Axler finite Robin stop or Nicolas effective
envelope premise. Those are extra conditions solely for the final
same-global-maximizer corollary in section 10.

### 2. Construct the entire positive law and compute exact moments

Use the finite product probability space of \(k\) copies of the uniform
law on \([-a,a]\). Let \(U_j\) be its coordinate variables, let
\(Y=\sum_{j=1}^k U_j\), and write

\[
 S(z)=\begin{cases}\sinh z/z&z\ne0,\\1&z=0,\end{cases}\quad
 d=k\log S(a),\quad C=e^{Y-d}.
\]

The original project uniform interval density is nonnegative, integrable
and of integral one. Its transform convention is
\(\int f(x)e^{izx}\,dx\). The existing theorem
`InfiniteSincProduct.uniformIntervalFourierLaplace_eq_complexSinc`
at frequency \(-iz\) gives

\[
 \mathbb E e^{zU_j}=\operatorname{complexSinc}(-iaz)=S(az).
\]

Alternatively the integral is \((2a)^{-1}\int_{-a}^a e^{zx}dx\), with
the removable value at \(z=0\). For each complex \(z\), its absolute
value is bounded on the finite product domain. Finite-product Fubini
and independence therefore give \(\mathbb E e^{zY}=S(az)^k\).
There is no infinite-product limit in this construction.

For \(C^z=e^{z\log C}\), with the real logarithm of \(C>0\),

\[
 H_C(s):=\mathbb E C^{s-1}
 =S(a(s-1))^k e^{-(s-1)d}.
\tag{GAK3}
\]

Every complex moment exists, and this is an entire function. In particular

\[
 \mathbb EC=1,\quad \mathbb EC^{-1}=S(a)^{2k},\quad
 \operatorname{Var} C=\mathbb E(C-1)^2
 =\frac{S(2a)^k}{S(a)^{2k}}-1=(a\coth a)^k-1.
\tag{GAK4}
\]

The last equality uses \(S(2a)=S(a)\cosh a\). The mean is exactly one
on the **whole** law, before any restriction to scales.

Let \(x=a^2\in(0,1)\). Positive series give

\[
 1\le S(a)=\sum_{n\ge0}\frac{x^n}{(2n+1)!}\le\frac1{1-x}.
\]

The coefficients in

\[
 \cosh a-S(a)=\frac{a\cosh a-\sinh a}{a}
 =\sum_{n\ge1}\frac{2n}{(2n+1)!}x^n
\]

start at \(1/3\). The ratio of coefficient \(n+1\) to coefficient
\(n\) is exactly \(1/[2n(2n+3)]\le1/10\). Thus all coefficients
are at most \(1/3\), and division by \(S(a)\ge1\) gives

\[
 0\le a\coth a-1\le\frac{x}{3(1-x)}=:b.
\]

For a nonnegative number \(b\) with \(kb<1\),
\((1+b)^k=\sum_{j=0}^k\binom kj b^j\le\sum_{j\ge0}(kb)^j\),
since \(\binom kj\le k^j\). Consequently

\[
 \operatorname{Var}C\le V_*:=\frac{kx}{3-(k+3)x},\qquad
 \mathbb EC^{-1}\le (1-x)^{-2k}\le M_*:=\frac1{1-2kx}.
\tag{GAK5}
\]

The inverse bound follows from \((1-x)^{2k}\ge1-2kx>0\), so
reciprocals have the displayed direction. All denominators are positive.

Furthermore \(0\le d\le kx/(1-x)\), because
\(-\log(1-x)=\log(1+x/(1-x))\le x/(1-x)\). Every point in the
support obeys

\[
 |\log C|\le\epsilon:=ka+\frac{kx}{1-x}<\frac1{1000}.
\]

The elementary inequalities \(e^{-\epsilon}\ge1-\epsilon\) and
\(e^\epsilon\le(1-\epsilon)^{-1}\), the latter by positive series,
give the stronger exact rational comparisons

\[
 \frac{99}{100}<1-\epsilon\le C\le\frac1{1-\epsilon}<\frac{101}{100}.
\tag{GAK6}
\]

These are support bounds, not high-probability bounds. No outside-law
event exists; in particular \(CA>1\) on the entire interval.

### 3. All-frequency sine bound and actual complex normalization

For all real \(v\) with \(|v|\ge5/2\),

\[
 \frac{|\sin v|}{|v|}\le\frac14.
\tag{GAK7}
\]

To prove it on \([5/2,\pi]\), \(\sin v/v\) is decreasing on
\((0,\pi)\): the numerator \(v\cos v-\sin v\) of its derivative
vanishes at zero and has derivative \(-v\sin v<0\). At \(5/2\),
the sine Taylor prefix through degree nine is
\(P_9=\sum_{j=0}^4(-1)^j(5/2)^{2j+1}/(2j+1)!<5/8\).
The omitted alternating tail starts negative and its terms decrease:
already the ratio from degree nine to degree eleven is
\((5/2)^2/(10\cdot11)<1\), and later ratios are smaller. This
justifies the upper bound even though the very first Taylor terms need
not decrease. On \([\pi,4]\),
\(|\sin v|\le v-\pi<v-3\le v/4\), by the derivative bound
\(|\cos v|\le1\), \(\pi>3\), and \(v\le4\). For \(v\ge4\)
use \(|\sin v|\le1\). Reflection proves the negative axis. The
classical \(3<\pi<4\) fixes these adjoining bands.

Now take the **actual** \(u=\beta-1\in(-1,0)\) and \(|\gamma|\ge H\).
The identity

\[
 |\sinh(a(u+i\gamma))|^2=\sinh^2(au)+\sin^2(a\gamma)
\]

and \(|a(u+i\gamma)|\ge|a\gamma|\ge5/2\) imply

\[
 |S(a(u+i\gamma))|
 \le\frac14+\frac25\sinh a
 \le\frac14+\frac25\frac{a}{1-x}.
\]

Here \(\sqrt{b^2+c^2}\le|b|+|c|\), \(|u|<1\), and the positive
hyperbolic series were used. The normalization is retained:
\(e^{-ud/k}=S(a)^{-u}\le S(a)\le(1-x)^{-1}\). Therefore (GAK3) gives

\[
 |H_C(\beta+i\gamma)|\le q_*^k<q^k,\quad
 q_*:=\frac{1/4+(2/5)a/(1-x)}{1-x}<q:=\frac{2501}{10000}.
\tag{GAK8}
\]

This is uniform for **all** \(0<\beta<1\) and every ordinate in the
tail, both signs. It does not substitute \(u=-1/2\).
For every zero, including the head, let \(\theta=1-\beta\in(0,1)\).
Positivity and concavity of \(t^\theta\) give

\[
 |H_C(\rho)|\le\mathbb EC^{-\theta}
 \le(\mathbb EC^{-1})^\theta\le M_*.
\tag{GAK9}
\]

This bound needs no head criticality. Criticality will be used separately
only to bound the head coefficient.

### 4. Consume the original complete coefficient and deterministic dilations

Retain

\[
 D(t)=\psi(t)-t,\quad k_0(t)=\frac{1+\log t}{t^2\log^2t},\quad
 w(t)=\frac{1+\log t}{\log^2t},\quad
 F_A(s)=\frac1s\int_A^\infty t^{s-2}w(t)dt.
\tag{GAK10}
\]

Thus \(F_A=A^{s-1}/(sL)-\operatorname{Ei}((s-1)L)\) in the source
convention. No replacement by just its leading term is made. For
\(h(t)=tw'(t)=-(\log t+2)/\log^3t\), two integrations by parts give
NC (H1), independently:

\[
 F_A(s)=\frac{w(A)A^{s-1}}{s(1-s)}
 +\frac{h(A)A^{s-1}+\int_A^\infty t^{s-1}h'(t)dt}{s(1-s)^2}.
\tag{GAK11}
\]

All boundary terms at infinity vanish for \(0<\Re s<1\),
\(h'(t)=2(\log t+3)/(t\log^4t)>0\), and
\(\int_A^\infty h'(t)dt=-h(A)\). The numerator of the second term
is consequently at most \(2|h(A)|A^{\beta-1}\) in modulus. This yields
the complete NC (GJ1) estimate

\[
 T|F_A(\beta+i\gamma)|
 \le(1+1/L)\frac{A^{\beta-1/2}}{|\rho||1-\rho|}
 \left(1+\frac{2(L+2)}{L(L+1)|1-\rho|}\right).
\tag{GAK12}
\]

NC (H5) is a compatible derived \(\gamma^{-2}\) leading-plus-error
envelope; it need not be assumed instead of (GAK11). For finite endpoints
\(R\ge A\), integration by parts using \(w'\le0\) gives

\[
 |F_{A,R}(s)|\le\frac{2w(A)A^{\beta-1}}{|s||1-s|}.
\tag{GAK13}
\]

This is NC (U2), uniform in \(R\), with the complete finite coefficient.
For \(|\gamma|\ge4\), it is at most \(2w(A)/\gamma^2\).

For a deterministic \(c>0\), define exactly the NC (GR5)–(GR7) objects

\[
 J_c(A)=-\frac1c\int_A^\infty D(cu)k_0(u)du,\quad
 Z_c(A)=\sum_\rho m_\rho c^{\rho-1}F_A(\rho),\quad r_c=J_c-Z_c.
\tag{GAK14}
\]

On our whole support, \(c\ge.99\) and \(cA>1\). The PNT premise
gives a constant independent of \(c\) with
\(|D(cu)|/c\le K u/\log^2u\) for \(u\ge A\). This follows directly
from \(\log(2+cu)\ge\log u+\log(.99)\ge\tfrac12\log u\).
After multiplication by \(k_0(u)\), the majorant is a constant times
\(1/[u\log^3u]\), which is integrable. Hence absolute Fubini proves
\(J_\mu:=\mathbb EJ_C\) exists and may be averaged inside its integral.

The entire **integrated coefficient** series can also be averaged
absolutely. Indeed (GAK13) bounds its high part uniformly by
\(2w(A)\gamma^{-2}\), since
\(c^{\beta-1}A^{\beta-1}=(cA)^{\beta-1}\le1\). The finitely many
lower zeros are uniformly bounded on the compact scale support. The
zero count supplies summability. Thus

\[
 Z_\mu:=\mathbb EZ_C
 =\sum_\rho m_\rho H_C(\rho)F_A(\rho),\quad
 J_\mu=Z_\mu+r_\mu,\quad r_\mu=\mathbb Er_C.
\tag{GAK15}
\]

This absolute exchange is for the integrated \(F_A\) series. It is
**not** an absolute interchange of the unsmoothed \(x^\rho/\rho\)
explicit-formula series with an infinite integral. For (GAK14)'s explicit
formula, take the source's finite-endpoint/truncated formula first,
then its integrated convergence and (GAK13); the uniform summable bound
pays the scale-endpoint limit, exactly as in GR7. The half-value change
at prime powers affects no Lebesgue integral. This analytic limiting
input remains one of the named premises in section 1.

Substitution \(x=cu\) in the full explicit formula gives the exact
elementary response for \(cA\ge1\):

\[
 r_c(A)=\frac{\log(2\pi)}{cAL}
 +\frac12\int_{cA}^\infty\log(1-x^{-2})
       \frac{1+\log(x/c)}{x^2\log^2(x/c)}dx.
\tag{GAK16}
\]

The second term is nonpositive and integrable. In fact our support has
\(cA\gg1\), so there is no logarithmic endpoint singularity; the
source also treats the integrable endpoint \(cA=1\). Since
\(\log(2\pi)<2\), this gives

\[
 T r_\mu\le\frac{2\mathbb EC^{-1}}{\sqrt A}
 \le\frac{5M_*}{\sqrt A}.
\tag{GAK17}
\]

The last relaxed allowance agrees with the candidate. It is directed,
not an absolute bound. The full pole/constant and trivial-zero terms
have been retained in (GAK16). NC (GE2) proves the bound for all \(c>0\),
including its separate \(cA<1\) branch using \(D(x)=-x\), GR6 and U2;
our law assigns that branch zero probability by (GAK6). GR8's unquantified
absolute constant is not used for the numerical budget.

Conjugation of actual zeros and (GAK3), (GAK10) shows \(Z_\mu\) is real.
The signed equality at \(c=1\) is \(J_1=-I_\psi(A)\), including its
original full elementary correction. The transport next compares this
entire \(J_1\) with \(J_\mu\); one must not drop or separately
double-count \(r_1\).

### 5. Derive law-centered transport, preserving all atoms

Set

\[
 h_A(t)=\frac1{\max(A,t)\log\max(A,t)},\quad
 w_c(t)=c^{-1}h_A(t/c),\quad
 a_A(t)=\begin{cases}-1/(AL)&0<t\le A,\\1/(t\log^2t)&t>A.\end{cases}
\]

NC (GP4)'s deterministic estimates give
\(\int|w_c-h_A|(d\psi+dt)\le K(c+c^{-1})/L\). For completeness,
below \(A\max(1,c)\) bound the two weights by their constants and
use \(\psi(t)\ll t\); above that point their absolute difference is

\[
 \frac{|\log c|}{t\log t\log(t/c)}
 \le\frac{|\log c|(1+|\log c|/L)}{t\log^2t}.
\]

Partial summation with \(\psi(t)\ll t\) makes the latter summable.
The constants are uniform on \([.99,1.01]\). Also
\(\int a_A dt=0\), and \(\int|a_A|(d\psi+dt)<\infty\).
Changing variables in finite integrals shows
\(\int(w_c-h_A)dt=0\); its upper endpoint difference is
\(\log\log(R/c)-\log\log R\to0\).

Integration by parts, with the PNT boundary at infinity and \(D(t)=-t\)
below 1, gives the deterministic GP5 identity

\[
 J_1-J_c=\int(w_c-h_A)d\psi=\int(w_c-h_A)dD.
\]

Only absolutely convergent differences are used. Define
\(B_c=w_c-h_A-(c-1)a_A\). Absolute Fubini and the exact **whole-law**
mean \(\mathbb E(C-1)=0\) give

\[
 J_1-J_\mu=\mathbb E\int B_C(t)dD(t).
\tag{GAK18}
\]

This is the law-general version of NC (GS6), derived before splitting.
It requires no Gamma identity.

For \(.99\le c\le1.01\), let \(e=c-1\), and split \(B_c=b_c+v_c\):

\[
 b_c(t)=\begin{cases}
 e^2/(cAL),&0<t\le A,\\
 [t(\log t-\log c)]^{-1}-(t\log t)^{-1}-e/(t\log^2t),&t>A.
 \end{cases}
\tag{GAK19}
\]

For \(t>A\), let \(v=\log t\), \(r=v-\log c\). The second
dilation derivative of \(1/[t(v-\log c)]\) and its \(t\)-derivative are

\[
 \frac{2-r}{tc^2r^3},\qquad \frac{r^2-6}{t^2c^2r^4}.
\]

Throughout the segment from 1 to \(c\), \(c\ge.99\),
\(r\ge v-.01\ge.999v\), and \(r>2\), \(r^2>6\), since
\(L>107>78\). Their moduli are at most
\(1.024/(t v^2)\) and \(1.024/(t^2v^2)\), respectively.
Taylor's integral remainder, whose weight integrates to \(e^2/2\),
therefore proves the deterministic GK2 bounds

\[
 |b_c(t)|\le\frac{.512e^2}{t\log^2t},\qquad
 |b'_c(t)|\le\frac{.512e^2}{t^2\log^2t}.
\]

Use the actual right-continuous \(D(A)\), including its atom. Partial
summation with the change of formula at \(A\) gives

\[
 \int b_c dD=
 [e^2/(cAL)-b_c(A+)]D(A)-\int_A^\infty D(t)b'_c(t)dt.
\]

The upper boundary vanishes. With
\(\eta_0(A)=\sup_{t\ge A}|D(t)|/t\), the three contributions give

\[
 \left|\int b_c dD\right|
 \le\frac{\eta_0(A)e^2}{L}
 [100/99+.512+.512/L]\le\frac{2\eta_0(A)e^2}{L}.
\tag{GAK20}
\]

Only values \(t\ge A\) of the global error were used. The contribution
below \(A\) is the constant part integrated exactly to \(D(A)\).

The residual \(v_c\) vanishes off the cutoff interval. Its exact values
are those of \(B_c-b_c\), not an arbitrary almost-everywhere version:

* For \(c>1\), on \(A<t<cA\) it equals
  \(1/(cAL)-1/[t\log(t/c)]\), and \(v_c(A)=v_c(cA)=0\).
* For \(c<1\), on \(cA<t\le A\) it equals
  \(1/[t\log(t/c)]-1/(cAL)\), and \(v_c(cA)=0\).
* For \(c=1\), it is zero everywhere.

The function \(1/[t\log(t/c)]\) decreases throughout these intervals,
so \(v_c\le0\), including its actual endpoint values. Thus the
nonnegative atomic measure \(d\psi\) gives

\[
 \int v_c dD=\int v_c d\psi-\int v_cdt\le-\int v_cdt.
\]

This retains an atom at \(A\) for \(c<1\) with its nonpositive sign;
an atom at \(cA\) has zero coefficient. For \(c>1\), the possibly
discontinuous right limit at \(A\) does not change the actual atom
value zero. There is no replacement of \(d\psi\) by a density.

On the whole cutoff interval \(t\ge.99A\),
\(\log(t/c)\ge L-.01\). Hence

\[
 \left|\frac{d}{dt}\frac1{t\log(t/c)}\right|
 \le\frac{1.034}{A^2L}.
\]

The worst ratio is bounded at \(L=78\) by
\(.99^{-2}[78/(78-.01)][1+1/(78-.01)]<1.034\); both logarithmic
factors decrease with \(L\). Since \(v_c(cA)=0\), a triangular
Lebesgue-area bound proves the deterministic GK4 inequality

\[
 \int v_c dD\le\frac{1.034(A|e|)^2}{2A^2L}<\frac{.52 e^2}{L}
\tag{GAK21}
\]

when \(e\ne0\); the non-strict form holds also at zero.
NC (GS9)'s bounded variation ensures the local integrals exist, but
its short-interval error bound is not used. In particular no error
estimate below \(A\) is needed to pay the \(c<1\) residual.

Averaging (GAK20)–(GAK21) in (GAK18), using the entire support and (GAK4), yields

\[
 T(J_1-J_\mu)\le(.52+2\eta_0(A))\sqrt A\operatorname{Var}C.
\tag{GAK22}
\]

There is no outside-scale cost and no conditional mean. We have thus
rederived the necessary GK3/GK4 averaging; NC's Gamma-specific GK1 or
GK6 is not an assumption. Combining (GAK15), (GAK17), (GAK22), and \(J_1=-I_\psi\),

\[
 -T I_\psi(A)\le T|Z_\mu(A)|
 +(.52+2\eta_0(A))\sqrt A V_*+\frac{5M_*}{\sqrt A}.
\tag{GAK23}
\]

### 6. Pay the entire actual zero spectrum and full remainder

For every zero,

\[
 \Re\frac1{\rho(1-\rho)}
 =\frac{\gamma^2+\beta(1-\beta)}{|\rho(1-\rho)|^2}>0.
\]

On the verified head it is the positive real weight
\(1/(\gamma^2+1/4)\). The classical identity for \(c_0\) therefore
bounds the head sum of absolute weights by \(c_0\); its tail cannot
cancel a positive head contribution. On the unverified tail,
\(|\rho||1-\rho|\ge\gamma^2\), so the complete tail weight is at
most \(2S_2(H)\). The factor two counts the negative ordinates by
conjugation with the same multiplicities, rather than creating another
zero population.

For \(L>78\), (GAK12)'s full remainder factor on the head is below 1.054,
since \(|1-\rho|\ge1/2\) and
\(4(L+2)/(L(L+1))\le4\cdot80/(78\cdot79)<.054\).
On the tail \(|1-\rho|\ge|\gamma|>H\), so the factor is below 1.0001.
The rational function \((L+2)/(L(L+1))\) decreases for positive \(L\).
Equations (GAK8), (GAK9), (GAK12) thus give, for the **complete** series,

\[
 T|Z_\mu(A)|<(1+1/L)
 [1.054 M_*c_0+2(1.0001)\sqrt A S_2(H)q^{23}].
\tag{GAK24}
\]

The head uses \(A^{\beta-1/2}=1\). Only there is criticality assumed.
The tail retains its actual \(\beta\), before the valid upper bound
\(A^{\beta-1/2}\le\sqrt A\). Its \(q^{23}\) already includes the
actual-real-part normalization, so no additional \(M_*\) factor is
required in that tail term. All heights through infinity are included.
This derives the replacement for the Gamma damping in GJ2; neither
GJ2 nor a Gamma moment law is invoked.

### 7. Uniform rational budget for every real clock

Use exact integer fractions throughout. For
transcendental enclosures use, for \(1\le y\le2\) and
\(z=(y-1)/(y+1)\),

\[
 q_m(y)=2\sum_{j=0}^{m-1}\frac{z^{2j+1}}{2j+1},\quad
 0\le\log y-q_m(y)
 \le\frac{2z^{2m+1}}{(2m+1)(1-z^2)}.
\tag{GAK25}
\]

This follows by integrating the geometric series for \((1-z^2)^{-1}\)
and bounding every omitted denominator by \(2m+1\). Divide a rational
\(y\ge1\) by powers of two to reach \([1,2)\), and add its multiple
of the enclosure for \(\log2\). At \(m=64\), the exact fractions give
\(\log10>2.3\) and \(\log(7/2)>1.25\). Thus on the **whole** interval,

\[
 L>46(2.3)+1.25=107.05>107,\quad \sqrt A>10^{23},\quad
 A^{2/3}>10^{30}.
\]

The stronger Dusart row applies to **every** \(t\ge A\), because even
the lower endpoint exceeds 7713133853. Proposition 3.2 and the decreasing
error functions give, independently of the upper endpoint,

\[
 \eta_0(A)\le\frac{.01}{L^2}+1.00007A^{-1/2}+1.78A^{-2/3}
 <\frac{.01}{107^2}+\frac{1.00007}{10^{23}}+
   \frac{1.78}{10^{30}}<10^{-6}.
\tag{GAK26}
\]

This is NC (GM3)'s lower-clock argument, not a restriction to its old
Gamma upper endpoint. Set \(r=(671/250)10^{23}=2.684\cdot10^{23}\).
Its square is \(7.203856\cdot10^{46}>A_+\). Hence
\(\sqrt A<r\) even at the included upper endpoint.

Define the following exact positive rational numbers:

\[
\begin{split}
 U_h&=\frac{108}{107}\frac{527}{500}\frac1{20}M_*,\\
 U_t&=2\frac{108}{107}\frac{10001}{10000}r
                \frac{37}{25\cdot10^{12}}\left(\frac{2501}{10000}\right)^{23},\\
 U_v&=\frac{260001}{500000}rV_*,\qquad
 U_e=\frac{5M_*}{10^{23}},\qquad U=U_h+U_t+U_v+U_e.
\end{split}
\tag{GAK27}
\]

Each replacement in (GAK23)–(GAK24) increases a positive allowance. All bounds
are uniform for real \(A\), not values sampled at endpoints. Exact rational substitution proves

\[
 U_h<.053193,\quad U_t<.011502,\quad U_v<.743074,\quad U_e<6\cdot10^{-23},
\]

and, using the full fractions rather than these rounded displays,

\[
 .003755<Q_R-U<.003756,
 \qquad Q_R-U>\frac3{1000}.
\tag{GAK28}
\]

The displayed allowances are exact rational definitions, so the final
comparison is an integer cross-multiplication. Positive-series enclosures
justify the logarithmic constants before this subtraction; they do not
certify the primary analytic suppliers.

### 8. Reuse the same effective unrestricted reserve

Use exactly the unrestricted pressure, including the integer one,
\[
 M(\lambda)=\max_{m\ge1}[\log(\sigma(m)/m)-\lambda\log m],
 \qquad R(x)=P_{\rm pp}(x)-\frac{\psi(x)}{x\log x}
              -M(1/(x\log x)).
\tag{GAK29}
\]
FIB §§87/98/111 provide the finite prime-prefix maximization, all ties,
and the nonnegative reserve. Its finite §93.2 bound and (250.3) give
\[
 0\le R(x)\le5x^{-2/3}+2/x+1/[2(\sqrt x-1)]\longrightarrow0.
\]
The event-safe argument in FIB §§249–250, already consumed in NC
(GAI3)–(GAI4), uses the exact Dusart reserve row
$(2,1/5,3594641)$, higher reference layers, paired left/right states,
and this zero-at-infinity anchor. Its explicit start is $x\ge e^{100}$;
it does not differentiate a reserve asymptotic or transfer the finite
Robin value at 5040. Reuse its complete conclusion (250.6):
\[
 R(x)>\frac{c_R+c_2/\log x}{\sqrt x\log x}
             +\frac1{\sqrt x(\log x+2)^3},
 \quad c_R=2(\sqrt2-1),\quad
 c_2=-2(\sqrt2-1)-\sqrt2\log2.
\tag{GAK36}
\]
At the present $x=A$, $L>107$ pays that start. Exact squaring and
(GAK25)'s positive log series certify
\[
 \rho_-=2828427/2000000<\sqrt2<\rho_+=1767767/1250000,
 \qquad \log2<\ell_+=2166085/3125000.
\]
Use the lower root in the positive term and upper root/logarithm in
the subtracted term, and then $L>107$. Thus the same actual reserve gives
\[
 TR(A)>Q_R+\frac{L}{(L+2)^3},\qquad
 Q_R=2(\rho_--1)-\frac{2(\rho_+-1)+\rho_+\ell_+}{107}
 =\frac{67838284064811}{83593750000000}.
\tag{GAK37}
\]
This is reuse of the paid lower-clock reserve, with its original full
assumptions and event conventions, rather than a new reserve theorem.

### 9. Keep each integer's actual defect

The PNT/Mertens tail identity, FIB 87.3 and NC's full-response formula,
is

\[
 I_\psi(A)=g+\log L-\frac1L-P_{\rm pp}(A)+\lambda\psi(A).
\tag{GAK38}
\]

It also follows by differentiating this continuous finite expression:
its derivative is \(-D(A)k_0(A)\), its prime-power jumps cancel,
and its limit is zero by the named PNT/Mertens input.
Define the actual nonnegative price defect

\[
 d_A(n)=M(\lambda)-W(n)+\lambda\log n\ge0.
\]

For \(A=\log n\), adding (GAK29), (GAK38) and this defect, with
\(\lambda A=1/L\), proves exactly

\[
 \Delta(n):=g+\log L-W(n)=I_\psi(A)+R(A)+d_A(n).
\tag{GAK39}
\]

The pressure and \(R(A)\) have not been replaced by a different
optimizer or a restricted maximum. Equations (GAK23)–(GAK28), (GAK37), (GAK39)
prove (GAK2), for every integer in the stated interval, including its
upper endpoint. Since \(T>0\), \(\Delta(n)>0\) is precisely
\(\sigma(n)<e^g n\log\log n\). No defect was set to zero, including
for a non-CA integer. There is no inference for every smaller integer
or for an unbounded clock interval.

### 10. Same least global maximizer corollary and remaining boundaries

For this separate corollary retain **all** original selection and
lower-clock suppliers, as spelled out in NC's section beginning at
line 6743 and its earlier G1–G9, GH/GL finite ladder:

* Under a Robin violation, CNS Theorems 4(ii), 5(iii) select the same
  least integer \(N>5040\) attaining the **global maximum** of
  \(G(n)=\sigma(n)/(n\log\log n)\), at level at least \(e^g\).
* CNS Fact 1 and GA2 give properness and \(N/p\ge4>e\) for deletion.
  Mantovanelli's archived direct tangent bridge supplies regular CA
  optimality at the exact price \(1/(A\log A)\). A support-based
  CA-family price is not substituted.
* The unrestricted-exponent SevenSmooth exclusion removes support
  index at most four. Kalyabin's stated endpoint hypotheses then give
  \(P=P^+(N)<A=\log N<P^+\), with exponent one at \(P\).
  This fixes the actual full-support minimization, \(d_A(N)=0\), and
  its core identity. None of these zero-defect statements are moved to
  arbitrary integers.
* Axler's cited finite stop through the \(K\)th primorial,
  \(K=999999476056\), supplies the initial clock. The exact Nicolas
  \(N^{(0)}\) threshold is paid by
  \(\log N^{(0)}<66(1000000007)<K/2<A\), so the effective
  6.78 branch is retained. GA2 pays the absent-prime suffix while
  keeping the primorial cutoff, support endpoint and clock distinct.
* The original Nicolas/Dusart core and finite signed-response ladder,
  including the original finite-height, density and zero-free suppliers
  where used, puts this **same** selected \(A\) above
  \((7/2)10^{46}\). Their source proofs, finite computations and
  preprint/archive statuses are unchanged conditional suppliers.

If that same \(N\) also had \(A\le7.2\cdot10^{46}\), (GAK2) would give
\(\Delta(N)>0\), contradicting its global counterexample level.
Therefore, with this complete unchanged extra chain,
\(\log N>7.2\cdot10^{46}\). This is **not** a least-counterexample
bound. The new all-integer interval argument itself does not require
this extra chain, and does not independently audit all its primary proofs.

For fixed \(a,k\), \(V_*>0\) and \(q^k>0\). Both the transport
and unverified-tail allowances grow with \(\sqrt A\). Thus the
fixed-law construction gives no unbounded signed Robin estimate,
full RH proof or official acceptance.

### 11. Library reuse and actual missing formal content

The immutable project toolchain is 4.33.0; its manifest pins Mathlib to
`db584cd6d46c92f209a44c0f1c829460d327499d`. Source inspection was of
the original three entire Lean modules, the related DyadicComplexDecay
module, and their complete Blueprints,
not their runtime evidence. The Blueprints' existing machine-check
claims are source descriptions, not new certifications by this derivation.

The reusable project declarations are:

* `InfiniteSincProduct.uniformIntervalDensity`, its nonnegativity,
  integrability and integral-one facts, and
  `uniformIntervalFourierLaplace_eq_complexSinc`, for the one-factor
  complex identity at frequency \(-iz\).
* `DyadicConvolutionDensity.dyadic_partial_convolution_fourierLaplace`
  and its tilt/convolution proof pattern, with actual nonnegativity,
  mass-one and compact-support results. The public finite theorem
  specifically uses dyadic widths and \(n+1\) factors; it is not already
  the 23 equal-width law. Its finite induction/Fubini machinery can be
  reused or factored through a general finite-width bridge. One must
  not silently instantiate equal widths in a dyadic-only signature.
* `DyadicTransformDecay.sinc_product_decay_bound` and
  `dyadic_density_transform_decay` concern the infinite dyadic density
  on **real frequencies**. They provide the existing finite-prefix
  norm argument and real sinc bounds, but do not directly prove the
  normalized finite-law bound for all actual \(\beta-1+i\gamma\).
* The related `DyadicComplexDecay.dyadic_transform_explicit_strip_decay`
  already proves explicit inverse-power decay for the infinite dyadic
  density at all complex frequencies. Its proof supplies the existing
  uniform-factor exponential/inverse bounds and the normalized-prefix
  argument. That general dyadic strip theorem should also be reused;
  its signature and constants do not themselves give the equal-width,
  mean-one law's sharper normalized factor \(.2501\) above \(H\).

Neither infinite dyadic nonvanishing nor all-order real decay is needed
as a premise of the present finite law. Do not duplicate these existing
uniform/sinc facts, or introduce an independent complex-sinc definition.

The genuinely missing consumed formal bridge comprises the finite
equal-width law and its pushforward by \(e^{Y}/S(a)^{23}\), its exact
whole-law centering and moments, the normalized complex-strip tail
bound, and the endpoint-inclusive deterministic centered transport
with absolute Fubini for the **full** \(F_A\) series and exact elementary
response. The unrestricted-pressure identity, event-safe reserve
start/infinity anchor, actual per-integer defect and conditional primary
supplier interfaces must accompany that bridge for the complete theorem.
A scalar wrapper of (GAK28), or an unproved law-general invocation of
Gamma GK6/GJ2, would not consume those obligations.

The OpenAI/math checkout at
`adc7f1241b42e322a6451854ab7e4b4c146bf78a`, toolchain 4.34.1, is not a
premise of this derivation. Its differently pinned closure is not claimed
to have compiled against this project toolchain.

The reasoning discipline was to check the positive law, complete
deterministic response and same actual reserve before combining their
scalar budgets; to retain signed identities until a directed bound
permits absolute values; and to distinguish an ordinary conditional
deduction from independent certification of primary analytics.

## Project application: complete event cells sample the own-size clock

Keep (ASC1)–(ASC7), the actual first-prime sample $\mathcal P_X$,
its inclusive largest optimizers $N_p=C_{b_p}$ and their own clocks
$A_p=\log N_p$. The full event construction in the
[Mantovanelli interface](../Analytic/mantovanelli2026primeworkload.md#actual-sample-and-finite-support)
supplies the underlying states. The application below uses ordinary
bounded-variation endpoint quadrature; it is not a new quadrature,
zero-density or prime-distribution theorem. It is a conditional
project deduction, without Lean certification or a historical
originality claim.

Put $L=\log X$, $H=X^{3/10}$ and $J_X=[X/2,4X]$. For each fixed
$X$, keep $H$ fixed while varying $A\in J_X$, and define

$$
V_X(A)=\sqrt A\log A\sum_{|\operatorname{Im}\rho|\le H}
 m_\rho F_A(\rho)+r_A,
\qquad f_X(A)=(V_X(A)-1/2)_+^2.
\tag{OCQ1}
$$

Here $F_A$ is the complete coefficient (M1), and $r_A$ is the complete
elementary correction after (G9). All distinct actual zeros retain
their multiplicities and real parts; both ordinate signs and every
zero exactly at $H$ remain in the head. Conjugate pairing makes $V_X$
real. At each actual sample, $V_X(A_p)=V_p(H)$ from (ASC3).

### Use every activation layer in the size partition

If there are no layer events in $[X,3X)$, the selected sample sum
is zero and the inequality is immediate. Otherwise enumerate all
distinct event prices $e_1<\cdots<e_k$ in this band. Let $B_i=\log C_{e_i}$ be the post-event size after all
ties, and let $B_0$ be the size immediately before $e_1$. Local
finiteness and the complete activation rule give

$$
B_i-B_{i-1}=\sum_{\tau_{p,j}=e_i}\log p=:h_i>0.
\tag{OCQ2}
$$

Thus $B_0<\cdots<B_k$ is a partition in the actual size coordinate,
even though the prices need not be equally spaced. If $X$ itself
is an event, its whole jump belongs to the first cell. An event at
$3X$ is excluded. Higher-layer events and every tied layer stay in
this partition.

For a first-prime event at $e_i=b_p$, the existing calibration
$p<b_p<p+1$ gives $p\ge X-1\ge X/2$ eventually. Hence

$$
h_i\ge\log p\ge L-\log2.
\tag{OCQ3}
$$

First-prime event prices are strictly increasing in $p$, so at most
one selected sample uses a given cell. The $j$th layer price is also
strictly increasing in its prime, so a tied event has at most one
prime for each fixed $j$.

Reuse the activation cutoff from
[FIB Proposition 420.2](../../docs/develop/theory/FIBONACCI_ATOMIC_RELATION_GENERATION.md#420-既有大间隙链的实际素层隔离与根位置的联合缺口):
every layer at a price below $3X$ has
$p^j<Q_X=3X\log(3X)/\log2$. In particular
$j\le d_X=\lfloor\log Q_X/\log2\rfloor$. For the complete tied jump,

$$
\mu_X:=\max_i h_i
\le\log Q_X\sum_{j=1}^{d_X}\frac1j
=O(L\log L)=O(L^2).
\tag{OCQ4}
$$

The existing full-clock estimate
$\log C_b=\psi(b)+O(\sqrt b[\log(2b)]^{5/2})$ and PNT give
$\log C_b=b+o(b)$ uniformly for $b\in[X,3X]$.
Together with (OCQ4), they put $B_0$ and every $B_i$ inside $J_X$
eventually. This uses the entire optimizer clock, not just (ASC2)'s
first-prime endpoints, and makes no substitution $A_p=b_p$.

For quadrature, directly reuse S. S. Dragomir, *The Ostrowski integral
inequality for mappings of bounded variation*, *Bulletin of the
Australian Mathematical Society* **60** (1999), 495–508,
[DOI 10.1017/S0004972700036662](https://doi.org/10.1017/S0004972700036662),
Corollary 7, equations (5.16)–(5.17), printed p. 507. Its arbitrary
partition is $(B_i)_{i=0}^k$, its sample in the $i$th cell is the
right endpoint $B_i$, and its mesh is $\mu_X$. The published error
bound is mesh times total variation; for absolutely continuous $f$,
that variation is $\int|f'|$. No generic quadrature proof is repeated.

For any nonnegative absolutely continuous $f$ on $J_X$, this supplier
and (OCQ3) give

$$
\begin{aligned}
\sum_{p\in\mathcal P_X}f(A_p)
&\le\frac1{L-\log2}\sum_{i=1}^k h_i f(B_i)\\
&\le\frac1{L-\log2}\left(
 \int_{B_0}^{B_k}f(A)\,dA+
 \mu_X\int_{B_0}^{B_k}|f'(A)|\,dA\right)\\
&\le\frac1{L-\log2}\left(
 \int_{J_X}f(A)\,dA+
 \mu_X\int_{J_X}|f'(A)|\,dA\right).
\end{aligned}
\tag{OCQ5}
$$

Both enlarged integrands are nonnegative. An empty selected sample
has left side zero; if there are no events, no partition is needed.
This estimate uses no prime-gap bound, sampling independence or
separate supremum payment for higher-layer mass: those layers supply
cells in the same partition.

### The complete moving coefficient pays the mesh error

The finite head in (OCQ1) has a fixed zero set at each $X$. Differentiating
the full (M1) integral with respect to its lower endpoint gives

$$
\partial_A F_A(\rho)
=-\frac{A^{\rho-2}(1+\log A)}{\rho\log^2A}.
\tag{OCQ6}
$$

Under the named ceiling (ASC1), directly reuse the complete
coefficient bound (GH2), the finite reciprocal-square
mass $\mathcal C_\zeta$ in (GE1), and the classical zero count
$\sum_{|\gamma|\le H}m_\rho/|\rho|=O(\log^2(2H))$. They give,
uniformly on $J_X$,

$$
|V_X(A)|=O(X^{3/8}),\qquad
|V_X'(A)|=O(X^{-5/8}L^2).
\tag{OCQ7}
$$

The full elementary response remains in this differentiation.
Its exact formula after (G9) gives
$r_A=O(A^{-1/2})$ and $r_A'=O(A^{-3/2})$, including the
trivial-zero integral. These contributions fit (OCQ7).
The positive-part square is $C^1$, including at $V_X=1/2$, with
$f_X'=2(V_X-1/2)_+V_X'$. Thus

$$
\int_{J_X}|f_X'(A)|\,dA=O(X^{3/4}L^2).
\tag{OCQ8}
$$

Substituting into (OCQ5) gives the own-clock sampling interface

$$
\boxed{\sum_{p\in\mathcal P_X}(V_p(H)-1/2)_+^2
\le\frac1{L-\log2}\int_{J_X}(V_X(A)-1/2)_+^2\,dA
 +O(X^{3/4}L^3).}
\tag{OCQ9}
$$

The coarse error is sufficient: relative to (ASC6)'s unchanged
$Q(X)$, its quotient is
$O(L^5e^{-L^{1/4}/2})\to0$. No refinement of the generic quadrature
theorem or new tail calculation is needed for this rate.

### The original fixed-exponent consumer and its remaining signed input

The proposed sufficient analytic input is still

$$
\int_{J_X}(V_X(A)-1/2)_+^2\,dA=o(LQ(X)).
\tag{OCQ10}
$$

This input is required along all sufficiently large scales carrying
the original source; a bound only on an unrelated subsequence does
not supply that quantifier. It is not established by (OCQ7), the zero ceiling, finite zero
verification, PNT or quadrature. Indeed, the unsigned bound (OCQ7)
only gives $O(X^{7/4})$ for this integral, which does not pay
(OCQ10). This route still lacks a sufficient directed estimate of the same
actual zero response; no independent phase or modified arithmetic source is
introduced.

If (OCQ10) were supplied, (OCQ9) and the already paid head-tail
norm transfer (ASC7) would give

$$
\sum_{p\in\mathcal P_X}(U_p-1/2)_+^2=o(Q(X)).
\tag{OCQ11}
$$

To identify its actual-source consumer, keep the original particular
fixed $0<\eta<1/2$ and power surplus supplied by the
[Caveney persistence application](../Arith/caveney2012sacaga.md#a-wider-actual-price-interval-for-the-same-supplied-power-excess),
where that exponent is denoted $\eta'$. Reuse the actual first-prime
count (R6) in the
[Stadlmann interface](../Analytic/stadlmann2022meansquaregaps.md#the-existing-uniform-prime-count-gives-a-stronger-source-specific-count).
On every scale carrying the same selected source, there are

$$
\gg\frac{X^{1-\eta/2}e^{L^{1/4}/2}}{L}
\tag{OCQ12}
$$

samples in $\mathcal P_X$ whose same actual $N_p=C_{b_p}$ satisfies
$\log G(N_p)-\gamma>\delta X^{-\eta}$, for the fixed positive
$\delta$ in that persistence application. The original exponent is
not decreased or reselected.

The argument does not transfer the original selected integer's
event-free, own-price, zero-defect properties to these post-event
integers. Instead consume
the already preserved unrestricted integer identity

$$
\Delta(n)=I_\psi(\log n)+R(\log n)+d_n,
\qquad d_n\ge0,
\qquad \Delta(n)=\gamma-\log G(n).
\tag{OCQ13}
$$

At $n=N_p$, its own clock and the unrestricted sufficiently large
reserve $R(A_p)>0$ supplied in (GAI3)–(GAI4) give

$$
U_p=T(A_p)\bigl(\log G(N_p)-\gamma+R(A_p)+d_{N_p}\bigr)
\ge T(A_p)\bigl(\log G(N_p)-\gamma\bigr).
\tag{OCQ14}
$$

Keep $d_{N_p}$; it is not set to zero. By (ASC2), each sample in
(OCQ12) has $U_p\gg X^{1/2-\eta}L\to\infty$ and hence $U_p\ge1$
eventually. Each contributes at least $1/4$ to (OCQ11). The ratio of
the lower count (OCQ12) to $Q(X)$ is
$\gg X^{1/4-\eta/2}L\to\infty$, contradicting (OCQ11) on the
same unbounded source scales.

Thus the displayed implication retains the original fixed-exponent
source and all post-event layers. It does not obtain (OCQ10), the
original one-sided $I_\psi$ estimate or RH. Standard quadrature and
the existing persistence count supply interfaces, not the missing
continuous signed-head bound. No new generic theorem, repeated
prime-count proof, parameter optimization or numerical replay is
claimed as mathematical progress.


## Project application: actual monotone layers at a shorter successor

This is a **repo-derived ordinary derivation**, not a compiled result. Its
substantive additional estimate is the whole weighted actual second-layer
increment and its one-sided combination below (candidate M6–M7, labelled
MS6–MS7 here to distinguish the earlier Mellin formulas). The unrestricted
pressure, packet identity, first-cutoff location and second-cutoff scale are
reused. The bounded source comparison does not certify literature priority.
The prior independent ordinary audit used the same model family; it is
design evidence, not a same-round peer review, diverse-model consensus,
Pro review, official acceptance or Lean/kernel evidence.

The original project sources are pinned at
`7f52221f2e23da81475058d5b5b6620e68709401`: this note's G1–G9 and PH
pressure section; [FIB §§85, 87, 98, 111, 247.4 and 249](../../docs/develop/theory/FIBONACCI_ATOMIC_RELATION_GENERATION.md);
and [ZE/5040's unrestricted/restricted pressure Theorem 3.2, own-price
Theorem 6.1 and equation (19), and actual-cutoff Definition 7.1/Theorem 8.1](../../docs/develop/theory/ZECKENDORF_EULER_5040.md).
The [Mantovanelli workload note](../Analytic/mantovanelli2026primeworkload.md)
identifies the primary Zenodo 22014299, version 1.0.0, manuscript SHA-256
`8208445c84c6cafc971a6f2a0637b06715a783f680de80d2ed3bb4a3be503d65`:
§4 `thm:direct-bridge`, Theorem 5.2 `thm:packet-identity`, and
Proposition 7.6 `prop:moment-workload` are existing inputs. Its packet
theorem has two regular selfmatching endpoints; the arbitrary endpoint
used here requires the retained concavity correction.

### Same actual state, finite support and endpoint correction

For \(x>1\), put

\[
f(x)=\log\log x,\qquad \lambda(x)=\frac1{x\log x},\qquad
w(x)=-\lambda'(x)=\frac{\log x+1}{x^2(\log x)^2}>0.
\]

For primes \(p\) and integers \(k\ge1\), define

\[
\beta_{p,k}=\log\left(1+\frac1{p+\cdots+p^k}\right),\quad
r_{p,k}=\frac{\beta_{p,k}}{\log p},\quad
a_p(x)=\#\{k\ge1:r_{p,k}>\lambda(x)\},
\]

\[
N_x=\prod_p p^{a_p(x)},\qquad
K_k(x)=\sum_{p:r_{p,k}>\lambda(x)}\log p,\qquad
K(x)=\sum_{k\ge1}K_k(x)=\log N_x.
\]

Every equality layer is excluded. For \(1<a\le b\), the common support
including possible ties is

\[
L_b=\{(p,k):r_{p,k}\ge\lambda(b)\}.
\]

Since \(0<r_{p,k}<1/(p^k\log p)\), membership implies

\[
p^k\log p<b\log b,\qquad p<b,\qquad 2^k\log2<b\log b.
\]

Thus \(L_b\) is finite. The decreasing price makes all actual layer sets
increase: \(K_k\) and \(K\) are finite step functions on \([a,b]\), and

\[
N_a\mid N_b,\qquad
\frac{N_b}{N_a}=\prod_p p^{a_p(b)-a_p(a)}\in\mathbb N.
\]

Finite sum/integral interchange holds on the whole interval with this
common support. Simultaneous events retain each layer's full \(\log p\)
weight; activation positions are the actual ones, not reference prime
powers.

Write \(W(n)=\log(\sigma(n)/n)\), \(G(n)=(\sigma(n)/n)/(\log\log n)\),
so \(\log G(n)=W(n)-f(\log n)\) for \(n>e\). Reuse the unrestricted
finite positive-part pressure

\[
S(\lambda)=\max_{n\ge1}(W(n)-\lambda\log n),\qquad
D(x)=\gamma+f(x)-\lambda(x)x-S(\lambda(x)).
\]

On \([a,b]\), reuse the exact finite expression

\[
S(\lambda(x))=\sum_{(p,k)\in L_b}\log p\,(r_{p,k}-\lambda(x))_+.
\]

It is absolutely continuous and gives \(D'(x)=(x-K(x))w(x)\) off the
finitely many events.
At the strict optimizer, with \(Y=K(x)>1\),

\[
\log G(N_x)=\gamma-D(x)+C_x(Y),\qquad
C_x(Y)=f(x)+\lambda(x)(Y-x)-f(Y)\ge0.
\]

Fix an actual **strict stable selfmatch** \(A>2\), meaning that \(A\) is
event-free and \(K(A)=A\), and set

\[
B=A+H,\qquad H>0,\qquad X=K(B)\ge A.
\]

Concavity gives \(C_B(X)\ge0\), with equality exactly when \(X=B\).
Integrating the existing pressure derivative yields

\[
\log\frac{G(N_B)}{G(N_A)}
=\int_A^B[K(t)-t]w(t)\,dt+C_B(X). \tag{MS0}
\]

This holds even if \(B\) is an event. If all ties at \(B\) were included,
write \(J_B=\sum_{r_{p,k}=\lambda(B)}\log p\) and \(X^+=X+J_B\).
Their reward is exactly \(\lambda(B)J_B\), giving the same integral with

\[
\log G(N_B^+)-\log G(N_B)=C_B(X^+)-C_B(X).
\]

Below the endpoint is consistently the strict \(N_B\). Neither \(X=B\)
nor zero own-price defect at the different clock \(X\) is assumed.

For any real \(A>2,H>0\), put \(\rho_A(u)=w(A+u)/w(A)\), and define

\[
\begin{aligned}
T_\theta(A,H)&=\int_0^H[\theta(A+u)-\theta(A)-u]\rho_A(u)\,du,\\
U_2(A,H)&=\int_0^H[K_2(A+u)-K_2(A)]\rho_A(u)\,du,\\
U_{\ge3}(A,H)&=\int_0^H\sum_{k\ge3}[K_k(A+u)-K_k(A)]\rho_A(u)\,du,\\
E_1(A,H)&=\int_0^H[K_1(A+u)-K_1(A)-\theta(A+u)+\theta(A)]\rho_A(u)\,du.
\end{aligned}
\]

Here \(\theta(t)=\sum_{p\le t}\log p\) uses the weak prime endpoint.
Subtracting the complete initial state \(K(A)=A\) gives the exact identity

\[
\log\frac{G(N_B)}{G(N_A)}
=w(A)[T_\theta+U_2+U_{\ge3}+E_1]+C_B(X). \tag{MS1}
\]

The literal finite \(U_{\ge3}\ge0\) follows pointwise from actual layer
monotonicity. It remains in every comparison.

The existing first cutoff solves

\[
\frac{\log(1+1/q_1(x))}{\log q_1(x)}=\lambda(x),\qquad x-1<q_1(x)<x
\quad(x>2).
\]

The inequalities follow from \(\log(1+t)<t\) and

\[
\log(1+1/(x-1))>1/x,\qquad \log(x-1)<\log x.
\]

Consequently the exact first-layer endpoint correction is

\[
\delta_1(x)=\theta(x)-K_1(x)
=\sum_{q_1(x)\le p\le x}\log p,\qquad 0\le\delta_1(x)\le\log x.
\]

The closed interval has length less than one and contains at most one
integer. A prime at either \(q_1(x)\) or \(x\) is included in this
correction. Direct differentiation gives

\[
\frac{w'(x)}{w(x)}=\frac1x\left[-2-\frac2{\log x}+\frac1{\log x+1}\right]<0,
\qquad 0<\rho_A(u)\le1.
\]

The \(E_1\) integrand is \(\delta_1(A)-\delta_1(A+u)\); hence

\[
-H\log B\le E_1(A,H)\le H\log A. \tag{MS2}
\]

Its lower loss is paid; its sign is not assumed favorable.

### Actual second cutoff and the uniform prime input

Let \(q=q_2(x)>1\) be the unique solution

\[
r_2(q)=\frac{\ell(q)}{\log q}=\lambda(x),\qquad
\ell(q)=\log\left(1+\frac1{q^2+q}\right).
\]

The smooth \(r_2\) decreases strictly from infinity to zero. Exact
differentiation and ordinary expansions give

\[
\ell'(q)=-\frac{2q+1}{(q^2+q)(q^2+q+1)},\quad
\ell(q)=q^{-2}-q^{-3}+O(q^{-4}),\quad
\ell'(q)=-2q^{-3}+3q^{-4}+O(q^{-5}).
\]

Set \(a(q)=q^2\ell(q)-1=-q^{-1}+O(q^{-2})\) and

\[
b(q)=-q^3\ell'(q)-2=-3q^{-1}+O(q^{-2}),\qquad
L=\log x,\quad l=\log q.
\]

The exact implicit equation and derivative are

\[
q^2l=(1+a(q))xL,\qquad
r_2'(q)=-\frac{q^{-3}}l\left[2+b(q)+\frac{1+a(q)}l\right],
\]

\[
q_2'(x)=\frac qx\,
\frac{(1+a(q))(1+1/L)}{2+b(q)+(1+a(q))/l}.
\]

For sufficiently large \(x\), comparison at \(\sqrt x\) and \(2\sqrt x\)
first bounds \(q\) between them. Thus \(l=L/2+O(1)\), and substitution
into these exact formulas proves

\[
q_2(x)=\sqrt{2x}[1+O(1/\log x)],\qquad
q_2'(x)=\frac1{\sqrt{2x}}[1+O(1/\log x+1/q_2(x))]. \tag{MS3}
\]

The \(1/q_2(x)\) term is smaller than \(1/\log x\). This derivative
comes from the smooth actual equation, not differentiation of a
pointwise prime-count asymptotic or an \(O(1)\) cutoff error. With common
constants for large \(A\), \(0<H\le A/2\), \(0\le u\le H\), integration
of the derivative gives

\[
v(u):=q_2(A+u)-q_2(A)
=\frac u{\sqrt{2A}}
+O\left(\frac u{\sqrt A\log A}+\frac{uH}{A^{3/2}}\right). \tag{MS4}
\]

Use **Corollary 1.3**, not the almost-all Corollary 1.4, of
[Guth–Maynard, arXiv:2405.20552v2](https://arxiv.org/html/2405.20552v2)
and its §13.2 proof; the [existing GM note](../Analytic/guthmaynard2024largevalues.md)
records this primary input. For each fixed \(\epsilon>0\) with a
nonempty range there exist constants \(C_\epsilon,Y_\epsilon>0\) such
that for **every real** \(y\ge Y_\epsilon\) and every real length

\[
y^{17/30+\epsilon}\le v\le y^{99/100},\qquad
\left|\pi(y+v)-\pi(y)-\frac v{\log y}\right|
\le C_\epsilon v e^{-(\log y)^{1/4}}.
\]

No numerical \(Y_\epsilon\) is supplied. Fix

\[
\epsilon=1/60,\quad H=A^{4/5},\quad y=q_2(A),\quad
V=v(H),\quad h_0=(2\sqrt A)^{7/12}=2^{7/12}A^{7/24}.
\]

Eventually \(y\sim\sqrt{2A}\le2\sqrt A\),

\[
y^{7/12}\le h_0\le V\sim A^{3/10}/\sqrt2,
\qquad h_0,V\le y^{99/100},\qquad y\ge Y_{1/60}.
\]

Indeed \(3/10-7/24=1/120>0\) and \(3/10<99/200\). All these
requirements are paid by one common eventual, unquantified threshold.
For \(h_0\le v\le V\), write \(n(v)=\pi(y+v)-\pi(y)\). Then

\[
0\le\theta(y+v)-\theta(y)-(\log y)n(v)
\le\log(1+v/y)n(v),\qquad n(v)\le2v/\log y
\]

eventually, uniformly. Thus multiplication of the **absolute \(\pi\)
error by \(\log y\)** gives

\[
\theta(y+v)-\theta(y)
=v+O\left(v\log y\,e^{-(\log y)^{1/4}}+\frac{v^2}{y\log y}\right).
\]

For fixed constants \(C,c>0\), use

\[
\eta_A=C\left(\log A\,e^{-(c\log A)^{1/4}}+H/A\right)\longrightarrow0,
\]

since \(V/y=O(H/A)\) and \(\log y\asymp\log A\). For \(0\le v<h_0\),
apply GM only at the enclosing length \(h_0\), then monotonicity:

\[
0\le\theta(y+v)-\theta(y)\le\theta(y+h_0)-\theta(y)\le2h_0.
\]

It follows, uniformly over **the whole** \(0\le v\le V\), that

\[
\theta(y+v)-\theta(y)=v+O(\eta_Av+h_0). \tag{MS5}
\]

GM has not been extended below its lower length. To retain both strict
second-cutoff atoms, let \(e(z)=\log z\) when \(z\) is an integer prime,
and \(e(z)=0\) otherwise. The exact formula is

\[
K_2(A+u)-K_2(A)=\theta(y+v(u))-\theta(y)+e(y)-e(y+v(u)).
\]

The initial atom has a plus sign and the final atom a minus sign. Their
difference is \(O(\log A)\) uniformly, including events at \(u=0,H\).
At a stable initial source \(e(y)=0\); the supplier does not need this.

### Whole weighted increment and retained higher layers

The exact logarithmic derivative of \(w\) gives

\[
\rho_A(u)=1+O(H/A)\quad(0\le u\le H\le A/2).
\]

Combining MS4–MS5 and the two atoms, with \(v(u)\le C u/\sqrt A\),
gives throughout \([0,H]\)

\[
K_2(A+u)-K_2(A)=\frac u{\sqrt{2A}}
+O\left(\frac u{\sqrt A\log A}+\frac{uH}{A^{3/2}}
+\eta_A\frac u{\sqrt A}+h_0+\log A\right).
\]

Integrating the entire interval, including the initial short lengths,
and paying the weight variation yields

\[
U_2(A,H)=\frac{\sqrt2}{4}\frac{H^2}{\sqrt A}
+O\left(\frac{H^2}{\sqrt A\log A}+\frac{H^3}{A^{3/2}}
+\eta_A\frac{H^2}{\sqrt A}+Hh_0+H\log A\right). \tag{MS6}
\]

In particular, put \(S_A=H^2/\sqrt A=A^{11/10}\). There exist constants
\(A_0,C,c>0\) such that for **every real \(A\ge A_0\)**, with \(H=A^{4/5}\),

\[
\left|\frac{U_2(A,H)}{S_A}-\frac{\sqrt2}{4}\right|
\le C\left(\frac1{\log A}+A^{-1/5}
+\log A\,e^{-(c\log A)^{1/4}}
+A^{-1/120}+A^{-3/10}\log A\right)=:\mathcal E(A).
\]

The constants depend on the fixed GM input and the ordinary calculus
bounds, not on \(A\) or its selfmatching status; none is given a numerical
value here. The short-range cost is exactly

\[
\frac{h_0\sqrt A}{H}=2^{7/12}A^{-1/120},\qquad
\frac{\sqrt A\log A}{H}=A^{-3/10}\log A\longrightarrow0.
\]

The first-layer loss MS2 is also paid by the latter scale. After increasing
\(C\), set \(\varepsilon_*(A)=\mathcal E(A)\ge0\), tending to zero.
The same bound gives, for every such real \(A\),

\[
U_2+E_1\ge(\sqrt2/4-\varepsilon_*(A))S_A,
\]

\[
U_2+U_{\ge3}+E_1
\ge(\sqrt2/4-\varepsilon_*(A))S_A+U_{\ge3}. \tag{MS7}
\]

Equivalently, for every \(\delta>0\) there exists \(A_\delta\) such that

\[
U_2(A,A^{4/5})+E_1(A,A^{4/5})\ge(\sqrt2/4-\delta)A^{11/10}
\quad\text{for every real }A\ge A_\delta.
\]

No actual higher layer is deleted. In contrast, integrating the old
coarse difference \(Q=K-\psi\) error

\[
O(A^{1/3}(\log A)^{7/3})
\]

would cost \(O(H A^{1/3}(\log A)^{7/3})\), or

\[
O(A^{1/30}(\log A)^{7/3})
\]

relative to \(S_A\). This need not vanish. MS7 keeps the monotone actual
higher layers instead; it does not assert a shorter-interval asymptotic
for the old signed \(Q\) difference.

For each fixed \(47/60<\alpha<199/200\), the same proof works with

\[
H=A^\alpha,\qquad 0<\epsilon<2\alpha-47/30,\qquad
h_{0,\epsilon}=(2\sqrt A)^{17/30+\epsilon}.
\]

The short-range relative exponent is \(47/60+\epsilon/2-\alpha<0\),
and the upper-range ratio is \(V/y^{99/100}=O(A^{\alpha-199/200})\to0\).
This choice also ensures \(17/30+\epsilon<99/100\). All other costs
vanish; constants and thresholds depend on the fixed \(\alpha,\epsilon\).
These are sufficient exponents, with no optimality or uniform endpoint
claim. The displayed \(4/5,1/60\) choice lies strictly inside this range.

### Actual integer consumer and the unpaid prime sign

Return to \(H=A^{4/5}\), \(B=A+H\), \(X=K(B)\). At a strict stable
selfmatch \(A\ge A_0\), suppose the same \(N_A\)
satisfies GA2 against all its multiples; in particular this holds if
\(N_A>5040\) is a global maximizer of \(G\) over integers greater than \(5040\).
Since \(N_A\mid N_B\), MS1 and MS7 imply the necessary condition

\[
T_\theta(A,H)\le-(\sqrt2/4-\varepsilon_*(A))S_A
-U_{\ge3}(A,H)-\frac{C_B(X)}{w(A)}. \tag{MS8}
\]

The exact endpoint-preserving finite prime sum is

\[
w(A)T_\theta(A,H)
=\sum_{A<p\le B}\log p\,[\lambda(p)-\lambda(B)]
-[f(B)-f(A)-H\lambda(B)]. \tag{MS9}
\]

Indeed integrate the finite indicators \(\mathbf1_{p\le t}\) against

\[
w(t),\qquad \int_p^B w=\lambda(p)-\lambda(B),\qquad
\int_A^B(t-A)w(t)\,dt=f(B)-f(A)-H\lambda(B).
\]

A prime at \(A\) is excluded; one at \(B\) has zero weight. This is the
original same-state identity, not a new standalone prime theorem.

For every fixed real \(\kappa<\sqrt2/4\), there exists a common
\(A_\kappa\ge A_0\) such that \(\varepsilon_*(A)<(\sqrt2/4-\kappa)/2\) for all
\(A\ge A_\kappa\).

At any actual strict stable selfmatch above that start, the **unproved**
condition

\[
T_\theta(A,A^{4/5})\ge-\kappa S_A \tag{MSP}
\]

would give the actual strict improvement

\[
\log\frac{G(N_B)}{G(N_A)}
\ge w(A)[(\sqrt2/4-\kappa-\varepsilon_*(A))S_A+U_{\ge3}]
+C_B(X)>0.
\]

Independently, MS6 implies \(U_2>0\) eventually, so at least one new
actual second layer is present before \(B\); thus \(N_B>N_A\). The
successor is the defined integer multiple, not an unrelated scalar witness.

MSP (candidate MP) is unpaid. GM at the \(A\)-centered first-layer scale
only permits a relative error of order \(\eta_AH^2\); the required signed
loss is of order \(H^2/\sqrt A\). The factor tending to zero in GM does
not pay the missing \(A^{-1/2}\). A general-center average or rough-shift
correlation does not establish MSP at these selected centers.

The conditional selected-source statement retains the CNS and
Mantovanelli premises in the existing notes: proper GA1/GA2 and the
direct prime-local bridge give the **same** stable selfmatching integer.
For that source one still needs MSP and \(A\ge A_\kappa\). The unbounded
stable-root chain of FIB §111 is not an unbounded family of global Robin
maxima; the separate unbounded GA2 family has no automatic stable-selfmatch
premise. No unbounded covered source family is supplied here. The
historical \(7.2\cdot10^{46}\) conclusion above remains only its existing,
separately sourced conditional context; it pays neither \(Y_{1/60}\)
nor \(A_0,A_\delta,A_\kappa\). No new finite interval, least-counterexample
bound, RH proof or new unconditional formal supplier follows.

### Reuse and formalization boundary

At the original project pin, reuse
`GoldenResourceOptimalLayerCount.positive_part_sum_finite_support`,
`positive_layers_eq_count_interval`, `optimal_layer_count_spec`,
`GoldenResourceSupremum.golden_resource_supremum_eq_positive_part_sum`,
the actual sigma objective factorization and equality-layer neutrality.
The searched D5/S3/Arith/Robin public and private declarations supply
prefix, curvature and moment facts, but not the weighted short actual
second-layer estimate MS6–MS7. This is a bounded search conclusion.

Mathlib is pinned at `db584cd6d46c92f209a44c0f1c829460d327499d`:
`Chebyshev.theta`, `theta_mono`, `theta_eq_sum_primesLE`, finite sums,
sigma prime-power/multiplicativity, interval FTC, asymptotics and implicit
function APIs are reusable. The bounded pinned NumberTheory search did not find a formal GM supplier.
OpenAI/math at `adc7f1241b42e322a6451854ab7e4b4c146bf78a`,
`preprints/Ordinary-two-point-correlations-of-multiplicative-functions-September-24-2026/build/qualitative/analytic-transfer.tex`,
has rough-multiplier supremum/fourth-moment and averaged correlation
statements with different variables and quantifiers. They are not
premises of this derivation and do not prove MSP.

MS6–MS7 remain ordinary, uncompiled estimates using the cited GM
analytic input. Substantive formal adoption must connect the actual
finite layer state, implicit cutoff derivative, endpoint atoms and whole
weighted integration to MS1 and MS9, and discharge GM or explicitly
retain its short-interval hypothesis. A scalar wrapper assuming the
finished supplier would not implement the missing mathematics. No axiom,
wrapper Lean declaration, current required check or kernel acceptance is
produced here. MSP, the common start/source coverage, the analytic formal
input and the substantive formal implementation remain open; the full
RH/Robin/5040 goal remains **ACTIVE**.
