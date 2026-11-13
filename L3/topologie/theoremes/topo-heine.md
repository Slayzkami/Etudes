---
aliases:
  - "Théorème de Heine"
  - "Heine"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-03
---

# ⭐ Théorème de Heine

*Théorème* · Chapitre : [[03-espaces-metriques-compacts|3 – Espaces métriques compacts]] · Th. 3.32 du cours (poly : Th. 3.4) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Si $E$ est compact et $f:(E,d)\to(F,\delta)$ est continue, alors $f$ est **uniformément continue**.

> [!SUCCESS]- Démonstration
> Sinon : $\varepsilon>0$ et $x_n,y_n$ avec $d(x_n,y_n)<\frac1n$, $\delta(f(x_n),f(y_n))\ge\varepsilon$. Une sous-suite $x_{n_k}\to x$, donc $y_{n_k}\to x$ aussi, et par continuité $\delta(f(x_{n_k}),f(y_{n_k}))\to0$ : contradiction.

> [!EXAMPLE] Exemple
> $x^2$ est U.C. sur $[-M,M]$ ; $\sqrt{\cdot}$ est U.C. sur $[0,1]$ (sans être lipschitzienne).

> [!WARNING] Pièges
> Il faut un **compact**, pas seulement un borné : $\sin\frac1x$ sur $]0,1]$ (Piège 3.5).

## 🔗 Liens

- **S'appuie sur** : [[topo-continuite-uniforme|Uniforme continuité]], [[topo-bolzano-weierstrass|Caractérisation séquentielle des compacts (Bolzano–Weierstrass)]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : —
- **Méthodes** : [[topo-uniforme-continuite|Méthode : montrer (ou réfuter) l'uniforme continuité]], [[topo-exploiter-compacite|Méthode : exploiter la compacité]]
- **Voir aussi** : —
