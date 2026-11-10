---
aliases:
  - "Matrice jacobienne"
  - "jacobienne"
  - "J_f(a)"
  - "jacobien"
tags:
  - cd
  - cd/definition
  - cd/chapitre-02
---

# 📘 Matrice jacobienne

*Définition* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Déf. 2.36 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> Si $f=(f_1,\dots,f_p):U\subset\mathbb R^n\to\mathbb R^p$ est différentiable en $a$, la **matrice jacobienne** de $f$ en $a$ est la matrice à $p$ lignes et $n$ colonnes
> $$J_f(a)=\Big(\frac{\partial f_i}{\partial x_j}(a)\Big)_{\substack{1\le i\le p\\1\le j\le n}}.$$
> C'est la matrice de $Df_a$ dans les bases canoniques : $Df_a(h)=J_f(a)\,h$.

> [!TIP] Lire une jacobienne
> **Ligne $i$ = composante $f_i$. Colonne $j$ = variable $x_j$.** Autant de lignes que de composantes à l'arrivée, autant de colonnes que de variables au départ.

> [!EXAMPLE] Exemple (Ex. 2.38, coordonnées polaires)
> $P(\rho,\theta)=(\rho\cos\theta,\rho\sin\theta)$ : $J_P(\rho,\theta)=\begin{pmatrix}\cos\theta&-\rho\sin\theta\\ \sin\theta&\rho\cos\theta\end{pmatrix}$, $\det J_P=\rho$.

> [!WARNING] Pièges (mes erreurs)
> - Ne pas **transposer** : les dérivées d'une même composante sont sur une même **ligne**.
> - Écrire la jacobienne ne prouve pas la différentiabilité : il faut l'avoir justifiée avant → [[calculer-jacobienne]].

## 🔗 Liens

- **S'appuie sur** : [[derivee-partielle|Dérivée partielle]], [[differentiabilite|Différentiabilité en un point, différentielle]]
- **Utilisé par (définitions)** : [[gradient|Gradient]]
- **Utilisé par (théorèmes)** : [[differentiabilite-par-composantes|Différentiabilité par composantes]], [[inversion-locale|Théorème d'inversion locale]], [[fonctions-implicites|Théorème des fonctions implicites (cas général)]]
- **Méthodes** : [[calculer-jacobienne|Calculer une jacobienne et une différentielle sur R^n]], [[calculer-derivee-directionnelle|Calculer une dérivée directionnelle]], [[montrer-diffeomorphisme|Montrer qu'une application est un difféomorphisme (local ou global)]]
