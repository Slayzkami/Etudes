---
aliases:
  - "Matrice hessienne"
  - "hessienne"
  - "H_f(a)"
  - "Hess f"
tags:
  - cd
  - cd/definition
  - cd/chapitre-04
---

# 📘 Matrice hessienne

*Définition* · Chapitre : [[04-differentielles-ordre-superieur|4 – Différentielles d'ordre supérieur]] · Déf. 4.13 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> Soit $f:U\subset\mathbb R^n\to\mathbb R$ deux fois différentiable en $a$. La **matrice hessienne** de $f$ en $a$ est
> $$H_f(a)=\big(\partial^2_{ij}f(a)\big)_{1\le i,j\le n}.$$
> Elle est **symétrique** ([[theoreme-de-schwarz]]) et, pour tous $h,k\in\mathbb R^n$ (Prop. 4.14),
> $$D^2f_a(h,k)={}^t\!h\,H_f(a)\,k.$$

> [!EXAMPLE] En dimension 2
> $H_f(a)=\begin{pmatrix}r&s\\ s&t\end{pmatrix}$ avec $r=\dfrac{\partial^2f}{\partial x^2}(a)$, $s=\dfrac{\partial^2f}{\partial x\partial y}(a)$, $t=\dfrac{\partial^2f}{\partial y^2}(a)$, et
> $${}^t\!h\,H_f(a)\,h=r\,h_1^2+2s\,h_1h_2+t\,h_2^2.$$
> Pour $f(x,y)=x^3-3x+y^2$ : $H_f(x,y)=\begin{pmatrix}6x&0\\0&2\end{pmatrix}$.

> [!WARNING] Pièges
> - Ne pas oublier le **$2s$** dans le développement.
> - La hessienne n'existe que pour $f$ à valeurs **réelles** ; la jacobienne, c'est l'ordre 1.

## 🔗 Liens

- **S'appuie sur** : [[derivees-partielles-ordre-2|Dérivées partielles d'ordre 2]], [[differentielle-seconde|Différentielle seconde, classe C2]]
- **Utilisé par (théorèmes)** : [[expression-differentielle-seconde|Expression de la différentielle seconde]], [[taylor-young-ordre-2|Formule de Taylor-Young à l'ordre 2]], [[extrema-et-hessienne|Extrema et différentielle seconde]]
- **Méthodes** : [[calculer-differentielle-seconde|Calculer une différentielle seconde, une hessienne]], [[etudier-points-critiques|Étudier les points critiques d'une fonction de R²]], [[ecrire-taylor-young|Écrire la formule de Taylor-Young à l'ordre 2 en un point]]
