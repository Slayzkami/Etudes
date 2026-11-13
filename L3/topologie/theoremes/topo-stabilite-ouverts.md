---
aliases:
  - "Stabilité des ouverts"
  - "O1 O2 O3"
  - "réunion d'ouverts"
  - "intersection finie d'ouverts"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-02
---

# ⭐ Stabilité des ouverts

*Théorème* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Th. 2.7 et Ex. 2.8 du cours (poly : Th. 2.1, Ex. 2.4) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> - **(O1)** $E$ et $\emptyset$ sont des ouverts.
> - **(O2)** Une réunion **quelconque** d'ouverts est un ouvert.
> - **(O3)** Une intersection **finie** d'ouverts est un ouvert.

> [!SUCCESS]- Démonstration
> (O2) Si $x\in\bigcup A_i$, $x\in A_{i_0}$ ouvert : $B(x,r)\subset A_{i_0}\subset\bigcup A_i$.
> (O3) Si $x\in\bigcap_{i=1}^pA_i$ : $B(x,r_i)\subset A_i$ ; $r=\min_ir_i>0$ (min **fini**) convient.

> [!WARNING] Pièges
> $\bigcap_{n\ge1}]-\frac1n,\frac1n[=\{0\}$ n'est pas ouvert : la preuve de (O3) échoue car $\inf_n\frac1n=0$.

## 🔗 Liens

- **S'appuie sur** : [[topo-ouvert|Ouvert]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-stabilite-fermes|Stabilité des fermés]], [[topo-ouverts-reunions-de-boules|Un ouvert est une réunion de boules ouvertes]]
- **Méthodes** : [[topo-montrer-ouvert-ferme|Méthode : montrer qu'une partie EST ouverte ou fermée]], [[topo-somme-a-plus-b|Méthode : la somme A + B]]
- **Voir aussi** : —
