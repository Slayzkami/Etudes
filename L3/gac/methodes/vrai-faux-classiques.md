---
aliases:
  - "Vrai/Faux classiques (avec justification)"
  - "vrai faux"
  - "contre-exemples"
  - "QCM"
tags:
  - gac
  - gac/methode
  - gac/chapitre-03
---

# 🛠️ Vrai/Faux classiques (avec justification)

*Méthode* · Chapitre : [[03-groupes-quotients|III – Groupes quotients]] · [[index-definitions|↩ Index]]

> [!ABSTRACT] Règle
> **Vrai** ⟹ une preuve courte. **Faux** ⟹ **un** contre-exemple explicite et vérifié.

| Affirmation | Réponse | Justification |
|---|---|---|
| Tout groupe abélien est cyclique | **Faux** | Klein $K=(\mathbb Z/2\mathbb Z)^2$ est abélien (calcul coordonnée par coordonnée) ; mais $2x=0$ pour tout $x\in K$, donc $o(x)\le2$ et $\langle x\rangle$ a au plus 2 éléments $\neq K$ (4 éléments) : non cyclique → [[groupe-abelien]] |
| Tout groupe cyclique est abélien | **Vrai** | $a^ka^l=a^{k+l}=a^la^k$ → [[groupe-monogene-cyclique]] |
| $(M_2(\mathbb R),\times)$ est un groupe | **Faux** | $\begin{pmatrix}0&0\\0&0\end{pmatrix}$ n'est pas inversible |
| $(M_2(\mathbb R),+)$ est un groupe abélien | **Vrai** | addition coefficient par coefficient, neutre $0$, opposé $-M$ |
| Dans un groupe, tout élément est simplifiable | **Vrai** | multiplier par $c^{-1}$ → [[regles-de-calcul]] |
| L'équation $x^2=x$ a pour seule solution le neutre | **Vrai** | $xx=x\cdot1$, simplifier par $x$ |
| Les éléments d'ordre 2 forment un sous-groupe | **Faux** | ne contient pas le neutre (ordre 1) ; et dans $\mathfrak S_3$, $\tau_1\tau_2=\gamma^2$ est d'ordre 3 |
| La réunion de deux sous-groupes est un sous-groupe | **Faux** | $2\mathbb Z\cup3\mathbb Z\not\ni5$ → [[intersection-sous-groupes]] |
| Tout sous-groupe d'ordre 2 est normal | **Faux** | $\{e,\tau_1\}\subset\mathfrak S_3$ |
| Tout sous-groupe d'indice 2 est distingué | **Vrai** | [[indice-2-distingue]] |
| Deux groupes de même ordre sont isomorphes | **Faux** | $\mathbb Z/4\mathbb Z\not\simeq$ Klein → [[montrer-non-isomorphes]] |
| Un morphisme conserve l'ordre des éléments | **Faux** | morphisme trivial $\mathbb Z/2\mathbb Z\to\{0\}$ : $o(\bar1)=2$, $o(0)=1$ (vrai si $f$ injectif) |
| Une partie non vide stable est un sous-groupe | **Faux** | $\mathbb N\subset\mathbb Z$ (vrai si $G$ fini) |
| Un groupe d'ordre 6 peut avoir un élément d'ordre 4 | **Faux** | [[lagrange]] : $4\nmid6$ |
| $\mathbb Z/2\mathbb Z\times\mathbb Z/3\mathbb Z$ est cyclique | **Vrai** | $o(\bar1,\bar1)=\operatorname{ppcm}(2,3)=6$ |
| $(xy)^{-1}=x^{-1}y^{-1}$ | **Faux** | dans $\mathfrak S_3$ ; c'est $y^{-1}x^{-1}$ |

## ✍️ Justifications rédigées (comme sur la copie)

Le tableau donne l'idée ; voici la rédaction complète des plus classiques. Cacher, chercher, puis déplier.

> [!SUCCESS]- « Tout groupe abélien est cyclique » : **Faux**
> Contre-exemple : $K=\mathbb Z/2\mathbb Z\times\mathbb Z/2\mathbb Z$.
> - $K$ est abélien : $(a,b)+(c,d)=(a+c,b+d)=(c+a,d+b)=(c,d)+(a,b)$.
> - $K$ n'est pas cyclique : pour tout $x=(a,b)\in K$, $2x=(2a,2b)=(\bar0,\bar0)$, donc $o(x)\le2$ et $\langle x\rangle$ a au plus 2 éléments. Or $K$ en a 4 : aucun $x$ ne vérifie $\langle x\rangle=K$.
>
> → [[groupe-abelien]]

> [!SUCCESS]- « Tout groupe cyclique est abélien » : **Vrai**
> Soit $G=\langle a\rangle$ et $x,y\in G$. Il existe $k,l\in\mathbb Z$ tels que $x=a^k$, $y=a^l$. Alors $xy=a^ka^l=a^{k+l}=a^{l+k}=a^la^k=yx$.

> [!SUCCESS]- « Deux groupes de même ordre sont isomorphes » : **Faux**
> $\mathbb Z/4\mathbb Z$ et $K=\mathbb Z/2\mathbb Z\times\mathbb Z/2\mathbb Z$ ont tous les deux 4 éléments.
> Supposons qu'il existe un isomorphisme $f:\mathbb Z/4\mathbb Z\to K$. Alors $f(\bar2)=f(\bar1+\bar1)=f(\bar1)+f(\bar1)=(\bar0,\bar0)=f(\bar0)$ (car $2x=0$ pour tout $x\in K$). Par injectivité, $\bar2=\bar0$ dans $\mathbb Z/4\mathbb Z$ : absurde.
> En clair : $\mathbb Z/4\mathbb Z$ possède un élément d'ordre 4 ($\bar1$), Klein n'en a pas.
> → [[montrer-non-isomorphes]]

> [!SUCCESS]- « La réunion de deux sous-groupes est un sous-groupe » : **Faux**
> Dans $(\mathbb Z,+)$ : $H=2\mathbb Z$ et $K=3\mathbb Z$ sont des sous-groupes. $2\in H\cup K$ et $3\in H\cup K$, mais $2+3=5$ n'est ni pair ni multiple de 3 : $5\notin H\cup K$. Donc $H\cup K$ n'est pas stable par $+$.
> → [[intersection-sous-groupes]]

> [!SUCCESS]- « Les éléments d'ordre 2 d'un groupe forment un sous-groupe » : **Faux**
> Un sous-groupe contient le neutre ; or le neutre est d'ordre 1, pas 2. Donc l'ensemble des éléments d'ordre 2 ne contient pas le neutre : ce n'est pas un sous-groupe.

> [!SUCCESS]- « Un morphisme conserve l'ordre des éléments » : **Faux**
> $f:\mathbb Z/2\mathbb Z\to\mathbb Z/2\mathbb Z$, $x\mapsto\bar0$ est un morphisme ($f(x+y)=\bar0=\bar0+\bar0$). Or $o(\bar1)=2$ et $o(f(\bar1))=o(\bar0)=1$.
> Ce qui est vrai : $o(f(x))$ **divise** $o(x)$ (car $f(x)^{o(x)}=f(x^{o(x)})=f(1)=1$), avec égalité si $f$ est injectif.

> [!SUCCESS]- « Une partie non vide et stable par la loi est un sous-groupe » : **Faux**
> $\mathbb N\subset(\mathbb Z,+)$ est non vide et stable par $+$, mais $1\in\mathbb N$ et son opposé $-1\notin\mathbb N$.
> (C'est vrai si le groupe est **fini** → [[caracterisation-sous-groupe]].)

> [!SUCCESS]- « Un groupe d'ordre 6 peut contenir un élément d'ordre 4 » : **Faux**
> D'après le [[lagrange|théorème de Lagrange]], l'ordre d'un élément divise l'ordre du groupe. Or $4\nmid6$.

> [!SUCCESS]- « $\mathbb Z/2\mathbb Z\times\mathbb Z/3\mathbb Z$ est cyclique » : **Vrai**
> Le groupe a 6 éléments. Calculons les multiples de $x=(\bar1,\bar1)$ :
> $1x=(\bar1,\bar1)$, $2x=(\bar0,\bar2)$, $3x=(\bar1,\bar0)$, $4x=(\bar0,\bar1)$, $5x=(\bar1,\bar2)$, $6x=(\bar0,\bar0)$.
> Les 6 éléments sont obtenus : $\langle x\rangle$ est le groupe entier, qui est donc cyclique (et $\simeq\mathbb Z/6\mathbb Z$ → [[lemme-chinois]]).

> [!SUCCESS]- « Dans un groupe, $x^2=x$ entraîne $x=e$ » : **Vrai**
> $x\star x=x=x\star e$ ; en composant à gauche par $x^{-1}$ : $x=e$ → [[regles-de-calcul]].

> [!SUCCESS]- « $(M_2(\mathbb R),\times)$ est un groupe » : **Faux**
> Le neutre ne pourrait être que $I_2$, et la matrice nulle $0$ n'a pas d'inverse : pour toute $M$, $0\times M=0\neq I_2$.

## 🔗 Liens

- **Utilisé par (définitions)** : [[ordre-element|Ordre d'un élément]]
- **Révision** : [[exercices-types-corriges|Exercices types corrigés]], [[mes-erreurs|Mes erreurs à ne plus faire]]
- **Voir aussi** : [[regles-de-calcul|Règles de calcul dans un groupe]], [[lagrange|Théorème de Lagrange]]
