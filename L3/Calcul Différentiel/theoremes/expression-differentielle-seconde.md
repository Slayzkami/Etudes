---
aliases:
  - "Expression de la différentielle seconde"
  - "Lemme 4.9"
  - "D²f_a(h,k) avec la hessienne"
  - "dériver la différentielle"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-04
---

# ⭐ Expression de la différentielle seconde

*Théorème* · Chapitre : [[04-differentielles-ordre-superieur|4 – Différentielles d'ordre supérieur]] · Lemme 4.9, Th. 4.11, Prop. 4.14 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Lemme 4.9 (dériver la différentielle)
> Soit $f:U\to F$ deux fois différentiable en $a$ et $h\in E$ **fixé**. Alors $\varphi:x\mapsto Df_x(h)$ est différentiable en $a$ et
> $$D\varphi_a(k)=D^2f_a(k)(h)=D^2f_a(k,h)\qquad(=D^2f_a(h,k)\text{ par Schwarz}).$$

> [!IMPORTANT] Sur $\mathbb R^n$ (Th. 4.11, Prop. 4.14)
> $$D^2f_a(h,k)=\sum_{i=1}^n\sum_{j=1}^n\partial^2_{ij}f(a)\,h_ik_j={}^t\!h\,H_f(a)\,k\quad(\text{si }F=\mathbb R).$$

> [!SUCCESS]- Démonstration
> **Lemme.** $\varphi=\mathrm{ev}_h\circ Df$ où $\mathrm{ev}_h:\mathcal L_c(E,F)\to F$, $L\mapsto L(h)$, est linéaire continue ($\lVert L(h)\rVert\le\lvert\!\lvert\!\lvert L\rvert\!\rvert\!\rvert\lVert h\rVert$). Par la règle de la chaîne, $D\varphi_a(k)=\mathrm{ev}_h(D(Df)_a(k))=D^2f_a(k)(h)$.
> **Th. 4.11.** Par bilinéarité, $D^2f_a(h,k)=\sum_{i,j}h_ik_j\,D^2f_a(e_i,e_j)$ et $D^2f_a(e_i,e_j)=\partial^2_{ij}f(a)$ (Th. 4.10). $\blacksquare$

> [!EXAMPLE] Exemple
> $f(X)=X^3$ : $Df_X(H)=HX^2+XHX+X^2H$. À $H$ fixé, on différentie en $X$ dans la direction $K$ :
> $D^2f_A(H,K)=HKA+HAK+KHA+AHK+KAH+AKH$ (symétrique en $(H,K)$ ✔).

## 🔗 Liens

- **S'appuie sur** : [[differentielle-seconde|Différentielle seconde, classe C2]], [[matrice-hessienne|Matrice hessienne]], [[regle-de-la-chaine|Règle de la chaîne (différentielle d'une composée)]]
- **Méthodes** : [[calculer-differentielle-seconde|Calculer une différentielle seconde, une hessienne]]
