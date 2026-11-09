---
aliases:
  - "Méthode : relation d'équivalence, classes et quotient"
  - "montrer qu'une relation est une relation d'équivalence"
  - "décrire les classes"
  - "décrire le quotient"
tags:
  - gac
  - gac/methode
  - gac/chapitre-00
---

# 🛠️ Méthode : relation d'équivalence, classes et quotient

*Méthode* · Chapitre : [[00-rappels-relations-equivalence|Rappels – Relations d'équivalence]] · [[index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> 1. **Réflexive** : « Soit $x\in E$. » Montrer $x\mathcal Rx$.
> 2. **Symétrique** : « Soient $x,y\in E$ tels que $x\mathcal Ry$. » Montrer $y\mathcal Rx$.
> 3. **Transitive** : « Soient $x,y,z\in E$ tels que $x\mathcal Ry$ et $y\mathcal Rz$. » Montrer $x\mathcal Rz$.
> 4. **Classe de $x$** : écrire $\bar x=\{y\in E\mid y\mathcal Rx\}$ et **résoudre** la condition en $y$.
> 5. **Quotient** : chercher une quantité $f(x)$ qui est la même sur toute une classe et différente d'une classe à l'autre ; alors $\bar x\mapsto f(x)$ est une bijection de $E/\mathcal R$ sur $f(E)$.
>
> **Raccourci** : si $x\mathcal Ry\iff f(x)=f(y)$ pour une application $f$, les trois propriétés viennent de celles de « $=$ ».
> **Dans un groupe** : $x\mathcal Ry\iff x^{-1}y\in H$ est une relation d'équivalence dès que $H$ est un sous-groupe ; ses classes sont les $xH$ → [[classes-modulo-sous-groupe]].

> [!EXAMPLE] Rédaction modèle : sur $\mathbb Z$, $x\mathcal Ry\iff n\mid x-y$
> - Réflexive : $x-x=0=n\times0$.
> - Symétrique : si $x-y=nk$, alors $y-x=n(-k)$.
> - Transitive : si $x-y=nk$ et $y-z=nl$, alors $x-z=n(k+l)$.
> - Classe : $\bar x=\{x+nk,\ k\in\mathbb Z\}=x+n\mathbb Z$. Il y a $n$ classes : $\bar0,\dots,\overline{n-1}$ (une par reste).
> - **Compatible avec $+$** : si $n\mid x-y$ et $n\mid x'-y'$, alors $n\mid(x+x')-(y+y')$. Donc $\bar x+\bar x'=\overline{x+x'}$ est bien définie → [[loi-quotient]].

> [!WARNING] Pièges
> - Pour **réfuter** : un contre-exemple chiffré à **une** des trois propriétés suffit. Ex. : « $x\mid y$ » sur $\mathbb N^*$ n'est pas symétrique ($1\mid2$ mais $2\nmid1$).
> - Compatibilité : pour réfuter, donner $x\mathcal Ry$, $x'\mathcal Ry'$ avec $x\star x'$ et $y\star y'$ non reliés. Ex. : $|x|=|y|$ sur $(\mathbb Z,+)$ : $1\mathcal R(-1)$, $1\mathcal R1$, mais $2$ et $0$ ne sont pas reliés.

## 🔗 Liens

- **S'appuie sur** : [[relation-equivalence|Relation d'équivalence]], [[classe-equivalence|Classe d'équivalence]], [[ensemble-quotient|Ensemble quotient]], [[relation-compatible|Relation compatible]]
- **Voir aussi** : [[classes-et-indice]], [[morphisme-sur-quotient]]
- **Corrigés** : [[exercices-types-corriges#6. Relation d'équivalence associée à une application|ex. 6]]
