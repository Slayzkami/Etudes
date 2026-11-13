---
aliases:
  - "Partie bornée, diamètre"
  - "borné"
  - "partie bornée"
  - "diamètre"
  - "diam"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-01
---

# 📘 Partie bornée, diamètre

*Définition* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Déf. 1.16 du cours (poly : Déf. 1.5) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> Une partie non vide $A\subset E$ est **bornée** si $\{d(x,y)\mid x,y\in A\}$ est majoré, c'est-à-dire
> $$\exists M\ge0,\ \forall x,y\in A,\ d(x,y)\le M.$$
> Son **diamètre** est $\operatorname{diam}A=\sup_{(x,y)\in A^2}d(x,y)$ ($=+\infty$ si $A$ n'est pas bornée).

> [!IMPORTANT] À retenir
> - $A$ bornée $\iff$ $A$ est contenue dans une boule → [[topo-proprietes-parties-bornees]].
> - « Borné » n'est **pas** une notion topologique : $\mathbb R$ est borné pour $\min(1,|x-y|)$ et pas pour $|x-y|$.
> - Deux distances **métriquement** équivalentes ont les mêmes parties bornées (poly, exercice 2.10).

## 🔗 Liens

- **S'appuie sur** : [[topo-distance|Distance, espace métrique]], [[topo-boules-spheres|Boules et sphères]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-proprietes-parties-bornees|Propriétés des parties bornées]]
- **Méthodes** : —
- **Voir aussi** : —
