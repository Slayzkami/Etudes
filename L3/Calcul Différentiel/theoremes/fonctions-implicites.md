---
aliases:
  - "Théorème des fonctions implicites (cas général)"
  - "fonctions implicites cas général"
  - "z = φ(x,y)"
  - "Théorème 5.19"
  - "Corollaire 5.20"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-05
---

# ⭐ Théorème des fonctions implicites (cas général)

*Théorème* · Chapitre : [[05-inversion-locale-fonctions-implicites|5 – Inversion locale et fonctions implicites]] · Th. 5.19, Cor. 5.20 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> Soit $f:U\subset\mathbb R^m\times\mathbb R^n\to\mathbb R^n$ de classe $\mathcal C^k$ ($k\ge1$) et $(x_0,y_0)\in U$ tel que
> $$f(x_0,y_0)=0\qquad\text{et}\qquad\det J_yf(x_0,y_0)\ne0,$$
> où $J_yf=\big(\frac{\partial f_i}{\partial y_j}\big)$ est la matrice **carrée** $n\times n$ des dérivées par rapport aux variables $y$. Alors il existe des voisinages ouverts $V$ de $x_0$, $W$ de $y_0$ et $\varphi:V\to W$ de classe $\mathcal C^k$ tels que
> $$\big[(x,y)\in V\times W\text{ et }f(x,y)=0\big]\iff\big[x\in V\text{ et }y=\varphi(x)\big],$$
> et
> $$J_\varphi(x)=-\big[J_yf(x,\varphi(x))\big]^{-1}J_xf(x,\varphi(x)).$$

> [!IMPORTANT] Cas $z=\varphi(x,y)$ (Cor. 5.20)
> Si $F:U\subset\mathbb R^3\to\mathbb R$ est $\mathcal C^k$, $F(a,b,c)=0$ et $\dfrac{\partial F}{\partial z}(a,b,c)\ne0$, alors près de $(a,b,c)$ : $F(x,y,z)=0\iff z=\varphi(x,y)$, avec
> $$\frac{\partial\varphi}{\partial x}=-\frac{\partial_xF}{\partial_zF},\qquad\frac{\partial\varphi}{\partial y}=-\frac{\partial_yF}{\partial_zF}\quad\text{en }(x,y,\varphi(x,y)).$$

> [!SUCCESS]- Idée de la démonstration
> Inversion locale appliquée à $\Phi(x,y)=(x,f(x,y))$ : $J_\Phi=\begin{pmatrix}I_m&0\\ J_xf&J_yf\end{pmatrix}$, de déterminant $\det J_yf\ne0$. Puis on différentie $f(x,\varphi(x))=0$ : $J_xf+J_yf\,J_\varphi=0$. $\blacksquare$

> [!WARNING] Pièges
> - $m$ équations ? Non : **$n$ équations** pour $n$ inconnues $y$ (matrice $J_yf$ carrée).
> - L'ordre du produit : $-[J_yf]^{-1}J_xf$.

## 🔗 Liens

- **S'appuie sur** : [[fonctions-implicites-une-variable|Théorème des fonctions implicites (une variable)]], [[matrice-jacobienne|Matrice jacobienne]], [[differentielle-partielle|Différentielle partielle]]
- **Méthodes** : [[fonction-implicite|Étudier une fonction implicite (existence, dérivée, DL)]]
