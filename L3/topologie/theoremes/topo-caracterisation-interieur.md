---
aliases:
  - "Caractérisation et propriétés de l'intérieur"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-02
---

# ⭐ Caractérisation et propriétés de l'intérieur

*Théorème* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Prop. 2.19 et 2.20 du cours (poly : Prop. 2.5, 2.6) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> 1. $x\in\operatorname{Int}A\iff\exists r>0,\ B(x,r)\subset A\iff A$ est un voisinage de $x$.
> 2. $A$ est ouvert $\iff\operatorname{Int}A=A$.
> 3. $\operatorname{Int}A$ est le plus grand ouvert contenu dans $A$ : si $O$ est ouvert et $O\subset A$, alors $O\subset\operatorname{Int}A$.

> [!SUCCESS]- Démonstration
> 1. Si $x\in\operatorname{Int}A$, $x$ est dans un ouvert $O\subset A$, qui contient une boule $B(x,r)$. Réciproquement, $B(x,r)$ est un ouvert contenu dans $A$, donc dans $\operatorname{Int}A$.
> 2. Si $A$ est ouvert, $A$ est un ouvert contenu dans $A$, donc $A\subset\operatorname{Int}A\subset A$.

> [!TIP] Réflexes
> - $A\subset B\Rightarrow\operatorname{Int}A\subset\operatorname{Int}B$ (car $\operatorname{Int}A$ est un ouvert contenu dans $B$).
> - $\operatorname{Int}(A\cap B)=\operatorname{Int}A\cap\operatorname{Int}B$ ; $\operatorname{Int}A\cup\operatorname{Int}B\subset\operatorname{Int}(A\cup B)$, stricte pour $A=[0,1]$, $B=[1,2]$ (TD, écrit 2025-26).

## 🔗 Liens

- **S'appuie sur** : [[topo-interieur|Intérieur]], [[topo-voisinages-et-boules|Voisinages et boules]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : —
- **Méthodes** : [[topo-calculer-interieur-adherence-frontiere|Méthode : calculer intérieur, adhérence, frontière]]
- **Voir aussi** : —
