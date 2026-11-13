---
aliases:
  - "Critère des boules (distances topologiquement équivalentes)"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-02
---

# ⭐ Critère des boules (distances topologiquement équivalentes)

*Théorème* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Prop. 2.59 du cours (poly : Prop. 2.14) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> $d_1$ et $d_2$ sont topologiquement équivalentes $\iff$ toute boule $B_{d_1}(a,r)$ contient une boule $B_{d_2}(a,s)$ de même centre, et réciproquement.

> [!SUCCESS]- Démonstration
> ($\Rightarrow$) $B_{d_1}(a,r)$ est ouverte pour $d_1$ donc pour $d_2$ et contient $a$. ($\Leftarrow$) Si $O$ est $d_1$-ouvert et $a\in O$ : $B_{d_1}(a,r)\subset O$ contient une $B_{d_2}(a,s)$ ; donc $O$ est $d_2$-ouvert.

> [!TIP] Réflexes
> **Écrit 2025-26, ex. 1** : si $\delta\le k\,d$, alors $B_d(a,\frac rk)\subset B_\delta(a,r)$, donc **tout ouvert de $\delta$ est un ouvert de $d$** (et tout fermé de $\delta$ est un fermé de $d$, par complémentaire).

## 🔗 Liens

- **S'appuie sur** : [[topo-distances-topologiquement-equivalentes|Distances topologiquement équivalentes]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-metriquement-implique-topologiquement|Métriquement équivalentes ⇒ topologiquement équivalentes]]
- **Méthodes** : [[topo-comparer-distances|Méthode : comparer deux distances]]
- **Voir aussi** : —
