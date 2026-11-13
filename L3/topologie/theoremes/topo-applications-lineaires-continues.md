---
aliases:
  - "Continuité d'une application linéaire"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-02
---

# ⭐ Continuité d'une application linéaire

*Théorème* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Th. 2.69 du cours (poly : Th. 2.11) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Pour $f:E\to F$ **linéaire**, sont équivalentes :
> (i) $f$ continue ; (ii) $f$ continue en $0$ ; (iii) $\exists C>0,\ \forall u\in E,\ \|f(u)\|_F\le C\|u\|_E$ ; (iv) $f$ lipschitzienne ; (v) $f$ bornée sur $B_E(0,1)$.

> [!SUCCESS]- Démonstration
> (ii)⇒(v) $\|v\|<\eta\Rightarrow\|f(v)\|<1$ ; pour $\|u\|<1$, $v=\eta u$ donne $\|f(u)\|<\frac1\eta$.
> (v)⇒(iii) $v=\frac{u}{2\|u\|}\in B(0,1)$ donne $\|f(u)\|\le2M\|u\|$.
> (iii)⇒(iv) $\|f(u)-f(v)\|=\|f(u-v)\|\le C\|u-v\|$.

> [!WARNING] Pièges
> « Linéaire donc continue » : vrai seulement si $E$ est de **dimension finie**. La dérivation sur $(C^\infty([0,1]),\|\cdot\|_\infty)$ n'est pas continue ($t^n$).

## 🔗 Liens

- **S'appuie sur** : [[topo-norme|Norme, espace vectoriel normé]], [[topo-continuite|Continuité en un point]], [[topo-application-lipschitzienne|Application lipschitzienne]]
- **Utilisé par (définitions)** : [[topo-norme-operateur|Norme d'une application linéaire continue]]
- **Utilisé par (théorèmes)** : —
- **Méthodes** : [[topo-application-lineaire-norme-operateur|Méthode : continuité d'une application linéaire, norme d'opérateur]]
- **Voir aussi** : —
