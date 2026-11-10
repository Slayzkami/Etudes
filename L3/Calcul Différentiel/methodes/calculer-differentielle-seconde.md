---
aliases:
  - "Méthode : calculer une différentielle seconde, une hessienne"
  - "calculer D²f"
  - "calculer la hessienne"
tags:
  - cd
  - cd/methode
  - cd/chapitre-04
---

# 🛠️ Méthode : calculer une différentielle seconde, une hessienne

*Méthode* · Chapitre : [[04-differentielles-ordre-superieur|4 – Différentielles d'ordre supérieur]] · Méthode 4.1 du cours · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> - **(a) Dériver la différentielle** (Lemme 4.9) : écrire $Df_x(h)$ comme fonction de $x$ ($h$ fixé), la différentier en $a$ dans la direction $k$ : on obtient $D^2f_a(h,k)$.
> - **(b) Dérivées partielles** ($\mathbb R^n\to\mathbb R$) : calculer $H_f(a)$, puis $D^2f_a(h,k)={}^t\!h\,H_f(a)\,k$.
> - **(c) Développement à l'ordre 2** : si $f(a+h)=f(a)+L(h)+B(h,h)+o(\lVert h\rVert^2)$ avec $B$ bilinéaire symétrique, alors $D^2f_a=2B$.
>
> **Vérification** : le résultat doit être bilinéaire et **symétrique** en $(h,k)$.

> [!EXAMPLE] Rédaction modèle (Écrit 2025-2026, ex. 1)
> $f(x,y)=x^3-3x+y^2$, polynomiale donc $\mathcal C^2$ sur $\mathbb R^2$.
> $\nabla f(x,y)=\binom{3x^2-3}{2y}$, $H_f(x,y)=\begin{pmatrix}6x&0\\0&2\end{pmatrix}$, $D^2f_{(x,y)}(h,k)=6x\,h_1k_1+2h_2k_2$.

> [!WARNING] Piège
> Méthode (c) : attention au facteur $2$ (Taylor contient $\frac12D^2f_a(h,h)$).

## 🔗 Liens

- **Voir aussi** : [[differentielle-seconde|Différentielle seconde, classe C2]], [[matrice-hessienne|Matrice hessienne]], [[expression-differentielle-seconde|Expression de la différentielle seconde]], [[theoreme-de-schwarz|Théorème de Schwarz]], [[critere-c2|Critère C2]]
