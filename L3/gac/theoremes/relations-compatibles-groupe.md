---
aliases:
  - "Relations compatibles avec la loi d'un groupe"
  - "compatible à gauche ssi x^-1y ∈ H"
  - "classification des relations compatibles"
tags:
  - gac
  - gac/theoreme
  - gac/chapitre-03
---

# ⭐ Relations compatibles avec la loi d'un groupe

*Théorème* · Chapitre : [[03-groupes-quotients|III – Groupes quotients]] · § III.3 du cours · [[index-definitions|↩ Index]]

> [!IMPORTANT] Théorèmes
> - Compatible **à gauche** $\iff$ $x\mathcal R y\iff x^{-1}y\in H$ pour un sous-groupe $H$ ($H=\bar1$) ; classes $xH$.
> - Compatible **à droite** $\iff$ $x\mathcal R y\iff yx^{-1}\in H$ ; classes $Hx$.
> - **Compatible** $\iff$ $x\mathcal R y\iff x^{-1}y\in H$ avec $\forall x,\ x^{-1}Hx=H$, i.e. $H\lhd G$ ; alors $xH=Hx$ ([[congruence-modulo-sous-groupe]]).
> - Si $\mathcal R$ est compatible, $G/\mathcal R$ est un groupe (neutre $\bar1$, inverse $\overline{x^{-1}}$) et $p$ est un morphisme surjectif.

> [!SUCCESS]- Démonstration (compatible à gauche ⟹ forme $x^{-1}y\in H$)
> $x\mathcal R y\Rightarrow 1\,\mathcal R\,x^{-1}y$ (multiplier à gauche par $x^{-1}$), donc $x^{-1}y\in\bar1$ ; réciproquement multiplier par $x$. $\bar1$ est un sous-groupe : $h,k\in\bar1\Rightarrow h\mathcal R k\Rightarrow h^{-1}k\in\bar1$ ; avec $k=1$, $h^{-1}\in\bar1$, puis $hk^{-1}\in\bar1$.

## 🔗 Liens

- **S'appuie sur** : [[relation-compatible|Relation compatible avec une loi]], [[classes-modulo-sous-groupe|Classes à gauche et à droite modulo un sous-groupe]], [[sous-groupe-distingue|Sous-groupe distingué]]
- **Utilisé par (définitions)** : [[congruence-modulo-sous-groupe|Congruence modulo un sous-groupe]]
- **Voir aussi** : [[groupe-quotient|Groupe quotient]]
