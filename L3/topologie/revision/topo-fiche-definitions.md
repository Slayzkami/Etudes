---
aliases:
  - "Fiche de définitions topologie"
  - "toutes les définitions topo"
tags:
  - topologie
  - topo/revision
---

# 📘 Fiche de révision – toutes les définitions

Toutes les définitions du programme sur une seule page, dans l'ordre du cours, **avec les quantificateurs**. Méthode : lire, fermer, réécrire de mémoire, comparer. · [[topo-plan-de-revision|↩ Plan de révision]] · [[topo-index-definitions|↩ Index]] · Suite : [[topo-fiche-theoremes]]

## [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]]

> [!note] **Distance, espace métrique** · *Déf. 1.1*
> Soit $E$ un ensemble non vide. Une **distance** sur $E$ est une application $d:E\times E\to\mathbb R_+$ telle que :
> - **(M1) séparation** : $\forall x,y\in E,\ d(x,y)=0\iff x=y$ ;
> - **(M2) symétrie** : $\forall x,y\in E,\ d(x,y)=d(y,x)$ ;
> - **(M3) inégalité triangulaire** : $\forall x,y,z\in E,\ d(x,y)\le d(x,z)+d(z,y)$.
>
> Un **espace métrique** est un couple $(E,d)$, avec $E\neq\emptyset$ et $d$ une distance sur $E$.
> → [[topo-distance|fiche complète]]

> [!note] **Distance discrète** · *Ex. 1.2 (3)*
> Sur un ensemble $E$ quelconque : $d(x,y)=\begin{cases}0 & \text{si } x=y\\ 1 & \text{si } x\neq y.\end{cases}$
> → [[topo-distance-discrete|fiche complète]]

> [!note] **Norme, espace vectoriel normé** · *Déf. 1.5*
> Soit $E$ un espace vectoriel sur $\mathbb K=\mathbb R$ ou $\mathbb C$. Une **norme** est une application $N:E\to\mathbb R_+$ telle que :
> - **(N1)** $\forall x\in E,\ N(x)=0\iff x=0_E$ ;
> - **(N2)** $\forall\lambda\in\mathbb K,\ \forall x\in E,\ N(\lambda x)=|\lambda|\,N(x)$ ;
> - **(N3)** $\forall x,y\in E,\ N(x+y)\le N(x)+N(y)$.
>
> $(E,N)$ est un **espace vectoriel normé** (e.v.n.) ; on note souvent $\|x\|$.
> → [[topo-norme|fiche complète]]

> [!note] **Distance associée à une norme** · *Déf. 1.7*
> Si $(E,N)$ est un e.v.n., $d(x,y)=N(x-y)$ est une distance sur $E$, appelée **distance associée** à $N$.
> → [[topo-distance-associee-norme|fiche complète]]

> [!note] **Normes usuelles de K^n et de C([a,b])** · *Ex. 1.10 et 1.11*
> Pour $x=(x_1,\dots,x_n)\in\mathbb K^n$ :
> $$\|x\|_1=\sum_{i=1}^n|x_i|,\qquad \|x\|_2=\Big(\sum_{i=1}^n|x_i|^2\Big)^{1/2},\qquad \|x\|_\infty=\max_{1\le i\le n}|x_i|.$$
> Sur $C([a,b])$ : $\|f\|_1=\int_a^b|f|$, $\|f\|_2=\big(\int_a^bf^2\big)^{1/2}$, $\|f\|_\infty=\sup_{[a,b]}|f|$.
> → [[topo-normes-usuelles|fiche complète]]

> [!note] **Boules et sphères** · *Déf. 1.13*
> Soit $(E,d)$ un espace métrique, $a\in E$ et $r>0$.
> - **Boule ouverte** : $B(a,r)=\{x\in E\mid d(a,x)<r\}$ ;
> - **Boule fermée** : $\bar B(a,r)=\{x\in E\mid d(a,x)\le r\}$ ;
> - **Sphère** : $S(a,r)=\{x\in E\mid d(a,x)=r\}$.
> → [[topo-boules-spheres|fiche complète]]

> [!note] **Partie bornée, diamètre** · *Déf. 1.16*
> Une partie non vide $A\subset E$ est **bornée** si $\{d(x,y)\mid x,y\in A\}$ est majoré, c'est-à-dire
> $$\exists M\ge0,\ \forall x,y\in A,\ d(x,y)\le M.$$
> Son **diamètre** est $\operatorname{diam}A=\sup_{(x,y)\in A^2}d(x,y)$ ($=+\infty$ si $A$ n'est pas bornée).
> → [[topo-partie-bornee-diametre|fiche complète]]

> [!note] **Distance induite, sous-espace métrique** · *Déf. 1.19*
> Soit $(E,d)$ un espace métrique et $F\subset E$ non vide. La restriction $d_F$ de $d$ à $F\times F$ ($d_F(x,y)=d(x,y)$) est une distance sur $F$ : la **distance induite**. $(F,d_F)$ est un **sous-espace métrique**.
> → [[topo-distance-induite|fiche complète]]

> [!note] **Distance produit** · *Prop. 1.22*
> Si $(E_1,d_1),\dots,(E_n,d_n)$ sont des espaces métriques et $E=E_1\times\dots\times E_n$, on pose pour $x=(x_i)$, $y=(y_i)$ :
> $$d(x,y)=\max_{1\le i\le n}d_i(x_i,y_i).$$
> C'est une distance sur $E$ (le **produit** des $E_i$).
> → [[topo-distance-produit|fiche complète]]

> [!note] **Suite convergente** · *Déf. 1.24*
> $(x_n)$ **converge** vers $\ell\in E$ (pour $d$) si
> $$\forall\varepsilon>0,\ \exists N_\varepsilon\in\mathbb N,\ \forall n\ge N_\varepsilon,\ d(x_n,\ell)<\varepsilon.$$
> On note $x_n\to\ell$.
> → [[topo-suite-convergente|fiche complète]]

> [!note] **Suite extraite** · *Déf. 1.26*
> $(y_n)$ est une **suite extraite** (sous-suite) de $(x_n)$ s'il existe $\varphi:\mathbb N\to\mathbb N$ **strictement croissante** telle que $\forall n,\ y_n=x_{\varphi(n)}$.
> → [[topo-suite-extraite|fiche complète]]

> [!note] **Suite bornée** · *Déf. 1.30*
> $(x_n)$ est **bornée** s'il existe une boule $B(a,r)$ telle que $\forall n\in\mathbb N,\ x_n\in B(a,r)$.
> → [[topo-suite-bornee|fiche complète]]

## [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]]

> [!note] **Ouvert** · *Déf. 2.1*
> Une partie $A\subset E$ est un **ouvert** de $E$ si $A=\emptyset$ ou si
> $$\forall x\in A,\ \exists r>0,\ B(x,r)\subset A.$$
> → [[topo-ouvert|fiche complète]]

> [!note] **Fermé** · *Déf. 2.2*
> Une partie $A\subset E$ est un **fermé** de $E$ si son complémentaire $A^c=E\setminus A$ est un ouvert, c'est-à-dire
> $$\forall x\notin A,\ \exists r>0,\ B(x,r)\cap A=\emptyset.$$
> → [[topo-ferme|fiche complète]]

> [!note] **Voisinage** · *Déf. 2.14*
> Soit $a\in E$ et $V\subset E$. $V$ est un **voisinage** de $a$ s'il existe un ouvert $O$ tel que $a\in O\subset V$. On note $\mathcal V(a)$ l'ensemble des voisinages de $a$.
> → [[topo-voisinage|fiche complète]]

> [!note] **Intérieur** · *Déf. 2.18*
> L'**intérieur** de $A$ est la réunion de tous les ouverts contenus dans $A$ :
> $$\operatorname{Int}A=\mathring A=\bigcup\{O\ \text{ouvert}\mid O\subset A\}.$$
> C'est le **plus grand ouvert contenu dans $A$**.
> → [[topo-interieur|fiche complète]]

> [!note] **Adhérence** · *Déf. 2.22*
> L'**adhérence** de $A$ est l'intersection de tous les fermés contenant $A$ :
> $$\bar A=\bigcap\{F\ \text{fermé}\mid F\supset A\}.$$
> C'est le **plus petit fermé contenant $A$**.
> → [[topo-adherence|fiche complète]]

> [!note] **Partie dense** · *Déf. 2.26*
> $A$ est **dense** dans $E$ si $\bar A=E$, c'est-à-dire si toute boule de $E$ rencontre $A$ : $\forall x\in E,\ \forall r>0,\ B(x,r)\cap A\neq\emptyset$.
> → [[topo-partie-dense|fiche complète]]

> [!note] **Frontière** · *Déf. 2.28*
> La **frontière** de $A$ est $\operatorname{Fr}A=\bar A\setminus\operatorname{Int}A$.
> → [[topo-frontiere|fiche complète]]

> [!note] **Continuité en un point** · *Déf. 2.31*
> $f:(E,d_E)\to(F,d_F)$ est **continue en $a$** si
> $$\forall\varepsilon>0,\ \exists\delta>0,\ \forall x\in E,\ d_E(a,x)<\delta\Rightarrow d_F(f(a),f(x))<\varepsilon,$$
> c'est-à-dire $f(B_E(a,\delta))\subset B_F(f(a),\varepsilon)$. $f$ est continue sur $A$ si elle l'est en tout point de $A$.
> → [[topo-continuite|fiche complète]]

> [!note] **Uniforme continuité** · *Déf. 2.38*
> $f:E\to F$ est **uniformément continue** si
> $$\forall\varepsilon>0,\ \exists\delta>0,\ \forall(x,y)\in E^2,\ d_E(x,y)<\delta\Rightarrow d_F(f(x),f(y))<\varepsilon.$$
> → [[topo-continuite-uniforme|fiche complète]]

> [!note] **Application lipschitzienne** · *Déf. 2.42*
> $f:E\to F$ est **lipschitzienne** s'il existe $k\ge0$ tel que
> $$\forall(x,y)\in E^2,\ d_F(f(x),f(y))\le k\,d_E(x,y).$$
> On dit que $f$ est $k$-lipschitzienne.
> → [[topo-application-lipschitzienne|fiche complète]]

> [!note] **Isométrie** · *Déf. 2.45*
> $f:E\to F$ est une **isométrie** si $\forall x,y\in E,\ d_F(f(x),f(y))=d_E(x,y)$.
> → [[topo-isometrie|fiche complète]]

> [!note] **Homéomorphisme** · *Déf. 2.52*
> $f:E\to F$ est un **homéomorphisme** si $f$ est **bijective** et **bicontinue** ($f$ et $f^{-1}$ continues). $E$ et $F$ sont **homéomorphes** s'il existe un homéomorphisme de l'un sur l'autre.
> → [[topo-homeomorphisme|fiche complète]]

> [!note] **Distances topologiquement équivalentes** · *Déf. 2.57*
> Deux distances $d_1,d_2$ sur $E$ sont **topologiquement équivalentes** si $\mathrm{id}:(E,d_1)\to(E,d_2)$ est un homéomorphisme.
> → [[topo-distances-topologiquement-equivalentes|fiche complète]]

> [!note] **Distances métriquement équivalentes** · *Déf. 2.60*
> $d_1$ et $d_2$ sont **métriquement équivalentes** s'il existe $\alpha>0$ et $\beta>0$ tels que
> $$\forall x,y\in E,\ \alpha\,d_1(x,y)\le d_2(x,y)\le\beta\,d_1(x,y).$$
> → [[topo-distances-metriquement-equivalentes|fiche complète]]

> [!note] **Normes équivalentes** · *Déf. 2.64*
> Deux normes $N_1,N_2$ sur $E$ sont **équivalentes** si les distances associées sont topologiquement équivalentes.
> → [[topo-normes-equivalentes|fiche complète]]

> [!note] **Norme d'une application linéaire continue** · *Déf. 2.71*
> Pour $f\in\mathcal L_c(E,F)$ (linéaire continue) :
> $$|||f|||=\sup_{u\neq0}\frac{\|f(u)\|_F}{\|u\|_E}=\sup_{\|u\|_E=1}\|f(u)\|_F=\sup_{\|u\|_E\le1}\|f(u)\|_F.$$
> → [[topo-norme-operateur|fiche complète]]

> [!note] **Distance d'un point à une partie, entre deux parties** · *TD, exercice 2.13 (corrigé dans le cours, § 2.17.4)*
> Pour $A,B$ non vides : $d(x,A)=\inf_{a\in A}d(x,a)$ et $d(A,B)=\inf_{x\in A,\ y\in B}d(x,y)$.
> → [[topo-distance-a-une-partie|fiche complète]]

## [[03-espaces-metriques-compacts|3 – Espaces métriques compacts]]

> [!note] **Recouvrement** · *Déf. 3.1*
> Soit $(A_i)_{i\in I}$ une famille de parties de $E$ et $F\subset E$.
> - $(A_i)$ est un **recouvrement** de $F$ si $F\subset\bigcup_{i\in I}A_i$.
> - Si $J\subset I$ et $F\subset\bigcup_{j\in J}A_j$, $(A_j)_{j\in J}$ est un **sous-recouvrement** ; il est **fini** si $J$ est fini.
> - Si les $A_i$ sont des ouverts : **recouvrement ouvert**.
> → [[topo-recouvrement|fiche complète]]

> [!note] **Espace compact** · *Déf. 3.3*
> $(E,d)$ est **compact** si de tout recouvrement ouvert de $E$ on peut extraire un sous-recouvrement fini :
> $$\forall(O_i)_{i\in I}\ \text{ouverts},\ E\subset\bigcup_{i\in I}O_i\ \Rightarrow\ \exists i_1,\dots,i_n\in I,\ E\subset O_{i_1}\cup\dots\cup O_{i_n}.$$
> → [[topo-espace-compact|fiche complète]]

> [!note] **Partie compacte** · *Déf. 3.8*
> $A\subset E$ est une **partie compacte** de $E$ si le sous-espace métrique $(A,d)$ est compact.
> → [[topo-partie-compacte|fiche complète]]

> [!note] **Suite de Cauchy, espace complet** · *Déf. 3.15*
> $(x_n)$ est **de Cauchy** si $\forall\varepsilon>0,\ \exists N_\varepsilon\in\mathbb N,\ \forall p,q\ge N_\varepsilon,\ d(x_p,x_q)\le\varepsilon$.
> $E$ est **complet** si toute suite de Cauchy de $E$ converge dans $E$.
> → [[topo-suite-de-cauchy-espace-complet|fiche complète]]
