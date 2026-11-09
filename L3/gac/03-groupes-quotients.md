---
aliases:
  - "III – Groupes quotients"
  - "Chapitre quotients"
tags:
  - gac
  - gac/chapitre
---

# Chapitre 03 – III. Groupes quotients

**Matière :** [[L3/gac/README|Groupes, anneaux, corps]]  
**Date du cours :** polycopié *GAC-Chap1-Groupes*, partie III (transparents 55 à 79)  
**Index :** [[index-definitions]]

## 🎯 L'essentiel en 3 lignes
- Les classes $xH$ découpent $G$ en paquets de même taille : c'est le [[lagrange|théorème de Lagrange]].
- $G/H$ est un groupe exactement quand $H$ est [[sous-groupe-distingue|distingué]] ([[groupe-quotient]]).
- Outil n°1 des exercices : $G/\mathrm{Ker} f\simeq\mathrm{Im} f$ ([[premier-theoreme-isomorphisme]]).

## 📝 Notes

### III.1–2 – Relations compatibles et groupe quotient
- Si $\mathcal R$ est [[relation-compatible|compatible]], $G/\mathcal R$ est un groupe, neutre $\bar1$, inverse $\overline{x^{-1}}$, et $p$ est un morphisme surjectif.

### III.3 – Classes modulo un sous-groupe
- [[classes-modulo-sous-groupe]] : compatible à gauche ⟺ $x^{-1}y\in H$, classes $xH$ ; à droite ⟺ $yx^{-1}\in H$, classes $Hx$.
- Compatible ⟺ $H\lhd G$ : [[congruence-modulo-sous-groupe]] ; théorème : [[relations-compatibles-groupe]].

### III.4 – Sous-groupes distingués, application aux groupes finis
- [[sous-groupe-distingue]] : il suffit de montrer $x^{-1}Hx\subset H$.
- [[indice]] $[G:H]$ ; [[lagrange]] et corollaire $x^{[G]}=1$ ; [[indice-2-distingue]].

### III.5 – Groupe quotient
- Cas abélien ($\bar x\dot+\bar y=\overline{x+y}$) et cas général ($(xH)(yH)=xyH$) → [[groupe-quotient]].
- Exemples : $\mathbb Z/n\mathbb Z$, $\mathbb R/2\pi\mathbb Z$.

### III.6 – Décomposition canonique d'un morphisme
- Lemme : $\bar x=\bar y\iff f(x)=f(y)$ ; [[application-induite]] $\bar f$ ; [[premier-theoreme-isomorphisme]] ; $f=i\circ\bar f\circ p$.
- Application : [[structure-groupes-monogenes]].
- Exercices types : [[lemme-chinois]], [[groupe-ordre-premier]], $\mathbb R^*/\{\pm1\}\simeq\mathbb R_+^*$, $\mathbb R/\mathbb Z\simeq\mathbb U$ → [[identifier-quotient]], [[morphisme-sur-quotient]].

## 🔑 Définitions / formules à retenir
| Terme | Définition |
|---|---|
| [[classes-modulo-sous-groupe]] | $xH=\{xh\}$, $Hx=\{hx\}$, $G/H$ |
| [[congruence-modulo-sous-groupe]] | $x\equiv y\ (H)\iff x^{-1}y\in H$, $H\lhd G$ |
| [[indice]] | $[G:H]=[G]/[H]$ |
| [[groupe-quotient]] | $(xH)(yH)=(xy)H$ |
| [[application-induite]] | $\bar f(\bar x)=f(x)$ |
| [[lagrange]] | $[H]\mid[G]$ |
| [[premier-theoreme-isomorphisme]] | $G/\mathrm{Ker} f\simeq\mathrm{Im} f$ |

## ❓ Ce que je n'ai pas compris
- 

## 🧠 Questions de révision
1. Énoncer et démontrer le théorème de Lagrange.
2. Montrer qu'un sous-groupe d'indice 2 est distingué.
3. Énoncer et démontrer le premier théorème d'isomorphisme.
4. $f:\mathbb Z/18\mathbb Z\to\mathbb Z/6\mathbb Z$, $x+18\mathbb Z\mapsto x+6\mathbb Z$ : bien définie ? morphisme ? noyau, image ? En déduire $(\mathbb Z/18\mathbb Z)/(6\mathbb Z/18\mathbb Z)\simeq\mathbb Z/6\mathbb Z$.
5. Identifier $\mathbb R/\mathbb Z$ et $\mathbb R^*/\{\pm1\}$.

## 🔗 Pour aller plus loin
- Précédent : [[02-sous-groupes]]
- Sujets d'entraînement : contrôle de seconde session 2025 (ex. 1, 3, 4), examen blanc n°1 (à faire en conditions réelles)
- Sources : polycopié `GAC-Chap1-Groupes` (partie III), cours rédigé → dossier [fichiers](fichiers/)
