---
aliases:
  - "1 – Espaces vectoriels normés"
  - "Chapitre e.v.n."
  - "CD chapitre 1"
tags:
  - cd
  - cd/chapitre
---

# Chapitre 01 – Espaces vectoriels normés et applications linéaires continues

**Matière :** [[L3/Calcul Différentiel/README|Calcul Différentiel]]  
**Source :** polycopié *CD – Chapitre 1* ; cours rédigé, chapitre 1 (pages 1 à 23)  
**Index :** [[cd-index-definitions]]

## 🎯 L'essentiel en 3 lignes
- Une [[norme]] mesure la taille des vecteurs ; en **dimension finie** toutes les normes sont équivalentes ([[equivalence-normes-dimension-finie]]), en dimension infinie non.
- Une application **linéaire** est continue ssi $\lVert f(u)\rVert\le C\lVert u\rVert$ ([[caracterisation-lineaires-continues|Th. 1.43]]) ; c'est automatique au départ d'une dimension finie ([[lineaire-en-dimension-finie|Th. 1.44]]).
- La [[norme-operateur|norme d'opérateur]] $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert$ est la plus petite constante $C$ : pour la calculer, **majorer puis atteindre** ([[calculer-norme-operateur]]).

## 📝 Notes

### 1.1 à 1.5 – Normes
- [[norme]] : (N1) séparation, (N2) homogénéité, (N3) inégalité triangulaire ; [[seconde-inegalite-triangulaire]].
- Exemples : $\lVert \cdot\rVert_1,\lVert \cdot\rVert_2,\lVert \cdot\rVert_\infty$ sur $\mathbb K^n$ et sur $\mathcal C([a,b])$.
- [[boules-spheres]] ; [[norme-produit]].
- [[normes-equivalentes]] : $\lVert x\rVert_\infty\le\lVert x\rVert_2\le\lVert x\rVert_1\le n\lVert x\rVert_\infty$. Méthodes : [[montrer-norme]], [[montrer-normes-equivalentes]].

### 1.6 à 1.8 – Topologie et continuité
- [[suite-convergente]] ; [[ouvert-ferme]], [[stabilite-ouverts-fermes]], [[caracterisation-sequentielle-fermes]] ; [[voisinage]]. Méthode : [[montrer-ouvert-ferme]].
- [[continuite]], [[continuite-uniforme]], [[application-lipschitzienne]] : lipschitzienne ⟹ uniformément continue ⟹ continue.
- [[continuite-et-composantes]]. Méthode : [[montrer-continue]].

### 1.9 à 1.11 – Applications linéaires et bilinéaires continues
- [[application-lineaire-continue]], [[caracterisation-lineaires-continues]], [[lineaire-en-dimension-finie]]. Méthode : [[continuite-application-lineaire]].
- [[norme-operateur]], [[caracterisations-norme-operateur]], [[norme-composee]]. Méthode : [[calculer-norme-operateur]].
- [[application-bilineaire]], [[caracterisation-bilineaires-continues]] (astuce d'ajout-retrait).

### 1.12 – Espaces de Banach
- [[suite-de-cauchy]], [[espace-de-banach]], [[espaces-de-banach-usuels]].

## 🔑 Définitions / formules à retenir
| Terme | Formule |
|---|---|
| [[norme]] | $N(x)=0\iff x=0$ ; $N(\lambda x)=\abs\lambda N(x)$ ; $N(x+y)\le N(x)+N(y)$ |
| [[normes-equivalentes]] | $\alpha N_1\le N_2\le\beta N_1$ |
| [[ouvert-ferme]] | $\forall x\in A,\ \exists r>0,\ B(x,r)\subset A$ |
| [[application-lipschitzienne]] | $\lVert f(x)-f(y)\rVert\le k\lVert x-y\rVert$ |
| [[caracterisation-lineaires-continues]] | $f$ linéaire continue $\iff\exists C,\ \lVert f(u)\rVert\le C\lVert u\rVert$ |
| [[norme-operateur]] | $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert=\sup_{\lVert u\rVert\le1}\lVert f(u)\rVert=\sup_{u\ne0}\frac{\lVert f(u)\rVert}{\lVert u\rVert}$ |
| [[caracterisations-norme-operateur]] | $\lVert f(u)\rVert\le\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert\lVert u\rVert$ |
| [[norme-composee]] | $\lvert\!\lvert\!\lvert g\circ f\rvert\!\rvert\!\rvert\le\lvert\!\lvert\!\lvert g\rvert\!\rvert\!\rvert\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert$ |
| [[application-bilineaire]] | continue $\iff\lVert B(u,v)\rVert\le C\lVert u\rVert\lVert v\rVert$ |

## ❓ Ce que je n'ai pas compris
- 

## 🧠 Questions de révision
1. Donner la définition d'une norme. Montrer que $\big|\lVert x\rVert-\lVert y\rVert\big|\le\lVert x-y\rVert$.
2. Montrer que $\lVert \cdot\rVert_1$ et $\lVert \cdot\rVert_\infty$ ne sont pas équivalentes sur $\mathcal C([0,1])$.
3. Énoncer et démontrer le Théorème 1.43 (les cinq propriétés équivalentes).
4. Donner un exemple d'application linéaire non continue.
5. Donner la définition de la norme d'une application linéaire continue (question de cours des Écrits 2022-2023 et 2025-2026).
6. Calculer $\lvert\!\lvert\!\lvert L\rvert\!\rvert\!\rvert$ pour $L(x,y)=2x-3y$ avec $\lVert \cdot\rVert_\infty$, puis avec $\lVert \cdot\rVert_1$.
7. Citer quatre espaces de dimension finie et deux de dimension infinie.

## 🔗 Pour aller plus loin
- Corrigés rédigés : [[cd-exercices-types-corriges]] (ex. 1, 2, 3) · pièges : [[cd-mes-erreurs]] · [[cd-vrai-faux-classiques]]
- Suivant : [[02-applications-differentiables]]
- TD1 et TD2 → dossier [fichiers](fichiers/)
- Sources : polycopié [chapitre 1](fichiers/cd-chap1-polycopie.pdf), [cours rédigé](fichiers/cd-cours-redige-ch1-5.pdf)
