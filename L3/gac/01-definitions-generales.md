---
aliases:
  - "I – Définitions générales"
  - "Chapitre groupes définitions"
tags:
  - gac
  - gac/chapitre
---

# Chapitre 01 – I. Définitions générales

**Matière :** [[L3/gac/README|Groupes, anneaux, corps]]  
**Date du cours :** polycopié *GAC-Chap1-Groupes*, partie I (transparents 6 à 24)  
**Index :** [[index-definitions]]

## 🎯 L'essentiel en 3 lignes
- Un [[groupe]] : loi interne associative, avec neutre, où tout élément a un symétrique (neutre et symétrique sont uniques).
- On calcule avec les [[regles-de-calcul|règles de calcul]] : simplification, $(ab)^{-1}=b^{-1}a^{-1}$, puissances.
- Un [[morphisme-de-groupes|morphisme]] respecte la loi ; un isomorphisme est un « renommage » : deux [[groupes-isomorphes|groupes isomorphes]] ont la même structure.

## 📝 Notes

### I.1 – Groupes : définition, exemples
- Déf. 1 : [[groupe]] (G1)–(G3) ; [[groupe-abelien]] si commutatif. Remarque 1 : [[unicite-neutre-symetrique]].
- Exemples : $(\mathbb Z,+)$, $(\mathbb R^*,\times)$, $\mathbb U$, $\mathbb Z/n\mathbb Z$ → catalogue [[exemples-de-groupes]].
- Lire une table : neutre = ligne et colonne recopiant l'en-tête ; symétrique = case contenant le neutre ; commutatif = table symétrique ; groupe ⟹ chaque élément une fois par ligne et par colonne.
- [[groupe-des-permutations]] $\mathcal S(E)$, $\mathfrak S_n$ ($n!$ éléments), table de $\mathfrak S_3$.
- [[groupe-produit]], groupe de Klein.

### I.2 – Notations et règles de calcul
- Notation multiplicative / additive ; [[puissances-multiples]].
- [[regles-de-calcul]] : inverses, puissances, simplification, équations $ax=b$.

### I.3 – Homomorphismes de groupes
- [[morphisme-de-groupes]] : endo-, iso-, automorphisme ; [[proprietes-morphismes]] ($f(1)=1$, $f(x^{-1})=f(x)^{-1}$, $f(x^n)=f(x)^n$, composée, réciproque).
- [[groupes-isomorphes]] ; « être isomorphe » est une relation d'équivalence.
- Exercices types : $\exp:(\mathbb R,+)\to(\mathbb R_+^*,\times)$ isomorphisme ; $\mathbb Z/4\mathbb Z\not\simeq$ Klein ([[montrer-non-isomorphes]]) ; $\mathrm{Aut}\,\mathbb Z/4\mathbb Z\simeq\mathbb Z/2\mathbb Z$ ; [[automorphismes]] intérieurs $f_a$ ; isométries du triangle $\simeq\mathfrak S_3$.

## 🔑 Définitions / formules à retenir
| Terme | Définition |
|---|---|
| [[loi-composition-interne]] | application $E\times E\to E$ |
| [[groupe]] | associativité, neutre, symétriques |
| [[groupe-abelien]] | $xy=yx$ pour tous $x,y$ |
| [[puissances-multiples]] | $x^n$, $x^{-n}=(x^{-1})^n$ ; $nx$ |
| [[groupe-des-permutations]] | bijections de $E$, loi $\circ$ |
| [[groupe-produit]] | loi composante par composante |
| [[morphisme-de-groupes]] | $f(xy)=f(x)f(y)$ |
| [[groupes-isomorphes]] | il existe un isomorphisme |
| [[automorphismes]] | $\mathrm{Aut}\,G$ ; $f_a(x)=axa^{-1}$ |

## ❓ Ce que je n'ai pas compris
- 

## 🧠 Questions de révision
1. Écrire (G1), (G2), (G3) avec les quantificateurs.
2. Démontrer l'unicité du symétrique.
3. Démontrer $(xy)^{-1}=y^{-1}x^{-1}$.
4. Montrer que $f(1_G)=1_{G'}$ pour un morphisme $f$.
5. Pourquoi $\mathbb Z/4\mathbb Z$ et $\mathbb Z/2\mathbb Z\times\mathbb Z/2\mathbb Z$ ne sont-ils pas isomorphes ?
6. Exercice type : montrer que $(\mathbb R\setminus\{-1\},\ a+b+ab)$ est un groupe → [[montrer-groupe]].

## 🔗 Pour aller plus loin
- Corrigés rédigés : [[exercices-types-corriges]] (ex. 4) · fiche : [[fiche-definitions]]
- Précédent : [[00-rappels-relations-equivalence]] · Suivant : [[02-sous-groupes]]
- TD1 : ex. 1 (monoïde), 2 (calculs), 4 ($\mathbb Z$-module), 15–16 ($D_3$, $D_4$)
- Sources : polycopié `GAC-Chap1-Groupes` (partie I), cours rédigé, correction du TD1 → dossier [fichiers](fichiers/)
