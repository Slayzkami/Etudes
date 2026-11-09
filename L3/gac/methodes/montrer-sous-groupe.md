---
aliases:
  - "Méthode : montrer qu'une partie est un sous-groupe"
  - "prouver sous-groupe"
tags:
  - gac
  - gac/methode
  - gac/chapitre-02
---

# 🛠️ Méthode : montrer qu'une partie est un sous-groupe

*Méthode* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · [[index-definitions|↩ Index]]

> [!ABSTRACT] Recette (caractérisation pratique)
> 1. $H\subset G$ ($G$ groupe connu, **même loi**).
> 2. $e\in H$.
> 3. Soient $x,y\in H$ : montrer $xy^{-1}\in H$ (additif : $x-y\in H$).
>
> **Variante express** : écrire $H=\mathrm{Ker} f$ (ou $\mathrm{Im} f$) pour un morphisme $f$ → [[noyau-et-image]]. Ex. : $\mathbb U_n=\mathrm{Ker}(z\mapsto z^n)$.
>
> **Pour réfuter** : $e\notin H$, ou $x,y\in H$ avec $xy\notin H$, ou $x\in H$ avec $x^{-1}\notin H$.

> [!EXAMPLE] Exemple rédigé (TD1 ex. 9)
> $K=\{\begin{pmatrix}a&b\\0&d\end{pmatrix}, ad\neq0\}$ : $I_2\in K$ ; $MN^{-1}$ a encore un $0$ en bas à gauche et est inversible ⟹ $K\le GL_2(\mathbb R)$.

## 🔗 Liens

- **Méthodes** : [[montrer-groupe|Méthode : montrer qu'un ensemble muni d'une loi est un groupe]]
- **Voir aussi** : [[caracterisation-sous-groupe|Caractérisations d'un sous-groupe]], [[sous-groupe|Sous-groupe]]
