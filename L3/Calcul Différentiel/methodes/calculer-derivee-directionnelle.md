---
aliases:
  - "Méthode : calculer une dérivée directionnelle"
  - "dérivée de f en a dans la direction v"
tags:
  - cd
  - cd/methode
  - cd/chapitre-02
---

# 🛠️ Méthode : calculer une dérivée directionnelle

*Méthode* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> - **Si $f$ est différentiable en $a$** (cas habituel) : la dérivée en $a$ dans la direction $v$ vaut $Df_a(v)=J_f(a)\,v$ (Prop. 2.9).
> - **Sinon** (point particulier) : revenir à la définition, $\lim_{t\to0}\dfrac{f(a+tv)-f(a)}{t}$.

> [!EXAMPLE] Rédaction modèle (Écrit 2025-2026, ex. 2)
> $f(x,y)=(\cos(x+2y),\sin(2x+y))$, $J_f(x,y)=\begin{pmatrix}-\sin(x+2y)&-2\sin(x+2y)\\2\cos(2x+y)&\cos(2x+y)\end{pmatrix}$.
> En $a=(\frac\pi2,0)$ : $J_f(a)=\begin{pmatrix}-1&-2\\-2&-1\end{pmatrix}$. Comme $f$ est différentiable en $a$, la dérivée dans la direction $v=(1,1)$ est
> $Df_a(v)=J_f(a)\binom11=\binom{-3}{-3}$.

> [!WARNING] Piège
> Le résultat est un **vecteur de l'espace d'arrivée** (ici $\mathbb R^2$), pas un nombre.

## 🔗 Liens

- **Voir aussi** : [[derivee-directionnelle|Dérivée directionnelle]], [[differentielle-et-derivees-directionnelles|Différentielle et dérivées directionnelles]], [[matrice-jacobienne|Matrice jacobienne]]
