---
bibkey: trureturing2026primepressure
authors: trureturing research
year: 2026
title: Prime pressure bounds
doi: null
url: https://github.com/the-omega-institute/trureturing/blob/727e10f660466a6dc69ea491c8f334969b9c9d87/Library/ArithSums/nicolas2025comparison.md#an-observation-transport-with-a-root-scale-averaged-pressure-margin
claim: Project calculations on the extremal envelopes studied in the Nicolas comparison note, under the hypotheses given in each section.
strata_touched: []
license: citation-only
triage: anchor
---

# Prime pressure bounds

These sections continue the project’s calculations on Nicolas’s comparison of the two extremal envelopes. [Source and section index](../ArithSums/nicolas2025comparison.md)

## An observation transport with a root-scale averaged-pressure margin

The following application reuses the whole BPY law, GPC's original
response estimates, APC's absolute cutoff bounds and the same actual
reserve. It changes the clock observation by an explicit signed
Stieltjes kernel. Standard integration by parts supplies the transport;
the additional application pays its variation and infinite clock tail
and estimates the resulting actual pressure average. No literature
priority, numerical common threshold, Lean certification, pressure-order
inequality or RH/Robin proof is claimed.

### Keep the two response kernels distinct

Retain $K(x)=(1+\log x)/(x^2\log^2x)$,
$\lambda(x)=1/(x\log x)$ and ACP's
$B(x)=\gamma+\log\log x-1/\log x$ for $x\ge e$.
Their derivatives are $\lambda'=-K$ and $B'=xK$. The original response is

$$
J_c^\psi(A)=-\frac1c\int_A^\infty[\psi(cu)-cu]K(u)\,du.
$$

In general $I_\psi(Ac)\ne-J_c^\psi(A)$: scaling also changes the
logarithmic kernel. The construction below transports this observation
explicitly instead of identifying the two integrals.

The actual pressure still satisfies
$M(\lambda(x))=B(x)-I_\psi(x)-R(x)$. Directly reuse the expansion of
this same reserve in
[FIB §247.3, (247.8)](../../docs/develop/theory/FIBONACCI_ATOMIC_RELATION_GENERATION.md#2473-实际双候选储备的二项展开):

$$
R(x)=\frac{c_R}{\sqrt x\log x}
 +O\!\left(\frac1{\sqrt x\log^2x}\right),
\qquad c_R=2(\sqrt2-1)>0.
\tag{KTO1}
$$

Its existing proof uses the actual two-candidate reserve and effective
unconditional PNT. No new reserve or PNT theorem is asserted.
The existing pressure and tail identities make $R$ and $I_\psi$ bounded
on $[e,\infty)$, with both tending to zero.

### A slower source and a paid inverse-moment correction

Use $R_t$ and $\nu_j$ from GPC2. Put $L=\log A$, $T_A=\sqrt A L$ and

$$
\mathcal T=\{0,-4,-3/4,-1/4,1/4\},\qquad
\epsilon=\frac1{8(1+\max_{t\in\mathcal T}\log R_t)},\qquad
k=\max\{1,\lfloor\epsilon\log L\rfloor\}.
$$

This degree differs from APC/ACP's $\lfloor L^{1/3}\rfloor$.
It depends only on the owned clock moments. GPC2 gives, eventually,

$$
M_t(k)\le C L^{1/4}\quad(t\in\mathcal T),\qquad
\int\bigl[|\log c|+c^{-1/2}(1+|\log c|)\bigr]\,d|\nu_k|(c)
\le C L^{1/4}.
\tag{KTO2}
$$

Indeed $\epsilon\log R_t\le1/8$, and neighboring quarter moments
bound both logarithmic factors. Also $k\to\infty$ and
$k\le\kappa L$ eventually, within GPC's common response cap.

Let $\tau=e/A$, $\bar\nu=(\chi_A)_\#\nu_k$, and define

$$
\delta_A=\int c^{-1}\,d\bar\nu(c)-1,\qquad
\eta_A=\bar\nu-2\delta_A(\delta_1-\delta_2).
\tag{KTO3}
$$

Then $\eta_A$ has mass one, inverse clock moment exactly one and support
$c\ge\tau$ for large $A$. The whole small-clock estimate is
$|\delta_A|\le2\tau^3M_{-4}(k)=O(A^{-3}L^{1/4})$.
Clamping decreases the needed negative weighted logarithms; its positive
quarter-moment change is bounded by $\tau^{1/4}M_0(k)$.
Thus the selected absolute and logarithmic moments of $\eta_A$ retain
the bounds KTO2. GPC and APC's absolute cutoff estimates, followed by
the negligible two-atom correction, give

$$
T_A\left|\int J_c^\psi(A)\,d\eta_A(c)\right|\longrightarrow0.
\tag{KTO4}
$$

The fixed-clock responses at $c=1,2$ are bounded by the existing PNT
bounds; their correction cost after multiplication by $T_A$ tends to
zero. All prime powers, zero heights and infinite response tails remain.
Exact xi zeros and source jets belong to $\nu_k$; cutoff and correction
errors for $\eta_A$ are paid rather than declared zero.

### A finite-variation observation kernel

For $c\ge\tau$ and $v\ge c$ define

$$
r_A(v,c)=\frac{c^{-2}K(Av/c)}{K(Av)},\qquad a_A(c)=r_A(c,c),
$$

$$
d\kappa_{A,c}(v)=a_A(c)\delta_c(dv)
 +\mathbf1_{v>c}\,\partial_v r_A(v,c)\,dv.
\tag{KTO5}
$$

The cumulative function is zero below $c$ and $r_A(v,c)$ above it.
Every kernel argument is at least $e$. With $g(z)=(1+z)/z^2$,
$r_A(v,c)=g(\log(Av)-\log c)/g(\log(Av))$ and
$a_A(c)=g(L)/g(L+\log c)$. Since
$g'/g=1/(z+1)-2/z$ is increasing, $r_A$ decreases to one for $c>1$
and increases to one for $c<1$. Consequently $\kappa_{A,c}$ has mass one;
it is positive for $c<1$, while for $c>1$ its atom is followed by a
negative density. Its variation satisfies

$$
\|\kappa_{A,c}-\delta_c\|_{\rm TV}=2|a_A(c)-1|,
\quad |a_A(c)-1|\le\frac{2|\log c|}{L},
\quad \|\kappa_{A,c}\|_{\rm TV}\le C(1+\log_+c/L).
\tag{KTO6}
$$

The middle bound uses $g(L)\le2/L$ and the $1$-Lipschitz function
$z^2/(z+1)$ on $z\ge1$.

At a finite endpoint $V\ge c$, Stieltjes integration by parts gives
three expressions, respectively:

$$
\begin{aligned}
\int_{[c,V]}\lambda(Av)\,d\kappa_{A,c}
 &=\lambda(AV)r_A(V,c)+\frac1c\int_A^{AV/c}K(u)\,du,\\
\int_{[c,V]}B(Av)\,d\kappa_{A,c}
 &=B(AV)r_A(V,c)-B(AV/c)+B(A),\\
\int_{[c,V]}I_\psi(Av)\,d\kappa_{A,c}
 &=I_\psi(AV)r_A(V,c)
   +\frac1c\int_A^{AV/c}[\psi(cu)-cu]K(u)\,du.
\end{aligned}
$$

The price and tail boundary terms vanish as $V\to\infty$.
Moreover $r_A(V,c)-1=O_c(1/\log(AV))$, so the benchmark boundary
difference also vanishes. Including the atom in KTO5 is essential.
The resulting exact observations are

$$
\int\lambda(Av)\,d\kappa_{A,c}=\frac{\lambda(A)}c,
\qquad \int B(Av)\,d\kappa_{A,c}=B(A),
\qquad \int I_\psi(Av)\,d\kappa_{A,c}=-J_c^\psi(A).
\tag{KTO7}
$$

These integrals are absolute. Price and $I_\psi$ are bounded on
$[e,\infty)$. For $B$, its lower bound and the positive kernel for
$c<1$ control the absolute integral by a constant depending on $A$.
For $c\ge1$, the single-sign density and the benchmark calculation
bound it by $C_A[1+(\log_+c)^2]$. The moments in KTO2 make all these
bounds integrable against $|\eta_A|$.

Define the actual signed clock measure by the absolutely integrable kernel

$$
\omega_A(E)=\int\kappa_{A,c}(E)\,d\eta_A(c).
$$

It has mass one, support $v\ge\tau$ and
$\|\omega_A-\eta_A\|_{\rm TV}=O(L^{-3/4})$. Absolute kernel Fubini,
KTO3 and KTO7 prove

$$
\int\lambda(Av)\,d\omega_A=\lambda(A),\qquad
\int B(Av)\,d\omega_A=B(A),\qquad
\int I_\psi(Av)\,d\omega_A=-\int J_c^\psi(A)\,d\eta_A(c).
\tag{KTO8}
$$

Thus the actual shifted-tail average is $o(1/T_A)$ by KTO4.
Positive power moments and exact Mellin zeros are not assumed for
$\omega_A$. Its new infinite clock tail has finite variation and the
absolute observation bounds just proved.

### Transport the same actual reserve at root scale

First KTO1–KTO3 imply

$$
T_A\int R(Ac)\,d\eta_A(c)=c_RH_k(1/2)+o(1).
\tag{KTO9}
$$

For completeness, before the tiny correction the original-source integral
is $\int R(A\chi_A(c))\,d\nu_k(c)$. Split that source at
$c<A^{-1/2}$ and retain this clamped integrand on the small-clock set.
Bounded $R$ and $M_{-4}(k)$ pay its entire contribution
by $O(L^{5/4}A^{-3/2})$. On the complement, $z=\log c$ and
$L+z\ge L/2$, so KTO1 gives

$$
T_A R(Ac)=c^{-1/2}
 \left[\frac{c_RL}{L+z}+O\!\left(\frac L{(L+z)^2}\right)\right].
$$

Its difference from $c_Rc^{-1/2}$ is at most
$(C/L)c^{-1/2}(1+|\log c|)$, costing $O(L^{-3/4})$ by KTO2.
The missing reference moment is at most $A^{-7/4}M_{-4}(k)$, and
the tiny KTO3 atoms cost $o(1)$ after root normalization. This uses
the quantitative reserve remainder, not a bare $o(1)$ multiplied by
growing signed variation.

For $c\ge A^{-1/2}$, the support of $\kappa_{A,c}$ lies in $v\ge c$,
and KTO1 bounds the whole later reserve by
$C/(\sqrt{Ac}\log(Ac))$. KTO6 therefore gives

$$
T_A\left|\int R(Av)\,d\kappa_{A,c}(v)-R(Ac)\right|
\le\frac C L c^{-1/2}|\log c|.
$$

Its $|\eta_A|$ integral is $O(L^{-3/4})$. For
$\tau\le c<A^{-1/2}$ the kernel is positive of mass one; bounded $R$
and the complete small-clock mass again cost
$O(L^{5/4}A^{-3/2})$. Hence

$$
T_A\int R(Av)\,d\omega_A(v)
=c_RH_k(1/2)+o(1)\longrightarrow c_R>0.
\tag{KTO10}
$$

Here $H_k(1/2)=1-Q(h(1/2))^k\to1$ by XLR2/GPC8.
No positivity of a general signed average was used, and the kernel's
entire infinite tail remains.

### Actual pressure and the same integer's remaining defect

The observation bounds establish absolute pressure integrability through
$M=B-I_\psi-R$. Integrating this exact identity and using KTO4,
KTO8 and KTO10 yields

$$
V_A:=\int M(\lambda(Av))\,d\omega_A(v)
=B(A)-\frac{c_R}{\sqrt A\log A}
 +o\!\left(\frac1{\sqrt A\log A}\right).
\tag{KTO11}
$$

In particular $V_A<B(A)-c_R/(2T_A)$ eventually.
This is an actual averaged-pressure margin for the transported
observation; it supplies no ordering of $M(\lambda(A))$ and $V_A$.
ACP's older two-degree pressure comparison retains its own observation
and remains unchanged.

For every original integer $n$ with its own $A=\log n$, keep the
pointwise defect $d_\lambda(n)=M(\lambda)-W(n)+\lambda\log n$ and define
$D_A(n)=\int d_{\lambda(Av)}(n)\,d\omega_A(v)$.
Exact mass and price mean give $D_A(n)=V_A-W(n)+1/L$, and therefore

$$
\Delta(n)=D_A(n)+B(A)-V_A,\qquad
T_A\Delta(n)=T_AD_A(n)+c_R+o(1).
\tag{KTO12}
$$

The same original integer is used throughout. The signed average
$D_A(n)$ has no proved lower bound sufficient to settle Robin.
All prime powers occur in the complete $\psi$ response, actual reserve,
actual pressure and exact account. GPC's original response is used at
its legitimate source, with the new observation transported by KTO7.
The compensated defect estimate, RH and strict Robin for all $n>5040$
remain unproved.

## A joint lower bound for the complete distant first-prime sector

This application combines the whole signed source before estimating a
prime sector. It reuses KTO's observer, GPC's moments, ACP's node-$1$
slope and Gamma comparison method, and the standard effective
unconditional PNT. The new lower bound concerns the actual distant
first-layer defect of the same original integer, including occupied
primes. Its complementary signed defect remains uncontrolled. No
literature priority, numerical common threshold, Lean certification or
RH/Robin proof is claimed.

### The actual sector and absolute clock budget

Keep KTO's $A=\log n$, $L=\log A$, $T_A=\sqrt A L$ and
$k=\max\{1,\lfloor\epsilon\log L\rfloor\}$. Put

$$
P=A^{16},\qquad Z=\log P=16L,\qquad
\mathcal C_A=[A^{-1/2},A^8],\qquad
r_p=\frac{\log(1+1/p)}{\log p},
$$

$$
F_P(q)=\sum_{p>P}\log p\,(r_p-q)_+,\qquad
U_A=\int F_P(\lambda(Av))\,d\omega_A(v),\qquad
H_A=\frac{\beta_1^k(k-1)!}{(16L)^k}.
\tag{JPT1}
$$

Here $\beta_1>0$ is ACP3's slope at node $1$. Each $F_P(q)$ is a
finite nonnegative sum bounded by the actual unrestricted pressure
$M(q)$. The sum over all $p>P$ after integration will be kept complete.
The real moments in GPC2 and KTO2, and the other side of ACP3's
analytic expansion, give

$$
M_t(k)\le CL^{1/4}\quad(t=0,-4,1/4),\qquad
\int|\log c|\,d|\nu_k|(c)\le CL^{1/4},
$$

$$
w(u):=Q(h(1+u))=\beta_1u\exp(O(u))>0
\quad(0<u\le u_0),\qquad 0<u_0\le1/16.
\tag{JPT2}
$$

Choose fixed $D$ with
$|\log(w(u)/(\beta_1u))|\le Du$ on that interval. These are
identities and bounds for the original source $\nu_k$; no Mellin
identity is assigned to $\eta_A$ or $\omega_A$.

The bounded $I_\psi,R$ in KTO allow a fixed $C_*$ such that
$0\le M(\lambda(x))\le F(x):=B(x)+C_*$ and $F(x)\ge1$ for $x\ge e$.
For $c<1$, positivity of $\kappa_{A,c}$ and KTO7 give
$\int F(Av)\,d|\kappa_{A,c}|=F(A)$. For $c\ge1$, the atom and
single-sign density give exactly

$$
\int F(Av)\,d|\kappa_{A,c}|=2a_A(c)F(Ac)-F(A).
$$

Use $a_A(c)\le1+2\log c/L$ and
$F(Ac)\le C+\log L+\log c/L$. Consequently

$$
\int F_P(\lambda(Av))\,d|\kappa_{A,c}|(v)
\le C(1+\log L)[1+(\log_+c)^2].
\tag{JPT3}
$$

This proves absolute kernel/source Fubini and, by Tonelli against
total variation, absolute interchange of the complete prime sum.
No positive power moment of $\omega_A$ is used.

Below $c=A^{-1/2}$, the clamped source has mass at most
$A^{-2}M_{-4}(k)$; the correction atoms $1,2$ are outside this set
for large $A$. Its full JPT3 cost is
$O(A^{-2}L^{1/4}(1+\log L))$. Above $c=A^8$, $\eta_A=\nu_k$ and

$$
1+\log^2c\le Cc^{1/8},\qquad c^{1/8}\le A^{-1}c^{1/4}.
$$

Thus the complete high-clock cost is
$O(A^{-1}L^{1/4}(1+\log L))$. On $\mathcal C_A$ the clamp is inactive;
replacing $\eta_A$ by $\nu_k$ costs
$O(|\delta_A|(1+\log L))$ at the two correction atoms. With
$G_A(c)=\int F_P(\lambda(Av))\,d\kappa_{A,c}(v)$, these bounds yield

$$
U_A=\int_{\mathcal C_A}G_A(c)\,d\nu_k(c)
 +O(A^{-1}L^{1/4}(1+\log L)).
\tag{JPT4}
$$

The displayed error is both $o(H_A)$ and $o(1/T_A)$. The comparison
with $H_A$ is justified by the moving-degree estimate below.

### Keep the actual activation and the infinite prime tail

Let $x_p$ solve $\lambda(x_p)=r_p$ for large $p$. Elementary logarithm
expansion and the explicit derivative of $\lambda$ give
$x_p>p$ and $x_p=p+O(1)$: the price difference at $p$ is
$O(1/(p^2\log p))$, the solution lies in $[p,2p]$ eventually, and the
mean-value denominator there is comparable to $1/(p^2\log p)$.
For $c\in\mathcal C_A$ and $p>P$, $x_p/A>A^{15}>c$, so the kernel
atom sees zero hinge. Finite-endpoint integration by parts gives

$$
\int(r_p-\lambda(Av))_+\,d\kappa_{A,c}(v)
=r_p-\frac1c\lambda(x_p/c)
=-\frac{\log c}{x_p\log x_p\log(x_p/c)}.
\tag{JPT5}
$$

The endpoint at infinity is $r_p$, since the cumulative kernel tends
to one. All arguments in this calculation exceed $e$. Its sign for
$c<1$ differs from its sign for $c>1$; neither is separately carried
through the signed source.

Put $z=\log c$, so $-L/2\le z\le8L$ and $\log p\ge16L$.
Replacing $x_p$ by $p$ in the $\log p$-weighted sum JPT5 costs at most
$C|z|\sum_{p>P}1/(p^2\log p)\le C|z|/(P\log P)$.
The reference summand is $-z/[p(\log p-z)]$.
Reuse the standard effective unconditional PNT in the form
$\pi(t)=\operatorname{li}(t)+O(t\exp(-a\sqrt{\log t}))$.
Partial summation applies uniformly because $|z|/\log t\le1/2$
for $t\ge P$, and the weight derivative is bounded by
$C|z|/(t^2\log t)$. The endpoint and complete infinite error tail are
$O(|z|\exp(-a_1\sqrt Z))$ for some fixed $a_1>0$.
The continuous integral is exactly

$$
-z\int_P^\infty\frac{dt}{t\log t(\log t-z)}
=\log(1-z/Z).
$$

Therefore, uniformly on $\mathcal C_A$,

$$
G_A(c)=\log(1-\log c/Z)
 +O\!\left(|\log c|e^{-a_1\sqrt Z}
             +\frac{|\log c|}{P\log P}\right).
\tag{JPT6}
$$

Its source-integrated error is
$O(L^{1/4}e^{-a_1\sqrt Z}+L^{1/4}/(P\log P))=o(H_A)$.
The PNT error is not asserted to be $o(1/T_A)$; relative control is
sufficient to determine this sector's sign.

### Combine the whole signed source before estimating

On $\mathcal C_A$ use

$$
\log(1-z/Z)=-\int_0^\infty e^{-Zu}(e^{zu}-1)\,\frac{du}{u}.
$$

Only $[0,u_0]$ is interchanged with the source. The removed tail is
bounded by $C\exp[-u_0(Z-\max(z,0))]\le Ce^{-8u_0L}$.
The bound $|(c^u-1)/u|\le|\log c|(1+c^{u_0})$ supplies absolute
Fubini. No two divergent $1/u$ terms are separated.
Extending this truncated expression from $\mathcal C_A$ to the
whole $\nu_k$ costs $O(A^{-2}LM_{-4}(k))$ below $A^{-1/2}$ and
$O(A^{-1}M_{1/4}(k))$ above $A^8$. For the former, use the maximum
of $c^4|\log c|$ on the small-clock set; for the latter use
$|\log c|(1+c^{u_0})\le Cc^{1/8}$.
Exact source mass and its Mellin identity now give

$$
\int_{\mathcal C_A}\log(1-\log c/Z)\,d\nu_k(c)
=\int_0^{u_0}e^{-Zu}Q(h(1+u))^k\,\frac{du}{u}+o(H_A).
\tag{JPT7}
$$

In particular the source factor is evaluated at $1+u$, whereas
ACP4 used $1-u$. The main integral here is positive for every $k$.

Apply the Gamma comparison method of ACP4–ACP5 with the explicit new
parameters $Z=16L$ and $k=O(\log L)$. JPT2 bounds the integral between
truncated Gamma integrals with rates $Z+Dk$ and $Z-Dk$.
Here $k^2/Z\to0$ and $k\log Z=o(Z)$, so the rate change costs
$O(k^2/Z)$ relatively, and the removed Gamma tails are exponentially
smaller. Hence

$$
\int_0^{u_0}e^{-Zu}w(u)^k\,\frac{du}{u}
=\frac{\beta_1^k\Gamma(k)}{Z^k}
 \left(1+O\!\left(\frac{k^2}{Z}\right)\right)
=H_A(1+o(1)).
\tag{JPT8}
$$

Stirling at this actual degree gives
$\log H_A=-\epsilon(\log L)^2+O(\log L\log\log L)$.
Thus every error in JPT4, JPT6 and JPT7 is $o(H_A)$, including the
whole source variation and prime tail. Combining them proves

$$
U_A=H_A(1+o(1))>0,\qquad T_AH_A\longrightarrow\infty.
\tag{JPT9}
$$

### The same integer's occupied and absent first layers

Let $D_{\mathrm{far},A}(n)$ average the complete first-layer defect
at primes $p>P$, including both occupied and absent primes:

$$
D_{\mathrm{far},A}(n)=\int\left[
 \sum_{\substack{p>P\\p\nmid n}}\log p\,(r_p-\lambda(Av))_+
 +\sum_{\substack{p>P\\p\mid n}}\log p\,(\lambda(Av)-r_p)_+
 \right]d\omega_A(v).
$$

This is an actual pointwise part of the same integer's defect; absolute
integration follows from the complete defect bounds in KTO.
The scalar hinge identity, exact mass and exact price mean give

$$
D_{\mathrm{far},A}(n)
=U_A+\sum_{\substack{p>P\\p\mid n}}
        (\lambda(A)-r_p)\log p.
\tag{JPT10}
$$

Every occupied-prime correction is nonnegative because
$r_p<\lambda(p)<\lambda(A)$ for $p>P>A$. Consequently, uniformly
for every original $n$ at its own $A=\log n$,

$$
D_{\mathrm{far},A}(n)\ge U_A\ge H_A/2>0
\quad\text{eventually}.
\tag{JPT11}
$$

No optimizer, CA/GA hypothesis or bound on the prime support of $n$
replaces this original integer. Define $E_A(n)$ by averaging the exact
complementary defect part: every first layer $p\le P$ and every higher
exponent layer at every prime remains in it. Then

$$
D_A(n)=D_{\mathrm{far},A}(n)+E_A(n)\ge E_A(n)+H_A/2,
$$

$$
T_A\Delta(n)=T_AE_A(n)+T_AD_{\mathrm{far},A}(n)+c_R+o(1).
\tag{JPT12}
$$

The complementary signed average $E_A(n)$ has no proved sufficient
lower bound. Its pointwise nonnegative integrand does not imply that
its signed average is nonnegative. The positive far-tail credit alone supplies no lower bound for this
complementary signed term. Discarding this tail in a lower bound is
justified after the complete signed average, not kernel by kernel.
No positivity of the complete defect, new total Robin upper or RH
proof follows.

## Growing source moments move the paid first-prime boundary

This application extends JPT's actual first-layer lower bound to a
moving cutoff whose logarithm is asymptotic to $\log A$. It keeps the
same KTO observer and degree. GPC's source moments, xi reflection,
positive-real Stirling, JPT's actual activation calculation and the
standard effective unconditional PNT are reused. The retained
application is the additional signed arithmetic band lower and its
same-integer consumer; the intermediate moment and Gamma estimates
are not separate new results. No literature priority, numerical
common threshold, Lean certification or RH/Robin proof is claimed.

### Uniform growing moments of the unchanged source

Keep $A=\log n$, $L=\log A$, $T_A=\sqrt A L$ and
$k=\max\{1,\lfloor\epsilon\log L\rfloor\}$ from KTO. Its original
source has

$$
h(s)=2m^{1-s}\xi(s),\qquad m=\pi/3,\qquad
Q(z)=(1-z)(1-z/m),\qquad H_k(s)=1-Q(h(s))^k.
$$

The clamped and calibrated source and its transported observer remain
$\eta_A=(\chi_A)_\#\nu_k-2\delta_A(\delta_1-\delta_2)$ and
$\omega_A=\int\kappa_{A,c}\,d\eta_A(c)$, with
$|\delta_A|=O(A^{-3}L^{1/4})$. Exact mass and price mean are still
$\int d\omega_A=1$ and
$\int\lambda(Av)\,d\omega_A(v)=\lambda(A)$.
All Mellin identities below belong to $\nu_k$.

GPC2 gives, for every real $t$ and integer $k\ge1$,
$M_t(k)=\int c^t\,d|\nu_k|(c)\le1+R_t^k$, where
$R_t=(1+b_t)(1+b_t/m)$ and $b_t=h(1+t)$.
For $t\ge2$, xi reflection gives
$b_t=2m^{-t}\xi(1+t)$ and $b_{-t}=2m^t\xi(t)$.
Use the standard positive-real log-Gamma Stirling expansion
([DLMF 5.11.1](https://dlmf.nist.gov/5.11.E1)) in
$\xi(s)=s(s-1)\pi^{-s/2}\Gamma(s/2)\zeta(s)/2$, for real
$s\ge2$, together with $\zeta(s)\le\zeta(2)$.
There is a fixed $C_m\ge1$ such that

$$
\log R_t,\ \log R_{-t}\le C_mt\log(t+2),\qquad
M_t(k)+M_{-t}(k)\le4e^{C_mkt\log(t+2)}
\quad(t\ge2,\ k\ge1).
\tag{GMW1}
$$

The constant is uniform in growing real $t$ and growing degree $k$.
No fixed-$t$ implicit constant or bounded-strip vertical Stirling
estimate is substituted at a growing real argument.

### A logarithmic clock window and its relative tail budget

For sufficiently large $A$, put

$$
t_A=\log L\ge4,\qquad
\ell_A=4(C_m+1)k\log(t_A+2),\qquad
\mathcal C'_A=[e^{-\ell_A},e^{\ell_A}],
$$

$$
P_A=Ae^{2\ell_A},\qquad Z_A=\log P_A=L+2\ell_A,\qquad
\widetilde H_A=\frac{\beta_1^k(k-1)!}{L^k}.
\tag{GMW2}
$$

Here $\beta_1>0$ is the same node-$1$ slope as in ACP3 and JPT2.
Retain JPT2's fixed $0<u_0\le1/16$ and
$w(u)=Q(h(1+u))=\beta_1u\exp(O(u))>0$ on $(0,u_0]$.
Since $k=O(t_A)$,
$\ell_A=O(t_A\log(t_A+2))=o(L)$ and $k\ell_A/L\to0$.
The clamp level $\tau=e/A$ is below $e^{-\ell_A}$ eventually, and
the correction atoms $1,2$ lie inside $\mathcal C'_A$.
In particular

$$
\frac{\log P_A}{\log A}\longrightarrow1,\qquad
P_A=A\exp\!\bigl(O(\log\log A\,\log\log\log A)\bigr)
 < A^{16}\quad\text{eventually}.
$$

This does not assert $P_A/A\to1$.
For $t=t_A\ge4$ and real $z$,
$(1+z^2)e^{u_0|z|}\le Ce^{t|z|/2}$ with an absolute constant
independent of $t$. On $|z|>\ell_A$, this is at most
$Ce^{-t\ell_A/2}e^{t|z|}$.
Integrating $c^t+c^{-t}$ with GMW1 gives

$$
\int_{|\log c|>\ell_A}(1+\log^2c)e^{u_0|\log c|}
       \,d|\nu_k|(c)
\le C\exp\!\bigl(-(C_m+2)kt_A\log(t_A+2)\bigr)
=:E_A^{\mathrm{clock}}.
\tag{GMW3}
$$

Stirling at the actual slow degree yields
$\log\widetilde H_A=-\epsilon(\log L)^2+
O(\log L\log\log L)$, whence
$(1+t_A)E_A^{\mathrm{clock}}=o(\widetilde H_A)$.
This is a relative error statement; these growing-window errors are
not asserted to be $o(1/T_A)$.

### The actual complete prime tail at the moving cutoff

Keep JPT's $r_p=\log(1+1/p)/\log p$ and the actual activation
$\lambda(x_p)=r_p$, with $x_p>p$ and $x_p=p+O(1)$. Define

$$
F_{P_A}(q)=\sum_{p>P_A}\log p\,(r_p-q)_+,\qquad
U'_A=\int F_{P_A}(\lambda(Av))\,d\omega_A(v).
\tag{GMW4}
$$

JPT3's global bound, valid at every cutoff because $F_{P_A}\le M$,
gives

$$
\int F_{P_A}(\lambda(Av))\,d|\kappa_{A,c}|(v)
\le C(1+\log L)[1+(\log_+c)^2].
$$

Thus absolute kernel/source integration retains the complete infinite
prime tail. GMW3 pays both excluded clock sets. Clamping only
decreases the low-clock logarithmic weight and keeps excluded low
clocks below $e^{-\ell_A}$; moreover
$|\chi_\#\nu_k|\le\chi_\#|\nu_k|$. On high clocks
$\eta_A=\nu_k$, and both correction atoms are inside the window.
Their replacement cost is
$O(|\delta_A|(1+\log L))=o(\widetilde H_A)$.
With $G'_A(c)=\int F_{P_A}(\lambda(Av))\,d\kappa_{A,c}(v)$,

$$
U'_A=\int_{\mathcal C'_A}G'_A(c)\,d\nu_k(c)
       +o(\widetilde H_A).
\tag{GMW5}
$$

The new tail budget is $O((1+t_A)E_A^{\mathrm{clock}})$; JPT4's
polynomial-window root-error assertion is not used outside its range.

For $c\in\mathcal C'_A$ and $p>P_A$, one has
$x_p/A>e^{2\ell_A}>c$, so the actual activation lies beyond the
kernel atom, as required in JPT5. Also
$|\log c|/\log p\le\ell_A/(L+2\ell_A)<1/2$.
These verified domain conditions permit JPT5's same finite-endpoint
calculation and JPT6's actual-activation replacement and effective-PNT
partial summation. They give, uniformly on the new window,

$$
G'_A(c)=\log(1-\log c/Z_A)
 +O\!\left(|\log c|e^{-a_1\sqrt{Z_A}}
          +\frac{|\log c|}{P_A\log P_A}\right),
\tag{GMW6}
$$

for a fixed $a_1>0$. The exact nonhomogeneous kernel, its atom,
actual prime thresholds and infinite tail are unchanged.
By KTO2, $\int|\log c|\,d|\nu_k|\le CL^{1/4}$.
Since $Z_A\sim L$ and $\sqrt L$ dominates $(\log L)^2$, the
source-integrated error in GMW6 is $o(\widetilde H_A)$, without a
root-smallness claim.

### Source cancellation and the moving Gamma comparison

On the new window set $z=\log c$ and use

$$
\log(1-z/Z_A)=-\int_0^\infty e^{-Z_Au}(e^{zu}-1)\,\frac{du}{u}.
$$

Only the finite interval $[0,u_0]$ is interchanged with the source.
The removed $u\ge u_0$ tail is at most
$Ce^{-u_0(Z_A-\max(z,0))}\le Ce^{-u_0(L+\ell_A)}$;
its source cost, including total variation $O(L^{1/4})$, is
$o(\widetilde H_A)$.
On the retained interval,
$|(c^u-1)/u|\le|\log c|(1+c^{u_0})$.
GMW3 therefore pays extension of this truncated expression to all
of $\nu_k$ with cost $O(E_A^{\mathrm{clock}})$.
Keep $c^u-1$ intact before Fubini; no divergent $1/u$ pieces are
separated. Exact source mass and its Mellin identity then give

$$
\int_{\mathcal C'_A}\log(1-\log c/Z_A)\,d\nu_k(c)
=\int_0^{u_0}e^{-Z_Au}Q(h(1+u))^k\,\frac{du}{u}
 +o(\widetilde H_A).
\tag{GMW7}
$$

Reuse the standard Gamma comparison of ACP4--ACP5 and JPT8 with
rates $Z_A\pm Dk$, where JPT2 supplies fixed $D$.
Here $k^2/Z_A\to0$ and $k\log Z_A=o(Z_A)$, so the integral is
$\beta_1^k\Gamma(k)Z_A^{-k}(1+o(1))$.
Moreover
$(L/Z_A)^k=\exp[-k\log(1+2\ell_A/L)]=1+o(1)$ because
$k\ell_A/L\to0$. Combining the actual tail, clock and source
errors proves

$$
U'_A=\widetilde H_A(1+o(1))>0,\qquad
T_A\widetilde H_A\longrightarrow\infty.
\tag{GMW8}
$$

### The additional paid band of the same original integer

For the same observer, $A$ and $k$, JPT9 gives the old actual tail
$U_A^{(16)}=16^{-k}\widetilde H_A(1+o(1))$ beyond $A^{16}$.
Since $k\to\infty$ and $P_A<A^{16}$ eventually, the actual
intervening band satisfies

$$
U_A^{\mathrm{band}}:=U'_A-U_A^{(16)}
=\int\sum_{P_A<p\le A^{16}}\log p\,(r_p-\lambda(Av))_+
            \,d\omega_A(v)
=\widetilde H_A(1+o(1))>0.
\tag{GMW9}
$$

Both terms use one realization and one clock; no separately optimized
sources are combined. For the same original integer $n$ at its own
$A=\log n$, let $D_A^{\mathrm{band}}(n)$ be the signed observer
average of the complete first-layer defect in $P_A<p\le A^{16}$:
absent primes contribute $\log p\,(r_p-\lambda(Av))_+$ and
occupied primes contribute $\log p\,(\lambda(Av)-r_p)_+$.
The scalar hinge identity, exact mass and exact price mean give

$$
D_A^{\mathrm{band}}(n)
=U_A^{\mathrm{band}}
 +\sum_{\substack{P_A<p\le A^{16}\\p\mid n}}
       (\lambda(A)-r_p)\log p
\ge U_A^{\mathrm{band}}
\ge\widetilde H_A/2>0\quad\text{eventually}.
\tag{GMW10}
$$

The occupied-prime correction is nonnegative because $p>P_A>A$.
This lower bound holds uniformly for every original integer at its
own clock. It pays an actual band previously inside JPT's
complementary defect, with no CA/GA assumption, prime-support bound
or optimizer substitution. The complete new far-first-layer sector
$p>P_A$ likewise has its nonnegative occupation correction and a
lower bound $\widetilde H_A/2$ eventually. These positive lower
bounds depend on $A$; they are not fixed positive constants.

Let $E'_A(n)$ average the exact remaining defect: all first layers
$p\le P_A$ and every higher exponent layer at every prime.
Writing $D_{\mathrm{far},A}^{(16)}(n)$ for the old JPT far sector,
the disjoint account is

$$
D_A(n)=E'_A(n)+D_A^{\mathrm{band}}(n)
                +D_{\mathrm{far},A}^{(16)}(n).
\tag{GMW11}
$$

One may instead combine the last two terms into the new far sector;
that overlapping sector is not counted again. KTO12's original
Robin margin remains

$$
T_A\Delta(n)=T_AE'_A(n)+T_AD_A^{\mathrm{band}}(n)
                 +T_AD_{\mathrm{far},A}^{(16)}(n)+c_R+o(1).
\tag{GMW12}
$$

No sufficient lower bound for $E'_A(n)$ is supplied. Its integrand is
pointwise nonnegative but its observer average is signed. The new
first-layer boundary and positive band do not prove complete-defect
positivity, RH or strict Robin for every $n>5040$.

## A root-small debit for the complete actual higher-layer defect

This application bounds every actual exponent layer $j\ge2$ of the
same original integer under the unchanged KTO observer. It reuses
the actual second cutoff MS3, the ordinary integral GPP4, KTO's
quantitative root-tail transport and the standard effective
unconditional PNT. These supporting estimates are not separate new
results. The application concerns the complete higher-layer defect;
the earlier reference prime-power transport is not assumed to bound
that defect. No literature priority, numerical common threshold,
Lean certification or RH/Robin proof is claimed.

For the classical actual-cutoff and full-exponent bookkeeping, see
Akatsuka, [arXiv:2411.19259v1, §3](https://arxiv.org/html/2411.19259v1#S3),
Lemma 3.1, Proposition 3.2 and (3.6)--(3.8), (3.11).
The correspondence is $\kappa=1$, the paper's price
$\varepsilon=\lambda(x)$, first cutoff $x_1(\varepsilon)$, and
higher cutoffs $y_j(x_1(\varepsilon))$.
These are the actual ratio thresholds used here, rather than reference
prime powers. Those source statements concern CA products and their
full-layer remainders; they do not state the signed-observer defect
lower bound consumed below. No claim of priority is attached to the
intermediate higher-pressure asymptotic.

### The actual higher pressure and its finite limit

Keep KTO's $A=\log n$, $L=\log A$, $T_A=\sqrt A L$,
$k=\max\{1,\lfloor\epsilon\log L\rfloor\}$, sources
$\nu_k,\eta_A$ and observer $\omega_A$.
Its mass is exactly one and its price mean is exactly $\lambda(A)$.
Keep $\lambda(x)=1/(x\log x)$ and $K(x)=-\lambda'(x)$.
Use the same actual increments

$$
\beta_{p,j}=\log\left(1+\frac1{p+\cdots+p^j}\right),\qquad
r_{p,j}=\frac{\beta_{p,j}}{\log p}.
$$

Define the full higher pressure and its tail by

$$
\mathcal M_{\ge2}(q)=\sum_p\sum_{j\ge2}\log p\,(r_{p,j}-q)_+,
\qquad C_2=\sum_p\sum_{j\ge2}\beta_{p,j}=\log\zeta(2),
$$

$$
F_2(x)=C_2-\mathcal M_{\ge2}(\lambda(x)),\qquad
\mathcal A_{\ge2}(x)=
 \sum_{\substack{p,\ j\ge2\\r_{p,j}>\lambda(x)}}\log p.
\tag{HLD1}
$$

The constant uses the ordinary telescope
$\sum_{j\ge2}\beta_{p,j}=-\log(1-p^{-2})$ and the convergent
Euler product for $\zeta(2)$. In particular $F_2$ is nonnegative,
bounded and decreases to zero on $[e,\infty)$.
Tonelli for nonnegative scalar hinges, followed by $q=\lambda(t)$,
gives the exact account

$$
F_2(x)=\sum_p\sum_{j\ge2}
       \min\{\beta_{p,j},\lambda(x)\log p\}
     =\int_x^\infty\mathcal A_{\ge2}(t)K(t)\,dt.
\tag{HLD2}
$$

The actual active set is finite at every finite $t$. The strict
threshold convention remains unchanged; isolated equality values do
not affect this ordinary integral.

### Insert the owned actual second cutoff and retain every higher layer

MS3 gives the actual second cutoff
$q_2(t)=\sqrt{2t}(1+O(1/\log t))$.
The effective PNT, including the possible strict endpoint atom
$O(\log t)$, therefore gives

$$
\sum_{p:r_{p,2}>\lambda(t)}\log p
=\vartheta(q_2(t)-)
=\sqrt{2t}+O(\sqrt t/\log t).
$$

For all growing indices $j\ge3$, reuse the owned activation bound
$p^j\log p<t\log t$. Put $X=t\log t/\log2$.
Then $j<\log X/\log2$ and $p<X^{1/j}$.
The elementary bound $\vartheta(y)\le y\log y$ yields

$$
\sum_{j\ge3}\sum_{p:r_{p,j}>\lambda(t)}\log p
\le\sum_{3\le j\le\log X/\log2}\vartheta(X^{1/j})
=O\!\left(X^{1/3}(\log X)^2\right)
=O\!\left(t^{1/3}(\log t)^3\right).
\tag{HLD3}
$$

This is uniform over the entire growing index range. Every actual
layer and its full weight remains; reference prime-power thresholds
are not substituted. The short-interval GM estimates elsewhere in
the MS3 application are not needed here.

Insert these bounds in HLD2 and reuse GPP4's integral estimate
$\int_x^\infty\sqrt tK(t)\,dt
=2/(\sqrt x\log x)+O(1/(\sqrt x\log^2x))$.
The second-layer error integrates to
$O(1/(\sqrt x\log^2x))$.
The entire $j\ge3$ term is $O(x^{-2/3}\log^2x)$, smaller than
that error. Consequently the actual pressure tail satisfies

$$
F_2(x)=\frac{2\sqrt2}{\sqrt x\log x}
       +O\!\left(\frac1{\sqrt x\log^2x}\right).
\tag{HLD4}
$$

### Use the same quantitative root-tail transport

Apply KTO9--KTO10's root-tail argument with $F_2$ in place of $R$
and $2\sqrt2$ in place of $c_R$, keeping the same sources,
degree and observer. The required input is HLD4 with its quantitative
extra logarithm, together with boundedness on $[e,\infty)$.
The correspondence of error bounds is as follows.

Below $c=A^{-1/2}$, the clamped bounded integrand and source mass
$A^{-2}M_{-4}(k)$ cost $O(A^{-3/2}L^{5/4})$ after multiplication
by $T_A$. On $c\ge A^{-1/2}$ put $z=\log c$, so $L+z\ge L/2$.
HLD4 gives

$$
T_AF_2(Ac)=c^{-1/2}
 \left[\frac{2\sqrt2 L}{L+z}
       +O\!\left(\frac L{(L+z)^2}\right)\right].
$$

Its difference from $2\sqrt2c^{-1/2}$ is bounded by
$(C/L)c^{-1/2}(1+|\log c|)$.
KTO2 makes its full source integral $O(L^{-3/4})$.
The omitted source reference moment is at most
$A^{-7/4}M_{-4}(k)$, and the same two correction atoms are negligible.
This gives
$T_A\int F_2(Ac)\,d\eta_A(c)
=2\sqrt2H_k(1/2)+O(L^{-3/4})$.

For $c\ge A^{-1/2}$ the entire kernel support has $v\ge c$.
HLD4 bounds every later $F_2(Av)$ by
$C/(\sqrt{Ac}\log(Ac))$. KTO6 therefore gives

$$
T_A\left|\int F_2(Av)\,d\kappa_{A,c}(v)-F_2(Ac)\right|
\le\frac C L c^{-1/2}|\log c|.
$$

Its $|\eta_A|$ integral is $O(L^{-3/4})$.
On the remaining small clocks the kernel is positive of mass one;
bounded $F_2$ and the same small-clock mass pay its complete infinite
tail. Thus the reused root-tail transport yields

$$
T_A\int F_2(Av)\,d\omega_A(v)
=2\sqrt2H_k(1/2)+O(L^{-3/4}).
\tag{HLD5}
$$

All source Mellin identities remain on $\nu_k$.
No positive-power moment of $\omega_A$ is used.
Bounded $F_2$ and finite variation also give absolute integration.

Since $\omega_A$ has exact mass one, HLD4--HLD5 imply the actual
higher-pressure gap

$$
\mathcal J_2(A):=
\int\mathcal M_{\ge2}(\lambda(Av))\,d\omega_A(v)
       -\mathcal M_{\ge2}(\lambda(A)),
$$

$$
T_A\mathcal J_2(A)
=2\sqrt2[1-H_k(1/2)]+O(L^{-3/4})
=2\sqrt2Q(h(1/2))^k+O(L^{-3/4})=o(1).
\tag{HLD6}
$$

Here $|Q(h(1/2))|<1$ by XLR2/GPC8.
No Jensen sign is asserted. In particular, for a fixed sufficiently
large $C$, put
$\varepsilon_A=C(|Q(h(1/2))|^k+L^{-3/4})\to0$;
then $|\mathcal J_2(A)|\le\varepsilon_A/T_A$ eventually.

### Compare with the same integer's nonnegative own-price defect

For the original integer $n$, let $a_p=v_p(n)$ and put
$W_2(n)=\sum_p\sum_{2\le j\le a_p}\beta_{p,j}$ and
$L_2(n)=\sum_p(a_p-1)_+\log p$.
Its pointwise complete higher-layer defect is

$$
d_2(n,q)=\mathcal M_{\ge2}(q)-W_2(n)+qL_2(n)
 =\sum_p\sum_{2\le j\le a_p}\log p\,(q-r_{p,j})_+
  +\sum_p\sum_{j\ge\max\{2,a_p+1\}}
                 \log p\,(r_{p,j}-q)_+\ge0.
\tag{HLD7}
$$

Every active and occupied sum at $q>0$ is finite.
This retains all higher layers and the original integer's exact
occupation pattern. Its observer average is absolute: the higher
pressure is bounded, $W_2(n),L_2(n)$ are finite, and KTO owns the
absolute price integral.
Define $D_{2,A}(n)=\int d_2(n,\lambda(Av))\,d\omega_A(v)$.
Exact mass and exact price mean give

$$
D_{2,A}(n)=d_2(n,\lambda(A))+\mathcal J_2(A)
\ge-\frac{\varepsilon_A}{T_A},\qquad
\varepsilon_A\longrightarrow0.
\tag{HLD8}
$$

The lower bound is uniform for every original integer at its own
$A=\log n$. It compares to the nonnegative defect at the original
price; it does not carry pointwise positivity through signed averaging
or replace $n$ by an optimizer. All remaining observer error depends
on $n$ only through $A$.

### The first-layer consumer and the remaining full target

Let $N_A(n)$ average the complete actual first-layer defect for
$p\le P_A$, with GMW2's cutoff and unchanged observer.
Let $D_{\mathrm{far,new},A}(n)$ average the first-layer complement
$p>P_A$. The disjoint account is

$$
D_A(n)=N_A(n)+D_{\mathrm{far,new},A}(n)+D_{2,A}(n),
$$

$$
D_{\mathrm{far,new},A}(n)
=D_A^{\mathrm{band}}(n)+D_{\mathrm{far},A}^{(16)}(n)
\ge\widetilde H_A/2>0\quad\text{eventually}.
\tag{HLD9}
$$

No overlapping GMW sector is counted twice.
KTO12, GMW and HLD8 therefore give

$$
\begin{aligned}
T_A\Delta(n)
&\ge T_AN_A(n)+T_AD_{\mathrm{far,new},A}(n)
                       +c_R-\varepsilon_A+o(1)\\
&\ge T_AN_A(n)+T_A\widetilde H_A/2+c_R-o(1).
\end{aligned}
\tag{HLD10}
$$

Every actual higher layer has a root-small possible debit.
The remaining signed estimate concerns the same integer's first
layers $p\le P_A$ and their joint compensation with the paid far
sector. No sufficient lower bound for $N_A(n)$ is supplied.
Complete-defect positivity, strict Robin for every $n>5040$ and RH
remain unproved.

## Root-scale localization of the remaining first-prime defect

This application controls the complete low-first-prime defect of the
same original integer under the unchanged KTO observer. It reuses
GMW1's uniform real-order source moments, the exact KTO kernel and
mass/price calibration, GMW's far-first-layer lower and HLD's complete
higher-layer lower. The new consumer leaves only a moving first-prime
window unpaid at root scale. The intermediate moment and affine
identities are supporting steps, not separate new results.
No literature priority, numerical common threshold, Lean certification
or RH/Robin proof is claimed.

### Use the same source with a larger negative moment order

Keep $A=\log n$, $L=\log A$, $T_A=\sqrt A L$,
$k=\max\{1,\lfloor\epsilon\log L\rfloor\}$ and the same
$\nu_k,\eta_A,\omega_A$ from KTO.
In particular the clamp is $\chi_A(c)=\max\{c,e/A\}$ and the
source correction atoms are $1,2$.
GMW1 has a fixed $C_m\ge1$ valid for every real moment order
$t\ge2$. For the lower prime cut use $t=L\ge4$ and put

$$
b_A=4(C_m+1)k\log(L+2),\qquad
Y_A=Ae^{-2b_A},\qquad a_A^{\mathrm{low}}=2Y_A/A=2e^{-2b_A},
$$

$$
\rho_A=4\exp\!\bigl(-(3C_m+4)kL\log(L+2)\bigr).
\tag{CPW1}
$$

Since $k=O(\log L)$, one has
$b_A=O((\log L)^2)=o(L)$.
Thus $Y_A\to\infty$, $\log Y_A/\log A\to1$,
$2Y_A<A$ and
$e/A<a_A^{\mathrm{low}}\le e^{-b_A}<1$ eventually.
Moreover

$$
\log(T_A\rho_A)=\log4+L/2+\log L
                    -(3C_m+4)kL\log(L+2)\longrightarrow-\infty,
\qquad T_A\rho_A\longrightarrow0.
\tag{CPW2}
$$

The changed moment order and buffer specify the lower prime cut;
the signed source, observer and slow degree remain unchanged.

### The actual low-prime pressure is affine above a common activation

Keep $r_p=\log(1+1/p)/\log p$ and $\beta_p=r_p\log p$.
For the finite set $p\le Y_A$, write
$\vartheta_Y=\sum_{p\le Y_A}\log p$ and
$S_Y=\sum_{p\le Y_A}\beta_p$, and define

$$
F_Y(q)=\sum_{p\le Y_A}\log p\,(r_p-q)_+,\qquad
B_Y(q)=\sum_{p\le Y_A}\log p\,(q-r_p)_+.
$$

The exact finite hinge identity gives

$$
F_Y(q)=S_Y-q\vartheta_Y+B_Y(q)\qquad(q\ge0).
\tag{CPW3}
$$

For every prime $p\le Y_A$, including $2$, the elementary actual
inequality $\log(1+1/p)>1/(p+1)$ gives

$$
r_p>\frac1{(p+1)\log p}
\ge\frac1{(Y_A+1)\log Y_A}
>\lambda(2Y_A)>\lambda(A)
\quad\text{eventually}.
\tag{CPW4}
$$

Thus $B_Y(\lambda(A))=0$, and
$B_Y(\lambda(Av))=0$ whenever $v\ge a_A^{\mathrm{low}}$.
No large-prime approximation to an activation point is applied to
small primes.

KTO5's entire kernel is supported on $v\ge c$.
For $c\ge a_A^{\mathrm{low}}$, its $B_Y$ observation is therefore
exactly zero, including arbitrarily high clocks and the signed
kernel density. For $e/A\le c<a_A^{\mathrm{low}}<1$, the kernel
is positive by KTO6. The exact KTO7 price observation yields

$$
0\le\int B_Y(\lambda(Av))\,d\kappa_{A,c}(v)
\le\vartheta_Y\int\lambda(Av)\,d\kappa_{A,c}(v)
=\frac{\vartheta_Y\lambda(A)}c.
\tag{CPW5}
$$

Positivity here concerns only these low-$c$ kernels. Neither the
source nor the final observer is assigned positivity.

### Pay the complete inverse-price-weighted low-clock tail

Put $J_{\mathrm{low}}(A)=
\int B_Y(\lambda(Av))\,d\omega_A(v)$.
The two source correction atoms lie outside
$c<a_A^{\mathrm{low}}$. Total variation decreases under pushforward,
and the clamp increases $c$, decreasing its inverse weight.
Using $a_A^{\mathrm{low}}\le e^{-b_A}$ and GMW1 at the actual
growing order $L$, one obtains

$$
\begin{aligned}
|J_{\mathrm{low}}(A)|
&\le\vartheta_Y\lambda(A)
       \int_{c<a_A^{\mathrm{low}}}c^{-1}\,d|\eta_A|(c)\\
&\le\vartheta_Y\lambda(A)
       \int_{c<a_A^{\mathrm{low}}}c^{-1}\,d|\nu_k|(c)\\
&\le e^{-2b_A}e^{-(L-1)b_A}M_{-L}(k)\\
&\le4\exp\!\bigl(-(L+1)b_A+C_mkL\log(L+2)\bigr)\\
&\le\rho_A=o(1/T_A).
\end{aligned}
\tag{CPW6}
$$

Here $\vartheta_Y\le Y_A\log Y_A$ gives
$\vartheta_Y\lambda(A)\le e^{-2b_A}$, and on $c<e^{-b_A}$,
$c^{-1}\le e^{-(L-1)b_A}c^{-L}$.
This proves absolute kernel/source Fubini as well: the integrand is
zero on the full support of every $c\ge a_A^{\mathrm{low}}$ kernel,
and the displayed positive-kernel bound controls all remaining clocks.
No inverse-price singularity, clamped source contribution or infinite
kernel tail is dropped. The uniform real-order input is GMW1;
no fixed-order implicit constant or weaker $u_0$-weighted clock
estimate is substituted at order $L$.

### Retain the same integer's actual missing low primes

For the original $n$, set
$W_{\mathrm{low}}(n)=\sum_{p\le Y_A,\ p\mid n}\beta_p$,
$L_{\mathrm{low}}(n)=\sum_{p\le Y_A,\ p\mid n}\log p$ and
$d_{\mathrm{low}}(n,q)=F_Y(q)-W_{\mathrm{low}}(n)+qL_{\mathrm{low}}(n)$.
This is exactly its complete first-layer defect on $p\le Y_A$:
occupied primes contribute $\log p(q-r_p)_+$ and absent primes
contribute $\log p(r_p-q)_+$.
By CPW4 its original-price baseline is

$$
G_{\mathrm{low},A}(n):=d_{\mathrm{low}}(n,\lambda(A))
=\sum_{\substack{p\le Y_A\\p\nmid n}}
             (\beta_p-\lambda(A)\log p)\ge0.
\tag{CPW7}
$$

Let $D_{\mathrm{low},A}(n)=
\int d_{\mathrm{low}}(n,\lambda(Av))\,d\omega_A(v)$.
Exact mass and exact price mean applied to CPW3 give

$$
D_{\mathrm{low},A}(n)
=G_{\mathrm{low},A}(n)+J_{\mathrm{low}}(A)
\ge G_{\mathrm{low},A}(n)-\rho_A\ge-\rho_A,
\qquad T_A\rho_A\longrightarrow0.
\tag{CPW8}
$$

This is uniform for every original integer at its own $A=\log n$.
The error depends on $n$ only through $A$; actual low-prime occupancy
is preserved in $G_{\mathrm{low},A}(n)$.
The finite prime set and KTO's absolute mass/price bounds give
absolute defect integration. No other integer, optimizer or
pointwise positivity transported through a signed measure is used.

### A disjoint central-window consumer

Retain GMW's upper cutoff
$P_A=Ae^{2\ell_A}$, where
$\ell_A=4(C_m+1)k\log(\log L+2)$, and its complete actual far-first
lower $D_{\mathrm{far,new},A}(n)\ge\widetilde H_A/2>0$ eventually.
Retain HLD's complete actual higher-layer lower
$D_{2,A}(n)\ge-\varepsilon_A/T_A$, with $\varepsilon_A\to0$.
All components use the same source, observer, degree and original $n$.

Let $C_A(n)$ average only the complete actual first-layer defect
on $Y_A<p\le P_A$. The exact disjoint account is

$$
D_A(n)=D_{\mathrm{low},A}(n)+C_A(n)
                  +D_{\mathrm{far,new},A}(n)+D_{2,A}(n).
\tag{CPW9}
$$

KTO12 and the three lower bounds yield

$$
\begin{aligned}
T_A\Delta(n)
&\ge T_AC_A(n)+T_AG_{\mathrm{low},A}(n)
 +T_AD_{\mathrm{far,new},A}(n)
 +c_R-\varepsilon_A-T_A\rho_A+o(1)\\
&\ge T_AC_A(n)+T_AG_{\mathrm{low},A}(n)
 +T_A\widetilde H_A/2+c_R-o(1).
\end{aligned}
\tag{CPW10}
$$

No far sector or higher layer is counted twice.
Both $\log Y_A/\log A$ and $\log P_A/\log A$ tend to one.
The logarithmic width of the unpaid prime window relative to
$\log A$ therefore tends to zero; the multiplicative window is not
claimed to shrink, and neither endpoint divided by $A$ is claimed
to tend to one.
No sufficient joint lower for
$C_A(n)+G_{\mathrm{low},A}(n)+D_{\mathrm{far,new},A}(n)$ is supplied.
Complete-defect positivity, RH and strict Robin for every $n>5040$
remain unproved.

## An actual integer family consumes the enlarged far-prime credit

The following application gives a cofinal family of actual integers
whose complete central first-layer debit cancels GMW's enlarged far
credit to leading order. It uses MS's strict actual products, the
owned effective PNT, HLD's full higher inventory and the unchanged
KTO/GMW/CPW observation. This is an obstruction to retaining a fixed
positive fraction of that credit through separate sector estimates.
It supplies no root-scale lower for the full defect, literature-priority
claim, Lean certification or RH/Robin proof.

### A complete pressure balance at the unchanged observation

Keep $A=\log n$, $L=\log A$, $T_A=\sqrt A L$, the same slow degree,
source and observer, and the exact cuts $Y_A,P_A$ from CPW and GMW.
Keep $\widetilde H_A=\beta_1^k(k-1)!/L^k$ and the actual far
pressure $U'_A$ from GMW4. KTO1 and KTO11 give

$$
\mathcal J(A):=V_A-M(\lambda(A))
=I_\psi(A)+o(1/T_A).
\tag{ACC1}
$$

Let
$F_{\mathrm{cen}}(q)=\sum_{Y_A<p\le P_A}\log p\,(r_p-q)_+$ and
$\mathcal J_{\mathrm{cen}}(A)
=\int F_{\mathrm{cen}}(\lambda(Av))\,d\omega_A(v)
-F_{\mathrm{cen}}(\lambda(A))$.
The original-price far pressure is zero: $p>P_A>A$ implies
$r_p<1/(p\log p)<\lambda(A)$.
CPW3 and exact mass/price identify the low pressure gap with
$J_{\mathrm{low}}(A)$; HLD6 retains the complete higher gap.
The disjoint pressure account therefore gives

$$
\mathcal J_{\mathrm{cen}}(A)
=I_\psi(A)-U'_A+o(1/T_A)
=-\widetilde H_A(1+o(1)).
\tag{ACC2}
$$

Here the effective PNT input used in ACP1 bounds
$|I_\psi(A)|\le Ce^{-a\sqrt L}=o(\widetilde H_A)$ for fixed
$C,a>0$. GMW8 and $T_A\widetilde H_A\to\infty$ pay the other
relative errors. No root-smallness of $U'_A$ is asserted.
All pressure integrals are absolute by KTO, GMW, HLD and CPW.
This balance alone concerns pressure: the complete central defect
still retains its nonnegative original-price baseline.

### Use actual strict products at their own size

Reuse MS's actual products

$$
N_x=\prod_p p^{a_p(x)},\qquad
 a_p(x)=\#\{j\ge1:r_{p,j}>\lambda(x)\},\qquad
 A_x=\log N_x.
$$

All equality layers are excluded. The owned finite-layer pressure
formula gives

$$
W(N_x)=M(\lambda(x))+\lambda(x)A_x.
\tag{ACC3}
$$

Every active first prime has $p<x$. Conversely, $p\le x-1$ gives
$r_p>1/((p+1)\log p)>\lambda(x)$. Thus the first active mass lies
between $\vartheta(x-1)$ and $\vartheta(x)$.
Use the same effective PNT, including the endpoint allowance
$O(\log x)$, and HLD3/MS3's bound $O(\sqrt x)$ for the complete
higher active mass. For some fixed $a>0$,

$$
A_x=x+O\!\left(xe^{-a\sqrt{\log x}}\right),\qquad A_x\sim x.
\tag{ACC4}
$$

This retains every growing exponent layer. In particular the actual
integers $N_x$ are unbounded. It does not assert $A_x=x$ or zero
defect at their own-size price.

For large $x$, one has $A_x\in[x/2,2x]$. On the price interval
between $\lambda(x)$ and $\lambda(A_x)$, all pressure slopes have
absolute value at most $Cx$: even the weak endpoint inventory at
$2x$ is bounded by the strict inventory at $3x$, which is $O(x)$
by ACC4. The finite piecewise-affine pressure is therefore
$Cx$-Lipschitz on that interval, including all ties.
Use ACC3 and $|\lambda'(y)|=O(1/(x^2\log x))$ for
$y\in[x/2,2x]$. The full original-price defect of this same integer
satisfies

$$
\begin{aligned}
0\le d_{A_x}(N_x)
&=M(\lambda(A_x))-M(\lambda(x))
       +(\lambda(A_x)-\lambda(x))A_x\\
&\le\frac{C|A_x-x|}{x\log x}
\le\frac{Ce^{-a\sqrt{\log x}}}{\log x}
=o(\widetilde H_{A_x}).
\end{aligned}
\tag{ACC5}
$$

The last comparison uses GMW2--GMW3's
$\log\widetilde H_A=-\epsilon(\log L)^2+
O(\log L\log\log L)$; $\sqrt L$ dominates $(\log L)^2$.
ACC5 is only relative to this larger scale. It does not give
$d_{A_x}(N_x)=o(1/T_{A_x})$.

The original-price defect is the classical CA benefit, as recorded in [Erdős–Nicolas 1975](../ArithSums/erdosnicolas1975repartition.md). ACC5 uses the unrestricted pressure slope; it assumes none of Proposition 5's additional localization hypotheses.

### The complete central debit and far credit are jointly realized

Put $n=N_x$ and $A=A_x$ in all unchanged cuts and observations.
Since $A\sim x$, one has $P_A>x$ and $2Y_A<x$ eventually.
Every prime factor of $N_x$ is below $x$, so the exact far occupation
correction vanishes. CPW4 gives
$r_p>\lambda(2Y_A)>\lambda(x)$ for every $p\le Y_A$;
hence all low primes divide this same $N_x$. Consequently

$$
D_{\mathrm{far,new},A}(N_x)=U'_A
=\widetilde H_A(1+o(1)),\qquad
G_{\mathrm{low},A}(N_x)=0.
\tag{ACC6}
$$

The original-price central and higher baselines are nonnegative
parts of the full $d_A(N_x)$ and are each bounded by ACC5.
Exact mass and price mean, ACC2, HLD8 and CPW8 now give

$$
C_A(N_x)=-\widetilde H_A(1+o(1)),\qquad
D_{\mathrm{low},A}(N_x)=o(1/T_A),\qquad
D_{2,A}(N_x)=o(\widetilde H_A).
\tag{ACC7}
$$

These are the complete occupied-and-absent defect contributions,
not just their pressure terms. In particular the disjoint CPW9
account yields

$$
D_A(N_x)-D_{\mathrm{far,new},A}(N_x)
=-\widetilde H_A(1+o(1)),\qquad
D_A(N_x)=o(\widetilde H_A).
\tag{ACC8}
$$

Thus, for every fixed real $\alpha<1$, eventually along this cofinal
actual integer family, with the threshold allowed to depend on the
fixed $\alpha$,

$$
\begin{aligned}
C_A(N_x)+\alpha D_{\mathrm{far,new},A}(N_x)&<0,\\
[D_A(N_x)-D_{\mathrm{far,new},A}(N_x)]
       +\alpha D_{\mathrm{far,new},A}(N_x)&<0.
\end{aligned}
\tag{ACC9}
$$

Uniform separate-sector estimates that leave a fixed positive fraction
of the enlarged far credit cannot hold on all original integers.
The same actual integers realize both sides of the cancellation;
no separately optimized configurations are combined.
The intermediate pressure balance and near-price estimates are used
only to establish this actual-integer obstruction.

The surviving target remains the root-scale compensated account
$T_A\Delta(N_x)=T_Ad_A(N_x)+T_AI_\psi(A)+c_R+o(1)$.
Neither term on the right has been bounded here sufficiently at that
scale. No sign of $D_A(N_x)$, $\Delta(N_x)$ or a Robin violation is
inferred. A joint arithmetic estimate preserving the root reserve
can still succeed; RH and strict Robin for every $n>5040$ remain
unproved.
