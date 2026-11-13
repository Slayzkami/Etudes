---
aliases:
  - "Distances qui viennent d'une norme"
  - "distance invariante par translation"
  - "P1 P2"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-01
---

# ⭐ Distances qui viennent d'une norme

*Théorème* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Prop. 1.8 du cours (poly : Rem. 1.1) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> 1. La distance associée à une norme vérifie **(P1)** $d(\lambda x,\lambda y)=|\lambda|d(x,y)$ et **(P2)** $d(x+z,y+z)=d(x,y)$.
> 2. Réciproquement, une distance sur un espace vectoriel vérifiant (P1) et (P2) est associée à la norme $N(x)=d(x,0)$.
> 3. La distance discrète (sur $E\neq\{0\}$) ne provient d'aucune norme.

> [!SUCCESS]- Démonstration
> 1. $d(\lambda x,\lambda y)=N(\lambda(x-y))=|\lambda|N(x-y)$ ; $d(x+z,y+z)=N(x-y)$.
> 2. (N1) $N(x)=0\iff d(x,0)=0\iff x=0$ ; (N2) $N(\lambda x)=d(\lambda x,\lambda0)=|\lambda|d(x,0)$ ; (N3) $N(x+y)\le d(x+y,y)+d(y,0)=d(x,0)+d(y,0)$ par (P2).
> 3. Pour $x\neq0$ : $d(2x,0)=1$ mais $|2|\,d(x,0)=2$ : (P1) est fausse.

> [!TIP] Réflexes
> **Interro 2026-27, Q2** : « existe-t-il une norme $N$ sur $\mathbb R^2$ dont la distance discrète est la distance associée ? » → **Non** : $N(x)=1$ et $N(\frac x2)=1$ pour $x\neq0$, alors que (N2) impose $N(\frac x2)=\frac12N(x)=\frac12$.

## 🔗 Liens

- **S'appuie sur** : [[topo-distance-associee-norme|Distance associée à une norme]], [[topo-distance-discrete|Distance discrète]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : —
- **Méthodes** : —
- **Voir aussi** : —
