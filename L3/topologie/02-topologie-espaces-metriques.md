---
aliases:
  - "2 – Topologie des espaces métriques"
  - "Topologie des espaces métriques"
  - "Chapitre 2 topologie"
tags:
  - topologie
  - topo/chapitre
---

# Chapitre 02 – Topologie des espaces métriques

**Matière :** [[L3/topologie/README|Topologie]]  
**Source :** cours rédigé, chapitre 2 (§ 2.1 à 2.18) ; polycopié chapitre 2 (Déf. 2.1 à 2.16, exercices 2.1 à 2.20)  
**Index :** [[topo-index-definitions]]

## 🎯 L'essentiel en 3 lignes
- [[topo-ouvert|Ouvert]] : une boule autour de chaque point reste dedans ; [[topo-ferme|fermé]] : complémentaire ouvert $\iff$ stable par passage à la limite ([[topo-caracterisation-sequentielle-fermes|suites]]).
- [[topo-interieur|Intérieur]] = plus grand ouvert dedans, [[topo-adherence|adhérence]] = plus petit fermé autour, [[topo-frontiere|frontière]] = la différence ; tout se calcule avec des **suites**.
- $f$ [[topo-continuite|continue]] $\iff$ $f^{-1}(\text{ouvert})$ ouvert $\iff$ $f(x_n)\to f(a)$ dès que $x_n\to a$ ; c'est l'outil n°1 pour montrer qu'un ensemble est ouvert ou fermé ([[topo-continuite-globale]]).

## 📝 Notes

### 2.1 – Ouverts et fermés
- [[topo-ouvert]] (Déf. 2.1), [[topo-ferme]] (Déf. 2.2) ; $[0,1[$ n'est ni l'un ni l'autre (Rem. 2.4).
- [[topo-boule-ouverte-ouverte]] (Prop. 2.5), [[topo-boule-fermee-fermee]] (Prop. 2.6) — **questions de cours**.
- [[topo-stabilite-ouverts]] (Th. 2.7), [[topo-ouverts-reunions-de-boules]] (Prop. 2.9), [[topo-stabilite-fermes]] (Th. 2.10), [[topo-exemples-fermes]] (Prop. 2.11).
- [[topo-caracterisation-sequentielle-fermes]] (Th. 2.12).
- Méthodes : [[topo-montrer-ouvert-ferme]], [[topo-montrer-pas-ouvert-pas-ferme]].

### 2.2 – Voisinages
- [[topo-voisinage]] (Déf. 2.14), [[topo-voisinages-et-boules]] (Prop. 2.15, 2.16, Th. 2.17).

### 2.3 à 2.5 – Intérieur, adhérence, frontière
- [[topo-interieur]] (Déf. 2.18), [[topo-caracterisation-interieur]] (Prop. 2.19, 2.20).
- [[topo-adherence]] (Déf. 2.22), [[topo-caracterisation-adherence]] (Prop. 2.23, 2.24), [[topo-complementaire-interieur-adherence]] (Prop. 2.25), [[topo-partie-dense]] (Déf. 2.26).
- [[topo-frontiere]] (Déf. 2.28), [[topo-proprietes-frontiere]] (Prop. 2.29).
- Méthode : [[topo-calculer-interieur-adherence-frontiere]].
- Complément TD : [[topo-distance-a-une-partie]] (exercice 2.13).

### 2.6 – Applications continues
- [[topo-continuite]] (Déf. 2.31), [[topo-caracterisations-continuite-point]] (Th. 2.33), [[topo-continuite-globale]] (Th. 2.34), [[topo-composition-continues]] (Th. 2.35), [[topo-operations-fonctions-continues]] (Prop. 2.36).
- Méthode : [[topo-continuite-deux-variables]].

### 2.7 – Uniforme continuité, lipschitziennes
- [[topo-continuite-uniforme]] (Déf. 2.38), [[topo-application-lipschitzienne]] (Déf. 2.42), [[topo-hierarchie-lipschitz-uc-continue]] (Prop. 2.39, 2.43), [[topo-isometrie]] (Déf. 2.45), [[topo-isometries]] (Prop. 2.46).
- Méthode : [[topo-uniforme-continuite]].

### 2.8 – Continuité dans les produits
- [[topo-continuite-composantes]] (Prop. 2.47, Th. 2.48, Prop. 2.50, Ex. 2.51).

### 2.9 – Homéomorphismes
- [[topo-homeomorphisme]] (Déf. 2.52), [[topo-bijections-continues-de-r]] (Ex. 2.53, Prop. 2.54, Ex. 2.55).

### 2.10 à 2.12 – Distances et normes équivalentes
- [[topo-distances-topologiquement-equivalentes]] (Déf. 2.57), [[topo-critere-des-boules]] (Prop. 2.59).
- [[topo-distances-metriquement-equivalentes]] (Déf. 2.60), [[topo-metriquement-implique-topologiquement]] (Prop. 2.61, Ex. 2.62).
- [[topo-normes-equivalentes]] (Déf. 2.64), [[topo-normes-equivalentes-encadrement]] (Prop. 2.65), [[topo-equivalence-normes-dimension-finie]] (Th. 2.67).
- Méthodes : [[topo-comparer-distances]], [[topo-montrer-normes-equivalentes]].

### 2.13 et 2.14 – Applications linéaires continues
- [[topo-applications-lineaires-continues]] (Th. 2.69), [[topo-norme-operateur]] (Déf. 2.71), [[topo-proprietes-norme-operateur]] (Prop. 2.72).
- Méthode : [[topo-application-lineaire-norme-operateur]].

## 🔑 Définitions / formules à retenir
| Notion | À retenir |
|---|---|
| [[topo-ouvert\|Ouvert]] | $\forall x\in A,\ \exists r>0,\ B(x,r)\subset A$ ; réunion quelconque, intersection **finie** |
| [[topo-ferme\|Fermé]] | $A^c$ ouvert $\iff$ toute suite de $A$ convergente a sa limite dans $A$ ; intersection quelconque, réunion **finie** |
| [[topo-interieur\|Intérieur]] | plus grand ouvert $\subset A$ ; $x\in\operatorname{Int}A\iff\exists r,\ B(x,r)\subset A$ |
| [[topo-adherence\|Adhérence]] | plus petit fermé $\supset A$ ; $x\in\bar A\iff\forall r,\ B(x,r)\cap A\ne\emptyset\iff\exists(x_n)\in A^{\mathbb N},\ x_n\to x$ |
| [[topo-complementaire-interieur-adherence\|Complémentaire]] | $(\bar A)^c=\operatorname{Int}(A^c)$ ; $(\operatorname{Int}A)^c=\overline{A^c}$ |
| [[topo-frontiere\|Frontière]] | $\operatorname{Fr}A=\bar A\setminus\operatorname{Int}A=\bar A\cap\overline{A^c}$ |
| [[topo-continuite-globale\|Continuité]] | $f^{-1}(\text{ouvert})$ ouvert $\iff f^{-1}(\text{fermé})$ fermé $\iff$ ($x_n\to a\Rightarrow f(x_n)\to f(a)$) |
| [[topo-hierarchie-lipschitz-uc-continue\|Hiérarchie]] | lipschitzienne ⟹ U.C. ⟹ continue |
| [[topo-distances-metriquement-equivalentes\|Distances]] | $\alpha d_1\le d_2\le\beta d_1$ ⟹ mêmes ouverts |
| [[topo-normes-equivalentes\|Normes]] | équivalentes $\iff\alpha N_1\le N_2\le\beta N_1$ ; toujours en dimension finie |
| [[topo-norme-operateur\|Norme d'opérateur]] | $\lVert f(u)\rVert\le\lvert\lvert\lvert f\rvert\rvert\rvert\,\lVert u\rVert$ |

## ❓ Ce que je n'ai pas compris
- 

## 🧠 Questions de révision
1. Démontrer qu'une boule ouverte est ouverte et qu'une boule fermée est fermée (deux méthodes).
2. Énoncer et démontrer la caractérisation séquentielle des fermés.
3. Montrer : $\overline{A\cup B}=\bar A\cup\bar B$, $\overline{A\cap B}\subset\bar A\cap\bar B$ (exemple strict), $\operatorname{Int}(A\cap B)=\operatorname{Int}A\cap\operatorname{Int}B$.
4. $f,g$ continues : nature de $\{f=g\}$, $\{f\neq g\}$, $\{f\le g\}$, $\{f<g\}$.
5. Étudier $]0,1]\cup\{2\}$, $\mathbb Z$, $\mathbb Q$, $\{\frac1n\}$ : ouvert ? fermé ? adhérence, intérieur, frontière.
6. Montrer que $V$ est un voisinage de $a$ ssi $V$ contient une boule $B(a,r)$.
7. $\frac{xy}{x^2+y^2}$ est-elle continue en $(0,0)$ ? Ses applications partielles ?
8. Montrer que $x^2$ n'est pas uniformément continue sur $\mathbb R$.
9. Montrer que deux distances métriquement équivalentes ont les mêmes fermés.

## 🔗 Pour aller plus loin
- Corrigés rédigés : [[topo-exercices-types-corriges#1. Une boule fermée est fermée|ex. 1]], [[topo-exercices-types-corriges#4. Les ensembles {f = g} et {f ≠ g}|ex. 4]], [[topo-exercices-types-corriges#5. Une partie de R – ouvert, fermé, adhérence, intérieur|ex. 5]], [[topo-exercices-types-corriges#14. Adhérence et intérieur d'une intersection, d'une réunion (écrit 2025-26)|ex. 14]]
- Pièges personnels : [[topo-mes-erreurs]] · Vrai/Faux : [[topo-vrai-faux-classiques]]
- Précédent : [[01-espaces-metriques]] · Suivant : [[03-espaces-metriques-compacts]]
- Sources : [cours rédigé ch. 1 à 3](fichiers/topo-cours-redige-ch1-3.pdf), [polycopié chapitre 2](fichiers/topo-chap2-polycopie.pdf)
