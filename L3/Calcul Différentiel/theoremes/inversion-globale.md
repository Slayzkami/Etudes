---
aliases:
  - "Théorème d'inversion globale"
  - "inversion globale"
  - "difféomorphisme global"
  - "Corollaire 5.13"
  - "forme pratique"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-05
---

# ⭐ Théorème d'inversion globale

*Théorème* · Chapitre : [[05-inversion-locale-fonctions-implicites|5 – Inversion locale et fonctions implicites]] · Th. 5.12, Cor. 5.13 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> Soit $U$ un ouvert de $\mathbb R^n$ et $f:U\to\mathbb R^n$ de classe $\mathcal C^1$, **injective**, et difféomorphisme local en tout point de $U$. Alors $f(U)$ est un ouvert de $\mathbb R^n$ et $f$ est un difféomorphisme de $U$ sur $f(U)$.

> [!IMPORTANT] Forme pratique (Cor. 5.13)
> Si $f:U\subset\mathbb R^n\to\mathbb R^n$ est $\mathcal C^1$ avec
> - (i) $f$ **injective** sur $U$,
> - (ii) $\det J_f(x)\ne0$ pour **tout** $x\in U$,
>
> alors $f(U)$ est ouvert, $f$ est un difféomorphisme de $U$ sur $f(U)$, et $J_{f^{-1}}(f(x))=J_f(x)^{-1}$.

> [!SUCCESS]- Démonstration
> 1. Soit $b=f(a)\in f(U)$. $f$ est un difféomorphisme de $U'\ni a$ sur $V'\ni b$, avec $V'$ ouvert et $V'=f(U')\subset f(U)$ : $f(U)$ est voisinage de $b$. Donc $f(U)$ est ouvert.
> 2. $f:U\to f(U)$ est bijective (injective) et $\mathcal C^1$. Sur $V'$, $f^{-1}$ coïncide avec la réciproque locale $g$ (car $f(g(y))=y=f(f^{-1}(y))$ et $f$ est injective), qui est $\mathcal C^1$. Donc $f^{-1}$ est $\mathcal C^1$ au voisinage de tout point de $f(U)$. $\blacksquare$

> [!TIP] Mode d'emploi
> → [[montrer-diffeomorphisme]] : $\mathcal C^1$, jacobien non nul partout, injectivité, image.

## 🔗 Liens

- **S'appuie sur** : [[inversion-locale|Théorème d'inversion locale]], [[diffeomorphisme|Difféomorphisme, difféomorphisme local]]
- **Méthodes** : [[montrer-diffeomorphisme|Montrer qu'une application est un difféomorphisme (local ou global)]]
