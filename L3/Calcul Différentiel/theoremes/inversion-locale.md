---
aliases:
  - "Théorème d'inversion locale"
  - "TIL"
  - "inversion locale"
  - "Théorème 5.7"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-05
---

# ⭐ Théorème d'inversion locale

*Théorème* · Chapitre : [[05-inversion-locale-fonctions-implicites|5 – Inversion locale et fonctions implicites]] · Th. 5.7 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> Soit $U$ un ouvert de $\mathbb R^n$ et $f:U\to\mathbb R^n$ **de classe $\mathcal C^1$**. Soit $a\in U$ tel que $Df_a$ soit **bijective** (c'est-à-dire $\det J_f(a)\ne0$). Alors $f$ est un difféomorphisme local en $a$ : il existe des ouverts $U'\ni a$ et $V'\ni f(a)$ tels que $f:U'\to V'$ soit un difféomorphisme de classe $\mathcal C^1$. De plus, pour tout $x\in U'$,
> $$D(f^{-1})_{f(x)}=(Df_x)^{-1}.$$
> Si $f$ est $\mathcal C^k$, la réciproque locale est $\mathcal C^k$.

> [!NOTE] Les trois choses à vérifier
> 1. $f$ est $\mathcal C^1$ sur un ouvert contenant $a$.
> 2. Même dimension au départ et à l'arrivée (jacobienne **carrée**).
> 3. $\det J_f(a)\ne0$.

> [!SUCCESS]- Idée de la démonstration
> 1. On se ramène à $Df_a=\mathrm{id}$ (en composant par $(Df_a)^{-1}$).
> 2. $g(x)=x-f(x)$ vérifie $Dg_a=0$ ; par continuité de $Dg$ ($f$ est $\mathcal C^1$), $\lvert\!\lvert\!\lvert Dg_x\rvert\!\rvert\!\rvert\le\frac12$ sur une boule fermée $\overline B(a,r)$, donc $g$ y est $\frac12$-lipschitzienne (IAF).
> 3. Pour $y$ proche de $f(a)$, $T_y(x)=y+g(x)$ est contractante de $\overline B(a,r)$ dans elle-même : par le [[point-fixe-banach-picard|point fixe]], il existe un unique $x$ avec $T_y(x)=x$, c'est-à-dire $f(x)=y$. Donc $f$ est bijective localement.
> 4. $\lVert x-x'\rVert\le2\lVert f(x)-f(x')\rVert$ : $f^{-1}$ est continue ; on montre ensuite qu'elle est différentiable de différentielle $(Df_x)^{-1}$, puis $\mathcal C^1$. $\blacksquare$

> [!WARNING] Pièges
> - Le résultat est **local** : $f$ peut ne pas être injective sur $U$ ($(x,y)\mapsto(e^x\cos y,e^x\sin y)$ a un jacobien $e^{2x}\ne0$ partout mais est $2\pi$-périodique en $y$).
> - Différentiable ne suffit pas, il faut $\mathcal C^1$ ($x+2x^2\sin\frac1x$).

## 🔗 Liens

- **S'appuie sur** : [[diffeomorphisme|Difféomorphisme, difféomorphisme local]], [[differentielle-de-la-reciproque|Différentielle de la réciproque]], [[point-fixe-banach-picard|Théorème du point fixe de Banach-Picard]], [[iaf|Inégalité des accroissements finis (IAF)]], [[matrice-jacobienne|Matrice jacobienne]]
- **Utilisé par (théorèmes)** : [[inversion-globale|Théorème d'inversion globale]], [[fonctions-implicites-une-variable|Théorème des fonctions implicites (une variable)]]
- **Méthodes** : [[montrer-diffeomorphisme|Montrer qu'une application est un difféomorphisme (local ou global)]]
