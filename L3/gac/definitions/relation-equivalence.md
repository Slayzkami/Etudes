---
aliases:
  - "Relation d'équivalence"
  - "relation d'équivalence"
  - "équivalence"
  - "réflexive"
  - "symétrique"
  - "transitive"
tags:
  - gac
  - gac/definition
  - gac/chapitre-00
---

# 📘 Relation d'équivalence

*Définition* · Chapitre : [[00-rappels-relations-equivalence|Rappels – Relations d'équivalence]] · § R.1 du cours · [[index-definitions|↩ Index]]

> [!NOTE] Définition
> Une relation binaire $\mathcal R$ sur un ensemble $E$ est une **relation d'équivalence** si elle est
> - **réflexive** : $\forall x\in E,\ x\mathcal R x$ ;
> - **symétrique** : $\forall x,y\in E,\ x\mathcal R y\Rightarrow y\mathcal R x$ ;
> - **transitive** : $\forall x,y,z\in E,\ (x\mathcal R y \text{ et } y\mathcal R z)\Rightarrow x\mathcal R z$.

> [!TIP] En clair
> $x\mathcal R y$ veut dire « $x$ et $y$ sont pareils de mon point de vue » (même reste, même distance, même image…).

> [!EXAMPLE] Exemples
> - Congruence modulo $n$ sur $\mathbb Z$ : $a\equiv b \pmod n \iff n\mid a-b$.
> - Sur le plan privé de $O$ : « être à la même distance de $O$ » (feuille 0, ex. 2).
> - Pour toute application $f:E\to F$ : $x\mathcal R_f y\iff f(x)=f(y)$ (feuille 0, ex. 4).
> - Dans un groupe, pour un sous-groupe $H$ : $x\mathcal R y\iff x^{-1}y\in H$ → [[classes-modulo-sous-groupe]].

## 🔗 Liens

- **Utilisé par (définitions)** : [[classe-equivalence|Classe d'équivalence]], [[classes-modulo-sous-groupe|Classes à gauche et à droite modulo un sous-groupe]], [[relation-compatible|Relation compatible avec une loi]]
- **Voir aussi** : [[ensemble-quotient|Ensemble quotient et projection canonique]]
- **Méthode** : [[montrer-relation-equivalence|relation d'équivalence, classes et quotient]]
