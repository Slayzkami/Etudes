---
aliases:
  - "Stabilité des fermés"
  - "F1 F2 F3"
  - "intersection de fermés"
  - "réunion finie de fermés"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-02
---

# ⭐ Stabilité des fermés

*Théorème* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Th. 2.10 du cours (poly : Th. 2.2) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> - **(F1)** $E$ et $\emptyset$ sont des fermés.
> - **(F2)** Une intersection **quelconque** de fermés est un fermé.
> - **(F3)** Une réunion **finie** de fermés est un fermé.

> [!SUCCESS]- Démonstration
> Passage au complémentaire dans (O1)–(O3) avec De Morgan : $(\bigcap F_i)^c=\bigcup F_i^c$, $(\bigcup F_i)^c=\bigcap F_i^c$.

> [!WARNING] Pièges
> **Réunion infinie de fermés** : pas forcément fermée. $\bigcup_{n\ge1}[\frac1n,1]=]0,1]$ ; $\{\frac1n\}=\bigcup_n\{\frac1n\}$ n'est pas fermé. (Mon erreur à l'interro 2025-26 sur $\{0\}\cup\{\frac1n\}$.)

## 🔗 Liens

- **S'appuie sur** : [[topo-ferme|Fermé]], [[topo-stabilite-ouverts|Stabilité des ouverts]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-version-fermes-compacite|Compacité : version « fermés » et fermés emboîtés]], [[topo-exemples-fermes|Singletons, parties finies et sphères sont fermés]]
- **Méthodes** : [[topo-montrer-ouvert-ferme|Méthode : montrer qu'une partie EST ouverte ou fermée]]
- **Voir aussi** : —
