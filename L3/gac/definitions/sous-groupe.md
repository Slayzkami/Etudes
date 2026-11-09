---
aliases:
  - "Sous-groupe"
  - "sous-groupe"
  - "sous-groupes"
  - "sous-groupes triviaux"
  - "stable"
tags:
  - gac
  - gac/definition
  - gac/chapitre-02
---

# 📘 Sous-groupe

*Définition* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · § II.1 du cours · [[index-definitions|↩ Index]]

> [!NOTE] Définition
> Soit $(G,\star)$ un [[groupe]] et $H\subset G$. $H$ est un **sous-groupe** de $G$ si :
> 1. $H$ est non vide ;
> 2. $H$ est stable par la loi : $\forall x,y\in G,\ (x,y)\in H^2\Rightarrow x\star y\in H$ ;
> 3. $H$ est stable par symétrisation : $\forall x\in G,\ x\in H\Rightarrow x^{-1}\in H$.

> [!IMPORTANT] À retenir
> - $G$ et $H$ ont **le même neutre** et les mêmes inverses.
> - En pratique : [[caracterisation-sous-groupe|$e\in H$ et $\forall x,y\in H,\ xy^{-1}\in H$]].
> - $G$ et $\{1\}$ sont les sous-groupes triviaux.

> [!EXAMPLE] Exemples
> $n\mathbb Z\subset\mathbb Z$ ; $\mathbb U_n\subset\mathbb U\subset\mathbb C^*$ ; $SL_n(\mathbb R)\subset GL_n(\mathbb R)$ ;
> $\{e,\gamma,\gamma^2\}\subset\mathfrak S_3$. Tous les sous-groupes de $\mathbb Z$ : [[sous-groupes-de-z]].

> [!WARNING] Pièges
> - $\mathbb N$ est stable par $+$ mais n'est pas un sous-groupe de $\mathbb Z$.
> - « Partie non vide stable ⟹ sous-groupe » est **faux** en général, **vrai** dans un groupe **fini**.
> - Une réunion de sous-groupes n'en est pas un en général → [[intersection-sous-groupes]].

## 🔗 Liens

- **S'appuie sur** : [[groupe|Groupe]]
- **Utilisé par (définitions)** : [[automorphismes|Automorphismes et automorphismes intérieurs]], [[classes-modulo-sous-groupe|Classes à gauche et à droite modulo un sous-groupe]], [[image-noyau|Image, noyau, image réciproque]], [[sous-groupe-distingue|Sous-groupe distingué]], [[sous-groupe-engendre|Sous-groupe engendré par une partie]]
- **Utilisé par (théorèmes)** : [[caracterisation-sous-groupe|Caractérisations d'un sous-groupe]], [[intersection-sous-groupes|Intersection et réunion de sous-groupes]], [[sous-groupes-de-z|Sous-groupes de (Z,+)]]
- **Méthodes** : [[montrer-groupe|Méthode : montrer qu'un ensemble muni d'une loi est un groupe]]
- **Voir aussi** : [[montrer-sous-groupe|Méthode : montrer qu'une partie est un sous-groupe]]
