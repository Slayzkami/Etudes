---
aliases:
  - "3 – Espaces métriques compacts"
  - "Espaces métriques compacts"
  - "Chapitre 3 topologie"
tags:
  - topologie
  - topo/chapitre
---

# Chapitre 03 – Espaces métriques compacts

**Matière :** [[L3/topologie/README|Topologie]]  
**Source :** cours rédigé, chapitre 3 (§ 3.1 à 3.9) ; polycopié chapitre 3 (Déf. 3.1 à 3.3, Th. 3.1 à 3.4)  
**Index :** [[topo-index-definitions]]

## 🎯 L'essentiel en 3 lignes
- [[topo-espace-compact|Compact]] : tout recouvrement ouvert a un sous-recouvrement fini $\iff$ toute suite a une sous-suite qui converge **dans** l'espace ([[topo-bolzano-weierstrass|Bolzano–Weierstrass]]).
- Une partie compacte est fermée et bornée ; dans $\mathbb R^n$ c'est une équivalence ([[topo-borel-lebesgue|Borel–Lebesgue]]) ; faux en dimension infinie ([[topo-riesz|Riesz]]).
- Sur un compact, une fonction continue est bornée et [[topo-bornes-atteintes|atteint ses bornes]], et elle est [[topo-heine|uniformément continue]].

## 📝 Notes

### 3.1 – Recouvrements
- [[topo-recouvrement]] (Déf. 3.1).

### 3.2 – Espaces compacts
- [[topo-espace-compact]] (Déf. 3.3), [[topo-version-fermes-compacite]] (Prop. 3.5, 3.6), [[topo-partie-compacte]] (Déf. 3.8, Prop. 3.9).
- Une suite et sa limite forment un compact (Ex. 3.10).
- [[topo-bolzano-weierstrass]] (Th. 3.11, Lemme 3.12), [[topo-bolzano-weierstrass-dans-r]] (Th. 3.13).

### 3.3 – Propriétés des compacts
- [[topo-suite-de-cauchy-espace-complet]] (Déf. 3.15), [[topo-convergente-cauchy]] (Prop. 3.16, Lemme 3.17).
- [[topo-compact-complet-borne]] (Prop. 3.18, 3.19, Rem. 3.20), [[topo-ferme-dans-compact]] (Prop. 3.21).
- [[topo-borel-lebesgue]] (Th. 3.22, Cor. 3.25), [[topo-reunions-intersections-compacts]] (Prop. 3.23), [[topo-produit-de-compacts]] (Prop. 3.24).

### 3.4 – Compacité et continuité
- [[topo-image-continue-compact]] (Prop. 3.27, 3.28), [[topo-bornes-atteintes]] (Th. 3.30), [[topo-heine]] (Th. 3.32).

### 3.5 – Normes en dimension finie
- [[topo-equivalence-normes-dimension-finie]] (Th. 3.34, Cor. 3.35), [[topo-riesz]] (Th. 3.36).

### Méthodes
- [[topo-montrer-compact]], [[topo-montrer-non-compact]], [[topo-exploiter-compacite]], [[topo-somme-a-plus-b]].

## 🔑 Définitions / formules à retenir
| Notion | À retenir |
|---|---|
| [[topo-espace-compact\|Compact]] | tout recouvrement ouvert a un sous-recouvrement fini $\iff$ toute suite a une sous-suite convergente dans l'espace |
| [[topo-compact-complet-borne\|Propriétés]] | compact ⟹ complet et borné ; partie compacte ⟹ fermée et bornée |
| [[topo-borel-lebesgue\|$\mathbb R$, $\mathbb R^n$]] | compact $\iff$ fermé et borné |
| [[topo-ferme-dans-compact\|Stabilité]] | fermé dans un compact ; réunion finie ; intersection ; produit fini ; image continue |
| [[topo-bornes-atteintes\|Bornes atteintes]] | $f:K\to\mathbb R$ continue ⟹ $\exists x_1,x_2,\ f(x_1)=\min f,\ f(x_2)=\max f$ |
| [[topo-heine\|Heine]] | continue sur un compact ⟹ U.C. |
| [[topo-riesz\|Riesz]] | $\bar B(0,1)$ compacte $\iff\dim E<\infty$ |

## ❓ Ce que je n'ai pas compris
- 

## 🧠 Questions de révision
1. Énoncer la définition d'un compact (recouvrements) et la caractérisation séquentielle.
2. Montrer qu'une partie compacte est fermée et bornée (par les suites).
3. Montrer que $\{0\}\cup\{\frac1n\}$ est compact, que $]0,1]$, $\mathbb R$, $\mathbb Z$ ne le sont pas.
4. $A$ compact, $B$ fermé : $A+B$ fermé ; $A$, $B$ compacts : $A+B$ compact ; contre-exemple avec deux fermés.
5. Montrer que $\{x^2+y^4\le1\}$ est compact et que $x+y$ y atteint un maximum.
6. Démontrer le théorème de Heine ; appliquer à $x^2$ sur $[-a,a]$.

## 🔗 Pour aller plus loin
- Corrigés rédigés : [[topo-exercices-types-corriges#3. La somme A + B|ex. 3]], [[topo-exercices-types-corriges#13. Un compact de R (interro 2025-26)|ex. 13]], [[topo-exercices-types-corriges#19. Compact de R² et maximum|ex. 19]]
- Pièges personnels : [[topo-mes-erreurs]] · Vrai/Faux : [[topo-vrai-faux-classiques]]
- Précédent : [[02-topologie-espaces-metriques]]
- Sources : [cours rédigé ch. 1 à 3](fichiers/topo-cours-redige-ch1-3.pdf)
