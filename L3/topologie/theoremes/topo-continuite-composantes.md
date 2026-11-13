---
aliases:
  - "Continuité dans un produit"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-02
---

# ⭐ Continuité dans un produit

*Théorème* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Prop. 2.47, Th. 2.48, Prop. 2.50 du cours (poly : Prop. 2.12, Th. 2.9, Prop. 2.13) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> - Les projections $\pi_i$ sont 1-lipschitziennes.
> - $f=(f_1,\dots,f_p):E\to F_1\times\dots\times F_p$ est continue (resp. U.C.) $\iff$ chaque $f_i$ l'est.
> - Si $f$ est continue en $(a_1,a_2)$, ses applications partielles $x_1\mapsto f(x_1,a_2)$ et $x_2\mapsto f(a_1,x_2)$ sont continues. **Réciproque fausse.**

> [!SUCCESS]- Démonstration
> $f_i=\pi_i\circ f$ ; réciproquement, si $x_n\to a$, chaque $f_i(x_n)\to f_i(a)$ donc $f(x_n)\to f(a)$ (convergence dans un produit).

> [!EXAMPLE] Exemple
> $f(x,y)=\frac{xy}{x^2+y^2}$, $f(0,0)=0$ : applications partielles nulles (continues) mais $f(\frac1n,\frac1n)=\frac12\not\to0$.

## 🔗 Liens

- **S'appuie sur** : [[topo-distance-produit|Distance produit]], [[topo-continuite|Continuité en un point]], [[topo-convergence-produit|Convergence dans un produit]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : —
- **Méthodes** : [[topo-continuite-deux-variables|Méthode : continuité d'une fonction de deux variables en (0,0)]]
- **Voir aussi** : —
