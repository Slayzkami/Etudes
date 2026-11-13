---
aliases:
  - "Inégalité triangulaire généralisée"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-01
---

# ⭐ Inégalité triangulaire généralisée

*Théorème* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Prop. 1.3 du cours (poly : exercice 1.1) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Pour tous $x,y,z_1,\dots,z_n\in E$ : $d(x,y)\le d(x,z_1)+d(z_1,z_2)+\dots+d(z_{n-1},z_n)+d(z_n,y)$.

> [!SUCCESS]- Démonstration
> Récurrence sur $n$ : $n=1$ est (M3). Si c'est vrai au rang $n$, on remplace $d(z_n,y)$ par $d(z_n,z_{n+1})+d(z_{n+1},y)$ grâce à (M3).

## 🔗 Liens

- **S'appuie sur** : [[topo-distance|Distance, espace métrique]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : —
- **Méthodes** : —
- **Voir aussi** : —
