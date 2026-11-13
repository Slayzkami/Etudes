---
aliases:
  - "Distance discrète"
  - "distance discrète"
  - "métrique discrète"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-01
---

# 📘 Distance discrète

*Définition* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Ex. 1.2 (3) du cours (poly : Ex. 1.1) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> Sur un ensemble $E$ quelconque : $d(x,y)=\begin{cases}0 & \text{si } x=y\\ 1 & \text{si } x\neq y.\end{cases}$

> [!IMPORTANT] À retenir
> - **Boules** : $B(a,r)=\{a\}$ si $r\le1$, $B(a,r)=E$ si $r>1$ ; $\bar B(a,r)=\{a\}$ si $r<1$, $=E$ si $r\ge1$.
> - **Toute partie est ouverte** ($B(x,\tfrac12)=\{x\}\subset A$) **donc toute partie est fermée**.
> - $x_n\to x\iff x_n=x$ à partir d'un certain rang.
> - $\overline{B(a,1)}=\{a\}\neq\bar B(a,1)=E$ : l'adhérence de la boule ouverte peut être plus petite que la boule fermée.
> - Elle ne vient d'**aucune norme** (si $E\neq\{0\}$) : $d(2x,0)=1\neq2\,d(x,0)$.
> - $E$ compact $\iff E$ fini ; $\mathbb N$ discret est fermé, borné, **non compact**.

> [!WARNING] Pièges
> - Diamètre : $\operatorname{diam}B(a,10)=1<20$ ; on a seulement $\operatorname{diam}\le2r$.
> - Une sphère peut être vide : $S(a,\tfrac12)=\emptyset$.

## 🔗 Liens

- **S'appuie sur** : [[topo-distance|Distance, espace métrique]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-distance-et-norme|Distances qui viennent d'une norme]]
- **Méthodes** : —
- **Corrigés** : [[topo-exercices-types-corriges#2. Adhérence de la boule ouverte et distance discrète|écrit 2022-23]], [[topo-exercices-types-corriges#11. Interro 2026-27 – questions de cours|interro 2026-27 Q2]]
- **Voir aussi** : [[topo-ouvert|Ouvert]], [[topo-boules-spheres|Boules et sphères]], [[topo-distance-et-norme|Distances qui viennent d'une norme]]
