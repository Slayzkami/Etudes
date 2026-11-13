---
aliases:
  - "Méthode : montrer qu'une partie est compacte"
  - "prouver compact"
  - "fermé et borné"
tags:
  - topologie
  - topo/methode
  - topo/chapitre-03
---

# 🛠️ Méthode : montrer qu'une partie est compacte

*Méthode* · Chapitre : [[03-espaces-metriques-compacts|3 – Espaces métriques compacts]] · Méthode 3.1 du cours · [[topo-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> Par ordre de rapidité :
> 1. **En dimension finie ($\mathbb R$, $\mathbb R^n$)** : **fermée** (image réciproque, suites, complémentaire) **et bornée** ($\|x\|\le M$).
> 2. **Image continue d'un compact** : $K=f(K_0)$.
> 3. **Fermé dans un compact**, réunion **finie**, intersection, **produit** de compacts.
> 4. **Par les suites** (espace général) : soit $(x_n)$ une suite de $K$ ; extraire une sous-suite convergente **dans $K$**.
> 5. **Par les recouvrements** : utile pour « suite + limite » (Ex. 3.10).

> [!EXAMPLE] Rédaction modèle (comme sur la copie)
> *$X=\{\frac1n\mid n\in\mathbb N^*\}\cup\{0\}$ (interro 2025-26).*
> « **Borné** : $X\subset[0,1]$. **Fermé** : $\mathbb R\setminus X=]-\infty,0[\cup]1,+\infty[\cup\bigcup_{n\ge1}]\frac1{n+1},\frac1n[$ est une réunion d'ouverts (un réel de $]0,1[$ qui n'est pas un $\frac1n$ est strictement entre deux termes consécutifs). Fermé et borné dans $\mathbb R$ : $X$ est compact (Borel–Lebesgue). »
>
> *$K=\{x^2+y^4\le1\}$ et $\max_K(x+y)$.* « $K=\varphi^{-1}([0,1])$ avec $\varphi(x,y)=x^2+y^4$ continue : fermé ; $|x|\le1$, $|y|\le1$ : borné. Donc $K$ est compact, et $(x,y)\mapsto x+y$, continue, y atteint son maximum. »

> [!WARNING] Pièges
> - « Fermé borné » **seulement** en dimension finie.
> - « Réunion de fermés » infinie : pas un argument (mon erreur).
> - Ne pas oublier de dire **pourquoi c'est borné** (même si c'est une ligne).

## 🔗 Liens

- **S'appuie sur** : [[topo-borel-lebesgue|Borel–Lebesgue : compacts de R et de R^n]], [[topo-image-continue-compact|Image continue d'un compact ; bijection continue sur un compact]], [[topo-ferme-dans-compact|Un fermé dans un compact est compact]], [[topo-produit-de-compacts|Produit de compacts]], [[topo-bolzano-weierstrass|Caractérisation séquentielle des compacts (Bolzano–Weierstrass)]]
- **Méthodes voisines** : —
- **Corrigés** : [[topo-exercices-types-corriges#13. Un compact de R (interro 2025-26)|ex. 13]]
- **Voir aussi** : —
