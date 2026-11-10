---
aliases:
  - "Différentielle et différentielles partielles"
  - "Proposition 2.29"
  - "Df_a(h) = somme des dérivées partielles"
  - "Corollaire 2.32"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-02
---

# ⭐ Différentielle et différentielles partielles

*Théorème* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Prop. 2.29, Cor. 2.32 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Proposition
> Si $f:U\subset E_1\times\dots\times E_n\to F$ est différentiable en $a$, alors $\partial_jf(a)$ existe pour tout $j$, et pour tout $h=(h_1,\dots,h_n)$ :
> $$Df_a(h)=\sum_{j=1}^n\partial_jf(a)(h_j).$$
> Cas $E=\mathbb R^n$ (Cor. 2.32) : $\displaystyle Df_a(h)=h_1\frac{\partial f}{\partial x_1}(a)+\dots+h_n\frac{\partial f}{\partial x_n}(a)$.

> [!SUCCESS]- Démonstration
> L'injection $I_j:x_j\mapsto(a_1,\dots,x_j,\dots,a_n)$ est affine, de différentielle $\iota_j:h_j\mapsto(0,\dots,h_j,\dots,0)$. Par la [[regle-de-la-chaine]], $\varphi_j=f\circ I_j$ est différentiable en $a_j$ et $\partial_jf(a)=Df_a\circ\iota_j$. Comme $h=\sum_j\iota_j(h_j)$ et $Df_a$ est linéaire : $Df_a(h)=\sum_jDf_a(\iota_j(h_j))=\sum_j\partial_jf(a)(h_j)$. $\blacksquare$

> [!WARNING] Piège
> La formule donne $Df_a$ **si on sait déjà** que $f$ est différentiable. Elle ne prouve pas la différentiabilité.

## 🔗 Liens

- **S'appuie sur** : [[differentielle-partielle|Différentielle partielle]], [[derivee-partielle|Dérivée partielle]]
