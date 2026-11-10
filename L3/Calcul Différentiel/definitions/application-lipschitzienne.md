---
aliases:
  - "Application lipschitzienne"
  - "lipschitzienne"
  - "k-lipschitzienne"
  - "Lipschitz"
tags:
  - cd
  - cd/definition
  - cd/chapitre-01
---

# 📘 Application lipschitzienne

*Définition* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Déf. 1.33 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> $f:E\to F$ est **lipschitzienne** s'il existe $k\ge0$ tel que
> $$\forall(x,y)\in E^2,\qquad \lVert f(x)-f(y)\rVert_F\le k\,\lVert x-y\rVert_E.$$
> On dit alors que $f$ est $k$-lipschitzienne.

> [!EXAMPLE] Exemples (Ex. 1.37)
> - La norme $x\mapsto\lVert x\rVert$ est $1$-lipschitzienne ([[seconde-inegalite-triangulaire]]).
> - Une application linéaire continue $f$ est $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert$-lipschitzienne.
> - Les projections $\pi_i$ sont $1$-lipschitziennes (Prop. 1.39).

> [!TIP] Le lien avec le chapitre 3
> Sur un ouvert **convexe**, si $\lvert\!\lvert\!\lvert Df_x\rvert\!\rvert\!\rvert\le M$ pour tout $x$, alors $f$ est $M$-lipschitzienne → [[iaf-sur-un-convexe]].

> [!WARNING] Piège
> $k$ ne dépend ni de $x$ ni de $y$. $x\mapsto x^2$ n'est pas lipschitzienne sur $\mathbb R$ (mais l'est sur tout intervalle borné).

## 🔗 Liens

- **S'appuie sur** : [[norme|Norme, espace vectoriel normé]]
- **Utilisé par (théorèmes)** : [[caracterisation-lineaires-continues|Caractérisations des applications linéaires continues]], [[iaf-sur-un-convexe|IAF sur un convexe : différentielle bornée implique lipschitzienne]], [[point-fixe-banach-picard|Théorème du point fixe de Banach-Picard]]
