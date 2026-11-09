---
aliases:
  - "Intersection et réunion de sous-groupes"
  - "intersection"
  - "réunion"
  - "union de sous-groupes"
tags:
  - gac
  - gac/theoreme
  - gac/chapitre-02
---

# ⭐ Intersection et réunion de sous-groupes

*Théorème* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · § II.3 du cours · [[index-definitions|↩ Index]]

> [!IMPORTANT] Énoncés
> 1. Une intersection (non vide d'indices) de [[sous-groupe|sous-groupes]] est un sous-groupe ; de sous-groupes distingués, un sous-groupe distingué (TD1 ex. 6).
> 2. $H\cup K$ est un sous-groupe $\iff H\subset K$ ou $K\subset H$.
> 3. La réunion d'une famille **totalement ordonnée** de sous-groupes est un sous-groupe (TD1 ex. 5).

> [!SUCCESS]- Démonstration de 2 (sens difficile)
> Si $h\in H\setminus K$ et $k\in K\setminus H$, alors $hk\in H\cup K$. Si $hk\in H$ : $k=h^{-1}(hk)\in H$, absurde. Si $hk\in K$ : $h=(hk)k^{-1}\in K$, absurde.

> [!EXAMPLE] Contre-exemples à connaître
> - $2\mathbb Z\cup3\mathbb Z$ : contient $2$ et $3$ mais pas $5$.
> - Dans $\mathbb Z/12\mathbb Z$ : $\langle\bar3\rangle\cup\langle\bar4\rangle\ni\bar3,\bar4$ mais pas $\bar7$.
> - Dans $\mathbb Z/18\mathbb Z$ : $\langle\bar6\rangle\cup\langle\bar9\rangle\ni\bar6,\bar9$ mais pas $\overline{15}$.

## 🔗 Liens

- **S'appuie sur** : [[sous-groupe|Sous-groupe]]
- **Utilisé par (définitions)** : [[sous-groupe-engendre|Sous-groupe engendré par une partie]]
- **Méthodes** : [[vrai-faux-classiques|Vrai/Faux classiques (avec justification)]]
