---
aliases:
  - "Rappels GAC"
  - "Relations d'équivalence (chapitre)"
tags:
  - gac
  - gac/chapitre
---

# Chapitre 00 – Rappels : relations d'équivalence

**Matière :** [[L3/gac/README|Groupes, anneaux, corps]]  
**Date du cours :** début du semestre (polycopié *GAC-Chap1-Groupes*, transparents 1 à 4 ; feuille 0)  
**Index :** [[index-definitions]]

## 🎯 L'essentiel en 3 lignes
- Une [[relation-equivalence|relation d'équivalence]] découpe un ensemble en [[classe-equivalence|classes]] disjointes : c'est une partition.
- L'[[ensemble-quotient|ensemble quotient]] $E/\mathcal R$ fait de chaque classe un seul point.
- Si la relation est [[relation-compatible|compatible]] avec une loi, cette loi « passe au quotient » ([[loi-quotient]]) : c'est la base des groupes quotients (chapitre 03).

## 📝 Notes

### R.1 – Relations d'équivalence et compatibilité
- Trois propriétés à vérifier : réflexive, symétrique, transitive.
- $\bar x=\bar y\iff x\mathcal R y$ : pour comparer deux classes, on compare les éléments.
- Compatible = compatible à gauche **et** à droite. Exemple fondamental : congruence modulo $n$ sur $\mathbb Z$, compatible avec $+$ et $\times$.
- Contre-exemple : $|x|=|y|$ sur $(\mathbb Z,+)$ n'est pas compatible.

### R.2 – Structure quotient
- Loi quotient $\bar x\,\dot\star\,\bar y=\overline{x\star y}$, indépendante des représentants grâce à la compatibilité.
- La projection $p:E\to E/\mathcal R$ transporte associativité, commutativité, neutre et symétriques.
- ⚠️ Une application définie sur un quotient doit être **bien définie** : voir [[morphisme-sur-quotient]].

### Feuille 0 – exercices types
- Plan privé de $O$, « même distance à $O$ » : classes = cercles de centre $O$ ; $E/\mathcal R$ en bijection avec $]0,+\infty[$ (classe ↦ rayon).
- $\mathbb Z$ modulo $n$ : $n$ classes $\bar0,\dots,\overline{n-1}$, bijection $\mathbb Z/\mathcal R_n\to\{0,\dots,n-1\}$ (reste).
- $x\mathcal R_f y\iff f(x)=f(y)$ : classes = ensembles où $f$ est constante ; $E/\mathcal R_f$ en bijection avec $f(E)$. Ex. : $z\mapsto|z|$ (cercles), $z\mapsto z/|z|$ (demi-droites ouvertes issues de $0$), $\sin$ (classe de $x$ : $\{x+2k\pi\}\cup\{\pi-x+2k\pi\}$).

## 🔑 Définitions / formules à retenir
| Terme | Définition |
|---|---|
| [[relation-equivalence]] | réflexive, symétrique, transitive |
| [[classe-equivalence]] | $\bar x=\{y\mid y\mathcal R x\}$ |
| [[ensemble-quotient]] | ensemble des classes ; $p:x\mapsto\bar x$ |
| [[relation-compatible]] | $x\mathcal R y,\ x'\mathcal R y'\Rightarrow (x\star x')\mathcal R(y\star y')$ |
| [[loi-quotient]] | $\bar x\,\dot\star\,\bar y=\overline{x\star y}$ |

## ❓ Ce que je n'ai pas compris
- 

## 🧠 Questions de révision
1. Énoncer les trois propriétés d'une relation d'équivalence, avec quantificateurs.
2. Montrer que les classes d'équivalence forment une partition de $E$.
3. Pourquoi la loi $\bar x+\bar y=\overline{x+y}$ est-elle bien définie sur $\mathbb Z/n\mathbb Z$ ?
4. Peut-on définir $\mathbb Z/4\mathbb Z\to\mathbb Z/3\mathbb Z$, $\bar k\mapsto\bar k$ ? Pourquoi ?

## 🔗 Pour aller plus loin
- Chapitre suivant : [[01-definitions-generales]]
- Sources : polycopié `GAC-Chap1-Groupes` ; feuille `GAC-Feuille0-Revisions` ; cours rédigé (partie « Rappels ») → dossier [fichiers](fichiers/)
