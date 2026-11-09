---
aliases:
  - "II – Sous-groupes"
  - "Chapitre sous-groupes"
tags:
  - gac
  - gac/chapitre
---

# Chapitre 02 – II. Sous-groupes

**Matière :** [[L3/gac/README|Groupes, anneaux, corps]]  
**Date du cours :** polycopié *GAC-Chap1-Groupes*, partie II (transparents 25 à 54)  
**Index :** [[index-definitions]]

## 🎯 L'essentiel en 3 lignes
- Pour montrer qu'une partie est un [[sous-groupe]] : $e\in H$ et $xy^{-1}\in H$ ([[caracterisation-sous-groupe]]).
- Noyau et image d'un morphisme sont des sous-groupes, le noyau est même **distingué** ; $f$ injectif ⟺ $\mathrm{Ker} f=\{1\}$ ([[noyau-et-image]]).
- L'[[ordre-element|ordre d'un élément]] est le cardinal du sous-groupe qu'il engendre ; un groupe monogène est $\simeq\mathbb Z$ ou $\mathbb Z/n\mathbb Z$ ([[structure-groupes-monogenes]]).

## 📝 Notes

### II.1 – Définition et exemples
- [[sous-groupe]] : non vide, stable par la loi, stable par inverse ; même neutre que $G$.
- Groupes de nombres : $n\mathbb Z\le\mathbb Z\le\mathbb Q\le\mathbb R\le\mathbb C$ ; $\mathbb U_n\le\mathbb U\le\mathbb C^*$. $\mathrm{Aut}\,G\le\mathcal S(G)$ ; $\mathcal I(G)\le\mathrm{Aut}\,G$.

### II.2 – Caractérisation
- [[caracterisation-sous-groupe]] ; dans un groupe fini, « non vide + stable » suffit.
- [[sous-groupes-de-z]] : ce sont les $a\mathbb Z$.

### II.2-bis – Sous-groupes distingués
- [[sous-groupe-distingue]] : $g^{-1}hg\in H$ ; équivalent à $gH=Hg$.
- [[centre]] $Z(G)$, toujours distingué.

### II.3 – Intersection
- [[intersection-sous-groupes]] : l'intersection est un sous-groupe, la réunion presque jamais.

### II.4 – Sous-groupe engendré
- [[sous-groupe-engendre]] = plus petit sous-groupe contenant $A$ ; $\langle x\rangle=\{x^n\}$ ; $\langle a,b\rangle=\operatorname{pgcd}(a,b)\mathbb Z$.
- [[groupe-monogene-cyclique|Monogène, cyclique]].

### II.5 – Image directe, image réciproque
- [[image-noyau]] et [[noyau-et-image]].

### II.6 – Ordre d'un élément
- [[ordre-element]] : cas 1 (ordre infini), cas 2 ($\mathrm{Ker}\,\varphi=m\mathbb Z$).
- Dans $\mathbb Z/n\mathbb Z$ : [[ordre-dans-znz]] ; exemple $\mathbb Z/12\mathbb Z$ (notes de cours).
- Méthode : [[calculer-ordre]].

### II.7 – Groupes monogènes, groupes cycliques
- [[ordre-groupe]] ; [[structure-groupes-monogenes]].
- Méthode : [[lister-sous-groupes-znz]] (treillis).

## 🔑 Définitions / formules à retenir
| Terme | Définition |
|---|---|
| [[sous-groupe]] | $\neq\emptyset$, stable, stable par inverse |
| [[sous-groupe-distingue]] | $\forall g,\forall h,\ g^{-1}hg\in H$ |
| [[centre]] | $\{g\mid\forall x,\ gx=xg\}$ |
| [[sous-groupe-engendre]] | intersection des sous-groupes contenant $A$ |
| [[groupe-monogene-cyclique]] | $G=\langle a\rangle$ (fini : cyclique) |
| [[image-noyau]] | $\mathrm{Im} f=f(G)$, $\mathrm{Ker} f=f^{-1}(\{1\})$ |
| [[ordre-element]] | plus petit $m\ge1$ avec $x^m=1$ |
| [[ordre-groupe]] | nombre d'éléments |

## ❓ Ce que je n'ai pas compris
- 

## 🧠 Questions de révision
1. Énoncer et démontrer la caractérisation pratique d'un sous-groupe.
2. Démontrer que les sous-groupes de $\mathbb Z$ sont les $a\mathbb Z$.
3. Démontrer que $\mathrm{Ker} f$ est un sous-groupe distingué et que $f$ injectif ⟺ $\mathrm{Ker} f=\{1\}$.
4. Ordre de $\bar2,\bar3,\bar4,\bar6,\bar9$ dans $\mathbb Z/12\mathbb Z$ ; liste des sous-groupes de $\mathbb Z/12\mathbb Z$ et de $\mathbb Z/18\mathbb Z$.
5. Donner deux sous-groupes de $\mathbb Z/12\mathbb Z$ dont la réunion n'est pas un sous-groupe.
6. Pourquoi Klein n'est-il pas cyclique ?

## 🔗 Pour aller plus loin
- Précédent : [[01-definitions-generales]] · Suivant : [[03-groupes-quotients]]
- TD1 : ex. 3, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14
- Sources : polycopié `GAC-Chap1-Groupes` (partie II), cours rédigé, correction du TD1 → dossier [fichiers](fichiers/)
