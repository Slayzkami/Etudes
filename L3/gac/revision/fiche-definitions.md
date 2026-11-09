---
aliases:
  - "Fiche de définitions GAC"
  - "toutes les définitions"
tags:
  - gac
  - gac/revision
---

# 📘 Fiche de révision – toutes les définitions

Toutes les définitions du programme du partiel sur une seule page, dans l'ordre du cours. Chaque encadré renvoie à sa fiche complète (exemples, pièges, liens). · [[plan-de-revision|↩ Plan de révision]] · [[index-definitions|↩ Index]] · Suite : [[fiche-theoremes]]

## Rappels – Relations d'équivalence

> [!note] **Relation d'équivalence**
> Une relation binaire $\mathcal R$ sur un ensemble $E$ est une **relation d'équivalence** si elle est
> - **réflexive** : $\forall x\in E,\ x\mathcal R x$ ;
> - **symétrique** : $\forall x,y\in E,\ x\mathcal R y\Rightarrow y\mathcal R x$ ;
> - **transitive** : $\forall x,y,z\in E,\ (x\mathcal R y \text{ et } y\mathcal R z)\Rightarrow x\mathcal R z$.
> → [[relation-equivalence|fiche complète]]

> [!note] **Classe d'équivalence**
> Soit $\mathcal R$ une [[relation-equivalence|relation d'équivalence]] sur $E$. La **classe** de $x\in E$ est
> $$\bar x=\operatorname{cl}(x)=\{y\in E \mid y\mathcal R x\}.$$
> Tout $y\in\bar x$ est un **représentant** de la classe ($\bar y=\bar x$).
> → [[classe-equivalence|fiche complète]]

> [!note] **Ensemble quotient et projection canonique**
> - L'**ensemble quotient** $E/\mathcal R$ est l'ensemble des [[classe-equivalence|classes d'équivalence]].
> - La **projection (surjection) canonique** est $p:E\to E/\mathcal R,\ x\mapsto\bar x$ ; elle est surjective.
> → [[ensemble-quotient|fiche complète]]

> [!note] **Relation compatible avec une loi**
> Soit $\star$ une [[loi-composition-interne|loi interne]] sur $E$ et $\mathcal R$ une [[relation-equivalence|relation d'équivalence]]. $\mathcal R$ est
> - **compatible à gauche** avec $\star$ : $\forall a,x,y\in E,\ x\mathcal R y\Rightarrow(a\star x)\,\mathcal R\,(a\star y)$ ;
> - **compatible à droite** : $\forall a,x,y\in E,\ x\mathcal R y\Rightarrow(x\star a)\,\mathcal R\,(y\star a)$ ;
> - **compatible** : $\forall x,y,x',y'\in E,\ (x\mathcal R y \text{ et } x'\mathcal R y')\Rightarrow(x\star x')\,\mathcal R\,(y\star y')$.
> → [[relation-compatible|fiche complète]]

> [!note] **Loi quotient**
> Si $\mathcal R$ est [[relation-compatible|compatible]] avec $\star$, on définit sur $E/\mathcal R$ :
> $$\forall x,y\in E,\qquad \bar x\,\dot\star\,\bar y=\overline{x\star y}.$$
> Le résultat **ne dépend pas des représentants** (c'est exactement la compatibilité), et $p(x\star y)=p(x)\,\dot\star\,p(y)$.
> → [[loi-quotient|fiche complète]]


## I – Définitions générales

> [!note] **Loi de composition interne**
> Une **loi de composition interne** sur $E$ est une application $E\times E\to E,\ (x,y)\mapsto x\star y$.
> → [[loi-composition-interne|fiche complète]]

> [!note] **Groupe**
> Soit $G$ un ensemble **non vide** muni d'une [[loi-composition-interne|l.c.i.]] $\star$. $(G,\star)$ est un **groupe** si :
> - **(G1)** associativité : $\forall x,y,z\in G,\ x\star(y\star z)=(x\star y)\star z$ ;
> - **(G2)** élément neutre : $\exists e\in G,\ \forall x\in G,\ x\star e=x=e\star x$ ;
> - **(G3)** symétrique : $\forall x\in G,\ \exists x'\in G,\ x\star x'=e=x'\star x$.
> → [[groupe|fiche complète]]

> [!note] **Groupe – Notations**
> - multiplicative : loi $xy$, neutre $1$, symétrique $x^{-1}$ (**inverse**) ;
> - additive (réservée aux groupes abéliens) : loi $x+y$, neutre $0$, symétrique $-x$ (**opposé**).
> → [[groupe|fiche complète]]

> [!note] **Groupe abélien**
> Un [[groupe]] $(G,\star)$ est **abélien** (ou commutatif) si $\forall x,y\in G,\ x\star y=y\star x$.
> → [[groupe-abelien|fiche complète]]

> [!note] **Puissances et multiples**
> Dans un [[groupe]] multiplicatif, pour $x\in G$ et $n\in\mathbb N^*$ :
> $$x^0=1,\qquad x^n=\underbrace{x\cdots x}_{n\text{ fois}},\qquad x^{-n}=(x^{-1})^n.$$
> En notation additive : $0x=0$, $nx=x+\dots+x$ ($n$ fois), $(-n)x=n(-x)$.
> → [[puissances-multiples|fiche complète]]

> [!note] **Groupe des permutations**
> Une **permutation** de $E$ est une bijection $E\to E$. $\mathcal S(E)$ est l'ensemble des permutations de $E$ ; muni de $\circ$, c'est un [[groupe]] (neutre $\mathrm{id}_E$, symétrique $f^{-1}$).
> $\mathfrak S_n=\mathcal S(\{1,\dots,n\})$ est le **groupe symétrique** ; $\mathrm{Card}(\mathfrak S_n)=n!$.
> → [[groupe-des-permutations|fiche complète]]

> [!note] **Groupe produit**
> Si $(G,\star)$ et $(G',\star')$ sont des [[groupe|groupes]], $G\times G'$ muni de
> $$(a,a')\top(b,b')=(a\star b,\ a'\star'b')$$
> est un groupe : neutre $(e,e')$, symétrique de $(a,a')$ : $(a^{-1},a'^{-1})$. Il est abélien si $G$ et $G'$ le sont.
> → [[groupe-produit|fiche complète]]

> [!note] **Morphisme de groupes**
> Soient $(G,\star)$, $(G',\star')$ deux [[groupe|groupes]]. $f:G\to G'$ est un **(homo)morphisme** si
> $$\forall x,y\in G,\qquad f(x\star y)=f(x)\star'f(y).$$
> - **endomorphisme** : $G=G'$ ;
> - **isomorphisme** : morphisme bijectif ;
> - **automorphisme** : endomorphisme bijectif.
> → [[morphisme-de-groupes|fiche complète]]

> [!note] **Groupes isomorphes**
> $G_1$ est **isomorphe** à $G_2$, noté $G_1\simeq G_2$, s'il existe un [[morphisme-de-groupes|isomorphisme]] de $G_1$ sur $G_2$.
> « Être isomorphe » est une relation d'équivalence (id, réciproque, composée).
> → [[groupes-isomorphes|fiche complète]]

> [!note] **Automorphismes et automorphismes intérieurs**
> - $\mathrm{Aut}\,G$ : ensemble des automorphismes de $G$ ; c'est un groupe pour $\circ$ (sous-groupe de $\mathcal S(G)$).
> - Pour $a\in G$, l'**automorphisme intérieur** associé à $a$ est $f_a:G\to G,\ x\mapsto axa^{-1}$.
> - $\mathcal I(G)=\{f_a\mid a\in G\}$ est un [[sous-groupe]] de $\mathrm{Aut}\,G$.
> → [[automorphismes|fiche complète]]


## II – Sous-groupes

> [!note] **Sous-groupe**
> Soit $(G,\star)$ un [[groupe]] et $H\subset G$. $H$ est un **sous-groupe** de $G$ si :
> 1. $H$ est non vide ;
> 2. $H$ est stable par la loi : $\forall x,y\in G,\ (x,y)\in H^2\Rightarrow x\star y\in H$ ;
> 3. $H$ est stable par symétrisation : $\forall x\in G,\ x\in H\Rightarrow x^{-1}\in H$.
> → [[sous-groupe|fiche complète]]

> [!note] **Sous-groupe distingué**
> Un [[sous-groupe]] $H$ de $G$ est **distingué** (normal, invariant), noté $H\lhd G$, si
> $$\forall g\in G,\ \forall h\in H,\qquad g^{-1}hg\in H.$$
> → [[sous-groupe-distingue|fiche complète]]

> [!note] **Centre d'un groupe**
> $$Z(G)=\{g\in G \mid \forall x\in G,\ gx=xg\}.$$
> → [[centre|fiche complète]]

> [!note] **Sous-groupe engendré par une partie**
> Pour $A\subset G$, $\mathrm{Gr}\langle A\rangle$ (ou $\langle A\rangle$) est l'**intersection de tous les sous-groupes de $G$ contenant $A$**.
> → [[sous-groupe-engendre|fiche complète]]

> [!note] **Groupe monogène, groupe cyclique**
> - $A$ **engendre** $G$ (partie génératrice) si $\mathrm{Gr}\langle A\rangle=G$.
> - $G$ est **monogène** s'il existe $a\in G$ tel que $G=\langle a\rangle$.
> - $G$ est **cyclique** s'il est monogène **et fini**.
> → [[groupe-monogene-cyclique|fiche complète]]

> [!note] **Image, noyau, image réciproque**
> Soit $f:G\to G'$ un [[morphisme-de-groupes|morphisme]].
> - **Image** : $\mathrm{Im} f=f(G)=\{f(x)\mid x\in G\}\subset G'$.
> - **Noyau** : $\mathrm{Ker} f=\{x\in G\mid f(x)=1_{G'}\}=f^{-1}(\{1_{G'}\})\subset G$.
> - **Image réciproque** de $H'\subset G'$ : $f^{-1}(H')=\{x\in G\mid f(x)\in H'\}$.
> → [[image-noyau|fiche complète]]

> [!note] **Ordre d'un élément**
> $o(x)$ est le **plus petit entier $m\ge1$ tel que $x^m=1$**, s'il existe ; sinon $x$ est **d'ordre infini**.
> (Additif : plus petit $m\ge1$ tel que $mx=0$.)
> → [[ordre-element|fiche complète]]

> [!note] **Ordre d'un groupe**
> L'**ordre** d'un groupe (ou sous-groupe) fini est son nombre d'éléments : $\mathrm{Card}(G)$, $\#G$, $|G|$ ou $[G]$.
> → [[ordre-groupe|fiche complète]]


## III – Groupes quotients

> [!note] **Classes à gauche et à droite modulo un sous-groupe**
> Soit $H$ un [[sous-groupe]] de $G$.
> - La relation $x\mathcal R y\iff x^{-1}y\in H$ est une [[relation-equivalence|relation d'équivalence]] [[relation-compatible|compatible à gauche]] ; la classe de $1$ est $H$.
> - **Classe à gauche** de $x$ : $xH=\{xh\mid h\in H\}$ (c'est la classe de $x$ pour $\mathcal R$).
> - **Classe à droite** : $Hx=\{hx\mid h\in H\}$ (classes de $x\mathcal R y\iff yx^{-1}\in H$, compatible à droite).
> - $G/H$ = ensemble des classes à gauche.
> → [[classes-modulo-sous-groupe|fiche complète]]

> [!note] **Congruence modulo un sous-groupe**
> Si $H$ est un sous-groupe tel que $\forall x\in G,\ x^{-1}Hx=H$ (c.-à-d. $H\lhd G$), la relation
> $$x\equiv y\pmod H\iff x^{-1}y\in H$$
> est la **congruence modulo $H$**. En additif : $x\equiv y\pmod H\iff x-y\in H$.
> → [[congruence-modulo-sous-groupe|fiche complète]]

> [!note] **Indice d'un sous-groupe**
> Pour $G$ fini et $H$ sous-groupe : $[G:H]=\dfrac{[G]}{[H]}$ = **nombre de classes à gauche** modulo $H$.
> → [[indice|fiche complète]]

> [!note] **Groupe quotient – Définition (cas général)**
> Si $H\lhd G$, l'ensemble $G/H$ des classes $\bar x=xH=Hx$, muni de
> $$\bar x\,\dot\times\,\bar y=\overline{xy}\quad\text{c.-à-d.}\quad (xH)(yH)=(xy)H,$$
> est un groupe, le **groupe quotient** : neutre $\bar1=H$, inverse de $\bar x$ : $\overline{x^{-1}}$.
> La projection $p:G\to G/H,\ x\mapsto\bar x$ est un morphisme surjectif de noyau $H$. Si $G$ est fini, $[G/H]=[G:H]$.
> → [[groupe-quotient|fiche complète]]

> [!note] **Groupe quotient – Cas abélien (notation additive)**
> $H$ sous-groupe de $(G,+)$ abélien : $\bar x\,\dot+\,\bar y=\overline{x+y}$ ; $G/H$ est un groupe abélien.
> → [[groupe-quotient|fiche complète]]

> [!note] **Application induite et décomposition canonique**
> Pour un [[morphisme-de-groupes|morphisme]] $f:G_1\to G_2$ :
> $$\bar f:G_1/\mathrm{Ker} f\to\mathrm{Im} f,\qquad \bar x\mapsto f(x).$$
> Elle est **bien définie** grâce au lemme : $\bar x=\bar y\iff f(x)=f(y)$.
> → [[application-induite|fiche complète]]

## 🔗 Liens

- [[fiche-theoremes]] · [[exemples-de-groupes]] · [[mes-erreurs]] · [[exercices-types-corriges]]
