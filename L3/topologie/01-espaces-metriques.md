---
aliases:
  - "1 – Espaces métriques, e.v.n."
  - "Espaces métriques, espaces vectoriels normés"
  - "Chapitre 1 topologie"
tags:
  - topologie
  - topo/chapitre
---

# Chapitre 01 – Espaces métriques, espaces vectoriels normés

**Matière :** [[L3/topologie/README|Topologie]]  
**Source :** cours rédigé, chapitre 1 (§ 1.1 à 1.11) ; polycopié chapitre 1 (Déf. 1.1 à 1.10, exercices 1.1 à 1.16)  
**Index :** [[topo-index-definitions]]

## 🎯 L'essentiel en 3 lignes
- Une [[topo-distance|distance]] vérifie séparation, symétrie, inégalité triangulaire ; une [[topo-norme|norme]] donne la distance $d(x,y)=N(x-y)$.
- Avec une distance on définit les [[topo-boules-spheres|boules]], les [[topo-partie-bornee-diametre|parties bornées]] et la [[topo-suite-convergente|convergence]] : $x_n\to\ell\iff d(x_n,\ell)\to0$.
- Une partie d'un espace métrique est un espace métrique ([[topo-distance-induite|distance induite]]) ; un produit aussi ([[topo-distance-produit|distance max]]).

## 📝 Notes

### 1.1 – Espaces métriques
- [[topo-distance]] (Déf. 1.1) ; exemples : $|x-y|$, $d_1,d_2,d_\infty$, [[topo-distance-discrete|distance discrète]].
- [[topo-inegalite-triangulaire-generalisee]] (Prop. 1.3), [[topo-seconde-inegalite-triangulaire]] (Prop. 1.4).
- Méthode : [[topo-montrer-distance]].

### 1.2 – Espaces vectoriels normés
- [[topo-norme]] (Déf. 1.5), [[topo-distance-associee-norme]] (Déf. 1.7), [[topo-distance-et-norme]] (Prop. 1.8 : la distance discrète ne vient d'aucune norme).
- [[topo-normes-usuelles]] de $\mathbb K^n$ et de $C([a,b])$ (Ex. 1.10, 1.11) ; Cauchy–Schwarz (Lemme 1.9).
- Méthode : [[topo-montrer-norme]].

### 1.3 – Boules et sphères
- [[topo-boules-spheres]] (Déf. 1.13), [[topo-proprietes-boules]] (Prop. 1.14) ; boules unité de $\mathbb R^2$ : losange, disque, carré (Ex. 1.15).
- Méthode : [[topo-determiner-boule]].

### 1.4 – Parties bornées
- [[topo-partie-bornee-diametre]] (Déf. 1.16), [[topo-proprietes-parties-bornees]] (Prop. 1.17).

### 1.5 – Sous-espaces métriques
- [[topo-distance-induite]] (Déf. 1.19), [[topo-boules-sous-espace]] (Prop. 1.20).

### 1.6 – Produit d'espaces métriques
- [[topo-distance-produit]] (Prop. 1.22), [[topo-boules-produit]] (Prop. 1.23).

### 1.7 – Convergence
- [[topo-suite-convergente]] (Déf. 1.24), [[topo-unicite-limite]] (Prop. 1.25), [[topo-suite-extraite]] (Déf. 1.26), [[topo-suites-extraites-convergentes]] (Prop. 1.28), [[topo-suite-bornee]] (Déf. 1.30), [[topo-convergente-bornee]] (Prop. 1.31), [[topo-convergence-produit]] (Prop. 1.32), [[topo-convergence-evn]] (Prop. 1.33).
- Méthode : [[topo-etudier-convergence-suite]].

## 🔑 Définitions / formules à retenir
| Notion | À retenir |
|---|---|
| [[topo-distance\|Distance]] | $d\ge0$ ; $d(x,y)=0\iff x=y$ ; $d(x,y)=d(y,x)$ ; $d(x,y)\le d(x,z)+d(z,y)$ |
| [[topo-seconde-inegalite-triangulaire\|2ᵉ inégalité triangulaire]] | $\lvert d(x,z)-d(z,y)\rvert\le d(x,y)$ ; $\lvert N(x)-N(y)\rvert\le N(x-y)$ |
| [[topo-norme\|Norme]] | $N(x)=0\iff x=0$ ; $N(\lambda x)=\lvert\lambda\rvert N(x)$ ; $N(x+y)\le N(x)+N(y)$ |
| [[topo-normes-usuelles\|Normes de $\mathbb K^n$]] | $\lVert x\rVert_\infty\le\lVert x\rVert_2\le\lVert x\rVert_1\le n\lVert x\rVert_\infty$ |
| [[topo-boules-spheres\|Boules]] | $B(a,r)=\{d(a,x)<r\}$, $\bar B(a,r)=\{d(a,x)\le r\}$, $S(a,r)=\{d(a,x)=r\}$ |
| [[topo-partie-bornee-diametre\|Borné]] | contenue dans une boule ; $\operatorname{diam}B(a,r)\le2r$ |
| [[topo-distance-induite\|Sous-espace]] | $B_F(a,r)=B_E(a,r)\cap F$ |
| [[topo-distance-produit\|Produit]] | $d=\max_id_i$ ; $d\le d''\le d'\le nd$ |
| [[topo-suite-convergente\|Convergence]] | $x_n\to\ell\iff d(x_n,\ell)\to0$ ; limite unique ; sous-suites même limite ; convergente ⟹ bornée |

## ❓ Ce que je n'ai pas compris
- 

## 🧠 Questions de révision
1. Montrer que $\min(1,d)$ et $\frac{d}{1+d}$ sont des distances. Pourquoi $(x-y)^3$ n'en est pas une ?
2. Déterminer les boules de la distance discrète ; montrer qu'elle ne vient d'aucune norme.
3. Dessiner les boules unité de $\|\cdot\|_1,\|\cdot\|_2,\|\cdot\|_\infty$ et de $\max(|x+y|,|x-2y|)$.
4. Démontrer : une suite convergente est bornée ; la limite est unique.
5. Donner une suite telle que $\|x_n\|\to\|\ell\|$ sans que $x_n\to\ell$.

## 🔗 Pour aller plus loin
- Corrigés rédigés : [[topo-exercices-types-corriges#20. Une norme sur R² et sa boule unité|ex. 20]], [[topo-exercices-types-corriges#9. Interro 2025-26 – la distance min(1, d)|ex. 9]]
- Pièges personnels : [[topo-mes-erreurs]] · Vrai/Faux : [[topo-vrai-faux-classiques]]
- Suivant : [[02-topologie-espaces-metriques]]
- Sources : [cours rédigé ch. 1 à 3](fichiers/topo-cours-redige-ch1-3.pdf), [polycopié chapitre 1](fichiers/topo-chap1-polycopie.pdf)
