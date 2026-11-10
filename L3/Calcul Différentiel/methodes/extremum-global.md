---
aliases:
  - "Méthode : montrer l'existence d'un extremum global"
  - "minimum global"
  - "maximum global"
  - "coercivité"
tags:
  - cd
  - cd/methode
  - cd/chapitre-04
---

# 🛠️ Méthode : montrer l'existence d'un extremum global

*Méthode* · Chapitre : [[04-differentielles-ordre-superieur|4 – Différentielles d'ordre supérieur]] · Méthode 4.3 du cours · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> - **Par une inégalité directe** : montrer $f(x)\ge m$ pour tout $x$ et trouver $x_0$ avec $f(x_0)=m$.
> - **Pour réfuter** : trouver un chemin où $f\to-\infty$ (pas de minimum global) ou $+\infty$.
> - **Par coercivité** (dimension finie) : si $f$ est continue sur $\mathbb R^n$ et $f(x)\to+\infty$ quand $\lVert x\rVert\to+\infty$, $f$ admet un minimum global, atteint en un point critique (si $f$ est différentiable) : comparer les valeurs aux points critiques.

> [!EXAMPLE] Exemple
> $f(x,y)=x^3-3x+y^2$ : $f(x,0)=x^3-3x\to-\infty$ quand $x\to-\infty$ et $\to+\infty$ quand $x\to+\infty$ : ni minimum ni maximum global. Le minimum local en $(1,0)$ n'est pas global.

## 🔗 Liens

- **Voir aussi** : [[extremum-local|Extremum local, extremum global]], [[condition-necessaire-extremum|Condition nécessaire d'extremum (ordre 1)]]
