---
aliases:
  - "Différentielle nulle : f constante"
  - "Df = 0 donc constante"
  - "Théorème 3.25"
  - "Proposition 3.18"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-03
---

# ⭐ Différentielle nulle : f constante

*Théorème* · Chapitre : [[03-accroissements-finis|3 – Accroissements finis]] · Prop. 3.18, Th. 3.25 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> Soit $U\subset E$ un ouvert **connexe** et $f:U\to F$ différentiable telle que $Df_x=0$ pour tout $x\in U$. Alors $f$ est constante sur $U$ (Th. 3.25).
> Cas particulier : $U$ ouvert **convexe** (Prop. 3.18) ; dans ce cas c'est une équivalence.

> [!SUCCESS]- Démonstration
> **Cas convexe.** $\lvert\!\lvert\!\lvert Df_x\rvert\!\rvert\!\rvert=0\le0$ sur $U$ convexe : par le Cor. 3.13 avec $M=0$, $\lVert f(b)-f(a)\rVert\le0$, donc $f(a)=f(b)$.
> **Cas connexe.** Fixons $x_0\in U$ et posons $A=\{x\in U\mid f(x)=f(x_0)\}$.
> - $A\ne\emptyset$ ($x_0\in A$).
> - $A$ est fermé dans $U$ : $f$ est continue (car différentiable).
> - $A$ est ouvert : si $x\in A$, il existe une boule $B(x,r)\subset U$, convexe ; par le cas convexe $f$ y est constante, donc $B(x,r)\subset A$.
> $U$ connexe et $A$ ouvert-fermé non vide : $A=U$ (Prop. 3.21). $\blacksquare$

> [!WARNING] Piège (question de cours, Écrit 2022-2023)
> Sur un ouvert **non connexe**, on peut seulement dire que $f$ est constante sur chaque morceau (localement constante). Exemple : $U=\mathbb R^*$, $f=1$ sur $]0,+\infty[$, $f=-1$ sur $]-\infty,0[$.

## 🔗 Liens

- **S'appuie sur** : [[iaf-sur-un-convexe|IAF sur un convexe : différentielle bornée implique lipschitzienne]], [[partie-connexe|Partie connexe]]
- **Méthodes** : [[montrer-constante|Montrer qu'une application est constante]]
