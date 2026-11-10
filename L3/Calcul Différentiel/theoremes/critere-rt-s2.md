---
aliases:
  - "Critère rt − s² (dimension 2)"
  - "Corollaire 4.25"
  - "rt-s²"
  - "nature d'un point critique"
  - "point-selle"
  - "point col"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-04
---

# ⭐ Critère rt − s² (dimension 2)

*Théorème* · Chapitre : [[04-differentielles-ordre-superieur|4 – Différentielles d'ordre supérieur]] · Cor. 4.25 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Corollaire
> Soit $U\subset\mathbb R^2$ ouvert, $f:U\to\mathbb R$ deux fois différentiable en un **point critique** $a$. On pose
> $$r=\frac{\partial^2f}{\partial x^2}(a),\quad s=\frac{\partial^2f}{\partial x\partial y}(a),\quad t=\frac{\partial^2f}{\partial y^2}(a).$$
> 1. Si $rt-s^2>0$ : extremum local strict en $a$ ; **minimum** si $r>0$, **maximum** si $r<0$.
> 2. Si $rt-s^2<0$ : **pas d'extremum** en $a$ (point-selle, ou col).
> 3. Si $rt-s^2=0$ : on **ne peut pas conclure** par ce critère.

> [!SUCCESS]- Démonstration (idée)
> $Q(h)={}^t\!h\,H_f(a)\,h=rh_1^2+2sh_1h_2+th_2^2$. Si $r\ne0$ : $Q(h)=r\big(h_1+\frac srh_2\big)^2+\frac{rt-s^2}{r}h_2^2$.
> - $rt-s^2>0$ : alors $r\ne0$ et les deux carrés ont le signe de $r$ : $Q$ est définie positive ($r>0$) ou négative ($r<0$) → Th. 4.23.
> - $rt-s^2<0$ : $Q$ prend des valeurs $>0$ et $<0$, donc la condition nécessaire du Th. 4.23 n'est vérifiée ni pour un min ni pour un max. $\blacksquare$

> [!EXAMPLE] Exemple (Écrit 2024-2025)
> $f(x,y)=3xy-x^3-y^3$ : points critiques $(0,0)$ et $(1,1)$. En $(0,0)$ : $r=t=0$, $s=3$, $rt-s^2=-9<0$ : point-selle. En $(1,1)$ : $r=t=-6$, $s=3$, $rt-s^2=27>0$, $r<0$ : maximum local strict.

> [!WARNING] Pièges
> - Vérifier d'abord que $a$ est un point **critique**.
> - $rt-s^2=0$ : étudier directement le signe de $f(a+h)-f(a)$ → [[etudier-points-critiques]].

## 🔗 Liens

- **S'appuie sur** : [[extrema-et-hessienne|Extrema et différentielle seconde]], [[point-critique|Point critique]]
- **Méthodes** : [[etudier-points-critiques|Étudier les points critiques d'une fonction de R²]]
