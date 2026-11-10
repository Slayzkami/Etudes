---
aliases:
  - "IAF sur un convexe : différentielle bornée implique lipschitzienne"
  - "Corollaire 3.13"
  - "lipschitzienne par l'IAF"
  - "Df bornée donc lipschitzienne"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-03
---

# ⭐ IAF sur un convexe : différentielle bornée implique lipschitzienne

*Théorème* · Chapitre : [[03-accroissements-finis|3 – Accroissements finis]] · Cor. 3.13 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Corollaire
> Soient $E,F$ des e.v.n., $C\subset E$ un ouvert **convexe** et $f:C\to F$ différentiable. S'il existe $M\ge0$ tel que $\lvert\!\lvert\!\lvert Df_x\rvert\!\rvert\!\rvert\le M$ pour tout $x\in C$, alors $f$ est $M$-lipschitzienne sur $C$ :
> $$\forall a,b\in C,\qquad \lVert f(b)-f(a)\rVert_F\le M\,\lVert b-a\rVert_E.$$

> [!SUCCESS]- Démonstration
> Soient $a,b\in C$. Comme $C$ est convexe, $[a,b]\subset C$. Sur ce segment $\lvert\!\lvert\!\lvert Df_x\rvert\!\rvert\!\rvert\le M$, donc l'IAF (Th. 3.11) donne $\lVert f(b)-f(a)\rVert\le M\lVert b-a\rVert$. $\blacksquare$

> [!TIP] Rédaction type (Écrit 2025-2026, ex. 2)
> « $\mathbb R^2$ est un ouvert convexe, $f$ est différentiable sur $\mathbb R^2$ et $\lvert\!\lvert\!\lvert Df_{(x,y)}\rvert\!\rvert\!\rvert\le3$ pour tout $(x,y)$. D'après le Corollaire 3.13, $f$ est $3$-lipschitzienne sur $\mathbb R^2$. »

> [!WARNING] Piège
> Sans la convexité, le résultat peut être faux. Toujours écrire « **ouvert convexe** ».

## 🔗 Liens

- **S'appuie sur** : [[iaf|Inégalité des accroissements finis (IAF)]], [[application-lipschitzienne|Application lipschitzienne]], [[segment-et-convexe|Segment, partie convexe]]
- **Utilisé par (théorèmes)** : [[differentielle-nulle|Différentielle nulle : f constante]]
- **Méthodes** : [[utiliser-iaf|Utiliser l'inégalité des accroissements finis (montrer lipschitzienne)]]
