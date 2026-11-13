---
aliases:
  - "Application lipschitzienne"
  - "lipschitzienne"
  - "k-lipschitzienne"
  - "Lipschitz"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-02
---

# 📘 Application lipschitzienne

*Définition* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Déf. 2.42 du cours (poly : Déf. 2.10) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> $f:E\to F$ est **lipschitzienne** s'il existe $k\ge0$ tel que
> $$\forall(x,y)\in E^2,\ d_F(f(x),f(y))\le k\,d_E(x,y).$$
> On dit que $f$ est $k$-lipschitzienne.

> [!IMPORTANT] À retenir
> - Lipschitzienne $\Rightarrow$ uniformément continue (prendre $\delta=\varepsilon/k$).
> - Exemples : une norme, $x\mapsto d(a,x)$, $x\mapsto d(x,A)$ (1-lipschitziennes) ; $\sin$ ; les projections d'un produit ; une application linéaire continue.

## 🔗 Liens

- **S'appuie sur** : [[topo-distance|Distance, espace métrique]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-applications-lineaires-continues|Continuité d'une application linéaire]], [[topo-hierarchie-lipschitz-uc-continue|Lipschitzienne ⇒ uniformément continue ⇒ continue]]
- **Méthodes** : —
- **Voir aussi** : [[topo-continuite-uniforme|Uniforme continuité]]
