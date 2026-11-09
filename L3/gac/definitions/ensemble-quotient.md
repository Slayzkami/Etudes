---
aliases:
  - "Ensemble quotient et projection canonique"
  - "ensemble quotient"
  - "projection canonique"
  - "surjection canonique"
  - "bien définie"
tags:
  - gac
  - gac/definition
  - gac/chapitre-00
---

# 📘 Ensemble quotient et projection canonique

*Définition* · Chapitre : [[00-rappels-relations-equivalence|Rappels – Relations d'équivalence]] · § R.2 du cours · [[index-definitions|↩ Index]]

> [!NOTE] Définition
> - L'**ensemble quotient** $E/\mathcal R$ est l'ensemble des [[classe-equivalence|classes d'équivalence]].
> - La **projection (surjection) canonique** est $p:E\to E/\mathcal R,\ x\mapsto\bar x$ ; elle est surjective.

> [!TIP] En clair
> On « recolle » les éléments équivalents : chaque classe devient **un seul point** de $E/\mathcal R$.

> [!EXAMPLE] Exemple
> $\mathbb Z/n\mathbb Z=\{\bar0,\bar1,\dots,\overline{n-1}\}$ (division euclidienne : chaque entier a un unique reste).

> [!WARNING] Application définie sur un quotient
> Définir $f(\bar x)=g(x)$ n'a de sens que si $g(x)$ ne dépend que de la classe :
> $x\mathcal R y\Rightarrow g(x)=g(y)$ (« $f$ est **bien définie** »).
> - $\mathbb Z/6\mathbb Z\to\mathbb Z/3\mathbb Z,\ \bar k\mapsto\bar k$ : OK car $6\mid k-l\Rightarrow3\mid k-l$.
> - $\mathbb Z/4\mathbb Z\to\mathbb Z/3\mathbb Z,\ \bar k\mapsto\bar k$ : **interdit** ($\bar0=\bar4$ mod 4 mais pas mod 3).
>
> Méthode : [[morphisme-sur-quotient]].

## 🔗 Liens

- **S'appuie sur** : [[classe-equivalence|Classe d'équivalence]]
- **Utilisé par (définitions)** : [[loi-quotient|Loi quotient]]
- **Voir aussi** : [[groupe-quotient|Groupe quotient]]
