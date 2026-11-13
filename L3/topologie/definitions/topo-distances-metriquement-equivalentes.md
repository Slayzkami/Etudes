---
aliases:
  - "Distances métriquement équivalentes"
  - "métriquement équivalentes"
  - "encadrement de distances"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-02
---

# 📘 Distances métriquement équivalentes

*Définition* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Déf. 2.60 du cours (poly : Déf. 2.15) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> $d_1$ et $d_2$ sont **métriquement équivalentes** s'il existe $\alpha>0$ et $\beta>0$ tels que
> $$\forall x,y\in E,\ \alpha\,d_1(x,y)\le d_2(x,y)\le\beta\,d_1(x,y).$$

> [!IMPORTANT] À retenir
> - Métriquement $\Rightarrow$ topologiquement ; **réciproque fausse** → [[topo-metriquement-implique-topologiquement]].
> - Conservent en plus : parties bornées, uniforme continuité, suites de Cauchy (Rem. 2.63).

> [!WARNING] Pièges
> Pour réfuter : un ensemble borné pour l'une et pas pour l'autre, ou $\frac{d_2(x_n,y_n)}{d_1(x_n,y_n)}\to+\infty$.

## 🔗 Liens

- **S'appuie sur** : [[topo-distance|Distance, espace métrique]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-metriquement-implique-topologiquement|Métriquement équivalentes ⇒ topologiquement équivalentes]]
- **Méthodes** : [[topo-comparer-distances|Méthode : comparer deux distances]]
- **Voir aussi** : [[topo-distances-topologiquement-equivalentes|Distances topologiquement équivalentes]]
