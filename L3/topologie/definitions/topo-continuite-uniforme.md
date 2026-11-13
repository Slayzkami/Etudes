---
aliases:
  - "Uniforme continuité"
  - "uniformément continue"
  - "uniforme continuité"
  - "U.C."
tags:
  - topologie
  - topo/definition
  - topo/chapitre-02
---

# 📘 Uniforme continuité

*Définition* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Déf. 2.38 du cours (poly : Déf. 2.9) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> $f:E\to F$ est **uniformément continue** si
> $$\forall\varepsilon>0,\ \exists\delta>0,\ \forall(x,y)\in E^2,\ d_E(x,y)<\delta\Rightarrow d_F(f(x),f(y))<\varepsilon.$$

> [!IMPORTANT] À retenir
> - Différence avec la continuité : **un même $\delta$ pour tous les points**.
> - Lipschitzienne $\Rightarrow$ uniformément continue $\Rightarrow$ continue ; réciproques fausses ($\sqrt{\cdot}$, puis $x^2$) → [[topo-hierarchie-lipschitz-uc-continue]].
> - **Heine** : continue sur un **compact** $\Rightarrow$ uniformément continue → [[topo-heine]].

> [!EXAMPLE] Exemples
> $x\mapsto x^2$ n'est pas U.C. sur $\mathbb R$ ($x_n=n$, $y_n=n+\frac1n$) mais l'est sur $[-M,M]$ ; $\sqrt{\cdot}$ est U.C. sur $[0,+\infty[$ sans être lipschitzienne.

> [!WARNING] Pièges
> « Continue sur $]0,1]$ (borné) donc U.C. » : faux, $\sin\frac1x$ ; il faut un **compact**.

## 🔗 Liens

- **S'appuie sur** : [[topo-continuite|Continuité en un point]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-composition-continues|Composition d'applications continues]], [[topo-hierarchie-lipschitz-uc-continue|Lipschitzienne ⇒ uniformément continue ⇒ continue]], [[topo-heine|Théorème de Heine]]
- **Méthodes** : [[topo-uniforme-continuite|Méthode : montrer (ou réfuter) l'uniforme continuité]]
- **Voir aussi** : —
