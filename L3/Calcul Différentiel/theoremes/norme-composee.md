---
aliases:
  - "Norme d'une composée"
  - "sous-multiplicativité"
  - "|||g∘f||| ≤ |||g||| |||f|||"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-01
---

# ⭐ Norme d'une composée

*Théorème* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Prop. 1.51 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Proposition
> Si $f\in\mathcal L_c(E,F)$ et $g\in\mathcal L_c(F,G)$, alors $g\circ f\in\mathcal L_c(E,G)$ et $\lvert\!\lvert\!\lvert g\circ f\rvert\!\rvert\!\rvert\le\lvert\!\lvert\!\lvert g\rvert\!\rvert\!\rvert\,\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert$.

> [!SUCCESS]- Démonstration
> Pour tout $u$ : $\lVert g(f(u))\rVert\le\lvert\!\lvert\!\lvert g\rvert\!\rvert\!\rvert\,\lVert f(u)\rVert\le\lvert\!\lvert\!\lvert g\rvert\!\rvert\!\rvert\,\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert\,\lVert u\rVert$ (Prop. 1.50 (i) deux fois). Par Prop. 1.50 (ii), $\lvert\!\lvert\!\lvert g\circ f\rvert\!\rvert\!\rvert\le\lvert\!\lvert\!\lvert g\rvert\!\rvert\!\rvert\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert$. $\blacksquare$

> [!TIP] Où ça sert
> Normes matricielles : $\lVert AB\rVert\le\lVert A\rVert\lVert B\rVert$ (hypothèse classique des sujets sur $\mathcal M_n(\mathbb R)$) → [[differentielle-sur-les-matrices]].

## 🔗 Liens

- **S'appuie sur** : [[norme-operateur|Norme d'opérateur]]
- **Utilisé par (théorèmes)** : [[regle-de-la-chaine|Règle de la chaîne (différentielle d'une composée)]]
- **Méthodes** : [[differentielle-sur-les-matrices|Calculer une différentielle sur les matrices]]
