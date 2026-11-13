---
aliases:
  - "Borel–Lebesgue : compacts de R et de R^n"
  - "fermé borné"
  - "Borel-Lebesgue"
  - "compacts de R^n"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-03
---

# ⭐ Borel–Lebesgue : compacts de R et de R^n

*Théorème* · Chapitre : [[03-espaces-metriques-compacts|3 – Espaces métriques compacts]] · Th. 3.22 et Cor. 3.25 du cours (poly : Th. 3.2 ; ajout) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> - Une partie de $\mathbb R$ est compacte $\iff$ elle est **fermée et bornée**.
> - Dans $\mathbb R^n$ (pour n'importe quelle norme, dimension finie) : compact $\iff$ **fermé et borné**.

> [!SUCCESS]- Démonstration
> ($\Leftarrow$) $A$ bornée $\Rightarrow A\subset[-M,M]^n$, produit de segments compacts, donc compact ; $A$ est un fermé contenu dans ce compact, donc compact.

> [!EXAMPLE] Exemple
> $\{x^2-y^2\le1\}\cap\{x^2+y^2\le2\}$ ; la sphère unité $\{\|x\|_2=1\}$ ; $\{|x|+|y|\le1\}$ ; $\{0\}\cup\{\frac1n\}$ ; $\{0\}\cup\{e^{-n}\}$. L'hyperbole $\{xy=1\}$ est fermée **non bornée** : pas compacte.

## 🔗 Liens

- **S'appuie sur** : [[topo-bolzano-weierstrass-dans-r|Bolzano–Weierstrass dans R ; les segments sont compacts]], [[topo-ferme-dans-compact|Un fermé dans un compact est compact]], [[topo-produit-de-compacts|Produit de compacts]], [[topo-compact-complet-borne|Un compact est complet et borné ; une partie compacte est fermée et bornée]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-bornes-atteintes|Une fonction continue sur un compact est bornée et atteint ses bornes]], [[topo-equivalence-normes-dimension-finie|Équivalence des normes en dimension finie]]
- **Méthodes** : [[topo-montrer-compact|Méthode : montrer qu'une partie est compacte]]
- **Voir aussi** : —
