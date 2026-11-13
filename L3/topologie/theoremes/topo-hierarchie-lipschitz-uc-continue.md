---
aliases:
  - "Lipschitzienne ⇒ uniformément continue ⇒ continue"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-02
---

# ⭐ Lipschitzienne ⇒ uniformément continue ⇒ continue

*Théorème* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Prop. 2.39 et 2.43 du cours (poly : Prop. 2.10, 2.11) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Toute application lipschitzienne est uniformément continue, et toute application uniformément continue est continue. **Les réciproques sont fausses.**

> [!SUCCESS]- Démonstration
> U.C. ⇒ continue : on fixe $y=a$. Lipschitzienne ⇒ U.C. : si $k>0$, $\delta=\varepsilon/k$ convient ($d(f(x),f(y))\le k\,d(x,y)<\varepsilon$).

> [!EXAMPLE] Exemple
> $x^2$ continue non U.C. sur $\mathbb R$ ($x_n=n$, $y_n=n+\frac1n$ : $|y_n^2-x_n^2|=2+\frac1{n^2}\ge2$) ; $\sqrt{\cdot}$ U.C. non lipschitzienne sur $[0,+\infty[$.

## 🔗 Liens

- **S'appuie sur** : [[topo-continuite-uniforme|Uniforme continuité]], [[topo-application-lipschitzienne|Application lipschitzienne]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : —
- **Méthodes** : [[topo-uniforme-continuite|Méthode : montrer (ou réfuter) l'uniforme continuité]]
- **Voir aussi** : —
