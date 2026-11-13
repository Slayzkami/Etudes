---
aliases:
  - "Distance induite, sous-espace métrique"
  - "distance induite"
  - "sous-espace métrique"
  - "topologie induite"
  - "ouvert relatif"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-01
---

# 📘 Distance induite, sous-espace métrique

*Définition* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Déf. 1.19 du cours (poly : Déf. 1.6) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> Soit $(E,d)$ un espace métrique et $F\subset E$ non vide. La restriction $d_F$ de $d$ à $F\times F$ ($d_F(x,y)=d(x,y)$) est une distance sur $F$ : la **distance induite**. $(F,d_F)$ est un **sous-espace métrique**.

> [!IMPORTANT] À retenir
> - $B_F(a,r)=B_E(a,r)\cap F$ et $\bar B_F(a,r)=\bar B_E(a,r)\cap F$ → [[topo-boules-sous-espace]].
> - Les ouverts de $F$ sont les $O\cap F$ avec $O$ ouvert de $E$ (preuve de la Prop. 3.9).
> - Une partie peut être **ouverte et fermée dans $F$** sans être ni l'un ni l'autre dans $E$.

> [!EXAMPLE] Exemples
> $I=[0,1[\cup]2,3]$ : $[0,1[=B_I(\tfrac12,1)$ est ouvert dans $I$, et fermé dans $I$ (son complémentaire $]2,3]=B_I(\tfrac52,1)$ est ouvert dans $I$).

## 🔗 Liens

- **S'appuie sur** : [[topo-distance|Distance, espace métrique]]
- **Utilisé par (définitions)** : [[topo-partie-compacte|Partie compacte]]
- **Utilisé par (théorèmes)** : [[topo-boules-sous-espace|Boules d'un sous-espace métrique]]
- **Méthodes** : [[topo-distance-induite-ouverts-relatifs|Méthode : ouverts et fermés d'un sous-espace (distance induite)]]
- **Corrigés** : [[topo-exercices-types-corriges#8. Distance induite sur une bande trouée|écrit 2025-26, ex. 2]]
- **Voir aussi** : —
