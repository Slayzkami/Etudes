---
aliases:
  - "Propriétés de la norme d'opérateur"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-02
---

# ⭐ Propriétés de la norme d'opérateur

*Théorème* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Prop. 2.72 et Ex. 2.73 du cours (poly : § 2.14) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> 1. $(\mathcal L_c(E,F),|||\cdot|||)$ est un e.v.n.
> 2. $\|f(u)\|\le|||f|||\,\|u\|$, et toute constante $C$ avec $\|f(u)\|\le C\|u\|$ vérifie $C\ge|||f|||$.
> 3. $|||g\circ f|||\le|||g|||\,|||f|||$.
> 4. Si $\dim E<\infty$, toute application linéaire $E\to F$ est continue.

> [!SUCCESS]- Démonstration
> 3. $\|g(f(u))\|\le|||g|||\,\|f(u)\|\le|||g|||\,|||f|||\,\|u\|$, puis 2.

> [!EXAMPLE] Exemple
> $f(u)(x)=\int_0^xu$ sur $(C([0,1]),\|\cdot\|_\infty)$ : $\|f(u)\|_\infty\le\|u\|_\infty$ et $u_0=1$ donne l'égalité, donc $|||f|||=1$.

## 🔗 Liens

- **S'appuie sur** : [[topo-norme-operateur|Norme d'une application linéaire continue]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : —
- **Méthodes** : [[topo-application-lineaire-norme-operateur|Méthode : continuité d'une application linéaire, norme d'opérateur]]
- **Voir aussi** : —
