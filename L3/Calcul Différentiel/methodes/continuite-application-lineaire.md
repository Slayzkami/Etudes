---
aliases:
  - "Méthode : continuité d'une application linéaire"
  - "linéaire continue ou non"
  - "justifier L continue"
tags:
  - cd
  - cd/methode
  - cd/chapitre-01
---

# 🛠️ Méthode : continuité d'une application linéaire

*Méthode* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Méthode 1.4 du cours · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> Soit $L:E\to F$ **linéaire** (le vérifier ou le dire).
> - **$E$ de dimension finie** : continue automatiquement (Th. 1.44).
> - **Sinon** : établir $\lVert L(u)\rVert_F\le C\lVert u\rVert_E$ pour tout $u$ (Th. 1.43 (iv)).
> - **Pour montrer qu'elle n'est pas continue** : une suite $u_n\ne0$ avec $\dfrac{\lVert L(u_n)\rVert}{\lVert u_n\rVert}\to+\infty$.

> [!EXAMPLE] Rédaction modèle (trace)
> « $\mathrm{tr}:\mathcal M_n(\mathbb R)\to\mathbb R$ est linéaire et $\mathcal M_n(\mathbb R)$ est de dimension finie, donc $\mathrm{tr}$ est continue (Th. 1.44). D'après le Th. 1.43 (iv), il existe $C\ge0$ tel que $\lvert \mathrm{tr}(X)\rvert\le C\lVert X\rVert$ pour tout $X$. » (Écrits 2022-2023 et 2024-2025.)

> [!EXAMPLE] Non-continuité
> $D:f\mapsto f'$ de $(\mathcal C^1([0,1]),\lVert \cdot\rVert_\infty)$ dans $(\mathcal C([0,1]),\lVert \cdot\rVert_\infty)$ : $u_n(t)=t^n$, $\lVert u_n\rVert_\infty=1$, $\lVert D(u_n)\rVert_\infty=n\to+\infty$.

## 🔗 Liens

- **Voir aussi** : [[caracterisation-lineaires-continues|Caractérisations des applications linéaires continues]], [[lineaire-en-dimension-finie|Linéaire au départ d'une dimension finie : continue]], [[application-lineaire-continue|Application linéaire continue, espace Lc(E,F)]]
