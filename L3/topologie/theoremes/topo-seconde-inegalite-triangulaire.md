---
aliases:
  - "Seconde inégalité triangulaire"
  - "|d(x,z)−d(z,y)| ≤ d(x,y)"
  - "|N(x)−N(y)| ≤ N(x−y)"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-01
---

# ⭐ Seconde inégalité triangulaire

*Théorème* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Prop. 1.4 et 1.6 du cours (poly : Prop. 1.1 et 1.2) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> - Dans un espace métrique : $\forall x,y,z\in E,\ |d(x,z)-d(z,y)|\le d(x,y)$.
> - Dans un e.v.n. : $\forall x,y\in E,\ |N(x)-N(y)|\le N(x-y)$.

> [!SUCCESS]- Démonstration
> (M3) : $d(x,z)\le d(x,y)+d(y,z)$, donc $d(x,z)-d(z,y)\le d(x,y)$. En échangeant $x$ et $y$ : $d(z,y)-d(x,z)\le d(x,y)$. D'où $-d(x,y)\le d(x,z)-d(z,y)\le d(x,y)$.
> Pour une norme : $x=(x-y)+y$ donne $N(x)-N(y)\le N(x-y)$, puis on échange $x,y$ et on utilise $N(y-x)=N(x-y)$ (N2).

> [!TIP] Réflexes
> Conséquences : $x\mapsto d(a,x)$ et $x\mapsto N(x)$ sont **1-lipschitziennes**, donc continues ; $x_n\to\ell\Rightarrow N(x_n)\to N(\ell)$.
> On s'en sert pour : une boule fermée est fermée, $d(x,y)\ge d(a,x)-r$, etc.

## 🔗 Liens

- **S'appuie sur** : [[topo-distance|Distance, espace métrique]], [[topo-norme|Norme, espace vectoriel normé]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-convergence-evn|Convergence dans un e.v.n.]], [[topo-boule-fermee-fermee|Une boule fermée est un fermé]]
- **Méthodes** : —
- **Voir aussi** : —
