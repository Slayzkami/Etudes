---
aliases:
  - "Différentiable implique continue"
  - "Proposition 2.18"
  - "différentiable donc continue"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-02
---

# ⭐ Différentiable implique continue

*Théorème* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Prop. 2.18 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Proposition
> Si $f$ est différentiable en $a$, alors $f$ est continue en $a$.

> [!SUCCESS]- Démonstration (question de cours, Écrit 2022-2023)
> Par définition, pour $x\in U$ : $f(x)-f(a)=Df_a(x-a)+\lVert x-a\rVert\,\varepsilon(x)$ avec $\varepsilon(x)\to0$. Donc
> $$\lVert f(x)-f(a)\rVert\le\lvert\!\lvert\!\lvert Df_a\rvert\!\rvert\!\rvert\,\lVert x-a\rVert+\lVert x-a\rVert\,\lVert \varepsilon(x)\rVert\xrightarrow[x\to a]{}0,$$
> car $Df_a$ est linéaire **continue** (Prop. 1.50 (i)). Donc $f(x)\to f(a)$. $\blacksquare$

> [!TIP] Usage (contraposée)
> $f$ non continue en $a$ $\Rightarrow$ $f$ non différentiable en $a$ : c'est le premier test à faire → [[montrer-non-differentiable]].

## 🔗 Liens

- **S'appuie sur** : [[differentiabilite|Différentiabilité en un point, différentielle]], [[continuite|Continuité en un point]]
- **Méthodes** : [[montrer-non-differentiable|Montrer qu'une application n'est pas différentiable en a]]
