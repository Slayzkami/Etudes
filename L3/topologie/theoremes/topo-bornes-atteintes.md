---
aliases:
  - "Une fonction continue sur un compact est bornée et atteint ses bornes"
  - "bornes atteintes"
  - "extremum sur un compact"
  - "max et min atteints"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-03
---

# ⭐ Une fonction continue sur un compact est bornée et atteint ses bornes

*Théorème* · Chapitre : [[03-espaces-metriques-compacts|3 – Espaces métriques compacts]] · Th. 3.30 du cours (poly : Th. 3.3) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Si $E$ est compact et $f:E\to\mathbb R$ est continue, $f$ est bornée et **atteint ses bornes** : $\exists x_1,x_2\in E,\ \forall x\in E,\ f(x_1)\le f(x)\le f(x_2)$.

> [!SUCCESS]- Démonstration
> $f(E)$ est un compact de $\mathbb R$, donc fermé borné. Avec $\beta=\sup f(E)$ : $y_n\in f(E)$, $\beta-\frac1n<y_n\le\beta$, donc $y_n\to\beta$ et $\beta\in f(E)$ (fermé).

> [!EXAMPLE] Exemple
> Indispensable : $\frac1x$ sur $]0,1]$ non bornée ; $\arctan$ sur $\mathbb R$ n'atteint pas $\frac\pi2$.

> [!TIP] Réflexes
> **Minoration stricte** : $f$ continue et $>0$ sur un compact $\Rightarrow\exists c>0,\ f\ge c$. Distance à un compact atteinte ; $d(K,F)>0$ si $K$ compact, $F$ fermé, disjoints.

## 🔗 Liens

- **S'appuie sur** : [[topo-image-continue-compact|Image continue d'un compact ; bijection continue sur un compact]], [[topo-borel-lebesgue|Borel–Lebesgue : compacts de R et de R^n]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-equivalence-normes-dimension-finie|Équivalence des normes en dimension finie]]
- **Méthodes** : [[topo-exploiter-compacite|Méthode : exploiter la compacité]]
- **Voir aussi** : —
