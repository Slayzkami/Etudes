---
aliases:
  - "Caractérisations des applications linéaires continues"
  - "Théorème 1.43"
  - "linéaire continue ssi"
  - "||f(u)|| ≤ C||u||"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-01
---

# ⭐ Caractérisations des applications linéaires continues

*Théorème* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Th. 1.43 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> Soit $f:E\to F$ **linéaire** entre deux e.v.n. Sont équivalentes :
> - (i) $f$ est continue sur $E$ ;
> - (ii) $f$ est continue en $0$ ;
> - (iii) $f$ est bornée sur la boule unité : $\exists M\ge0,\ \forall u\in\overline B_E(0,1),\ \lVert f(u)\rVert_F\le M$ ;
> - (iv) $\exists C\ge0,\ \forall u\in E,\ \lVert f(u)\rVert_F\le C\,\lVert u\rVert_E$ ;
> - (v) $f$ est lipschitzienne.

> [!SUCCESS]- Démonstration (à savoir)
> (i)$\Rightarrow$(ii) : évident.
> (ii)$\Rightarrow$(iii) : avec $\varepsilon=1$, il existe $\delta>0$ tel que $\lVert x\rVert\le\delta\Rightarrow\lVert f(x)\rVert\le1$ (car $f(0)=0$). Si $\lVert u\rVert\le1$, alors $\lVert \delta u\rVert\le\delta$, donc $\lVert f(\delta u)\rVert\le1$, soit $\lVert f(u)\rVert\le\frac1\delta$ par linéarité. $M=\frac1\delta$ convient.
> (iii)$\Rightarrow$(iv) : pour $u\ne0$, $\frac{u}{\lVert u\rVert}$ est de norme $1$, donc $\lVert f(\frac{u}{\lVert u\rVert})\rVert\le M$, soit $\lVert f(u)\rVert\le M\lVert u\rVert$ ; vrai aussi pour $u=0$.
> (iv)$\Rightarrow$(v) : $\lVert f(x)-f(y)\rVert=\lVert f(x-y)\rVert\le C\lVert x-y\rVert$ par linéarité.
> (v)$\Rightarrow$(i) : lipschitzienne $\Rightarrow$ continue. $\blacksquare$

> [!TIP] En pratique
> Pour une application linéaire, on prouve (iv) : **une seule majoration** $\lVert f(u)\rVert\le C\lVert u\rVert$ → [[continuite-application-lineaire]].

> [!WARNING] Piège
> Ce théorème ne vaut que pour $f$ **linéaire**. Il faut le dire avant de l'utiliser.

## 🔗 Liens

- **S'appuie sur** : [[application-lineaire-continue|Application linéaire continue, espace Lc(E,F)]], [[application-lipschitzienne|Application lipschitzienne]]
- **Utilisé par (théorèmes)** : [[lineaire-en-dimension-finie|Linéaire au départ d'une dimension finie : continue]], [[caracterisations-norme-operateur|Caractérisations de la norme d'opérateur]]
- **Méthodes** : [[continuite-application-lineaire|Continuité d'une application linéaire]]
