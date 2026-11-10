---
aliases:
  - "Seconde inégalité triangulaire"
  - "inégalité triangulaire inverse"
  - "la norme est 1-lipschitzienne"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-01
---

# ⭐ Seconde inégalité triangulaire

*Théorème* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Prop. 1.2 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Proposition
> Dans un e.v.n. : $\forall(x,y)\in E^2,\quad \big|\,\lVert x\rVert-\lVert y\rVert\,\big|\le\lVert x-y\rVert$.

> [!SUCCESS]- Démonstration
> $\lVert x\rVert=\lVert (x-y)+y\rVert\le\lVert x-y\rVert+\lVert y\rVert$, donc $\lVert x\rVert-\lVert y\rVert\le\lVert x-y\rVert$.
> En échangeant $x$ et $y$ : $\lVert y\rVert-\lVert x\rVert\le\lVert y-x\rVert=\lVert x-y\rVert$ (homogénéité avec $\lambda=-1$).
> Les deux inégalités donnent le résultat. $\blacksquare$

> [!TIP] Conséquence
> La norme est $1$-[[application-lipschitzienne|lipschitzienne]], donc continue : si $x_n\to\ell$ alors $\lVert x_n\rVert\to\lVert \ell\rVert$ (Prop. 1.17).

## 🔗 Liens

- **S'appuie sur** : [[norme|Norme, espace vectoriel normé]]
- **Méthodes** : [[montrer-norme|Montrer qu'une application est une norme]]
