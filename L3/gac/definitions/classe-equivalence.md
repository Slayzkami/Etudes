---
aliases:
  - "Classe d'équivalence"
  - "classe"
  - "classes d'équivalence"
  - "partition"
  - "représentant"
tags:
  - gac
  - gac/definition
  - gac/chapitre-00
---

# 📘 Classe d'équivalence

*Définition* · Chapitre : [[00-rappels-relations-equivalence|Rappels – Relations d'équivalence]] · § R.2 du cours · [[index-definitions|↩ Index]]

> [!NOTE] Définition
> Soit $\mathcal R$ une [[relation-equivalence|relation d'équivalence]] sur $E$. La **classe** de $x\in E$ est
> $$\bar x=\operatorname{cl}(x)=\{y\in E \mid y\mathcal R x\}.$$
> Tout $y\in\bar x$ est un **représentant** de la classe ($\bar y=\bar x$).

> [!IMPORTANT] Propriétés (les classes forment une partition)
> Pour tous $x,y\in E$ :
> 1. $x\in\bar x$ ;
> 2. $\bar x=\bar y\iff x\mathcal R y$ ;
> 3. $\bar x\cap\bar y\neq\emptyset\Rightarrow\bar x=\bar y$.
>
> Donc $E$ est la réunion **disjointe** des classes.

> [!EXAMPLE] Exemple
> Modulo $3$ dans $\mathbb Z$ : trois classes $3\mathbb Z=\bar0$, $1+3\mathbb Z=\bar1$, $2+3\mathbb Z=\bar2$.

> [!WARNING] Piège
> Pour prouver $\bar x=\bar y$, on ne compare pas des ensembles : on montre simplement $x\mathcal R y$.

## 🔗 Liens

- **S'appuie sur** : [[relation-equivalence|Relation d'équivalence]]
- **Utilisé par (définitions)** : [[ensemble-quotient|Ensemble quotient et projection canonique]]
- **Voir aussi** : [[classes-modulo-sous-groupe|Classes à gauche et à droite modulo un sous-groupe]]
