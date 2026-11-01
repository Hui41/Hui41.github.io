---
layout: note
title: Pseudo-Hermitian Geometry
permalink: /notes/PseuHerm
---

## Preliminaries

Let $M^{2m+1}$ be a $(2m+1)$-dimensional smooth orientable manifold. A \emph{%
CR structure} on $M^{2m+1}$ is a complex rank-$m$ subbundle $H^{1,0} $ of $%
T(M)\otimes \mathbb{C}$ with the following properties 
\begin{align}
    H^{1,0} \cap H^{0,1}  =& \{0\}, \quad H^{0,1}  = \overline{H^{1,0} } \notag \\
    [\Gamma (H^{1,0} ),\Gamma (H^{1,0} )] \subseteq &\, \Gamma(H^{1,0} ). \label{1.1}
    \end{align}    
The complex subbundle $H^{1,0} $ corresponds to a real rank $2m$ subbundle 
$H :=\Re\{H^{1,0} \oplus H^{0,1} \}$ of $T(M)$, which carries a
complex structure $J_{b}$ defined by 
\begin{equation*}
J_{b}(V+\overline{V})=i(V-\overline{V})
\end{equation*}%
for any $V\in H^{1,0} $. The synthetic object $(M,H^{1,0} )$ or $%
(M,H ,J_{b})$ is called a \emph{CR manifold}.

\begin{remark}
	Formally integrable condition is equivalent to
$$
\begin{gathered}
{\left[J_{b} X, Y\right]+\left[X, J_{b} Y\right] \in \Gamma^{\infty}(U, H(M)),} \\
{\left[J_{b} X, J_{b} Y\right]-[X, Y]=J_{b}\left\{\left[J_{b} X, Y\right]+\left[X, J_{b} Y\right]\right\}}
\end{gathered}
$$
for all $X, Y \in \mathfrak{X}_{\mathcal{H}}$. 
\end{remark}

Let $E$ be a real line bundle of $T^{\ast }M$, whose fiber at each point $%
x\in M$ is given by%
\begin{equation*}
E_{x}=\{\omega \in T_{x}^{\ast }M:\ker \omega \supseteq H_{x} \}.
\end{equation*}%
Since both $TM$ and $H $ are orientable vector bundles on $M$, the real
line bundle $E$ is orientable, so $E$ has globally defined nowhere vanishing
sections. Any such a section $\theta \in \Gamma (E\backslash \{0\})$ is
referred to as a \emph{pseudo-Hermitian 1-form} on $M$.

Given a pseudo-Hermitian $1$-form $\theta $ on $M$, we have the \textit{Levi form} $%
L_{\theta }$ corresponding to $\theta $, which is defined by%
\begin{equation}
L_{\theta }(X,Y)=d\theta (X,J_{b}Y)  \label{1.2}
\end{equation}%
for any $X,Y\in H $. The second condition in (\ref{1.1}) implies that $%
L_{\theta }$ is $J_{b}$-invariant, and thus symmetric. If $L_{\theta }$ is
positive definite on $H $ for some $\theta $, $(M,H^{1,0} )$ is said to
be \textit{strictly pseudoconvex}. From now on, we will always assume that $%
(M,H^{1,0} )$ is a strictly pseudoconvex CR manifold endowed with a
pseudo-Hermitian $1$-form $\theta $, such that its Levi form $L_{\theta }$
is positive definite. In this case  the synthetic object $(M,H^{1,0} ,\theta )$ is
referred to as a \textit{pseudo-Hermitian manifold}.

\begin{remark}
    For any $Z,W \in H^{1,0}(M)$,  
    $$
L_{\theta}(Z, \overline{W})=-i(d \theta)(Z, \overline{W}):=G_{\theta }(Z, \overline{W}).
$$
\end{remark}

Let $(M^{2m+1},H^{1,0} , \theta )$ be a pseudo-Hermitian manifold. Clearly $%
\theta $ is a contact form. Thus there is a unique vector field $\xi \in
\Gamma (T(M))$, called the \emph{Reeb vector field}, such that
\begin{equation}
\theta (\xi )=1\text{, \ }i_{\xi }d\theta =0 , \label{1.3}
\end{equation}
where $i_{\xi }$ denotes the interior product with respect to $\xi $. The
collection of all its integral curves forms an oriented one-dimensional
foliation $\mathcal{F}_{\xi }$ on $M$, which is called the \emph{Reeb
foliation}. The first condition in (\ref{1.3}) implies that $\xi $ is
transversal to $H $. Therefore $T(M)$ admits a decomposition%
\begin{equation}
T(M)=H \oplus V_{\xi },  \label{1.4}
\end{equation}%
where $V_{\xi }:=%
%TCIMACRO{\U{211d} }%
%BeginExpansion
\mathbb{R}
%EndExpansion
\xi $ is a trivial line bundle on $M$. In terms of terminology from
foliation theory, $H $ and $V_{\xi }$ are called the horizontal and
vertical distributions respectively. Let $\pi _{H}:TM\rightarrow H $ and $%
\pi _{V}:TM\rightarrow V_{\xi }$ be the natural projections associated with
the direct sum decomposition (\ref{1.4}). In terms of $\theta $, the Levi
form $L_{\theta }$ can be extended to a Riemannian metric
\begin{equation}
g_{\theta }=L_{\theta }(\pi _{H},\pi _{H})+\theta \otimes \theta,  \label{1.5}
\end{equation}
which is called the Webster metric. It is convenient to extend the complex
structure $J_{b}$ on $H $ to an endomorphism $J$ of $T(M)$ by requiring
that 
\begin{equation}
J\mid _{H }=J_{b}\text{ \ and \ }J\mid _{V_{\xi }}=0 , \label{1.6}
\end{equation}%
where $\mid $ denotes the fiberwise restriction.
 Define the $2$-form $\Omega$ by 
 \begin{equation}
    \Omega(X,Y):=g_{\theta}(X,JY)=-d \theta (X,Y).
 \end{equation}


It is known that there exists a unique linear connection $\nabla $ on $%
(M^{2m+1},H^{1,0} ,\theta )$, called the \emph{Tanaka-Webster connection},
such that (cf. \cite{DT2006differential}, \cite{TA1975adifferential}, \cite{We1978pseudo})
\begin{enumerate}
\item $\nabla _{X}\Gamma (H )\subseteq \Gamma (H )$ and $\nabla _{X}J=0$
for any $X\in \Gamma (TM)$;

\item $\nabla g_{\theta }=0$;

\item $T_{\nabla }(X,Y)=2d\theta (X,Y)\xi $ \ and $T_{\nabla }(\xi
,JX)+JT_{\nabla }(\xi ,X)=0$ for any $X,Y\in H $, where $T_{\nabla }(\cdot
,\cdot )$ denotes the torsion of the connection $\nabla $.
\end{enumerate}

Note that (3) is equivalent to that $T_{\nabla }$ is pure(compared to Chern connection), that is, 
$$ \begin{aligned}
    T_{\nabla }(Z,W)=&0,\\
    T_{\nabla }(Z,\overline{W})=& 2 i L_{\theta }(Z,\overline{W}) \xi ,\\
    \tau \circ J+J \circ \tau =&0,
\end{aligned}  $$ 
for any $Z,W \in H^{1,0}(M)$. See \cite{dongren2024dgpseudo} for more information.
\begin{remark}
    One has 
    $$ T^{\nabla }(X,Y) = 2 g_{\theta }(JX,Y) \xi +\theta (X) \tau Y-\theta (Y) \tau X,  $$
    or (be careful with the wedge convention)
     $$ T_{\nabla }=2(\theta  \wedge \tau -\Omega \otimes  \xi ) .$$ 
     Also, 
    $$ \tau \circ J+J \circ \tau =0; $$
    $$ J^2 Y=-Y+\theta (Y) \xi , \quad \forall Y \in T(M); $$
    $$ [\xi ,X] \in \mathfrak{X}_{H}, \quad \forall X \in \mathfrak{X}_H.$$
\end{remark}



One important partial component of $T_{\nabla }$ is the pseudo-Hermitian
torsion $\tau $ given by%
\begin{equation}
\tau (X)=T_{\nabla }(\xi ,X)  \label{1.7}
\end{equation}%
for any $X\in TM$. Then $(M,H^{1,0} ,\theta )$ is said to be \emph{Sasakian%
} if $\tau =0$.

For the pseudo-Hermitian manifold $(M,H^{1,0} ,\theta )$, we choose a
local orthonormal frame field $\{e_{A}\}_{A=0}^{2m}=\{\xi
,e_{1},...,e_{m},e_{m+1},...,e_{2m}\}$ with respect to $g_{\theta }$ such
that 
\begin{equation*}
\{e_{m+1},...,e_{2m}\}=\{Je_{1},...,Je_{m}\}.
\end{equation*}%
Such a frame field $\{e_{A}\}_{A=0}^{2m}$ is referred to as an adapted frame
field $M$. Set 
\begin{equation}
\eta _{j}=\frac{1}{\sqrt{2}}\left( e_{j}-\sqrt{-1}Je_{j}\right) \text{, \ }%
\eta _{\bar{j}}=\overline{\eta _{j}}\text{ \ (}j=1,...,m\text{).}
\label{1.8}
\end{equation}%
Let $\{\theta ^{j}\}_{j =1}^{m}$ be the dual frame field of $\{\eta
_{j}\}_{j=1}^{m}$. By the properties of the Tanaka-Webster connection $%
\nabla $, we have (cf. \cite{DT2006differential})%
\begin{equation}
\nabla \xi =0\text{, \ }\nabla \eta _{j}=\theta _{j}^{i}\otimes \eta _{i}%
\text{, \ }\nabla \eta _{\overline{j}}=\theta _{\overline{j}}^{\overline{i}%
}\otimes \eta _{\overline{i}} , \label{1.9}
\end{equation}%
where $\{\theta _{j}^{i}\}$ denotes the connection $1$-forms with respect to
the frame field. Since 
$$\tau (H^{1,0} )\subset H^{0,1} ,$$ 
one may write 
\begin{eqnarray}
\tau &=&\tau ^{i}\eta _{i}+\tau ^{\overline{i}}\eta _{\overline{i}}  \notag
\\
&=&A_{\overline{j}}^{i}\theta ^{\overline{j}}\otimes \eta _{i}+A_{j}^{%
\overline{i}}\theta ^{j}\otimes \eta _{\overline{i}}.  \label{1.10}
\end{eqnarray}

\begin{remark}
    Set 
    $$ A(X,Y)=g_{\theta }(\tau X,Y) $$
    for any $X,Y \in T(M) .$ 
    Then we have $A(X,Y)=A(Y,X)$. 
    Writing $A_{ij}=A(\eta_i,\eta_j)$ and $h_{i \bar j}=g_{\theta }(\eta_i,\eta_{\bar j})$, then 
    $$A_{ij}=A_{i}^{\bar k}h_{\bar k j}.$$  
\end{remark}

From \cite{We1978pseudo}, we know that $\{\theta ,\theta ^{i},\theta_{j}^{i}\}$
satisfy the following structure equations (cf. also \S 1.4 in \cite{DT2006differential}%
)%
\begin{eqnarray}
d\theta &=&2\sqrt{-1}\theta ^{i}\wedge \theta ^{\overline{i}}\text{,}  \notag
\\
d\theta ^{i} &=&-\theta _{j}^{i}\wedge \theta ^{j}+A_{\bar{j}%
}^{i}\theta \wedge \theta ^{\overline{j}}\text{,}  \label{1.11} \\
d\theta _{j}^{i} &=&-\theta _{k}^{i}\wedge \theta _{j}^{k}+\Pi _{j}^{i} 
\notag
\end{eqnarray}%
with
\begin{eqnarray}
\Pi _{j}^{i} &=&2\sqrt{-1}(\theta ^{i}\wedge \tau ^{\overline{j}}-\tau
^{i}\wedge \theta ^{\overline{j}})+R_{jk\bar{l}}^{i}\theta ^{k}\wedge
\theta ^{\overline{l}}  \notag \\
&&+W_{j\overline{k}}^{i}\theta \wedge \theta ^{\overline{k}%
}-W_{jk}^{i}\theta \wedge \theta ^{k} , \label{1.12}
\end{eqnarray}%
where $W_{j\overline{k}}^{i}=A_{\overline{k},j}^{i}$, $W_{jk}^{i}=A_{j,%
\overline{i}}^{\overline{k}}$ are the covariant derivatives of $A$ and $R_{jk%
\bar{l}}^{i}$ are the components of curvature tensor of the
Tanaka-Webster connection.



\begin{lemma}[{\protect\cite{CDRY2019onharm}}]\label{lemDiv}
Let $(M^{2m+1},H,J,\theta )$ be a pseudo-Hermitian manifold with
Tanaka-Webster connection $\nabla $. Let $X$ and $\rho $ be a vector field
and $1$-form on $M$ respectively. Then%
\begin{equation*}
\di X=\sum_{A=0}^{2m}g_{\theta }(\nabla _{e_{A}}X,e_{A})\text{ \ and \ 
}\delta \rho =-\sum_{A=0}^{2m}(\nabla _{e_{A}}\rho )(e_{A}),
\end{equation*}%
where $\{e_{A}\}_{A=0}^{2m}=\{\xi ,e_{1},...,e_{2m}\}$ is an orthonormal
frame field on $M$. Here $\di(\cdot )$ and $\delta (\cdot )$ denote
the divergence and codifferential respectively.
\end{lemma}


\begin{proposition}[Relation with Levi-Civita connection]
    Let $\nabla ^{\theta }$ be the Levi-Civita connection of Webster metric, then  
    \begin{equation}
        \nabla ^{\theta }=\nabla +(\Omega -A) \xi +\tau  \otimes \theta +2 \theta \odot  J 
    \end{equation}
   and
   \begin{equation}\label{15}
     \trace_{g_{\theta }}(\nabla ^{\theta }-\nabla )=\trace_{G_{\theta }}(\nabla ^{\theta }-\nabla )=0. 
   \end{equation}
   
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
\end{proposition}

\begin{remark}
    One has 
    $$ \nabla ^{\theta }_{\xi }\xi =0, \qquad \di \xi =0. $$
\end{remark}

\begin{proposition}
    The Levi distribution $H(M)$ is minimal and 
    $$ \trace (\tau) =0. $$ 
\end{proposition}
