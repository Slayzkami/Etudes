---
aliases:
  - "Distance d'un point à une partie, entre deux parties"
  - "distance à une partie"
  - "d(x,A)"
  - "d(A,B)"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-02
---

# 📘 Distance d'un point à une partie, entre deux parties

*Définition* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · TD, exercice 2.13 (corrigé dans le cours, § 2.17.4) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> Pour $A,B$ non vides : $d(x,A)=\inf_{a\in A}d(x,a)$ et $d(A,B)=\inf_{x\in A,\ y\in B}d(x,y)$.

> [!IMPORTANT] À retenir
> - $|d(x,A)-d(y,A)|\le d(x,y)$ : $x\mapsto d(x,A)$ est **1-lipschitzienne** donc continue.
> - $d(x,A)=0\iff x\in\bar A$ ; donc $\bar A=\{d(\cdot,A)=0\}$ est fermé.
> - $A\cap B\neq\emptyset\Rightarrow d(A,B)=0$ ; réciproque **fausse**, même pour deux fermés ($\{n\}$ et $\{n+\frac1n\}$).
> - $K$ compact, $F$ fermé, disjoints $\Rightarrow d(K,F)>0$ (§ 3.8.2).

## 🔗 Liens

- **S'appuie sur** : [[topo-distance|Distance, espace métrique]], [[topo-adherence|Adhérence]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : —
- **Méthodes** : —
- **Corrigés** : [[topo-exercices-types-corriges#15. Distance à une partie et à un compact|ex. 15]]
- **Voir aussi** : —
