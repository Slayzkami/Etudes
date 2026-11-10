---
aliases:
  - "Méthode : calculer une norme d'opérateur"
  - "calculer |||f|||"
  - "majorer puis atteindre"
  - "norme triple d'une matrice"
tags:
  - cd
  - cd/methode
  - cd/chapitre-01
---

# 🛠️ Méthode : calculer une norme d'opérateur

*Méthode* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Méthode 1.5 du cours · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette : majorer, puis atteindre
> Pour montrer $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert=C$ :
> 1. **Majorer** : établir $\lVert f(u)\rVert\le C\lVert u\rVert$ pour **tout** $u$. Donc $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert\le C$ (Prop. 1.50 (ii)).
> 2. **Atteindre** : trouver $u_0\ne0$ avec $\lVert f(u_0)\rVert=C\lVert u_0\rVert$ (ou une suite $u_n$ avec $\frac{\lVert f(u_n)\rVert}{\lVert u_n\rVert}\to C$). Donc $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert\ge C$ (Prop. 1.50 (i)).
> 3. **Conclure** : $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert=C$.

> [!TIP] Pour une matrice $A$ ($u\mapsto Au$)
> - $\lVert \cdot\rVert_\infty$ au départ et à l'arrivée : $\lvert\!\lvert\!\lvert A\rvert\!\rvert\!\rvert=$ **plus grosse ligne** ($\max_i\sum_j\lvert a_{ij}\rvert$). Vecteur qui atteint : les signes $\pm1$ des coefficients de cette ligne.
> - $\lVert \cdot\rVert_1$ au départ et à l'arrivée : $\lvert\!\lvert\!\lvert A\rvert\!\rvert\!\rvert=$ **plus grosse colonne** ($\max_j\sum_i\lvert a_{ij}\rvert$). Vecteur qui atteint : le vecteur de base $e_j$ de cette colonne.

> [!EXAMPLE] Rédaction modèle
> $L:(\mathbb R^2,\lVert \cdot\rVert_\infty)\to(\mathbb R,\abs\cdot)$, $L(x,y)=2x-3y$.
> **Majoration.** $\lvert L(x,y)\rvert\le2\abs x+3\abs y\le5\max(\abs x,\abs y)=5\lVert (x,y)\rVert_\infty$, donc $\lvert\!\lvert\!\lvert L\rvert\!\rvert\!\rvert\le5$.
> **Atteinte.** $u_0=(1,-1)$ : $\lVert u_0\rVert_\infty=1$ et $\lvert L(u_0)\rvert=5$, donc $\lvert\!\lvert\!\lvert L\rvert\!\rvert\!\rvert\ge5$.
> **Conclusion.** $\lvert\!\lvert\!\lvert L\rvert\!\rvert\!\rvert=5$.
> Avec $\lVert \cdot\rVert_1$ au départ : $\lvert L(x,y)\rvert\le3(\abs x+\abs y)$ et $u_0=(0,1)$ donne $3$ : $\lvert\!\lvert\!\lvert L\rvert\!\rvert\!\rvert=3$.

> [!WARNING] Pièges (mes erreurs)
> - S'arrêter à la majoration : on a seulement $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert\le C$.
> - Oublier de vérifier que $\lVert u_0\rVert$ vaut bien $1$ (ou diviser par $\lVert u_0\rVert$).
> - La valeur dépend des normes choisies.

## 🔗 Liens

- **Voir aussi** : [[norme-operateur|Norme d'opérateur]], [[caracterisations-norme-operateur|Caractérisations de la norme d'opérateur]]
