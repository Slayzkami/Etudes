---
aliases:
  - "Exemples et contre-exemples topologie"
  - "catalogue topologie"
tags:
  - topologie
  - topo/exemples
---

# 🧩 Exemples et contre-exemples classiques

Les objets qui reviennent partout (cours, TD, sujets). Les connaître par cœur permet de répondre aux Vrai/Faux et de trouver vite une suite ou un contre-exemple. · [[topo-index-definitions|↩ Index]]

## Parties de R

| Partie | Ouvert | Fermé | Adhérence | Intérieur | Frontière | Compact |
|---|---|---|---|---|---|---|
| $]a,b[$ | oui | non | $[a,b]$ | $]a,b[$ | $\{a,b\}$ | non |
| $[a,b]$ | non | oui | $[a,b]$ | $]a,b[$ | $\{a,b\}$ | **oui** |
| $[0,1[$ | non | non | $[0,1]$ | $]0,1[$ | $\{0,1\}$ | non |
| $]0,1]\cup\{2\}$ | non | non | $[0,1]\cup\{2\}$ | $]0,1[$ | $\{0,1,2\}$ | non |
| $]0,+\infty[$ | oui | non | $[0,+\infty[$ | $]0,+\infty[$ | $\{0\}$ | non |
| $\mathbb Z$ | non | oui | $\mathbb Z$ | $\emptyset$ | $\mathbb Z$ | non (non borné) |
| $\mathbb Q$ | non | non | $\mathbb R$ | $\emptyset$ | $\mathbb R$ | non |
| $\{\frac1n\mid n\ge1\}$ | non | non | $\{\frac1n\}\cup\{0\}$ | $\emptyset$ | $\{\frac1n\}\cup\{0\}$ | non |
| $\{\frac1n\}\cup\{0\}$ | non | oui | lui-même | $\emptyset$ | lui-même | **oui** |
| $\{e^{-n}\mid n\in\mathbb N\}$ | non | non | $\{e^{-n}\}\cup\{0\}$ | $\emptyset$ | $\{e^{-n}\}\cup\{0\}$ | non |
| $\{(-1)^n+\frac1n\}$ | non | non | ajoute $1$ et $-1$ | $\emptyset$ | adhérence | non |
| $\mathbb R$, $\emptyset$ | oui | oui | lui-même | lui-même | $\emptyset$ | $\emptyset$ oui, $\mathbb R$ non |

## Parties de R²

| Partie | Nature | Adhérence | Intérieur |
|---|---|---|---|
| $\{y>0\}$ | ouvert, non fermé | $\{y\ge0\}$ | lui-même |
| $\{x>0,\ y\ge0\}$ | ni ouvert ni fermé | $\{x\ge0,\ y\ge0\}$ | $\{x>0,\ y>0\}$ |
| $\{x^2+y^2<1,\ y\ge0\}$ (demi-disque) | ni l'un ni l'autre | $\{x^2+y^2\le1,\ y\ge0\}$ | $\{x^2+y^2<1,\ y>0\}$ |
| $\{0<x^2+y^2\le1\}$ (disque pointé) | ni l'un ni l'autre | disque fermé | $\{0<x^2+y^2<1\}$ |
| $\{x>0,\ y=x^2\}$ (interro 25-26) | ni l'un ni l'autre | $\{x\ge0,\ y=x^2\}$ | $\emptyset$ |
| $\{y=e^{x^2}\}$, graphe d'une fonction continue | **fermé**, non ouvert | lui-même | $\emptyset$ |
| $\{xy=1\}$ (hyperbole) | fermé, non borné | lui-même | $\emptyset$ ; **non compact** |
| $\{(\frac1n,0)\}$ ou $\{(0,e^{-n})\}$ | ni l'un ni l'autre | ajoute $(0,0)$ | $\emptyset$ |
| $([-1,0[\cup]0,1])\times\mathbb R$ (écrit 25-26) | ni l'un ni l'autre | $[-1,1]\times\mathbb R$ | $(]-1,0[\cup]0,1[)\times\mathbb R$ |
| $\{\lvert x\rvert+\lvert y\rvert\le1\}$, $\{x^2+y^4\le1\}$ | fermé borné | lui-même | inégalité stricte ; **compact** |

## Distances et normes

| Objet | À retenir | Fiche |
|---|---|---|
| Distance discrète | boules $\{a\}$ ou $E$ ; toute partie ouverte et fermée ; pas de norme ; compact $\iff$ fini | [[topo-distance-discrete]] |
| $\min(1,d)$ | distance ; mêmes ouverts que $d$ ; tout est borné ; pas métriquement équivalente si $E$ non borné | [[topo-montrer-distance]] |
| $\lvert f(x)-f(y)\rvert$, $f$ injective | distance ; ex. $\frac x{1+\lvert x\rvert}$ (R borné, boules $]-\frac r{1-r},\frac r{1-r}[$), $\arctan$ | [[topo-montrer-distance]] |
| $\lvert x-y\rvert$ et $\lvert x^2-y^2\rvert$ sur $[0,+\infty[$ | topologiquement, pas métriquement équivalentes | [[topo-metriquement-implique-topologiquement]] |
| $(x-y)^3$ ; $\min(\lvert x-x'\rvert,\lvert y-y'\rvert)$ | **pas** des distances (positivité ; séparation) | [[topo-distance]] |
| $\lVert\cdot\rVert_1,\lVert\cdot\rVert_2,\lVert\cdot\rVert_\infty$ sur $\mathbb R^n$ | équivalentes ; boules losange, disque, carré | [[topo-normes-usuelles]] |
| Les mêmes sur $C([a,b])$ | **pas** équivalentes ($x^n$) | [[topo-equivalence-normes-dimension-finie]] |
| $\max(\lvert x+y\rvert,\lvert x-2y\rvert)$ | norme ; boule = parallélogramme | [[topo-montrer-norme]] |

## Fonctions

| Fonction | Propriété | Fiche |
|---|---|---|
| $\frac{xy}{x^2+y^2}$ | partielles continues, **pas continue** en $(0,0)$ | [[topo-continuite-composantes]] |
| $\frac{x^2y}{x^2+y^2}$, $\frac{x^3+y^3}{x^2+y^2}$ | continues en $(0,0)$ (majoration) | [[topo-continuite-deux-variables]] |
| $\frac{x^2}{x^2+y^2}$ | pas continue : $(\frac1n,0)$ donne $1$ | [[topo-continuite-deux-variables]] |
| $x^2$ sur $\mathbb R$ | continue, **pas U.C.** ; U.C. sur $[-a,a]$ | [[topo-uniforme-continuite]] |
| $\sqrt x$ sur $[0,+\infty[$ | U.C., **pas lipschitzienne** | [[topo-hierarchie-lipschitz-uc-continue]] |
| $\sin\frac1x$ sur $]0,1]$ | continue sur un borné, **pas U.C.** | [[topo-heine]] |
| $\frac1x$ sur $]0,1]$ ; $\arctan$ sur $\mathbb R$ | non bornée ; bornée mais bornes non atteintes | [[topo-bornes-atteintes]] |
| $x\mapsto d(x,A)$, une norme | 1-lipschitziennes | [[topo-distance-a-une-partie]] |
| $t\mapsto(\cos t,\sin t)$ sur $[0,2\pi[$ | bijection continue **non** bicontinue | [[topo-bijections-continues-de-r]] |
| $\arctan$ (rééchelonnée) | homéomorphisme $\mathbb R\to]a,b[$ | [[topo-bijections-continues-de-r]] |

## Compacts et non-compacts

| Compacts | Non compacts (raison) |
|---|---|
| $[a,b]$, ensemble fini, $\{\frac1n\}\cup\{0\}$ | $\mathbb R$, $\mathbb Z$, $[0,+\infty[$ (non bornés) |
| sphère unité de $\mathbb R^n$, $\{\lvert x\rvert+\lvert y\rvert\le1\}$ | $]0,1]$, $[0,1[$, $\{\frac1n\}$ (non fermés) |
| $[0,1]\times[2,3]$, image continue d'un compact | $\mathbb N$ discret (fermé borné, mais $d(x_n,x_m)=1$) |
| | boule unité de $C([0,1])$ (Riesz) |

## Sommes A + B

| $A$ | $B$ | $A+B$ |
|---|---|---|
| $[0,1]$ | $[2,3]\cup\{5\}$ | $[2,4]\cup[5,6]$, compact |
| $[0,1]$ | $\{\frac1n\}$ (non fermé) | $]0,2]$, non fermé |
| $\mathbb N$ | $\{-n+\frac1n\mid n\ge2\}$ | contient $\frac1n$, pas $0$ : non fermé |
| ouvert | quelconque | ouvert |

## 🔗 Liens

- [[topo-vrai-faux-classiques]] · [[topo-reconnaitre-exercice]] · [[topo-exercices-types-corriges]]
