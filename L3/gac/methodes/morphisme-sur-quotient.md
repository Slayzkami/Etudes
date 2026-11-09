---
aliases:
  - "Méthode : application définie sur un quotient (bien définie, morphisme)"
  - "bien définie"
  - "f(x+18Z)=x+6Z"
  - "Z/18Z vers Z/6Z"
tags:
  - gac
  - gac/methode
  - gac/chapitre-03
---

# 🛠️ Méthode : application définie sur un quotient (bien définie, morphisme)

*Méthode* · Chapitre : [[03-groupes-quotients|III – Groupes quotients]] · [[index-definitions|↩ Index]]

> [!ABSTRACT] Recette pour $f:\mathbb Z/n\mathbb Z\to\mathbb Z/m\mathbb Z,\ \bar x\mapsto\bar x$
> 1. **Bien définie** : si $\bar x=\bar y$ dans $\mathbb Z/n\mathbb Z$, alors $n\mid x-y$ ; il faut $m\mid x-y$. C'est vrai **ssi $m\mid n$**.
> 2. **Morphisme** : $f(\bar x+\bar y)=f(\overline{x+y})=\overline{x+y}=\bar x+\bar y=f(\bar x)+f(\bar y)$.
> 3. **Noyau** : $f(\bar x)=\bar0\iff m\mid x$ : $\mathrm{Ker} f=m\mathbb Z/n\mathbb Z=\langle\bar m\rangle$, de cardinal $n/m$.
> 4. **Image** : surjective ($\bar k=f(\bar k)$).
> 5. **Conclusion** : [[premier-theoreme-isomorphisme]] ⟹ $(\mathbb Z/n\mathbb Z)/(m\mathbb Z/n\mathbb Z)\simeq\mathbb Z/m\mathbb Z$.

> [!EXAMPLE] Rédaction modèle ($n=18$, $m=6$)
> Si $x+18\mathbb Z=y+18\mathbb Z$, alors $18\mid x-y$, donc $6\mid x-y$, donc $x+6\mathbb Z=y+6\mathbb Z$ : $f$ est bien définie. […] $\mathrm{Ker} f=\{\bar0,\bar6,\overline{12}\}=6\mathbb Z/18\mathbb Z$, $\mathrm{Im} f=\mathbb Z/6\mathbb Z$, d'où $(\mathbb Z/18\mathbb Z)/(6\mathbb Z/18\mathbb Z)\simeq\mathbb Z/6\mathbb Z$ via $\overline{\bar x}\mapsto x+6\mathbb Z$.

> [!WARNING] Piège
> Dans l'autre sens, $g:\mathbb Z/6\mathbb Z\to\mathbb Z/18\mathbb Z,\ \bar x\mapsto\bar x$ **n'est pas bien définie** : $\bar0=\bar6$ dans $\mathbb Z/6\mathbb Z$ mais $\bar0\neq\bar6$ dans $\mathbb Z/18\mathbb Z$.
> Et « $\mathbb Z/6\mathbb Z$ sous-groupe de $\mathbb Z/18\mathbb Z$ ? » : **non**, ce ne sont pas des parties l'un de l'autre (les éléments sont des classes différentes) ; mais $\mathbb Z/18\mathbb Z$ contient un sous-groupe **isomorphe** à $\mathbb Z/6\mathbb Z$ : $\langle\bar3\rangle$.

## 🔗 Liens

- **Utilisé par (définitions)** : [[ensemble-quotient|Ensemble quotient et projection canonique]]
- **Voir aussi** : [[groupe-quotient|Groupe quotient]], [[identifier-quotient|Méthode : identifier un groupe quotient G/H]]
