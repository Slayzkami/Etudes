---
aliases:
  - "Mes erreurs topologie"
  - "pièges personnels topo"
  - "erreurs topo"
tags:
  - topologie
  - topo/revision
---

# 🚨 Mes erreurs à ne plus faire

Les erreurs que j'ai **réellement** faites (bilan du 5 novembre, séances du 6 au 8, interro 2025-26 refaite le 8 novembre). Chacune : version fausse, version juste, comment la contrôler. À compléter à chaque séance, à relire **juste avant l'examen**. · [[topo-plan-de-revision|↩ Plan de révision]] · [[topo-index-definitions|↩ Index]]

## Définitions

> [!WARNING] 1. Prendre un théorème pour la définition de « compact »
> ❌ « Une partie $K$ est compacte ssi elle est fermée bornée. »
> ✅ Définition : de tout recouvrement ouvert on extrait un sous-recouvrement fini ; en pratique : toute suite de $K$ a une sous-suite qui converge **vers un point de $K$**. « Fermé borné » est un **théorème**, vrai seulement en dimension finie.
> **Contrôle** : si je cite « fermé borné », je dois avoir écrit « dans $\mathbb R^n$ ».
> → [[topo-espace-compact]], [[topo-borel-lebesgue]]

> [!WARNING] 2. Confondre adhérence et complémentaire
> ❌ « $A=]0,1]\cup\{2\}$, donc $\bar A=]-\infty,0]\cup]1,+\infty[\setminus\{2\}$. »
> ✅ L'adhérence **contient** $A$ : $\bar A=A$ + les points « collés » à $A$ $=[0,1]\cup\{2\}$.
> **Contrôle** : vérifier $A\subset\bar A$ (un point de $A$, comme $\frac12$, doit être dans ma réponse).
> → [[topo-adherence]]

## Fermés, ouverts, adhérence

> [!WARNING] 3. « Réunion de fermés, donc fermé » avec une réunion infinie
> ❌ « $X=\bigcup_n\{\frac1n\}\cup\{0\}$ est une réunion de fermés donc fermé. » (interro 2025-26)
> ✅ Seule une réunion **finie** de fermés est fermée ($\{\frac1n\}$ n'est pas fermé). Pour $X$ : complémentaire $=$ réunion d'intervalles ouverts, ou par les suites.
> **Contrôle** : chaque fois que j'écris « réunion », je me demande « finie ? ».
> → [[topo-stabilite-fermes]]

> [!WARNING] 4. Oublier la deuxième inclusion de l'adhérence
> ❌ « $(0,0)=\lim u_n$, donc $\bar X=\{x\ge0,\ y=x^2\}$. » (interro 2025-26)
> ✅ Deux inclusions : (1) les points ajoutés sont limites de suites de $X$ ; (2) **le candidat est fermé et contient $X$**, donc contient $\bar X$.
> **Contrôle** : ma rédaction de $\bar A$ contient-elle les mots « fermé » et « contient $A$ » ?
> → [[topo-calculer-interieur-adherence-frontiere]]

> [!WARNING] 5. Justifier l'intérieur avec les points d'un autre exercice
> ❌ Pour $A_1=[1,2[\cup\{5\}$ : « $2=\lim(2+\frac1{n+1})$ et $3=\lim(3+\frac1n)$… » (recopié de $]0,1]\cup\{2\}$).
> ✅ Seuls les points **de $A_1$** hors du candidat sont à traiter : $1$ et $5$ ($1-\frac1n\notin A_1\to1$, $5+\frac1n\notin A_1\to5$).
> **Contrôle** : lister d'abord « $A\setminus\text{candidat}=\{\dots\}$ ».

> [!WARNING] 6. Se tromper de signe pour sortir de l'ensemble
> ❌ Demi-disque $\{x^2+y^2<1,\ y\ge0\}$ : « $(0,\frac1{n+1})\notin X$ ».
> ✅ $(0,\frac1{n+1})$ est **dans** $X$ dès que $n\ge1$ ; pour sortir il faut $y<0$ : $(0,-\frac1{n+1})$.
> **Contrôle** : vérifier explicitement chaque condition de l'ensemble sur le point choisi.

> [!WARNING] 7. Comparer la mauvaise quantité
> ❌ $X=\{y=x^2\}$, $v_n=(1,1-\frac1n)$ : « $\notin X$ car $(1-\frac1n)^2\neq1$ ». (interro 2025-26)
> ✅ On compare $y$ à $x^2$ : $1-\frac1n\neq1^2$.
> **Contrôle** : réécrire la condition de l'ensemble avec les coordonnées du point.

> [!WARNING] 8. Image réciproque avec une fonction mal définie
> ❌ « On pose $f:A_2\to\mathbb R$ continue ; $\{f>0\}$ est ouvert. »
> ✅ « $f:\mathbb R\to\mathbb R$, $f(x)=x$ est continue et $A_2=f^{-1}(]0,+\infty[)$. » La fonction est **explicite** et définie sur **tout l'espace**.

## Rédaction

> [!WARNING] 9. Notations de suite
> ❌ « Soit $x_n=\frac1n$… $\lim_{x\to+\infty}x_n=0$ ».
> ✅ « Pour $n\in\mathbb N^*$, $x_n=\frac1n$… $x_n\to0$ quand $n\to+\infty$. » Dire **pourquoi** $x_n\in A$ ($0<\frac1n\le1$).

> [!WARNING] 10. Mauvaise formulation de « pas fermé »
> ❌ « Une suite de $A$ ne tend pas vers un point de $A$. »
> ✅ « Une suite de $A$ **converge vers un point hors de** $A$. »

> [!WARNING] 11. Coquilles qui changent le résultat
> ❌ « $[1,2]\cup\{2\}$ est fermé… » au lieu de $[1,2]\cup\{5\}$.
> ✅ Relire chaque ensemble recopié.

> [!WARNING] 12. Laisser une question vide
> ❌ « ∅ » (bilan, interro 2025-26 ex. 2.2 et 4).
> ✅ Écrire au moins la définition et la première phrase de la méthode : ça rapporte des points partiels.

## Distances, continuité

> [!WARNING] 13. Affirmer l'étape clé sans la prouver
> ❌ « $\inf(1,d(x,y)+d(y,z))\le\inf(1,d(x,y))+\inf(1,d(y,z))$ » écrit sans justification.
> ✅ C'est justement ce qu'il faut démontrer : **deux cas** (un des termes $\ge1$, ou aucun).
> → [[topo-montrer-distance]]

> [!WARNING] 14. « $|g|\le1$, donc $g$ n'est pas continue »
> ❌ Une majoration par une constante ne prouve rien.
> ✅ Une suite $u_n\to(0,0)$ avec $g(u_n)\not\to g(0,0)$ : $g(\frac1n,0)=1\not\to0$.
> → [[topo-continuite-deux-variables]]

> [!TIP] Mes 6 réflexes de contrôle
> 1. Adhérence : **deux inclusions**, la seconde dit « fermé qui contient $A$ ».
> 2. « Réunion de fermés » : **finie** ?
> 3. Chaque point choisi : je vérifie **toutes** les conditions de l'ensemble (signe, stricte/large).
> 4. « Fermé borné ⟹ compact » : seulement **dans $\mathbb R^n$**.
> 5. Pour « pas continue / pas ouvert / pas fermé » : **une suite**, pas une majoration.
> 6. Aucune question vide.

## 🔗 Liens

- [[topo-montrer-pas-ouvert-pas-ferme]] · [[topo-calculer-interieur-adherence-frontiere]] · [[topo-vrai-faux-classiques]] · [[topo-exercices-types-corriges]]
