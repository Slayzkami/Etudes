---
aliases:
  - "Méthode : calculer une jacobienne et une différentielle sur R^n"
  - "écrire la jacobienne"
  - "Df_a(h) = J_f(a) h"
tags:
  - cd
  - cd/methode
  - cd/chapitre-02
---

# 🛠️ Méthode : calculer une jacobienne et une différentielle sur R^n

*Méthode* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Méthode 2.4 du cours · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> 1. **Justifier la différentiabilité** (composantes $\mathcal C^1$).
> 2. **Écrire la matrice des expressions** : ligne $i$ = composante $f_i$, colonne $j$ = variable $x_j$.
> 3. **Calculer chaque dérivée partielle** (les autres variables sont des constantes).
> 4. **Différentielle** : $Df_a(h)=J_f(a)\,h$ (produit matrice-vecteur colonne).

> [!EXAMPLE] Rédaction modèle (Écrit 2022-2023, ex. 1)
> $f(x_1,x_2,x_3)=(x_1^2+x_2^2+5x_3,\ 3x_1x_2x_3+2,\ x_1^3+x_2^3+x_3)$. Les composantes sont polynomiales donc $\mathcal C^1$ : $f$ est différentiable sur $\mathbb R^3$ et
> $$J_f(x)=\begin{pmatrix}2x_1&2x_2&5\\3x_2x_3&3x_1x_3&3x_1x_2\\3x_1^2&3x_2^2&1\end{pmatrix},\quad Df_x(h)=\begin{pmatrix}2x_1h_1+2x_2h_2+5h_3\\3x_2x_3h_1+3x_1x_3h_2+3x_1x_2h_3\\3x_1^2h_1+3x_2^2h_2+h_3\end{pmatrix}.$$

> [!WARNING] Pièges (mes erreurs)
> - Jacobienne **transposée** : vérifier la taille ($p$ lignes, $n$ colonnes) et que la première ligne ne contient que des dérivées de $f_1$.
> - $e^0=1$, $\cos0=1$, $\sin0=0$, $\ln1=0$ : relire les valeurs numériques.

## 🔗 Liens

- **Voir aussi** : [[matrice-jacobienne|Matrice jacobienne]], [[differentiabilite-par-composantes|Différentiabilité par composantes]], [[critere-c1|Critère C1 par les dérivées partielles]], [[gradient|Gradient]]
