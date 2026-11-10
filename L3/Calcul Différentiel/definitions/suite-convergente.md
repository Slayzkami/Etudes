---
aliases:
  - "Suite convergente"
  - "convergence d'une suite"
  - "limite d'une suite"
tags:
  - cd
  - cd/definition
  - cd/chapitre-01
---

# 📘 Suite convergente

*Définition* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Déf. 1.15 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> Soit $(E,\lVert \cdot\rVert)$ un e.v.n., $(x_n)$ une suite de $E$ et $\ell\in E$. La suite $(x_n)$ **converge vers** $\ell$ si
> $$\forall\varepsilon>0,\ \exists N_\varepsilon\in\mathbb N,\ \forall n\ge N_\varepsilon,\quad \lVert x_n-\ell\rVert<\varepsilon.$$
> Autrement dit : $x_n\to\ell$ dans $E$ $\iff$ la suite **réelle** $\lVert x_n-\ell\rVert$ tend vers $0$.

> [!IMPORTANT] Propriétés (Prop. 1.16 à 1.19)
> - La limite est unique.
> - Si $x_n\to\ell$ alors $\lVert x_n\rVert\to\lVert \ell\rVert$ (réciproque fausse).
> - $x_n\to\ell$, $y_n\to m$ $\Rightarrow$ $x_n+y_n\to\ell+m$ et $\alpha x_n\to\alpha\ell$.
> - Dans un produit : convergence $\iff$ convergence de chaque composante.

> [!WARNING] Piège
> La convergence dépend de la norme en dimension infinie (pas en dimension finie → [[equivalence-normes-dimension-finie]]).

## 🔗 Liens

- **S'appuie sur** : [[norme|Norme, espace vectoriel normé]]
- **Utilisé par (définitions)** : [[suite-de-cauchy|Suite de Cauchy]]
- **Utilisé par (théorèmes)** : [[caracterisation-sequentielle-fermes|Caractérisation séquentielle des fermés]]
