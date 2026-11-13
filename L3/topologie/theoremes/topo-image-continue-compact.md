---
aliases:
  - "Image continue d'un compact ; bijection continue sur un compact"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-03
---

# ⭐ Image continue d'un compact ; bijection continue sur un compact

*Théorème* · Chapitre : [[03-espaces-metriques-compacts|3 – Espaces métriques compacts]] · Prop. 3.27 et 3.28 du cours (poly : Prop. 3.5, 3.6) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> 1. Si $f:E\to F$ est continue et $A$ est une partie compacte de $E$, alors $f(A)$ est compacte.
> 2. Si $E$ est compact et $f:E\to F$ est continue et bijective, $f$ est un **homéomorphisme**.

> [!SUCCESS]- Démonstration
> 1. $y_n=f(x_n)$, $x_n\in A$ ; $x_{\varphi(n)}\to\ell\in A$, donc $y_{\varphi(n)}=f(x_{\varphi(n)})\to f(\ell)\in f(A)$.
> 2. Pour $A$ fermé de $E$ : $(f^{-1})^{-1}(A)=f(A)$ est compact (car $A$ compact), donc fermé.

> [!EXAMPLE] Exemple
> $A,B$ compacts de $\mathbb R^n$ $\Rightarrow A+B=s(A\times B)$ compact avec $s(x,y)=x+y$ (interro 2025-26).

> [!WARNING] Pièges
> L'**image réciproque** d'un compact n'est pas compacte : $\sin^{-1}([-1,1])=\mathbb R$ (Piège 3.4).

## 🔗 Liens

- **S'appuie sur** : [[topo-partie-compacte|Partie compacte]], [[topo-continuite|Continuité en un point]], [[topo-bolzano-weierstrass|Caractérisation séquentielle des compacts (Bolzano–Weierstrass)]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-bornes-atteintes|Une fonction continue sur un compact est bornée et atteint ses bornes]]
- **Méthodes** : [[topo-montrer-compact|Méthode : montrer qu'une partie est compacte]], [[topo-somme-a-plus-b|Méthode : la somme A + B]]
- **Voir aussi** : —
