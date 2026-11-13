---
aliases:
  - "Normes usuelles de K^n et de C([a,b])"
  - "norme 1"
  - "norme 2"
  - "norme infini"
  - "norme euclidienne"
  - "d1 d2 d∞"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-01
---

# 📘 Normes usuelles de K^n et de C([a,b])

*Définition* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Ex. 1.10 et 1.11 du cours (poly : Ex. 1.2, exercice 1.2) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> Pour $x=(x_1,\dots,x_n)\in\mathbb K^n$ :
> $$\|x\|_1=\sum_{i=1}^n|x_i|,\qquad \|x\|_2=\Big(\sum_{i=1}^n|x_i|^2\Big)^{1/2},\qquad \|x\|_\infty=\max_{1\le i\le n}|x_i|.$$
> Sur $C([a,b])$ : $\|f\|_1=\int_a^b|f|$, $\|f\|_2=\big(\int_a^bf^2\big)^{1/2}$, $\|f\|_\infty=\sup_{[a,b]}|f|$.

> [!IMPORTANT] À retenir
> - $\|x\|_\infty\le\|x\|_2\le\|x\|_1\le n\|x\|_\infty$ (Ex. 2.66).
> - Boules unité de $\mathbb R^2$ : losange ($\|\cdot\|_1$), disque ($\|\cdot\|_2$), carré ($\|\cdot\|_\infty$) → [[topo-boules-spheres]].
> - Sur $C([a,b])$ elles ne sont **pas** équivalentes (Rem. 2.68).

## 🔗 Liens

- **S'appuie sur** : [[topo-norme|Norme, espace vectoriel normé]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-riesz|Théorème de Riesz]]
- **Méthodes** : —
- **Voir aussi** : [[topo-normes-equivalentes|Normes équivalentes]]
