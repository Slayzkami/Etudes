---
aliases:
  - "Espaces de Banach usuels"
  - "C([a,b]) est complet"
  - "Lc(E,F) est un Banach"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-01
---

# ⭐ Espaces de Banach usuels

*Théorème* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Th. 1.60 et 1.61 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorèmes
> - Tout e.v.n. de dimension finie est un Banach.
> - $(\mathcal C([a,b],\mathbb R),\lVert \cdot\rVert_\infty)$ est un Banach (Th. 1.60). $(\mathcal C([a,b]),\lVert \cdot\rVert_1)$ n'en est **pas** un.
> - Si $F$ est un Banach, $(\mathcal L_c(E,F),\lvert\!\lvert\!\lvert \cdot\rvert\!\rvert\!\rvert)$ est un Banach (Th. 1.61).

> [!SUCCESS]- Idée de la démonstration (Th. 1.60)
> Soit $(f_n)$ de Cauchy pour $\lVert \cdot\rVert_\infty$. Pour chaque $t$, $\lvert f_p(t)-f_q(t)\rvert\le\lVert f_p-f_q\rVert_\infty$ : $(f_n(t))$ est de Cauchy dans $\mathbb R$ complet, donc converge vers un réel $f(t)$. En faisant $q\to\infty$ dans $\lvert f_p(t)-f_q(t)\rvert\le\varepsilon$ on obtient $\lVert f_p-f\rVert_\infty\le\varepsilon$ : la convergence est uniforme, donc $f$ est continue et $f_n\to f$ dans $E$. $\blacksquare$

## 🔗 Liens

- **S'appuie sur** : [[espace-de-banach|Espace complet, espace de Banach]], [[norme-operateur|Norme d'opérateur]]
