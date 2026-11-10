---
aliases:
  - "Caractérisations de la norme d'opérateur"
  - "Proposition 1.50"
  - "plus petite constante"
  - "||f(u)|| ≤ |||f||| ||u||"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-01
---

# ⭐ Caractérisations de la norme d'opérateur

*Théorème* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Prop. 1.50 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Proposition
> Soit $f\in\mathcal L_c(E,F)$, $E\ne\{0\}$.
> - (i) Pour tout $u\in E$ : $\lVert f(u)\rVert_F\le\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert\,\lVert u\rVert_E$.
> - (ii) Si $C\ge0$ vérifie $\lVert f(u)\rVert_F\le C\lVert u\rVert_E$ pour tout $u$, alors $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert\le C$.
> - (iii) $\displaystyle\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert=\sup_{u\ne0}\frac{\lVert f(u)\rVert}{\lVert u\rVert}=\sup_{\lVert u\rVert=1}\lVert f(u)\rVert$.

> [!SUCCESS]- Démonstration
> (i) Si $u\ne0$, $\frac u{\lVert u\rVert}$ est de norme $1\le1$, donc $\lVert f(\frac u{\lVert u\rVert})\rVert\le\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert$, d'où $\lVert f(u)\rVert\le\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert\lVert u\rVert$. Vrai pour $u=0$.
> (ii) Si $\lVert u\rVert\le1$ alors $\lVert f(u)\rVert\le C\lVert u\rVert\le C$ : $C$ majore l'ensemble dont $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert$ est le sup, donc $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert\le C$.
> (iii) Par (i), $\frac{\lVert f(u)\rVert}{\lVert u\rVert}\le\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert$ pour $u\ne0$. Inversement, si $0<\lVert u\rVert\le1$, $\lVert f(u)\rVert\le\frac{\lVert f(u)\rVert}{\lVert u\rVert}$, donc $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert\le\sup_{u\ne0}\frac{\lVert f(u)\rVert}{\lVert u\rVert}$. Enfin $\frac{\lVert f(u)\rVert}{\lVert u\rVert}=\lVert f(\frac u{\lVert u\rVert})\rVert$ donne l'égalité avec le sup sur la sphère. $\blacksquare$

> [!TIP] Mode d'emploi
> (ii) sert à **majorer** $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert$ ; puis un vecteur $u_0$ avec $\lVert f(u_0)\rVert=C\lVert u_0\rVert$ donne $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert\ge C$ par (i) → [[calculer-norme-operateur]].

## 🔗 Liens

- **S'appuie sur** : [[norme-operateur|Norme d'opérateur]], [[caracterisation-lineaires-continues|Caractérisations des applications linéaires continues]]
- **Méthodes** : [[calculer-norme-operateur|Calculer une norme d'opérateur]]
