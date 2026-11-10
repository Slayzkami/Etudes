---
aliases:
  - "Formules de Taylor (ordre n)"
  - "Taylor-Lagrange"
  - "Taylor reste intégral"
  - "Taylor-Young ordre n"
  - "inégalité de Taylor-Lagrange"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-04
---

# ⭐ Formules de Taylor (ordre n)

*Théorème* · Chapitre : [[04-differentielles-ordre-superieur|4 – Différentielles d'ordre supérieur]] · Th. 4.35, 4.37, 4.38, Cor. 4.39 du cours · [[cd-index-definitions|↩ Index]]

Notation : $D^kf_a(h)^k=D^kf_a(h,\dots,h)$.

> [!IMPORTANT] Taylor-Young (Th. 4.35, admis)
> Si $f:U\to F$ est $n$ fois différentiable en $a$ :
> $$f(a+h)=f(a)+\frac1{1!}Df_a(h)+\frac1{2!}D^2f_a(h,h)+\dots+\frac1{n!}D^nf_a(h)^n+o(\lVert h\rVert^n).$$

> [!IMPORTANT] Taylor-Lagrange (Th. 4.37) – valeurs **réelles**
> Si $f:U\to\mathbb R$ est $(n+1)$ fois différentiable sur $U$ et $[a,a+h]\subset U$, il existe $\theta\in\,]0,1[$ tel que
> $$f(a+h)=\sum_{k=0}^n\frac1{k!}D^kf_a(h)^k+\frac1{(n+1)!}D^{n+1}f_{a+\theta h}(h)^{n+1}.$$

> [!IMPORTANT] Taylor avec reste intégral (Th. 4.38) – $F$ Banach, $f$ de classe $\mathcal C^{n+1}$
> $$f(a+h)=\sum_{k=0}^n\frac1{k!}D^kf_a(h)^k+\int_0^1\frac{(1-t)^n}{n!}D^{n+1}f_{a+th}(h)^{n+1}\,\mathrm dt.$$
> Conséquence (Cor. 4.39) : si $\lVert D^{n+1}f_x\rVert\le M$ sur $[a,a+h]$, le reste est majoré par $\dfrac{M\lVert h\rVert^{n+1}}{(n+1)!}$.

> [!SUCCESS]- Idée commune des démonstrations
> On pose $g(t)=f(a+th)$ sur $[0,1]$. Par le Lemme 4.34, $g^{(k)}(t)=D^kf_{a+th}(h)^k$. On applique à $g$ la formule de Taylor correspondante **en une variable** entre $0$ et $1$. $\blacksquare$

> [!TIP] Lequel utiliser ?
> | Formule | Hypothèse | Nature |
> |---|---|---|
> | Young | $n$ fois différentiable **en $a$** | locale ($h\to0$) : extrema, DL |
> | Lagrange | $(n+1)$ fois différentiable, **à valeurs réelles** | égalité avec un point $\theta$ inconnu |
> | Reste intégral | $\mathcal C^{n+1}$, $F$ Banach | égalité exacte, donne des majorations |

## 🔗 Liens

- **S'appuie sur** : [[classe-cn|Différentiabilité d'ordre n, classes Cn et C∞]], [[taylor-young-ordre-2|Formule de Taylor-Young à l'ordre 2]], [[espace-de-banach|Espace complet, espace de Banach]]
