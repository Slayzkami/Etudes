---
aliases:
  - "Fiche des théorèmes topologie"
  - "tous les énoncés topo"
tags:
  - topologie
  - topo/revision
---

# ⭐ Fiche de révision – tous les énoncés

Tous les théorèmes et propositions du cours sur une page (énoncés seulement ; les démonstrations sont dans chaque fiche). Les ⭐ sont tombés en annales. · [[topo-plan-de-revision|↩ Plan de révision]] · [[topo-index-definitions|↩ Index]] · Avant : [[topo-fiche-definitions]]

## [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]]

> [!important] **Inégalité triangulaire généralisée** · *Prop. 1.3*
> Pour tous $x,y,z_1,\dots,z_n\in E$ : $d(x,y)\le d(x,z_1)+d(z_1,z_2)+\dots+d(z_{n-1},z_n)+d(z_n,y)$.
> → [[topo-inegalite-triangulaire-generalisee|énoncé + démonstration]]

> [!important] **Seconde inégalité triangulaire** · *Prop. 1.4 et 1.6*
> - Dans un espace métrique : $\forall x,y,z\in E,\ |d(x,z)-d(z,y)|\le d(x,y)$.
> - Dans un e.v.n. : $\forall x,y\in E,\ |N(x)-N(y)|\le N(x-y)$.
> → [[topo-seconde-inegalite-triangulaire|énoncé + démonstration]]

> [!important] ⭐ **Distances qui viennent d'une norme** · *Prop. 1.8*
> 1. La distance associée à une norme vérifie **(P1)** $d(\lambda x,\lambda y)=|\lambda|d(x,y)$ et **(P2)** $d(x+z,y+z)=d(x,y)$.
> 2. Réciproquement, une distance sur un espace vectoriel vérifiant (P1) et (P2) est associée à la norme $N(x)=d(x,0)$.
> 3. La distance discrète (sur $E\neq\{0\}$) ne provient d'aucune norme.
> → [[topo-distance-et-norme|énoncé + démonstration]]

> [!important] **Premières propriétés des boules** · *Prop. 1.14*
> 1. $a\in B(a,r)\subset\bar B(a,r)$ : les boules sont non vides (une sphère peut être vide).
> 2. $\bar B(a,r)=B(a,r)\cup S(a,r)$, réunion disjointe.
> 3. Si $0<r<r'$ : $B(a,r)\subset\bar B(a,r)\subset B(a,r')\subset\bar B(a,r')$.
> → [[topo-proprietes-boules|énoncé + démonstration]]

> [!important] **Propriétés des parties bornées** · *Prop. 1.17*
> 1. $A$ est bornée $\iff$ $A$ est contenue dans une boule.
> 2. $\operatorname{diam}B\le2r$ pour toute boule de rayon $r$.
> 3. $\emptyset\neq B\subset A$, $A$ bornée $\Rightarrow B$ bornée et $\operatorname{diam}B\le\operatorname{diam}A$.
> 4. $A,B$ bornées $\Rightarrow A\cup B$ bornée.
> → [[topo-proprietes-parties-bornees|énoncé + démonstration]]

> [!important] ⭐ **Boules d'un sous-espace métrique** · *Prop. 1.20*
> Pour $a\in F$ et $r>0$ : $B_F(a,r)=B_E(a,r)\cap F$ et $\bar B_F(a,r)=\bar B_E(a,r)\cap F$.
> → [[topo-boules-sous-espace|énoncé + démonstration]]

> [!important] **Boules d'un produit, autres distances produit** · *Prop. 1.23*
> 1. $B_E(a,r)=\prod_{i=1}^nB_{E_i}(a_i,r)$ et $\bar B_E(a,r)=\prod_{i=1}^n\bar B_{E_i}(a_i,r)$.
> 2. $d'=\sum_id_i$ et $d''=(\sum_id_i^2)^{1/2}$ sont des distances, et $d\le d''\le d'\le n\,d$.
> → [[topo-boules-produit|énoncé + démonstration]]

> [!important] **Unicité de la limite** · *Prop. 1.25*
> La limite d'une suite, si elle existe, est unique.
> → [[topo-unicite-limite|énoncé + démonstration]]

> [!important] **Suites extraites d'une suite convergente** · *Prop. 1.28 (et Lemme 1.27)*
> Si $x_n\to\ell$, toute suite extraite $(x_{\varphi(n)})$ converge vers $\ell$. (Lemme : $\varphi$ strictement croissante $\Rightarrow\varphi(n)\ge n$.)
> → [[topo-suites-extraites-convergentes|énoncé + démonstration]]

> [!important] **Toute suite convergente est bornée** · *Prop. 1.31*
> Toute suite convergente est bornée.
> → [[topo-convergente-bornee|énoncé + démonstration]]

> [!important] **Convergence dans un produit** · *Prop. 1.32*
> Dans $E=E_1\times\dots\times E_p$ muni de la distance produit : $x^{(n)}\to\ell\iff$ pour tout $i$, $x^{(n)}_i\to\ell_i$ dans $E_i$.
> → [[topo-convergence-produit|énoncé + démonstration]]

> [!important] **Convergence dans un e.v.n.** · *Prop. 1.33*
> 1. $x_n\to\ell\iff x_n-\ell\to0_E$.
> 2. $x_n\to x$, $y_n\to y\Rightarrow x_n+y_n\to x+y$ et $\alpha x_n\to\alpha x$.
> 3. $x_n\to\ell\Rightarrow N(x_n)\to N(\ell)$ ; la **réciproque est fausse** ($x_n=(-1)^n$).
> → [[topo-convergence-evn|énoncé + démonstration]]

## [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]]

> [!important] ⭐ **Une boule ouverte est un ouvert** · *Prop. 2.5*
> Dans un espace métrique, toute boule ouverte $B(a,\rho)$ est un ouvert.
> → [[topo-boule-ouverte-ouverte|énoncé + démonstration]]

> [!important] ⭐ **Une boule fermée est un fermé** · *Prop. 2.6*
> Dans un espace métrique, toute boule fermée $\bar B(a,\rho)$ est un fermé.
> → [[topo-boule-fermee-fermee|énoncé + démonstration]]

> [!important] **Stabilité des ouverts** · *Th. 2.7 et Ex. 2.8*
> - **(O1)** $E$ et $\emptyset$ sont des ouverts.
> - **(O2)** Une réunion **quelconque** d'ouverts est un ouvert.
> - **(O3)** Une intersection **finie** d'ouverts est un ouvert.
> → [[topo-stabilite-ouverts|énoncé + démonstration]]

> [!important] **Un ouvert est une réunion de boules ouvertes** · *Prop. 2.9*
> Une partie non vide est ouverte si et seulement si elle est réunion de boules ouvertes.
> → [[topo-ouverts-reunions-de-boules|énoncé + démonstration]]

> [!important] **Stabilité des fermés** · *Th. 2.10*
> - **(F1)** $E$ et $\emptyset$ sont des fermés.
> - **(F2)** Une intersection **quelconque** de fermés est un fermé.
> - **(F3)** Une réunion **finie** de fermés est un fermé.
> → [[topo-stabilite-fermes|énoncé + démonstration]]

> [!important] **Singletons, parties finies et sphères sont fermés** · *Prop. 2.11*
> Tout singleton $\{a\}$, toute partie finie, toute sphère $S(a,r)$ est un fermé.
> → [[topo-exemples-fermes|énoncé + démonstration]]

> [!important] ⭐ **Caractérisation séquentielle des fermés** · *Th. 2.12*
> $A\subset E$ est fermé si et seulement si **toute suite d'éléments de $A$ qui converge dans $E$ a sa limite dans $A$**.
> → [[topo-caracterisation-sequentielle-fermes|énoncé + démonstration]]

> [!important] ⭐ **Voisinages et boules** · *Prop. 2.15, 2.16 et Th. 2.17*
> 1. $V$ est un voisinage de $a$ $\iff\exists r>0,\ B(a,r)\subset V$.
> 2. $A$ est ouvert $\iff$ $A$ est un voisinage de chacun de ses points.
> 3. (V1)–(V5) : un voisinage contient $a$ ; tout sur-ensemble d'un voisinage en est un ; réunion quelconque et intersection **finie** de voisinages de $a$ sont des voisinages de $a$.
> → [[topo-voisinages-et-boules|énoncé + démonstration]]

> [!important] ⭐ **Caractérisation et propriétés de l'intérieur** · *Prop. 2.19 et 2.20*
> 1. $x\in\operatorname{Int}A\iff\exists r>0,\ B(x,r)\subset A\iff A$ est un voisinage de $x$.
> 2. $A$ est ouvert $\iff\operatorname{Int}A=A$.
> 3. $\operatorname{Int}A$ est le plus grand ouvert contenu dans $A$ : si $O$ est ouvert et $O\subset A$, alors $O\subset\operatorname{Int}A$.
> → [[topo-caracterisation-interieur|énoncé + démonstration]]

> [!important] ⭐ **Caractérisations de l'adhérence** · *Prop. 2.23 et 2.24*
> Pour $x\in E$, sont équivalentes :
> (i) $x\in\bar A$ ; (ii) $\forall r>0,\ B(x,r)\cap A\neq\emptyset$ ; (iii) il existe une suite $(x_n)$ de $A$ qui converge vers $x$.
> De plus, $A$ est fermé $\iff\bar A=A$.
> → [[topo-caracterisation-adherence|énoncé + démonstration]]

> [!important] ⭐ **Intérieur et adhérence échangés par complémentaire** · *Prop. 2.25*
> $$(\bar A)^c=\operatorname{Int}(A^c)\qquad\text{et}\qquad(\operatorname{Int}A)^c=\overline{A^c}.$$
> → [[topo-complementaire-interieur-adherence|énoncé + démonstration]]

> [!important] **Propriétés de la frontière** · *Prop. 2.29*
> (i) $x\in\operatorname{Fr}A\iff$ toute boule $B(x,r)$ contient au moins un point de $A$ et au moins un point de $A^c$.
> (ii) $\operatorname{Fr}A=\bar A\cap\overline{A^c}$ est un fermé.
> (iii) $A$ est fermé $\iff\operatorname{Fr}A\subset A$.
> → [[topo-proprietes-frontiere|énoncé + démonstration]]

> [!important] **Caractérisations de la continuité en un point** · *Th. 2.33*
> Sont équivalentes :
> (i) $f$ est continue en $a$ ;
> (ii) l'image réciproque de tout voisinage de $f(a)$ est un voisinage de $a$ ;
> (iii) pour toute boule $B=B(f(a),r)$, $f^{-1}(B)$ est un voisinage de $a$ ;
> (iv) **pour toute suite $x_n\to a$, $f(x_n)\to f(a)$.**
> → [[topo-caracterisations-continuite-point|énoncé + démonstration]]

> [!important] ⭐ **Continuité globale : image réciproque** · *Th. 2.34*
> Sont équivalentes :
> (i) $f$ est continue sur $E$ ;
> (ii) l'image réciproque de **tout ouvert** de $F$ est un ouvert de $E$ ;
> (iii) l'image réciproque de **tout fermé** de $F$ est un fermé de $E$.
> → [[topo-continuite-globale|énoncé + démonstration]]

> [!important] **Composition d'applications continues** · *Th. 2.35 et 2.41*
> - $f$ continue en $a$ et $g$ continue en $f(a)$ $\Rightarrow g\circ f$ continue en $a$.
> - La composée de deux applications **uniformément** continues est uniformément continue.
> → [[topo-composition-continues|énoncé + démonstration]]

> [!important] **Opérations sur les fonctions continues réelles** · *Prop. 2.36*
> Si $f,g:E\to\mathbb R$ sont continues et $\lambda\in\mathbb R$ : $f+g$, $f-g$, $\lambda f$, $|f|$, $fg$, $\max(f,g)$, $\min(f,g)$ sont continues, et $f/g$ est continue là où $g\neq0$.
> Toute fonction polynomiale en les coordonnées est continue sur $\mathbb R^n$ ; une fraction rationnelle l'est là où son dénominateur ne s'annule pas.
> → [[topo-operations-fonctions-continues|énoncé + démonstration]]

> [!important] **Lipschitzienne ⇒ uniformément continue ⇒ continue** · *Prop. 2.39 et 2.43*
> Toute application lipschitzienne est uniformément continue, et toute application uniformément continue est continue. **Les réciproques sont fausses.**
> → [[topo-hierarchie-lipschitz-uc-continue|énoncé + démonstration]]

> [!important] **Propriétés des isométries** · *Prop. 2.46*
> Une isométrie est injective et 1-lipschitzienne. Si $f$ est une isométrie bijective, $f^{-1}$ est une isométrie.
> → [[topo-isometries|énoncé + démonstration]]

> [!important] **Continuité dans un produit** · *Prop. 2.47, Th. 2.48, Prop. 2.50*
> - Les projections $\pi_i$ sont 1-lipschitziennes.
> - $f=(f_1,\dots,f_p):E\to F_1\times\dots\times F_p$ est continue (resp. U.C.) $\iff$ chaque $f_i$ l'est.
> - Si $f$ est continue en $(a_1,a_2)$, ses applications partielles $x_1\mapsto f(x_1,a_2)$ et $x_2\mapsto f(a_1,x_2)$ sont continues. **Réciproque fausse.**
> → [[topo-continuite-composantes|énoncé + démonstration]]

> [!important] **Bijections continues de R ; homéomorphismes classiques** · *Ex. 2.53, Prop. 2.54, Ex. 2.55*
> - $f:\mathbb R\to\mathbb R$ continue et injective $\Rightarrow$ $I=f(\mathbb R)$ est un intervalle, $f$ est strictement monotone et $f:\mathbb R\to I$ est un homéomorphisme.
> - $]a,b[$ est homéomorphe à $\mathbb R$ (via $\arctan$).
> - Bijection continue **non** bicontinue : $t\mapsto(\cos t,\sin t)$ de $[0,2\pi[$ sur le cercle.
> → [[topo-bijections-continues-de-r|énoncé + démonstration]]

> [!important] ⭐ **Critère des boules (distances topologiquement équivalentes)** · *Prop. 2.59*
> $d_1$ et $d_2$ sont topologiquement équivalentes $\iff$ toute boule $B_{d_1}(a,r)$ contient une boule $B_{d_2}(a,s)$ de même centre, et réciproquement.
> → [[topo-critere-des-boules|énoncé + démonstration]]

> [!important] ⭐ **Métriquement équivalentes ⇒ topologiquement équivalentes** · *Prop. 2.61, Ex. 2.62, Rem. 2.63*
> Deux distances métriquement équivalentes sont topologiquement équivalentes. La **réciproque est fausse**.
> → [[topo-metriquement-implique-topologiquement|énoncé + démonstration]]

> [!important] **Normes équivalentes : caractérisation par encadrement** · *Prop. 2.65 et Ex. 2.66*
> $N_1$ et $N_2$ sont équivalentes $\iff\exists\alpha,\beta>0,\ \forall x\in E,\ \alpha N_1(x)\le N_2(x)\le\beta N_1(x)$.
> Dans $\mathbb R^n$ : $\|x\|_\infty\le\|x\|_2\le\|x\|_1\le n\|x\|_\infty$.
> → [[topo-normes-equivalentes-encadrement|énoncé + démonstration]]

> [!important] **Continuité d'une application linéaire** · *Th. 2.69*
> Pour $f:E\to F$ **linéaire**, sont équivalentes :
> (i) $f$ continue ; (ii) $f$ continue en $0$ ; (iii) $\exists C>0,\ \forall u\in E,\ \|f(u)\|_F\le C\|u\|_E$ ; (iv) $f$ lipschitzienne ; (v) $f$ bornée sur $B_E(0,1)$.
> → [[topo-applications-lineaires-continues|énoncé + démonstration]]

> [!important] **Propriétés de la norme d'opérateur** · *Prop. 2.72 et Ex. 2.73*
> 1. $(\mathcal L_c(E,F),|||\cdot|||)$ est un e.v.n.
> 2. $\|f(u)\|\le|||f|||\,\|u\|$, et toute constante $C$ avec $\|f(u)\|\le C\|u\|$ vérifie $C\ge|||f|||$.
> 3. $|||g\circ f|||\le|||g|||\,|||f|||$.
> 4. Si $\dim E<\infty$, toute application linéaire $E\to F$ est continue.
> → [[topo-proprietes-norme-operateur|énoncé + démonstration]]

## [[03-espaces-metriques-compacts|3 – Espaces métriques compacts]]

> [!important] **Équivalence des normes en dimension finie** · *Th. 2.67 = Th. 3.34 et Cor. 3.35*
> Sur un espace vectoriel de **dimension finie**, toutes les normes sont équivalentes. Conséquences : les compacts sont les fermés bornés, l'espace est complet, toute application linéaire est continue.
> → [[topo-equivalence-normes-dimension-finie|énoncé + démonstration]]

> [!important] **Compacité : version « fermés » et fermés emboîtés** · *Prop. 3.5 et 3.6*
> 1. $E$ est compact $\iff$ pour toute famille de fermés $(F_i)$ d'intersection vide, on peut extraire une sous-famille finie d'intersection vide.
> 2. Si $E$ est compact et $(F_n)$ est une suite **décroissante** de fermés **non vides**, alors $\bigcap_nF_n\neq\emptyset$.
> → [[topo-version-fermes-compacite|énoncé + démonstration]]

> [!important] **Caractérisation séquentielle des compacts (Bolzano–Weierstrass)** · *Th. 3.11 et Lemme 3.12*
> Un espace métrique $(E,d)$ est compact **si et seulement si** de toute suite de $E$ on peut extraire une sous-suite convergente **dans $E$**.
> → [[topo-bolzano-weierstrass|énoncé + démonstration]]

> [!important] **Bolzano–Weierstrass dans R ; les segments sont compacts** · *Th. 3.13*
> Toute suite réelle **bornée** admet une sous-suite convergente. En conséquence, tout segment $[a,b]$ est compact.
> → [[topo-bolzano-weierstrass-dans-r|énoncé + démonstration]]

> [!important] **Suites de Cauchy : convergente ⇒ Cauchy ; Cauchy + sous-suite convergente ⇒ convergente** · *Prop. 3.16 et Lemme 3.17*
> 1. Toute suite convergente est de Cauchy.
> 2. Une suite de Cauchy qui admet une sous-suite convergente converge (vers la même limite).
> → [[topo-convergente-cauchy|énoncé + démonstration]]

> [!important] ⭐ **Un compact est complet et borné ; une partie compacte est fermée et bornée** · *Prop. 3.18, 3.19 et Rem. 3.20*
> 1. Si $(E,d)$ est compact, $E$ est **complet** et **borné**.
> 2. Une partie compacte $A$ d'un espace métrique est **fermée et bornée** dans $E$.
> 3. **Réciproques fausses** en général : $\mathbb R$ complet non compact ; $[0,1[$ borné non compact ; $\mathbb N$ discret fermé borné non compact.
> → [[topo-compact-complet-borne|énoncé + démonstration]]

> [!important] **Un fermé dans un compact est compact** · *Prop. 3.21*
> Si $E$ est compact, une partie $A\subset E$ est compacte $\iff$ elle est fermée.
> → [[topo-ferme-dans-compact|énoncé + démonstration]]

> [!important] ⭐ **Borel–Lebesgue : compacts de R et de R^n** · *Th. 3.22 et Cor. 3.25*
> - Une partie de $\mathbb R$ est compacte $\iff$ elle est **fermée et bornée**.
> - Dans $\mathbb R^n$ (pour n'importe quelle norme, dimension finie) : compact $\iff$ **fermé et borné**.
> → [[topo-borel-lebesgue|énoncé + démonstration]]

> [!important] **Réunion finie et intersection de compacts** · *Prop. 3.23*
> 1. Une réunion **finie** de parties compactes est compacte.
> 2. Une intersection (non vide) d'une famille quelconque de parties compactes est compacte.
> → [[topo-reunions-intersections-compacts|énoncé + démonstration]]

> [!important] **Produit de compacts** · *Prop. 3.24*
> Un produit fini d'espaces métriques compacts, muni de la distance produit, est compact.
> → [[topo-produit-de-compacts|énoncé + démonstration]]

> [!important] ⭐ **Image continue d'un compact ; bijection continue sur un compact** · *Prop. 3.27 et 3.28*
> 1. Si $f:E\to F$ est continue et $A$ est une partie compacte de $E$, alors $f(A)$ est compacte.
> 2. Si $E$ est compact et $f:E\to F$ est continue et bijective, $f$ est un **homéomorphisme**.
> → [[topo-image-continue-compact|énoncé + démonstration]]

> [!important] ⭐ **Une fonction continue sur un compact est bornée et atteint ses bornes** · *Th. 3.30*
> Si $E$ est compact et $f:E\to\mathbb R$ est continue, $f$ est bornée et **atteint ses bornes** : $\exists x_1,x_2\in E,\ \forall x\in E,\ f(x_1)\le f(x)\le f(x_2)$.
> → [[topo-bornes-atteintes|énoncé + démonstration]]

> [!important] ⭐ **Théorème de Heine** · *Th. 3.32*
> Si $E$ est compact et $f:(E,d)\to(F,\delta)$ est continue, alors $f$ est **uniformément continue**.
> → [[topo-heine|énoncé + démonstration]]

> [!important] **Théorème de Riesz** · *Th. 3.36 et Ex. 3.37*
> Dans un e.v.n. $E$, la boule unité fermée $\bar B(0,1)$ est compacte **si et seulement si** $E$ est de dimension finie.
> → [[topo-riesz|énoncé + démonstration]]
