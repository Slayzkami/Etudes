---
aliases:
  - "Caractérisations d'un sous-groupe"
  - "caractérisation pratique"
  - "xy^-1"
  - "x-y"
  - "sous-groupe d'un groupe fini"
tags:
  - gac
  - gac/theoreme
  - gac/chapitre-02
---

# ⭐ Caractérisations d'un sous-groupe

*Théorème* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · § II.2 du cours · [[index-definitions|↩ Index]]

> [!IMPORTANT] Énoncés
> 1. $H$ est un [[sous-groupe]] de $G$ $\iff$ $H$ est stable et $(H,\star)$ est un groupe.
> 2. **Caractérisation pratique** : $H$ sous-groupe $\iff$ **$e\in H$** et **$\forall x,y\in H,\ x\star y^{-1}\in H$**
>    (additif : $0\in H$ et $x-y\in H$).
> 3. Si $G$ est **fini** : $H\neq\emptyset$ sous-groupe $\iff$ $H$ stable par la loi.

> [!SUCCESS]- Démonstration de 2
> ($\Leftarrow$) $H\ni e$. Avec $(e,y)$ : $y^{-1}\in H$. Avec $(x,y^{-1})$ : $xy\in H$.
> ($\Rightarrow$) $e\in H$ ; $y^{-1}\in H$ puis $xy^{-1}\in H$.

> [!SUCCESS]- Démonstration de 3
> Pour $x\in H$, les $x^k$ ($k\ge1$) sont dans $H$ ; $G$ fini ⟹ $x^i=x^j$ ($i<j$) ⟹ $x^{j-i}=1$, $k=j-i\ge1$. Donc $1=x^k\in H$ et $x^{-1}=x^{k-1}\in H$.
> Faux si $G$ infini : $\mathbb N\subset\mathbb Z$.

## 🔗 Liens

- **S'appuie sur** : [[sous-groupe|Sous-groupe]]
- **Voir aussi** : [[montrer-sous-groupe|Méthode : montrer qu'une partie est un sous-groupe]]
