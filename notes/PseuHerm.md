---
layout: note
title: Pseudo-Hermitian Geometry
permalink: /notes/PseuHerm
---

{% raw %}

# Preliminaries

Let $M^{2m+1}$ be a $(2m+1)$-dimensional smooth orientable manifold. A *CR structure* on $M^{2m+1}$ is a complex rank-$m$ subbundle $H^{1,0} $ of $ T(M)\otimes \mathbb{C}$ with the following properties 

$$
\begin{aligned}
H^{1,0} \cap H^{0,1}  =& \{0\}, \quad H^{0,1}  = \overline{H^{1,0} } \\
    [\Gamma (H^{1,0} ),\Gamma (H^{1,0} )] \subseteq &\, \Gamma(H^{1,0} ).
\end{aligned}
\tag{1.1}\label{1.1}
$$

    
The complex subbundle $H^{1,0} $ corresponds to a real rank $2m$ subbundle 
$H :=\Re\{H^{1,0} \oplus H^{0,1} \}$ of $T(M)$, which carries a
complex structure $J_{b}$ defined by 

$$
J_{b}(V+\overline{V})=i(V-\overline{V})
$$

 for any $V\in H^{1,0} $. The synthetic object $(M,H^{1,0} )$ or $ (M,H ,J_{b})$ is called a *CR manifold*.

**Remark.**
	Formally integrable condition is equivalent to
$$
\begin{gathered}
{\left[J_{b} X, Y\right]+\left[X, J_{b} Y\right] \in \Gamma^{\infty}(U, H(M)),} \\
{\left[J_{b} X, J_{b} Y\right]-[X, Y]=J_{b}\left\{\left[J_{b} X, Y\right]+\left[X, J_{b} Y\right]\right\}}
\end{gathered}
$$
for all $X, Y \in \mathfrak{X}_{\mathcal{H}}$. 

Let $E$ be a real line bundle of $T^{\ast }M$, whose fiber at each point $ x\in M$ is given by 

$$
E_{x}=\{\omega \in T_{x}^{\ast }M:\ker \omega \supseteq H_{x} \}.
$$

 Since both $TM$ and $H $ are orientable vector bundles on $M$, the real
line bundle $E$ is orientable, so $E$ has globally defined nowhere vanishing
sections. Any such a section $\theta \in \Gamma (E\backslash \{0\})$ is
referred to as a *pseudo-Hermitian 1-form* on $M$.

Given a pseudo-Hermitian $1$-form $\theta $ on $M$, we have the *Levi form* $ L_{\theta }$ corresponding to $\theta $, which is defined by 

$$
L_{\theta }(X,Y)=d\theta (X,J_{b}Y)
\tag{1.2}\label{1.2}
$$

 for any $X,Y\in H $. The second condition in $\ref{1.1}$ implies that $ L_{\theta }$ is $J_{b}$-invariant, and thus symmetric. If $L_{\theta }$ is
positive definite on $H $ for some $\theta $, $(M,H^{1,0} )$ is said to
be *strictly pseudoconvex*. From now on, we will always assume that $ (M,H^{1,0} )$ is a strictly pseudoconvex CR manifold endowed with a
pseudo-Hermitian $1$-form $\theta $, such that its Levi form $L_{\theta }$
is positive definite. In this case  the synthetic object $(M,H^{1,0} ,\theta )$ is
referred to as a *pseudo-Hermitian manifold*.

**Remark.**
    For any $Z,W \in H^{1,0}(M)$,  
    $$
L_{\theta}(Z, \overline{W})=-i(d \theta)(Z, \overline{W}):=G_{\theta }(Z, \overline{W}).
$$

Let $(M^{2m+1},H^{1,0} , \theta )$ be a pseudo-Hermitian manifold. Clearly $ \theta $ is a contact form. Thus there is a unique vector field $\xi \in
\Gamma (T(M))$, called the *Reeb vector field*, such that

$$
\theta (\xi )=1\text{, \ }i_{\xi }d\theta =0 ,
\tag{1.3}\label{1.3}
$$

where $i_{\xi }$ denotes the interior product with respect to $\xi $. The
collection of all its integral curves forms an oriented one-dimensional
foliation $\mathcal{F}_{\xi }$ on $M$, which is called the *Reeb foliation*. The first condition in $\ref{1.3}$ implies that $\xi $ is
transversal to $H $. Therefore $T(M)$ admits a decomposition 

$$
T(M)=H \oplus V_{\xi },
\tag{1.4}\label{1.4}
$$

 where $V_{\xi }:= \mathbb{R}
\xi $ is a trivial line bundle on $M$. In terms of terminology from
foliation theory, $H $ and $V_{\xi }$ are called the horizontal and
vertical distributions respectively. Let $\pi _{H}:TM\rightarrow H $ and $ \pi _{V}:TM\rightarrow V_{\xi }$ be the natural projections associated with
the direct sum decomposition $\ref{1.4}$. In terms of $\theta $, the Levi
form $L_{\theta }$ can be extended to a Riemannian metric

$$
g_{\theta }=L_{\theta }(\pi _{H},\pi _{H})+\theta \otimes \theta,
\tag{1.5}\label{1.5}
$$

which is called the Webster metric. It is convenient to extend the complex
structure $J_{b}$ on $H $ to an endomorphism $J$ of $T(M)$ by requiring
that 

$$
J\mid _{H }=J_{b}\text{ \ and \ }J\mid _{V_{\xi }}=0 ,
\tag{1.6}\label{1.6}
$$

 where $\mid $ denotes the fiberwise restriction.
 Define the $2$-form $\Omega$ by 
 

$$
\Omega(X,Y):=g_{\theta}(X,JY)=-d \theta (X,Y).
$$

It is known that there exists a unique linear connection $\nabla $ on $ (M^{2m+1},H^{1,0} ,\theta )$, called the *Tanaka-Webster connection*,
such that (cf. [DT2006differential], [TA1975adifferential], [We1978pseudo])

1. $\nabla _{X}\Gamma (H )\subseteq \Gamma (H )$ and $\nabla _{X}J=0$
for any $X\in \Gamma (TM)$;

2. $\nabla g_{\theta }=0$;

3. $T_{\nabla }(X,Y)=2d\theta (X,Y)\xi $ \ and $T_{\nabla }(\xi
,JX)+JT_{\nabla }(\xi ,X)=0$ for any $X,Y\in H $, where $T_{\nabla }(\cdot
,\cdot )$ denotes the torsion of the connection $\nabla $.

Note that (3) is equivalent to that $T_{\nabla }$ is pure(compared to Chern connection), that is, 
$$ \begin{aligned}
    T_{\nabla }(Z,W)=&0,\\
    T_{\nabla }(Z,\overline{W})=& 2 i L_{\theta }(Z,\overline{W}) \xi ,\\
    \tau \circ J+J \circ \tau =&0,
\end{aligned}  $$ 
for any $Z,W \in H^{1,0}(M)$. See [dongren2024dgpseudo] for more information.
**Remark.**
    One has 
    $$ T^{\nabla }(X,Y) = 2 g_{\theta }(JX,Y) \xi +\theta (X) \tau Y-\theta (Y) \tau X,  $$
    or (be careful with the wedge convention)
     $$ T_{\nabla }=2(\theta  \wedge \tau -\Omega \otimes  \xi ) .$$ 
     Also, 
    $$ \tau \circ J+J \circ \tau =0; $$
    $$ J^2 Y=-Y+\theta (Y) \xi , \quad \forall Y \in T(M); $$
    $$ [\xi ,X] \in \mathfrak{X}_{H}, \quad \forall X \in \mathfrak{X}_H.$$

One important partial component of $T_{\nabla }$ is the pseudo-Hermitian
torsion $\tau $ given by 

$$
\tau (X)=T_{\nabla }(\xi ,X)
\tag{1.7}\label{1.7}
$$

 for any $X\in TM$. Then $(M,H^{1,0} ,\theta )$ is said to be *Sasakian* if $\tau =0$.

For the pseudo-Hermitian manifold $(M,H^{1,0} ,\theta )$, we choose a
local orthonormal frame field $\{e_{A}\}_{A=0}^{2m}=\{\xi
,e_{1},...,e_{m},e_{m+1},...,e_{2m}\}$ with respect to $g_{\theta }$ such
that 

$$
\{e_{m+1},...,e_{2m}\}=\{Je_{1},...,Je_{m}\}.
$$

 Such a frame field $\{e_{A}\}_{A=0}^{2m}$ is referred to as an adapted frame
field $M$. Set 

$$
\eta _{j}=\frac{1}{\sqrt{2}}\left( e_{j}-\sqrt{-1}Je_{j}\right) \text{, \ } \eta _{\bar{j}}=\overline{\eta _{j}}\text{ \ (}j=1,...,m\text{).}
\tag{1.8}\label{1.8}
$$

 Let $\{\theta ^{j}\}_{j =1}^{m}$ be the dual frame field of $\{\eta
_{j}\}_{j=1}^{m}$. By the properties of the Tanaka-Webster connection $ \nabla $, we have (cf. [DT2006differential]) 

$$
\nabla \xi =0\text{, \ }\nabla \eta _{j}=\theta _{j}^{i}\otimes \eta _{i} \text{, \ }\nabla \eta _{\overline{j}}=\theta _{\overline{j}}^{\overline{i} }\otimes \eta _{\overline{i}} ,
\tag{1.9}\label{1.9}
$$

 where $\{\theta _{j}^{i}\}$ denotes the connection $1$-forms with respect to
the frame field. Since 
$$\tau (H^{1,0} )\subset H^{0,1} ,$$ 
one may write 

$$
\begin{aligned}
\tau &=\tau ^{i}\eta _{i}+\tau ^{\overline{i}}\eta _{\overline{i}}  \\
&=A_{\overline{j}}^{i}\theta ^{\overline{j}}\otimes \eta _{i}+A_{j}^{ \overline{i}}\theta ^{j}\otimes \eta _{\overline{i}}.
\end{aligned}
\tag{1.10}\label{1.10}
$$

**Remark.**
    Set 
    $$ A(X,Y)=g_{\theta }(\tau X,Y) $$
    for any $X,Y \in T(M) .$ 
    Then we have $A(X,Y)=A(Y,X)$. 
    Writing $A_{ij}=A(\eta_i,\eta_j)$ and $h_{i \bar j}=g_{\theta }(\eta_i,\eta_{\bar j})$, then 
    $$A_{ij}=A_{i}^{\bar k}h_{\bar k j}.$$  

From [We1978pseudo], we know that $\{\theta ,\theta ^{i},\theta_{j}^{i}\}$
satisfy the following structure equations (cf. also Section 1.4 in [DT2006differential] ) 

$$
\begin{aligned}
d\theta &=2\sqrt{-1}\theta ^{i}\wedge \theta ^{\overline{i}}\text{,}  \\
d\theta ^{i} &=-\theta _{j}^{i}\wedge \theta ^{j}+A_{\bar{j} }^{i}\theta \wedge \theta ^{\overline{j}}\text{,}   \\
d\theta _{j}^{i} &=-\theta _{k}^{i}\wedge \theta _{j}^{k}+\Pi _{j}^{i}
\end{aligned}
\tag{1.11}\label{1.11}
$$

 with

$$
\begin{aligned}
\Pi _{j}^{i} &=2\sqrt{-1}(\theta ^{i}\wedge \tau ^{\overline{j}}-\tau
^{i}\wedge \theta ^{\overline{j}})+R_{jk\bar{l}}^{i}\theta ^{k}\wedge
\theta ^{\overline{l}}  \\
&+W_{j\overline{k}}^{i}\theta \wedge \theta ^{\overline{k} }-W_{jk}^{i}\theta \wedge \theta ^{k} ,
\end{aligned}
\tag{1.12}\label{1.12}
$$

 where $W_{j\overline{k}}^{i}=A_{\overline{k},j}^{i}$, $W_{jk}^{i}=A_{j, \overline{i}}^{\overline{k}}$ are the covariant derivatives of $A$ and $R_{jk \bar{l}}^{i}$ are the components of curvature tensor of the
Tanaka-Webster connection.

**Lemma** (CDRY2019onharm).  <!-- lemDiv -->
Let $(M^{2m+1},H,J,\theta )$ be a pseudo-Hermitian manifold with
Tanaka-Webster connection $\nabla $. Let $X$ and $\rho $ be a vector field
and $1$-form on $M$ respectively. Then 

$$
\\operatorname{div} X=\sum_{A=0}^{2m}g_{\theta }(\nabla _{e_{A}}X,e_{A})\text{ \ and \ 
}\delta \rho =-\sum_{A=0}^{2m}(\nabla _{e_{A}}\rho )(e_{A}),
$$

 where $\{e_{A}\}_{A=0}^{2m}=\{\xi ,e_{1},...,e_{2m}\}$ is an orthonormal
frame field on $M$. Here $\\operatorname{div}(\cdot )$ and $\delta (\cdot )$ denote
the divergence and codifferential respectively.

**Proposition (Relation with Levi-Civita connection).**
    Let $\nabla ^{\theta }$ be the Levi-Civita connection of Webster metric, then  
    

$$
\nabla ^{\theta }=\nabla +(\Omega -A) \xi +\tau  \otimes \theta +2 \theta \odot  J
$$

   and
   

$$
\\operatorname{tr}_{g_{\theta }}(\nabla ^{\theta }-\nabla )=\\operatorname{tr}_{G_{\theta }}(\nabla ^{\theta }-\nabla )=0.
\tag{15}\label{15}
$$

   
   For curvature tensor, we have 
       $$ \begin{aligned}
    R^\theta(X, Y) Z=R(X, Y) & Z+(L X \wedge L Y) Z-2 \Omega(X, Y) J Z \\
    & -g_\theta(S(X, Y), Z) \xi +\theta(Z) S(X, Y) \\
    & -2 g_\theta((\theta \wedge \mathcal{O})(X, Y), Z) \xi +2 \theta(Z)(\theta \wedge \mathcal{O})(X, Y),
    \end{aligned} $$
    for any $X,Y,Z \in TM$. 
    where 
    $$ S(X,Y)=(\nabla _{X}\tau )Y-(\nabla _{Y}\tau )X ,$$
    $$ \mathcal{O}=\tau ^2+2J \tau -I ,\quad L:=\nabla ^{\theta } \xi =\tau +J.$$

**Remark.**
    One has 
    $$ \nabla ^{\theta }_{\xi }\xi =0, \qquad \\operatorname{div} \xi =0. $$

**Proposition.**
    The Levi distribution $H(M)$ is minimal and 
    $$ \\operatorname{tr} (\tau) =0. $$

{% endraw %}
