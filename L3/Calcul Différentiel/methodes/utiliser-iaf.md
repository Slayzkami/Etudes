---
aliases:
  - "Méthode : utiliser l'inégalité des accroissements finis (montrer lipschitzienne)"
  - "appliquer l'IAF"
  - "montrer k-lipschitzienne"
  - "majorer |||Df|||"
tags:
  - cd
  - cd/methode
  - cd/chapitre-03
---

# 🛠️ Méthode : utiliser l'inégalité des accroissements finis (montrer lipschitzienne)

*Méthode* · Chapitre : [[03-accroissements-finis|3 – Accroissements finis]] · Méthode 3.1 du cours · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> 1. **Segment** : $[a,b]\subset U$ (automatique si $U$ est **convexe** : $\mathbb R^n$, une boule…). L'écrire.
> 2. **Différentiabilité** de $f$ sur $U$.
> 3. **Borner la différentielle** : montrer $\lVert Df_x(h)\rVert\le M\lVert h\rVert$ pour tout $h$, donc $\lvert\!\lvert\!\lvert Df_x\rvert\!\rvert\!\rvert\le M$ (Prop. 1.50 (ii)), pour tout $x$.
> 4. **Conclure** : $\lVert f(b)-f(a)\rVert\le M\lVert b-a\rVert$ ; sur un convexe, $f$ est $M$-lipschitzienne (Cor. 3.13).

> [!EXAMPLE] Rédaction modèle (Écrit 2025-2026, ex. 2)
> $f(x,y)=(\cos(x+2y),\sin(2x+y))$, $\mathbb R^2$ muni de $\lVert \cdot\rVert_1$.
> $Df_{(x,y)}(h)=\big(-\sin(x+2y)(h_1+2h_2),\ \cos(2x+y)(2h_1+h_2)\big)$. Comme $\lvert \sin\rvert,\lvert \cos\rvert\le1$ :
> $\lVert Df_{(x,y)}(h)\rVert_1\le\lvert h_1+2h_2\rvert+\lvert 2h_1+h_2\rvert\le3\lvert h_1\rvert+3\lvert h_2\rvert=3\lVert h\rVert_1$.
> Donc $\lvert\!\lvert\!\lvert Df_{(x,y)}\rvert\!\rvert\!\rvert\le3$ pour tout $(x,y)$. $\mathbb R^2$ est un ouvert convexe et $f$ y est différentiable : par le Cor. 3.13, $f$ est $3$-lipschitzienne.

> [!TIP] Astuce
> Pour comparer $f$ à une application linéaire $L$ : appliquer l'IAF à $g=f-L$, dont la différentielle est $Df_x-L$.

> [!WARNING] Pièges
> - Oublier « convexe » (ou le segment).
> - Écrire l'**égalité** des accroissements finis pour une fonction à valeurs dans $\mathbb R^p$, $p\ge2$ → [[taf]].

## 🔗 Liens

- **Voir aussi** : [[iaf|Inégalité des accroissements finis (IAF)]], [[iaf-sur-un-convexe|IAF sur un convexe : différentielle bornée implique lipschitzienne]], [[calculer-norme-operateur|Calculer une norme d'opérateur]]
