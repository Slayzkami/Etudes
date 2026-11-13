---
aliases:
  - "Distance produit"
  - "produit d'espaces métriques"
  - "distance max"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-01
---

# 📘 Distance produit

*Définition* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Prop. 1.22 du cours (poly : Déf. 1.7) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> Si $(E_1,d_1),\dots,(E_n,d_n)$ sont des espaces métriques et $E=E_1\times\dots\times E_n$, on pose pour $x=(x_i)$, $y=(y_i)$ :
> $$d(x,y)=\max_{1\le i\le n}d_i(x_i,y_i).$$
> C'est une distance sur $E$ (le **produit** des $E_i$).

> [!IMPORTANT] À retenir
> - $B_E(a,r)=\prod_iB_{E_i}(a_i,r)$ → [[topo-boules-produit]].
> - $d\le d''\le d'\le n\,d$ avec $d'=\sum d_i$, $d''=(\sum d_i^2)^{1/2}$ : dans $\mathbb R^n$ ce sont $d_\infty,d_2,d_1$.
> - Une suite converge dans le produit $\iff$ chaque composante converge → [[topo-convergence-produit]].

## 🔗 Liens

- **S'appuie sur** : [[topo-distance|Distance, espace métrique]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-boules-produit|Boules d'un produit, autres distances produit]], [[topo-continuite-composantes|Continuité dans un produit]], [[topo-convergence-produit|Convergence dans un produit]]
- **Méthodes** : —
- **Voir aussi** : —
