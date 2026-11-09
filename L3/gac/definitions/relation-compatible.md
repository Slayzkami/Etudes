---
aliases:
  - "Relation compatible avec une loi"
  - "compatible"
  - "compatible à gauche"
  - "compatible à droite"
  - "compatibilité"
tags:
  - gac
  - gac/definition
  - gac/chapitre-00
---

# 📘 Relation compatible avec une loi

*Définition* · Chapitre : [[00-rappels-relations-equivalence|Rappels – Relations d'équivalence]] · § R.1 du cours · [[index-definitions|↩ Index]]

> [!NOTE] Définition
> Soit $\star$ une [[loi-composition-interne|loi interne]] sur $E$ et $\mathcal R$ une [[relation-equivalence|relation d'équivalence]]. $\mathcal R$ est
> - **compatible à gauche** avec $\star$ : $\forall a,x,y\in E,\ x\mathcal R y\Rightarrow(a\star x)\,\mathcal R\,(a\star y)$ ;
> - **compatible à droite** : $\forall a,x,y\in E,\ x\mathcal R y\Rightarrow(x\star a)\,\mathcal R\,(y\star a)$ ;
> - **compatible** : $\forall x,y,x',y'\in E,\ (x\mathcal R y \text{ et } x'\mathcal R y')\Rightarrow(x\star x')\,\mathcal R\,(y\star y')$.

> [!IMPORTANT] Proposition
> $\mathcal R$ est compatible $\iff$ elle est compatible à gauche **et** à droite.

> [!TIP] En clair
> On peut remplacer chaque facteur par un élément équivalent sans changer la classe du résultat,
> comme avec les congruences : $17\equiv2 \pmod 5\Rightarrow 17\times4\equiv2\times4 \pmod 5$.

> [!EXAMPLE] Exemples
> - Congruence modulo $n$ : compatible avec $+$ et $\times$ ($xx'-yy'=x(x'-y')+y'(x-y)$).
> - Contre-exemple : sur $(\mathbb Z,+)$, $x\mathcal R y\iff|x|=|y|$ : $1\mathcal R(-1)$ mais $1+1=2$ et $-1+1=0$ ne sont pas en relation.
> - Dans un groupe : les relations compatibles sont exactement les [[congruence-modulo-sous-groupe|congruences modulo un sous-groupe distingué]].

## 🔗 Liens

- **S'appuie sur** : [[relation-equivalence|Relation d'équivalence]], [[loi-composition-interne|Loi de composition interne]]
- **Utilisé par (définitions)** : [[classes-modulo-sous-groupe|Classes à gauche et à droite modulo un sous-groupe]], [[groupe-quotient|Groupe quotient]], [[loi-quotient|Loi quotient]]
- **Utilisé par (théorèmes)** : [[relations-compatibles-groupe|Relations compatibles avec la loi d'un groupe]]
