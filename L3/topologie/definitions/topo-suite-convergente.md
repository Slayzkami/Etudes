---
aliases:
  - "Suite convergente"
  - "convergence"
  - "suite convergente"
  - "limite d'une suite"
  - "x_n → ℓ"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-01
---

# 📘 Suite convergente

*Définition* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Déf. 1.24 du cours (poly : Déf. 1.8) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> $(x_n)$ **converge** vers $\ell\in E$ (pour $d$) si
> $$\forall\varepsilon>0,\ \exists N_\varepsilon\in\mathbb N,\ \forall n\ge N_\varepsilon,\ d(x_n,\ell)<\varepsilon.$$
> On note $x_n\to\ell$.

> [!IMPORTANT] À retenir
> - $x_n\to\ell\iff d(x_n,\ell)\to0$ dans $\mathbb R$ : on se ramène à une suite **réelle positive**.
> - Limite unique ([[topo-unicite-limite]]) ; sous-suites de même limite ([[topo-suites-extraites-convergentes]]) ; convergente $\Rightarrow$ bornée ([[topo-convergente-bornee]]).

> [!WARNING] Pièges
> - La convergence **dépend de la distance** : $t^n\to0$ pour $\|\cdot\|_1$ sur $C([0,1])$, pas pour $\|\cdot\|_\infty$.
> - $N(x_n)\to N(\ell)$ n'implique pas $x_n\to\ell$ : $x_n=(-1)^n$.

## 🔗 Liens

- **S'appuie sur** : [[topo-distance|Distance, espace métrique]]
- **Utilisé par (définitions)** : [[topo-suite-de-cauchy-espace-complet|Suite de Cauchy, espace complet]], [[topo-suite-extraite|Suite extraite]]
- **Utilisé par (théorèmes)** : [[topo-caracterisation-sequentielle-fermes|Caractérisation séquentielle des fermés]], [[topo-convergence-evn|Convergence dans un e.v.n.]], [[topo-convergence-produit|Convergence dans un produit]], [[topo-convergente-bornee|Toute suite convergente est bornée]], [[topo-unicite-limite|Unicité de la limite]]
- **Méthodes** : [[topo-etudier-convergence-suite|Méthode : montrer qu'une suite converge (ou non)]]
- **Voir aussi** : —
