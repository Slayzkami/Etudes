---
aliases:
  - "Fiche des théorèmes GAC"
  - "tous les théorèmes"
tags:
  - gac
  - gac/revision
---

# ⭐ Fiche de révision – tous les énoncés

Tous les théorèmes et propositions du programme, énoncés seuls. Les démonstrations sont dans les fiches complètes (encadrés repliables). · [[plan-de-revision|↩ Plan de révision]] · [[index-definitions|↩ Index]] · Avant : [[fiche-definitions]]

## I – Définitions générales

> [!important] **Unicité du neutre et du symétrique**
> Dans un [[groupe]] (et même dans un monoïde) : le neutre est unique ; le symétrique d'un élément est unique.
> → [[unicite-neutre-symetrique|fiche complète]]

> [!important] **Règles de calcul dans un groupe**
> Pour $a,b,c$ dans un [[groupe]] multiplicatif :
> 1. $1^{-1}=1$, $(a^{-1})^{-1}=a$, $(ab)^{-1}=b^{-1}a^{-1}$ ;
> 2. $\forall m,n\in\mathbb Z$ : $a^na^m=a^{n+m}$, $(a^n)^m=a^{nm}$, $(a^n)^{-1}=a^{-n}$ ;
> 3. **simplification** : $ac=bc\Rightarrow a=b$ et $ca=cb\Rightarrow a=b$ ;
> 4. **équations** : $ax=b\iff x=a^{-1}b$ ; $xa=b\iff x=ba^{-1}$ ;
> 5. si $ab=ba$ : $(ab)^n=a^nb^n$.
> → [[regles-de-calcul|fiche complète]]

> [!important] **Propriétés des morphismes**
> Si $f:G\to G'$ est un [[morphisme-de-groupes|morphisme]] :
> 1. $f(1_G)=1_{G'}$ ; 2. $f(x^{-1})=f(x)^{-1}$ ; 3. $\forall n\in\mathbb Z,\ f(x^n)=f(x)^n$.
>
> La composée de deux morphismes (isomorphismes) est un morphisme (isomorphisme) ; la réciproque d'un isomorphisme est un isomorphisme.
> → [[proprietes-morphismes|fiche complète]]


## II – Sous-groupes

> [!important] **Caractérisations d'un sous-groupe**
> 1. $H$ est un [[sous-groupe]] de $G$ $\iff$ $H$ est stable et $(H,\star)$ est un groupe.
> 2. **Caractérisation pratique** : $H$ sous-groupe $\iff$ **$e\in H$** et **$\forall x,y\in H,\ x\star y^{-1}\in H$**
>    (additif : $0\in H$ et $x-y\in H$).
> 3. Si $G$ est **fini** : $H\neq\emptyset$ sous-groupe $\iff$ $H$ stable par la loi.
> → [[caracterisation-sous-groupe|fiche complète]]

> [!important] **Intersection et réunion de sous-groupes**
> 1. Une intersection (non vide d'indices) de [[sous-groupe|sous-groupes]] est un sous-groupe ; de sous-groupes distingués, un sous-groupe distingué (TD1 ex. 6).
> 2. $H\cup K$ est un sous-groupe $\iff H\subset K$ ou $K\subset H$.
> 3. La réunion d'une famille **totalement ordonnée** de sous-groupes est un sous-groupe (TD1 ex. 5).
> → [[intersection-sous-groupes|fiche complète]]

> [!important] **Sous-groupes de (Z,+)**
> Les sous-groupes de $(\mathbb Z,+)$ sont exactement les $a\mathbb Z=\{an\mid n\in\mathbb Z\}$, $a\in\mathbb N$, et $a$ est unique (si $H\neq\{0\}$, $a=\min(H\cap\mathbb N^*)$).
> Inclusions : $a\mathbb Z\subset b\mathbb Z\iff b\mid a$.
> → [[sous-groupes-de-z|fiche complète]]

> [!important] **Noyau distingué, image sous-groupe, injectivité**
> Soit $f:G\to G'$ un morphisme, $H\le G$, $H'\le G'$.
> 1. $f(H)$ est un sous-groupe de $G'$ ; $f^{-1}(H')$ est un sous-groupe de $G$, distingué si $H'\lhd G'$.
> 2. **$\mathrm{Ker} f$ est un sous-groupe distingué de $G$** ; $\mathrm{Im} f$ est un sous-groupe de $G'$.
> 3. **$f$ injectif $\iff\mathrm{Ker} f=\{1_G\}$.**
> → [[noyau-et-image|fiche complète]]

> [!important] **Ordre d'un élément de Z/nZ**
> Dans $(\mathbb Z/n\mathbb Z,+)$ : $\displaystyle o(\bar k)=\frac{n}{\operatorname{pgcd}(n,k)}$. En particulier $\bar k$ engendre $\mathbb Z/n\mathbb Z\iff\operatorname{pgcd}(n,k)=1$.
> → [[ordre-dans-znz|fiche complète]]

> [!important] **Structure des groupes monogènes**
> - Tout [[groupe-monogene-cyclique|groupe monogène]] infini est isomorphe à $(\mathbb Z,+)$.
> - Tout groupe cyclique d'ordre $n$ est isomorphe à $(\mathbb Z/n\mathbb Z,+)$ : si $G=\langle a\rangle$, alors $o(a)=n$, $G=\{1,a,\dots,a^{n-1}\}$ et $\bar k\mapsto a^k$ est un isomorphisme.
> - Un groupe monogène est abélien.
> → [[structure-groupes-monogenes|fiche complète]]


## III – Groupes quotients

> [!important] **Relations compatibles avec la loi d'un groupe**
> - Compatible **à gauche** $\iff$ $x\mathcal R y\iff x^{-1}y\in H$ pour un sous-groupe $H$ ($H=\bar1$) ; classes $xH$.
> - Compatible **à droite** $\iff$ $x\mathcal R y\iff yx^{-1}\in H$ ; classes $Hx$.
> - **Compatible** $\iff$ $x\mathcal R y\iff x^{-1}y\in H$ avec $\forall x,\ x^{-1}Hx=H$, i.e. $H\lhd G$ ; alors $xH=Hx$ ([[congruence-modulo-sous-groupe]]).
> - Si $\mathcal R$ est compatible, $G/\mathcal R$ est un groupe (neutre $\bar1$, inverse $\overline{x^{-1}}$) et $p$ est un morphisme surjectif.
> → [[relations-compatibles-groupe|fiche complète]]

> [!important] **Théorème de Lagrange**
> Soit $G$ un groupe fini et $H$ un sous-groupe. Alors **$[H]$ divise $[G]$**, et $[G]=[G:H]\,[H]$ ([[indice]]).
> → [[lagrange|fiche complète]]

> [!important] **Théorème de Lagrange – Corollaire**
> $\forall x\in G$ : $o(x)\mid[G]$ et $x^{[G]}=1$.
> (Car $o(x)=\mathrm{Card}\,\langle x\rangle$ ; si $[G]=k\,o(x)$, $x^{[G]}=(x^{o(x)})^k=1$.)
> → [[lagrange|fiche complète]]

> [!important] **Un sous-groupe d'indice 2 est distingué**
> Si $H$ n'a que deux classes à gauche ($[G:H]=2$), alors $H\lhd G$.
> → [[indice-2-distingue|fiche complète]]

> [!important] **Premier théorème d'isomorphisme**
> Pour tout morphisme $f:G_1\to G_2$ :
> $$G_1/\mathrm{Ker} f\ \simeq\ \mathrm{Im} f\qquad\text{via}\qquad \bar f:\bar x\mapsto f(x).$$
> Décomposition canonique : $f=i\circ\bar f\circ p$ → [[application-induite]].
> Si $G_1$ est fini : $[G_1]=[\mathrm{Ker} f]\cdot[\mathrm{Im} f]$.
> → [[premier-theoreme-isomorphisme|fiche complète]]

> [!important] **Groupe d'ordre premier**
> Si $[G]=p$ premier : $G$ n'a pas de sous-groupe propre non trivial, $G$ est cyclique, engendré par **tout** $x\neq1$, et $G\simeq\mathbb Z/p\mathbb Z$.
> → [[groupe-ordre-premier|fiche complète]]

> [!important] **Lemme chinois (groupes)**
> Si $\operatorname{pgcd}(m_1,m_2)=1$ : $\mathbb Z/m_1m_2\mathbb Z\simeq\mathbb Z/m_1\mathbb Z\times\mathbb Z/m_2\mathbb Z$, via $\bar n\mapsto(n\bmod m_1,\ n\bmod m_2)$.
> → [[lemme-chinois|fiche complète]]

## 🔗 Liens

- [[fiche-definitions]] · [[vrai-faux-classiques]] · [[exercices-types-corriges]]
