---
aliases:
  - "Fiche de théorèmes CD"
  - "tous les théorèmes de calcul différentiel"
tags:
  - cd
  - cd/revision
---

# ⭐ Fiche de révision – tous les énoncés

Tous les énoncés du cours sur une seule page (hypothèses comprises). Les démonstrations sont dans les fiches complètes. · [[cd-plan-de-revision|↩ Plan de révision]] · [[cd-index-definitions|↩ Index]] · Avant : [[cd-fiche-definitions]]

## 1 – Espaces vectoriels normés

> [!important] **Seconde inégalité triangulaire** (Prop. 1.2)
> Dans un e.v.n. : $\forall(x,y)\in E^2,\quad \big|\,\lVert x\rVert-\lVert y\rVert\,\big|\le\lVert x-y\rVert$.
> → [[seconde-inegalite-triangulaire|fiche complète]]

> [!important] **Équivalence des normes en dimension finie** (Th. 1.13)
> Sur un espace vectoriel de **dimension finie**, toutes les normes sont équivalentes.
> → [[equivalence-normes-dimension-finie|fiche complète]]

> [!important] **Stabilité des ouverts et des fermés** (Th. 1.22 et 1.23)
> - **(O1)** $E$ et $\emptyset$ sont ouverts. **(O2)** Une réunion **quelconque** d'ouverts est un ouvert. **(O3)** Une intersection **finie** d'ouverts est un ouvert.
> - **(F1)** $E$ et $\emptyset$ sont fermés. **(F2)** Une intersection **quelconque** de fermés est un fermé. **(F3)** Une réunion **finie** de fermés est un fermé.
> → [[stabilite-ouverts-fermes|fiche complète]]

> [!important] **Caractérisation séquentielle des fermés** (Th. 1.24)
> $A\subset E$ est fermé si et seulement si toute suite d'éléments de $A$ qui converge dans $E$ a sa limite dans $A$.
> → [[caracterisation-sequentielle-fermes|fiche complète]]

> [!important] **Continuité et composantes** (Th. 1.40)
> Soit $f=(f_1,\dots,f_p):E\to F=F_1\times\dots\times F_p$ (norme produit). $f$ est continue (resp. uniformément continue) si et seulement si toutes ses composantes $f_i=\pi_i\circ f$ le sont.
> → [[continuite-et-composantes|fiche complète]]

> [!important] **Caractérisations des applications linéaires continues** (Th. 1.43)
> Soit $f:E\to F$ **linéaire** entre deux e.v.n. Sont équivalentes :
> - (i) $f$ est continue sur $E$ ;
> - (ii) $f$ est continue en $0$ ;
> - (iii) $f$ est bornée sur la boule unité : $\exists M\ge0,\ \forall u\in\overline B_E(0,1),\ \lVert f(u)\rVert_F\le M$ ;
> - (iv) $\exists C\ge0,\ \forall u\in E,\ \lVert f(u)\rVert_F\le C\,\lVert u\rVert_E$ ;
> - (v) $f$ est lipschitzienne.
> → [[caracterisation-lineaires-continues|fiche complète]]

> [!important] **Linéaire au départ d'une dimension finie : continue** (Th. 1.44)
> Si $E$ est de **dimension finie**, toute application linéaire $f:E\to F$ est continue.
> → [[lineaire-en-dimension-finie|fiche complète]]

> [!important] **Caractérisations de la norme d'opérateur** (Prop. 1.50)
> Soit $f\in\mathcal L_c(E,F)$, $E\ne\{0\}$.
> - (i) Pour tout $u\in E$ : $\lVert f(u)\rVert_F\le\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert\,\lVert u\rVert_E$.
> - (ii) Si $C\ge0$ vérifie $\lVert f(u)\rVert_F\le C\lVert u\rVert_E$ pour tout $u$, alors $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert\le C$.
> - (iii) $\displaystyle\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert=\sup_{u\ne0}\frac{\lVert f(u)\rVert}{\lVert u\rVert}=\sup_{\lVert u\rVert=1}\lVert f(u)\rVert$.
> → [[caracterisations-norme-operateur|fiche complète]]

> [!important] **Norme d'une composée** (Prop. 1.51)
> Si $f\in\mathcal L_c(E,F)$ et $g\in\mathcal L_c(F,G)$, alors $g\circ f\in\mathcal L_c(E,G)$ et $\lvert\!\lvert\!\lvert g\circ f\rvert\!\rvert\!\rvert\le\lvert\!\lvert\!\lvert g\rvert\!\rvert\!\rvert\,\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert$.
> → [[norme-composee|fiche complète]]

> [!important] **Caractérisation des applications bilinéaires continues** (Prop. 1.53 et 1.55)
> Soit $B:E_1\times E_2\to F$ bilinéaire. $B$ est continue si et seulement si
> $$\exists C\ge0,\ \forall(u,v)\in E_1\times E_2,\qquad \lVert B(u,v)\rVert_F\le C\,\lVert u\rVert_{E_1}\lVert v\rVert_{E_2}.$$
> Si $E_1$ et $E_2$ sont de dimension finie, toute application bilinéaire est continue (Prop. 1.55).
> → [[caracterisation-bilineaires-continues|fiche complète]]

> [!important] **Espaces de Banach usuels** (Th. 1.60 et 1.61)
> - Tout e.v.n. de dimension finie est un Banach.
> - $(\mathcal C([a,b],\mathbb R),\lVert \cdot\rVert_\infty)$ est un Banach (Th. 1.60). $(\mathcal C([a,b]),\lVert \cdot\rVert_1)$ n'en est **pas** un.
> - Si $F$ est un Banach, $(\mathcal L_c(E,F),\lvert\!\lvert\!\lvert \cdot\rvert\!\rvert\!\rvert)$ est un Banach (Th. 1.61).
> → [[espaces-de-banach-usuels|fiche complète]]


## 2 – Applications différentiables

> [!important] **Différentielle et dérivées directionnelles** (Prop. 2.9)
> Si $f$ est différentiable en $a$, alors $f$ est dérivable en $a$ dans **toutes** les directions $v\in E$, et
> $$Df_a(v)=\lim_{t\to0}\frac{f(a+tv)-f(a)}{t}=\frac{\mathrm d}{\mathrm dt}f(a+tv)\Big|_{t=0}.$$
> → [[differentielle-et-derivees-directionnelles|fiche complète]]

> [!important] **Différentielles de référence : constante, linéaire, bilinéaire** (Ex. 2.15, 2.16, 2.17)
> 1. **Constante** (Ex. 2.15) : $f(x)=c$ est différentiable partout et $Df_a=0$.
> 2. **Linéaire continue** (Ex. 2.16) : si $\varphi\in\mathcal L_c(E,F)$, alors $\varphi$ est différentiable partout et $D\varphi_a=\varphi$ pour tout $a$, c'est-à-dire $D\varphi_a(h)=\varphi(h)$.
> 3. **Bilinéaire continue** (Ex. 2.17) : si $B:E_1\times E_2\to F$ est bilinéaire continue, alors $B$ est différentiable partout et
> $$DB_{(a_1,a_2)}(h_1,h_2)=B(h_1,a_2)+B(a_1,h_2).$$
> → [[differentielles-de-reference|fiche complète]]

> [!important] **Différentiable implique continue** (Prop. 2.18)
> Si $f$ est différentiable en $a$, alors $f$ est continue en $a$.
> → [[differentiable-implique-continue|fiche complète]]

> [!important] **Linéarité de la différentielle** (Th. 2.19)
> Si $f,g:U\to F$ sont différentiables en $a$, alors pour tous $\alpha,\beta\in\mathbb K$, $\alpha f+\beta g$ est différentiable en $a$ et
> $$D(\alpha f+\beta g)_a=\alpha\,Df_a+\beta\,Dg_a.$$
> → [[linearite-differentielle|fiche complète]]

> [!important] **Règle de la chaîne (différentielle d'une composée)** (Th. 2.20, Cor. 2.26, Prop. 2.37)
> Soient $E,F,G$ trois e.v.n., $U\subset E$ et $V\subset F$ deux ouverts, $f:U\to F$ et $g:V\to G$ avec $f(U)\subset V$. Si $f$ est différentiable en $a$ et $g$ est différentiable en $f(a)$, alors $g\circ f$ est différentiable en $a$ et
> $$D(g\circ f)_a=Dg_{f(a)}\circ Df_a,\qquad\text{soit}\qquad D(g\circ f)_a(h)=Dg_{f(a)}\big(Df_a(h)\big).$$
> → [[regle-de-la-chaine|fiche complète]]

> [!important] **Différentielle et différentielles partielles** (Prop. 2.29, Cor. 2.32)
> Si $f:U\subset E_1\times\dots\times E_n\to F$ est différentiable en $a$, alors $\partial_jf(a)$ existe pour tout $j$, et pour tout $h=(h_1,\dots,h_n)$ :
> $$Df_a(h)=\sum_{j=1}^n\partial_jf(a)(h_j).$$
> Cas $E=\mathbb R^n$ (Cor. 2.32) : $\displaystyle Df_a(h)=h_1\frac{\partial f}{\partial x_1}(a)+\dots+h_n\frac{\partial f}{\partial x_n}(a)$.
> → [[differentielle-et-differentielles-partielles|fiche complète]]

> [!important] **Différentiabilité par composantes** (Prop. 2.33, Cor. 2.35)
> Soit $f=(f_1,\dots,f_p):U\to F_1\times\dots\times F_p$. $f$ est différentiable en $a$ si et seulement si chaque composante $f_i$ est différentiable en $a$. Dans ce cas, pour tout $h\in E$ :
> $$Df_a(h)=\big(D(f_1)_a(h),\dots,D(f_p)_a(h)\big).$$
> Cas $\mathbb R^n\to\mathbb R^p$ (Cor. 2.35) : $Df_a(h)=J_f(a)\,h$.
> → [[differentiabilite-par-composantes|fiche complète]]

> [!important] **Différentielle d'un « produit » B(f1, f2)** (Prop. 2.34)
> Soient $f_1:U\to F_1$, $f_2:U\to F_2$ différentiables en $a$ et $B:F_1\times F_2\to G$ bilinéaire continue. Alors $P:x\mapsto B(f_1(x),f_2(x))$ est différentiable en $a$ et
> $$DP_a(h)=B\big(D(f_1)_a(h),f_2(a)\big)+B\big(f_1(a),D(f_2)_a(h)\big).$$
> → [[differentielle-produit-bilineaire|fiche complète]]


## 3 – Accroissements finis

> [!important] **Théorème des accroissements finis (TAF)** (Th. 3.2 et 3.6)
> Soient $a<b$ et $f:[a,b]\to\mathbb R$ continue sur $[a,b]$, dérivable sur $]a,b[$. Il existe $c\in\,]a,b[$ tel que $f(b)-f(a)=f'(c)(b-a)$.
> → [[taf|fiche complète]]

> [!important] **Inégalité des accroissements finis (IAF)** (Th. 3.8, 3.9 et 3.11)
> Soient $E,F$ des e.v.n., $U\subset E$ un ouvert et $f:U\to F$ différentiable sur $U$. Soient $a,b\in U$ tels que **$[a,b]\subset U$**. S'il existe $M\ge0$ tel que $\lvert\!\lvert\!\lvert Df_x\rvert\!\rvert\!\rvert\le M$ pour tout $x\in[a,b]$, alors
> $$\lVert f(b)-f(a)\rVert_F\le M\,\lVert b-a\rVert_E.$$
> → [[iaf|fiche complète]]

> [!important] **IAF sur un convexe : différentielle bornée implique lipschitzienne** (Cor. 3.13)
> Soient $E,F$ des e.v.n., $C\subset E$ un ouvert **convexe** et $f:C\to F$ différentiable. S'il existe $M\ge0$ tel que $\lvert\!\lvert\!\lvert Df_x\rvert\!\rvert\!\rvert\le M$ pour tout $x\in C$, alors $f$ est $M$-lipschitzienne sur $C$ :
> $$\forall a,b\in C,\qquad \lVert f(b)-f(a)\rVert_F\le M\,\lVert b-a\rVert_E.$$
> → [[iaf-sur-un-convexe|fiche complète]]

> [!important] **Critère C1 par les dérivées partielles** (Th. 3.15, Cor. 3.16)
> Soit $E=E_1\times\dots\times E_n$, $U\subset E$ ouvert, $f:U\to F$. $f$ est de classe $\mathcal C^1$ sur $U$ si et seulement si, pour tout $j$, $\partial_jf(x)$ existe en tout point $x\in U$ et $x\mapsto\partial_jf(x)$ est continue sur $U$.
>
> **Cas $E=\mathbb R^n$ (Cor. 3.16)** : $f$ est $\mathcal C^1$ sur $U$ $\iff$ les dérivées partielles $\dfrac{\partial f}{\partial x_j}$ existent en tout point de $U$ et sont **continues sur $U$**.
> → [[critere-c1|fiche complète]]

> [!important] **Différentielle nulle : f constante** (Prop. 3.18, Th. 3.25)
> Soit $U\subset E$ un ouvert **connexe** et $f:U\to F$ différentiable telle que $Df_x=0$ pour tout $x\in U$. Alors $f$ est constante sur $U$ (Th. 3.25).
> Cas particulier : $U$ ouvert **convexe** (Prop. 3.18) ; dans ce cas c'est une équivalence.
> → [[differentielle-nulle|fiche complète]]

> [!important] **Tout convexe est connexe** (Prop. 3.21 et 3.22)
> - (Prop. 3.21) Si $X$ est connexe, les seules parties de $X$ à la fois ouvertes et fermées dans $X$ sont $X$ et $\emptyset$.
> - (Prop. 3.22) Dans un e.v.n., toute partie convexe est connexe.
> → [[convexe-implique-connexe|fiche complète]]


## 4 – Différentielles d'ordre supérieur

> [!important] **Théorème de Schwarz** (Th. 4.6 et 4.10)
> Si $f:U\to F$ est deux fois différentiable en $a\in U$, alors $D^2f_a$ est **symétrique** :
> $$\forall(h,k)\in E\times E,\qquad D^2f_a(h,k)=D^2f_a(k,h).$$
> Sur $\mathbb R^n$ (Th. 4.10) : $\partial^2_{ij}f(a)=D^2f_a(e_i,e_j)$, donc
> $$\frac{\partial^2f}{\partial x_i\partial x_j}(a)=\frac{\partial^2f}{\partial x_j\partial x_i}(a).$$
> → [[theoreme-de-schwarz|fiche complète]]

> [!important] **Expression de la différentielle seconde** (Lemme 4.9, Th. 4.11, Prop. 4.14)
> Soit $f:U\to F$ deux fois différentiable en $a$ et $h\in E$ **fixé**. Alors $\varphi:x\mapsto Df_x(h)$ est différentiable en $a$ et
> $$D\varphi_a(k)=D^2f_a(k)(h)=D^2f_a(k,h)\qquad(=D^2f_a(h,k)\text{ par Schwarz}).$$
> → [[expression-differentielle-seconde|fiche complète]]

> [!important] **Critère C2** (Th. 4.12)
> $f:U\subset\mathbb R^n\to F$ est de classe $\mathcal C^2$ sur $U$ si et seulement si $f$ admet des dérivées partielles d'ordre 1 et 2 en tout point de $U$, et si celles-ci sont continues sur $U$.
> → [[critere-c2|fiche complète]]

> [!important] **Formule de Taylor-Young à l'ordre 2** (Prop. 4.15)
> Si $f:U\subset\mathbb R^n\to\mathbb R$ est deux fois différentiable en $a$, alors, pour $h$ assez petit,
> $$f(a+h)=f(a)+Df_a(h)+\frac12\,{}^t\!h\,H_f(a)\,h+\lVert h\rVert^2\varepsilon(h),\qquad\lim_{h\to0}\varepsilon(h)=0.$$
> → [[taylor-young-ordre-2|fiche complète]]

> [!important] **Condition nécessaire d'extremum (ordre 1)** (Prop. 4.20)
> Soit $U$ un **ouvert** de $E$ et $f:U\to\mathbb R$ différentiable en $a$. Si $f$ admet un extremum local en $a$, alors $a$ est un point critique : $Df_a=0$.
> → [[condition-necessaire-extremum|fiche complète]]

> [!important] **Extrema et différentielle seconde** (Th. 4.23)
> Soit $U\subset\mathbb R^n$ un ouvert et $f:U\to\mathbb R$ deux fois différentiable en $a\in U$.
> 1. **Condition nécessaire.** Si $f$ admet un minimum (resp. maximum) local en $a$, alors $Df_a=0$ et $H_f(a)$ est semi-définie positive (resp. négative) : ${}^t\!h\,H_f(a)\,h\ge0$ (resp. $\le0$) pour tout $h$.
> 2. **Condition suffisante.** Si $Df_a=0$ et $H_f(a)$ est **définie positive** (resp. définie négative), c'est-à-dire ${}^t\!h\,H_f(a)\,h>0$ (resp. $<0$) pour tout $h\ne0$, alors $f$ admet en $a$ un minimum (resp. maximum) local **strict**.
> → [[extrema-et-hessienne|fiche complète]]

> [!important] **Critère rt − s² (dimension 2)** (Cor. 4.25)
> Soit $U\subset\mathbb R^2$ ouvert, $f:U\to\mathbb R$ deux fois différentiable en un **point critique** $a$. On pose
> $$r=\frac{\partial^2f}{\partial x^2}(a),\quad s=\frac{\partial^2f}{\partial x\partial y}(a),\quad t=\frac{\partial^2f}{\partial y^2}(a).$$
> 1. Si $rt-s^2>0$ : extremum local strict en $a$ ; **minimum** si $r>0$, **maximum** si $r<0$.
> 2. Si $rt-s^2<0$ : **pas d'extremum** en $a$ (point-selle, ou col).
> 3. Si $rt-s^2=0$ : on **ne peut pas conclure** par ce critère.
> → [[critere-rt-s2|fiche complète]]

> [!important] **Formules de Taylor (ordre n)** (Th. 4.35, 4.37, 4.38, Cor. 4.39)
> Si $f:U\to F$ est $n$ fois différentiable en $a$ :
> $$f(a+h)=f(a)+\frac1{1!}Df_a(h)+\frac1{2!}D^2f_a(h,h)+\dots+\frac1{n!}D^nf_a(h)^n+o(\lVert h\rVert^n).$$
> → [[formules-de-taylor|fiche complète]]


## 5 – Inversion locale et fonctions implicites

> [!important] **Différentielle de la réciproque** (Prop. 5.4)
> Si $f:U\to V$ est un difféomorphisme, alors pour tout $a\in U$, $Df_a$ est un isomorphisme de $E$ sur $F$ et
> $$D(f^{-1})_{f(a)}=(Df_a)^{-1}.$$
> En particulier $\dim E=\dim F$. En dimension finie : $J_{f^{-1}}(f(a))=[J_f(a)]^{-1}$.
> → [[differentielle-de-la-reciproque|fiche complète]]

> [!important] **Théorème du point fixe de Banach-Picard** (Lemme 5.10)
> Soit $X$ une partie **fermée** non vide d'un espace de Banach et $T:X\to X$ une application **contractante** : il existe $k\in[0,1[$ tel que $\lVert T(x)-T(y)\rVert\le k\lVert x-y\rVert$ pour tous $x,y\in X$. Alors $T$ admet un **unique** point fixe dans $X$.
> → [[point-fixe-banach-picard|fiche complète]]

> [!important] **Théorème d'inversion locale** (Th. 5.7)
> Soit $U$ un ouvert de $\mathbb R^n$ et $f:U\to\mathbb R^n$ **de classe $\mathcal C^1$**. Soit $a\in U$ tel que $Df_a$ soit **bijective** (c'est-à-dire $\det J_f(a)\ne0$). Alors $f$ est un difféomorphisme local en $a$ : il existe des ouverts $U'\ni a$ et $V'\ni f(a)$ tels que $f:U'\to V'$ soit un difféomorphisme de classe $\mathcal C^1$. De plus, pour tout $x\in U'$,
> $$D(f^{-1})_{f(x)}=(Df_x)^{-1}.$$
> Si $f$ est $\mathcal C^k$, la réciproque locale est $\mathcal C^k$.
> → [[inversion-locale|fiche complète]]

> [!important] **Théorème d'inversion globale** (Th. 5.12, Cor. 5.13)
> Soit $U$ un ouvert de $\mathbb R^n$ et $f:U\to\mathbb R^n$ de classe $\mathcal C^1$, **injective**, et difféomorphisme local en tout point de $U$. Alors $f(U)$ est un ouvert de $\mathbb R^n$ et $f$ est un difféomorphisme de $U$ sur $f(U)$.
> → [[inversion-globale|fiche complète]]

> [!important] **Théorème des fonctions implicites (une variable)** (Th. 5.15)
> Soit $f:U\to\mathbb R$ de classe $\mathcal C^k$ ($k\ge1$) sur un ouvert $U\subset\mathbb R^2$, et $(a,b)\in U$ tel que
> $$f(a,b)=0\qquad\text{et}\qquad\frac{\partial f}{\partial y}(a,b)\ne0.$$
> Alors il existe un voisinage ouvert $V$ de $(a,b)$ inclus dans $U$, un intervalle $I=\,]a-\varepsilon,a+\varepsilon[$ et $\varphi:I\to\mathbb R$ de classe $\mathcal C^k$ tels que
> $$\big[(x,y)\in V\text{ et }f(x,y)=0\big]\iff\big[x\in I\text{ et }y=\varphi(x)\big].$$
> De plus $\varphi(a)=b$ et $f(x,\varphi(x))=0$ pour tout $x\in I$.
> → [[fonctions-implicites-une-variable|fiche complète]]

> [!important] **Théorème des fonctions implicites (cas général)** (Th. 5.19, Cor. 5.20)
> Soit $f:U\subset\mathbb R^m\times\mathbb R^n\to\mathbb R^n$ de classe $\mathcal C^k$ ($k\ge1$) et $(x_0,y_0)\in U$ tel que
> $$f(x_0,y_0)=0\qquad\text{et}\qquad\det J_yf(x_0,y_0)\ne0,$$
> où $J_yf=\big(\frac{\partial f_i}{\partial y_j}\big)$ est la matrice **carrée** $n\times n$ des dérivées par rapport aux variables $y$. Alors il existe des voisinages ouverts $V$ de $x_0$, $W$ de $y_0$ et $\varphi:V\to W$ de classe $\mathcal C^k$ tels que
> $$\big[(x,y)\in V\times W\text{ et }f(x,y)=0\big]\iff\big[x\in V\text{ et }y=\varphi(x)\big],$$
> et
> $$J_\varphi(x)=-\big[J_yf(x,\varphi(x))\big]^{-1}J_xf(x,\varphi(x)).$$
> → [[fonctions-implicites|fiche complète]]

