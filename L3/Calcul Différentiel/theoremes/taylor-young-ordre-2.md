---
aliases:
  - "Formule de Taylor-Young à l'ordre 2"
  - "Taylor-Young"
  - "Taylor Young ordre 2"
  - "développement limité à l'ordre 2"
  - "T-Y"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-04
---

# ⭐ Formule de Taylor-Young à l'ordre 2

*Théorème* · Chapitre : [[04-differentielles-ordre-superieur|4 – Différentielles d'ordre supérieur]] · Prop. 4.15 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Proposition (admis)
> Si $f:U\subset\mathbb R^n\to\mathbb R$ est deux fois différentiable en $a$, alors, pour $h$ assez petit,
> $$f(a+h)=f(a)+Df_a(h)+\frac12\,{}^t\!h\,H_f(a)\,h+\lVert h\rVert^2\varepsilon(h),\qquad\lim_{h\to0}\varepsilon(h)=0.$$

> [!NOTE] En dimension 2, tout écrit (question de cours, Écrit 2025-2026)
> Pour $g:\mathbb R^2\to\mathbb R$ au point $a=(a_1,a_2)$, avec $h=(h_1,h_2)$ :
> $$g(a_1+h_1,a_2+h_2)=g(a)+\frac{\partial g}{\partial x_1}(a)h_1+\frac{\partial g}{\partial x_2}(a)h_2+\frac12\Big(\frac{\partial^2g}{\partial x_1^2}(a)h_1^2+2\frac{\partial^2g}{\partial x_1\partial x_2}(a)h_1h_2+\frac{\partial^2g}{\partial x_2^2}(a)h_2^2\Big)+\lVert h\rVert^2\varepsilon(h).$$

> [!EXAMPLE] Exemple
> $f(x,y)=x^3-3x+y^2$ en $(1,0)$ : $f(1,0)=-2$, $\nabla f(1,0)=0$, $H_f(1,0)=\begin{pmatrix}6&0\\0&2\end{pmatrix}$, donc
> $f(1+h_1,h_2)=-2+3h_1^2+h_2^2+\lVert h\rVert^2\varepsilon(h)$ : $f(x,y)-f(1,0)\ge0$ près de $(1,0)$ (minimum local).

> [!WARNING] Pièges
> - Le facteur $\frac12$ et le **$2$** devant le terme croisé.
> - Ne pas oublier le reste $\lVert h\rVert^2\varepsilon(h)$ avec $\varepsilon(h)\to0$.

## 🔗 Liens

- **S'appuie sur** : [[matrice-hessienne|Matrice hessienne]], [[differentielle-seconde|Différentielle seconde, classe C2]], [[petit-o|Petit o]]
- **Utilisé par (théorèmes)** : [[extrema-et-hessienne|Extrema et différentielle seconde]], [[formules-de-taylor|Formules de Taylor (ordre n)]]
- **Méthodes** : [[etudier-points-critiques|Étudier les points critiques d'une fonction de R²]], [[ecrire-taylor-young|Écrire la formule de Taylor-Young à l'ordre 2 en un point]], [[fonction-implicite|Étudier une fonction implicite (existence, dérivée, DL)]]
