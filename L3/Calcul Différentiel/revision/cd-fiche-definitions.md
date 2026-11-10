---
aliases:
  - "Fiche de définitions CD"
  - "toutes les définitions de calcul différentiel"
tags:
  - cd
  - cd/revision
---

# 📘 Fiche de révision – toutes les définitions

Toutes les définitions du cours sur une seule page, dans l'ordre des chapitres, avec leurs quantificateurs. Mode d'emploi : lire un encadré, le cacher, le réécrire de mémoire, comparer. · [[cd-plan-de-revision|↩ Plan de révision]] · [[cd-index-definitions|↩ Index]] · Suite : [[cd-fiche-theoremes]]

## 1 – Espaces vectoriels normés

> [!note] **Norme, espace vectoriel normé** (Déf. 1.1)
> Soit $E$ un espace vectoriel sur $\mathbb K$ ($\mathbb R$ ou $\mathbb C$). Une **norme** sur $E$ est une application $N:E\to\mathbb R_+$ vérifiant :
> - **(N1) séparation** : $\forall x\in E,\ N(x)=0\iff x=0_E$ ;
> - **(N2) homogénéité** : $\forall\lambda\in\mathbb K,\ \forall x\in E,\ N(\lambda x)=\lvert \lambda\rvert\,N(x)$ ;
> - **(N3) inégalité triangulaire** : $\forall (x,y)\in E^2,\ N(x+y)\le N(x)+N(y)$.
>
> Un espace vectoriel muni d'une norme est un **espace vectoriel normé** (e.v.n.). On note souvent $\lVert x\rVert$ au lieu de $N(x)$.
> → [[norme|fiche complète]]

> [!note] **Boules et sphères** (Déf. 1.6)
> Soit $(E,\lVert \cdot\rVert)$ un e.v.n., $a\in E$ et $r>0$.
> - **boule ouverte** : $B(a,r)=\{x\in E\mid \lVert a-x\rVert<r\}$ ;
> - **boule fermée** : $\overline B(a,r)=\{x\in E\mid \lVert a-x\rVert\le r\}$ ;
> - **sphère** : $S(a,r)=\{x\in E\mid \lVert a-x\rVert=r\}$.
> → [[boules-spheres|fiche complète]]

> [!note] **Norme produit** (Prop. 1.8)
> Soient $(E_1,N_1),\dots,(E_p,N_p)$ des e.v.n. et $E=E_1\times\dots\times E_p$. Pour $x=(x_1,\dots,x_p)\in E$ on pose
> $$N(x)=\max_{1\le i\le p}N_i(x_i).$$
> $N$ est une norme sur $E$ : c'est la **norme produit**.
> → [[norme-produit|fiche complète]]

> [!note] **Normes équivalentes** (Déf. 1.10)
> Deux normes $N_1$ et $N_2$ sur $E$ sont **équivalentes** s'il existe $\alpha>0$ et $\beta>0$ tels que
> $$\forall x\in E,\qquad \alpha N_1(x)\le N_2(x)\le\beta N_1(x).$$
> → [[normes-equivalentes|fiche complète]]

> [!note] **Suite convergente** (Déf. 1.15)
> Soit $(E,\lVert \cdot\rVert)$ un e.v.n., $(x_n)$ une suite de $E$ et $\ell\in E$. La suite $(x_n)$ **converge vers** $\ell$ si
> $$\forall\varepsilon>0,\ \exists N_\varepsilon\in\mathbb N,\ \forall n\ge N_\varepsilon,\quad \lVert x_n-\ell\rVert<\varepsilon.$$
> Autrement dit : $x_n\to\ell$ dans $E$ $\iff$ la suite **réelle** $\lVert x_n-\ell\rVert$ tend vers $0$.
> → [[suite-convergente|fiche complète]]

> [!note] **Ouvert, fermé** (Déf. 1.20)
> Soit $(E,\lVert \cdot\rVert)$ un e.v.n. et $A\subset E$.
> - $A$ est un **ouvert** si $A=\emptyset$ ou si $\forall x\in A,\ \exists r>0,\ B(x,r)\subset A$.
> - $A$ est un **fermé** si son complémentaire $E\setminus A$ est ouvert.
> → [[ouvert-ferme|fiche complète]]

> [!note] **Voisinage** (Déf. 1.26)
> Soit $a\in E$. Une partie $V$ contenant $a$ est un **voisinage** de $a$ s'il existe un ouvert $O$ tel que $a\in O\subset V$.
> → [[voisinage|fiche complète]]

> [!note] **Continuité en un point** (Déf. 1.28)
> $f:E\to F$ est **continue en** $a\in E$ si
> $$\forall\varepsilon>0,\ \exists\delta>0,\ \forall x\in E,\quad \lVert x-a\rVert_E<\delta\ \Longrightarrow\ \lVert f(x)-f(a)\rVert_F<\varepsilon.$$
> $f$ est continue sur $A\subset E$ si elle est continue en tout point de $A$.
> → [[continuite|fiche complète]]

> [!note] **Continuité uniforme** (Déf. 1.31)
> $f:E\to F$ est **uniformément continue** si
> $$\forall\varepsilon>0,\ \exists\delta>0,\ \forall(x,y)\in E^2,\quad \lVert x-y\rVert_E<\delta\ \Longrightarrow\ \lVert f(x)-f(y)\rVert_F<\varepsilon.$$
> → [[continuite-uniforme|fiche complète]]

> [!note] **Application lipschitzienne** (Déf. 1.33)
> $f:E\to F$ est **lipschitzienne** s'il existe $k\ge0$ tel que
> $$\forall(x,y)\in E^2,\qquad \lVert f(x)-f(y)\rVert_F\le k\,\lVert x-y\rVert_E.$$
> On dit alors que $f$ est $k$-lipschitzienne.
> → [[application-lipschitzienne|fiche complète]]

> [!note] **Application linéaire continue, espace Lc(E,F)** (§ 1.9)
> On note $\mathcal L_c(E,F)$ l'espace vectoriel des applications **linéaires et continues** de $E$ dans $F$. Une application linéaire $f:E\to F$ est continue si et seulement si
> $$\exists C\ge0,\ \forall u\in E,\qquad \lVert f(u)\rVert_F\le C\,\lVert u\rVert_E$$
> ([[caracterisation-lineaires-continues|Théorème 1.43]]).
> → [[application-lineaire-continue|fiche complète]]

> [!note] **Norme d'opérateur** (Déf. 1.48)
> Pour $f\in\mathcal L_c(E,F)$, on pose
> $$\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert=\sup_{\lVert u\rVert_E\le1}\lVert f(u)\rVert_F.$$
> Ce sup est fini (Th. 1.43 (iii)), et $(\mathcal L_c(E,F),\lvert\!\lvert\!\lvert \cdot\rvert\!\rvert\!\rvert)$ est un e.v.n. (Prop. 1.49).
> → [[norme-operateur|fiche complète]]

> [!note] **Application bilinéaire (continue)** (Déf. 1.52)
> Soient $E_1,E_2,F$ des e.v.n. $B:E_1\times E_2\to F$ est **bilinéaire** si elle est linéaire par rapport à chaque variable, l'autre étant fixée :
> $$B(u+\lambda u',v)=B(u,v)+\lambda B(u',v),\qquad B(u,v+\lambda v')=B(u,v)+\lambda B(u,v').$$
> → [[application-bilineaire|fiche complète]]

> [!note] **Suite de Cauchy** (Déf. 1.56)
> Une suite $(x_n)$ de $(E,\lVert \cdot\rVert)$ est **de Cauchy** si
> $$\forall\varepsilon>0,\ \exists N_\varepsilon\in\mathbb N,\ \forall p,q\ge N_\varepsilon,\qquad \lVert x_p-x_q\rVert<\varepsilon.$$
> → [[suite-de-cauchy|fiche complète]]

> [!note] **Espace complet, espace de Banach** (Déf. 1.58)
> Un e.v.n. est **complet** si toute suite de Cauchy y converge. Un e.v.n. complet est un **espace de Banach**.
> → [[espace-de-banach|fiche complète]]


## 2 – Applications différentiables

> [!note] **Petit o** (Déf. 2.1)
> Soit $W\subset E$ un voisinage de $0_E$ et $\delta:W\to F$. On écrit $\delta(h)=o(h)$ au voisinage de $0$ si
> $$\lim_{h\to0_E}\frac{\lVert \delta(h)\rVert_F}{\lVert h\rVert_E}=0.$$
> De façon équivalente : $\delta(h)=\lVert h\rVert\,\varepsilon(h)$ avec $\varepsilon(h)\to0$ quand $h\to0$.
> → [[petit-o|fiche complète]]

> [!note] **Différentiabilité en un point, différentielle** (Déf. 2.3)
> $f$ est **différentiable en** $a$ s'il existe une application **linéaire continue** $L\in\mathcal L_c(E,F)$ et une application $\varepsilon:U\to F$ telles que
> - $\forall x\in U,\quad f(x)=f(a)+L(x-a)+\lVert x-a\rVert\,\varepsilon(x)$ ;
> - $\displaystyle\lim_{x\to a}\varepsilon(x)=0$.
> → [[differentiabilite|fiche complète]]

> [!note] **Dérivée directionnelle** (Déf. 2.8)
> Soit $v\in E$. $f$ est **dérivable en $a$ dans la direction $v$** si la fonction d'une variable réelle $f_v:t\mapsto f(a+tv)$, définie au voisinage de $0$, est dérivable en $0$. On note
> $$f_v'(0)=\lim_{t\to0}\frac{f(a+tv)-f(a)}{t}\ \in F.$$
> → [[derivee-directionnelle|fiche complète]]

> [!note] **Application de classe C1** (Déf. 2.12, 2.13 et 3.14)
> - $f$ est **différentiable sur $U$** si elle l'est en tout point de $U$. Sa différentielle est alors l'application $Df:U\to\mathcal L_c(E,F)$, $a\mapsto Df_a$.
> - $f$ est **de classe $\mathcal C^1$ sur $U$** si $f$ est différentiable sur $U$ et si $Df:U\to(\mathcal L_c(E,F),\lvert\!\lvert\!\lvert \cdot\rvert\!\rvert\!\rvert)$ est continue, c'est-à-dire
> $$\forall a\in U,\qquad \lvert\!\lvert\!\lvert Df_x-Df_a\rvert\!\rvert\!\rvert\xrightarrow[x\to a]{}0.$$
> → [[classe-c1|fiche complète]]

> [!note] **Différentielle partielle** (Déf. 2.27)
> La $j$-ème **application partielle** en $a$ est $\varphi_j:x_j\mapsto f(a_1,\dots,a_{j-1},x_j,a_{j+1},\dots,a_n)$. Si $\varphi_j$ est différentiable en $a_j$, sa différentielle $D(\varphi_j)_{a_j}\in\mathcal L_c(E_j,F)$ est la $j$-ème **différentielle partielle** de $f$ en $a$, notée $\partial_jf(a)$ ou $D_jf(a)$.
> → [[differentielle-partielle|fiche complète]]

> [!note] **Dérivée partielle** (Déf. 2.30)
> Soit $f:U\subset\mathbb R^n\to F$ et $a\in U$. La **dérivée partielle** de $f$ en $a$ par rapport à sa $j$-ème variable est, quand la limite existe,
> $$\frac{\partial f}{\partial x_j}(a)=\lim_{t\to0}\frac{f(a+te_j)-f(a)}{t}\ \in F,$$
> où $(e_1,\dots,e_n)$ est la base canonique. C'est la dérivée de $f$ en $a$ dans la direction $e_j$ (Rem. 2.31).
> → [[derivee-partielle|fiche complète]]

> [!note] **Matrice jacobienne** (Déf. 2.36)
> Si $f=(f_1,\dots,f_p):U\subset\mathbb R^n\to\mathbb R^p$ est différentiable en $a$, la **matrice jacobienne** de $f$ en $a$ est la matrice à $p$ lignes et $n$ colonnes
> $$J_f(a)=\Big(\frac{\partial f_i}{\partial x_j}(a)\Big)_{\substack{1\le i\le p\\1\le j\le n}}.$$
> C'est la matrice de $Df_a$ dans les bases canoniques : $Df_a(h)=J_f(a)\,h$.
> → [[matrice-jacobienne|fiche complète]]

> [!note] **Gradient** (Déf. 2.39)
> Soit $f:\Omega\subset\mathbb R^n\to\mathbb R$ différentiable en $a$. Le **gradient** de $f$ en $a$ est le vecteur colonne
> $$\nabla f(a)={}^t\!\big(J_f(a)\big)=\begin{pmatrix}\frac{\partial f}{\partial x_1}(a)\\ \vdots\\ \frac{\partial f}{\partial x_n}(a)\end{pmatrix},\qquad Df_a(h)=\sum_{j=1}^n h_j\frac{\partial f}{\partial x_j}(a).$$
> → [[gradient|fiche complète]]


## 3 – Accroissements finis

> [!note] **Segment, partie convexe** (Déf. 3.3 et 3.4)
> - Pour $a,b\in E$, le **segment** $[a,b]$ est $\{a+t(b-a)\ :\ t\in[0,1]\}$ ; le segment ouvert est $]a,b[=\{a+t(b-a)\ :\ t\in\,]0,1[\}$.
> - Une partie $C\subset E$ est **convexe** si, pour tous $a,b\in C$, le segment $[a,b]$ est inclus dans $C$.
> → [[segment-et-convexe|fiche complète]]

> [!note] **Partie connexe** (Déf. 3.20)
> Un espace topologique $X$ est **connexe** si, pour tout couple $(U_1,U_2)$ d'ouverts de $X$ tels que $U_1\cap U_2=\emptyset$ et $U_1\cup U_2=X$, on a $U_1=\emptyset$ ou $U_2=\emptyset$.
> → [[partie-connexe|fiche complète]]


## 4 – Différentielles d'ordre supérieur

> [!note] **Différentielle seconde, classe C2** (Déf. 4.1 et 4.4)
> $f:U\to F$ est **deux fois différentiable en** $a$ si $f$ est différentiable sur un voisinage de $a$ et si $Df$ est différentiable en $a$. On note
> $$D^2f_a:=D(Df)_a\in\mathcal L(E,\mathcal L(E,F))$$
> la **différentielle seconde** de $f$ en $a$. Si $f$ est deux fois différentiable sur $U$ et si $D^2f$ est continue sur $U$, $f$ est **de classe $\mathcal C^2$** sur $U$.
> → [[differentielle-seconde|fiche complète]]

> [!note] **Dérivées partielles d'ordre 2** (Déf. 4.8)
> On note $\partial^2_{ij}f(a)$, ou $\dfrac{\partial^2f}{\partial x_i\partial x_j}(a)$, la dérivée partielle par rapport à $x_i$, en $a$, de la fonction $x\mapsto\partial_jf(x)$ :
> $$\partial^2_{ij}f(a)=\partial_i(\partial_jf)(a)$$
> (on dérive d'abord par rapport à $x_j$, puis par rapport à $x_i$).
> → [[derivees-partielles-ordre-2|fiche complète]]

> [!note] **Matrice hessienne** (Déf. 4.13)
> Soit $f:U\subset\mathbb R^n\to\mathbb R$ deux fois différentiable en $a$. La **matrice hessienne** de $f$ en $a$ est
> $$H_f(a)=\big(\partial^2_{ij}f(a)\big)_{1\le i,j\le n}.$$
> Elle est **symétrique** ([[theoreme-de-schwarz]]) et, pour tous $h,k\in\mathbb R^n$ (Prop. 4.14),
> $$D^2f_a(h,k)={}^t\!h\,H_f(a)\,k.$$
> → [[matrice-hessienne|fiche complète]]

> [!note] **Extremum local, extremum global** (Déf. 4.17 et 4.18)
> Soit $U\subset E$ un ouvert et $f:U\to\mathbb R$.
> - $f$ admet en $a\in U$ un **minimum local** (resp. **maximum local**) s'il existe un ouvert $V\subset U$ contenant $a$ tel que $\forall x\in V,\ f(x)\ge f(a)$ (resp. $f(x)\le f(a)$). Si l'inégalité est stricte pour $x\ne a$ : extremum local **strict**.
> - $f$ admet en $a$ un **minimum global** (resp. maximum global) si $f(x)\ge f(a)$ (resp. $\le$) pour **tout** $x\in U$.
> → [[extremum-local|fiche complète]]

> [!note] **Point critique** (Déf. 4.19)
> Soit $f:U\to\mathbb R$ différentiable en $a\in U$. Le point $a$ est un **point critique** de $f$ si $Df_a=0$.
> Sur $\mathbb R^n$ : $\dfrac{\partial f}{\partial x_1}(a)=\dots=\dfrac{\partial f}{\partial x_n}(a)=0$, c'est-à-dire $\nabla f(a)=0$.
> → [[point-critique|fiche complète]]

> [!note] **Différentiabilité d'ordre n, classes Cn et C∞** (Déf. 4.29)
> Soit $n\ge2$.
> - $f$ est **$n$ fois différentiable en $a$** s'il existe un ouvert $V\subset U$ contenant $a$ sur lequel $f$ est $(n-1)$ fois différentiable, et si $D^{n-1}f$ est différentiable en $a$. On note $D^nf_a:=D(D^{n-1}f)_a$, vue comme une application $n$-linéaire continue (Déf. 4.27) : $D^nf_a(h_1,\dots,h_n)$.
> - $f$ est **de classe $\mathcal C^n$** sur $U$ si elle est $n$ fois différentiable sur $U$ et si $D^nf$ est continue. $f$ est $\mathcal C^\infty$ si elle est $\mathcal C^n$ pour tout $n$.
> → [[classe-cn|fiche complète]]


## 5 – Inversion locale et fonctions implicites

> [!note] **Difféomorphisme, difféomorphisme local** (Déf. 5.1)
> Soient $E,F$ deux e.v.n., $U$ un ouvert de $E$, $V$ un ouvert de $F$ et $f:U\to V$.
> 1. $f$ est un **difféomorphisme de classe $\mathcal C^1$** de $U$ sur $V$ si
>    - (a) $f$ est une **bijection** de $U$ sur $V$ ;
>    - (b) $f$ est de classe $\mathcal C^1$ sur $U$ ;
>    - (c) sa réciproque $f^{-1}$ est de classe $\mathcal C^1$ sur $V$.
> 2. Soit $a\in U$. $f$ est un **difféomorphisme local en $a$** s'il existe un voisinage ouvert $U'\subset U$ de $a$ et un voisinage ouvert $V'\subset V$ de $f(a)$ tels que $f$ soit un difféomorphisme de $U'$ sur $V'$.
> → [[diffeomorphisme|fiche complète]]

