---
aliases:
  - "Théorème du point fixe de Banach-Picard"
  - "point fixe"
  - "application contractante"
  - "Picard"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-05
---

# ⭐ Théorème du point fixe de Banach-Picard

*Théorème* · Chapitre : [[05-inversion-locale-fonctions-implicites|5 – Inversion locale et fonctions implicites]] · Lemme 5.10 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> Soit $X$ une partie **fermée** non vide d'un espace de Banach et $T:X\to X$ une application **contractante** : il existe $k\in[0,1[$ tel que $\lVert T(x)-T(y)\rVert\le k\lVert x-y\rVert$ pour tous $x,y\in X$. Alors $T$ admet un **unique** point fixe dans $X$.

> [!SUCCESS]- Démonstration
> **Unicité.** Si $T(x)=x$ et $T(y)=y$ : $\lVert x-y\rVert\le k\lVert x-y\rVert$ avec $k<1$, donc $\lVert x-y\rVert=0$.
> **Existence.** Soit $x_0\in X$ et $x_{n+1}=T(x_n)$. Alors $\lVert x_{n+1}-x_n\rVert\le k^n\lVert x_1-x_0\rVert$, donc pour $p>q$ :
> $\lVert x_p-x_q\rVert\le\sum_{j=q}^{p-1}k^j\lVert x_1-x_0\rVert\le\frac{k^q}{1-k}\lVert x_1-x_0\rVert\to0$.
> La suite est de Cauchy, donc converge (espace complet) vers $\ell$, et $\ell\in X$ ($X$ fermé). $T$ est continue (lipschitzienne), donc $T(\ell)=\lim T(x_n)=\lim x_{n+1}=\ell$. $\blacksquare$

> [!TIP] Où ça sert
> Dans la preuve de l'[[inversion-locale]] : résoudre $f(x)=y$ revient à chercher un point fixe de $x\mapsto x+(Df_a)^{-1}(y-f(x))$.

## 🔗 Liens

- **S'appuie sur** : [[espace-de-banach|Espace complet, espace de Banach]], [[application-lipschitzienne|Application lipschitzienne]]
- **Utilisé par (théorèmes)** : [[inversion-locale|Théorème d'inversion locale]]
