---
aliases:
  - "Méthode : écrire la formule de Taylor-Young à l'ordre 2 en un point"
  - "Taylor-Young en un point"
  - "signe de f(x,y) - f(a)"
tags:
  - cd
  - cd/methode
  - cd/chapitre-04
---

# 🛠️ Méthode : écrire la formule de Taylor-Young à l'ordre 2 en un point

*Méthode* · Chapitre : [[04-differentielles-ordre-superieur|4 – Différentielles d'ordre supérieur]] · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> 1. Justifier : $f$ est $\mathcal C^2$, donc deux fois différentiable en $a$.
> 2. Calculer $f(a)$, $\partial_xf(a)$, $\partial_yf(a)$, puis $r,s,t$ en $a$.
> 3. Écrire, avec $h=(h_1,h_2)$ :
> $$f(a+h)=f(a)+\partial_xf(a)h_1+\partial_yf(a)h_2+\tfrac12\big(rh_1^2+2sh_1h_2+th_2^2\big)+\lVert h\rVert^2\varepsilon(h),\quad\varepsilon(h)\xrightarrow[h\to0]{}0.$$
> 4. **Signe de $f(a+h)-f(a)$** (si $a$ est critique) : c'est celui de la forme quadratique pour $h$ petit, quand elle garde un signe strict.

> [!EXAMPLE] Rédaction modèle (Écrit 2025-2026, ex. 1)
> $f(x,y)=x^3-3x+y^2$.
> - En $(1,0)$ : $f=-2$, gradient nul, $r=6$, $s=0$, $t=2$ :
> $f(1+h_1,h_2)=-2+3h_1^2+h_2^2+\lVert h\rVert^2\varepsilon(h)$. Comme $3h_1^2+h_2^2\ge\lVert h\rVert_2^2$, on a $f(x,y)-f(1,0)\ge\lVert h\rVert_2^2(1+\varepsilon(h))>0$ pour $h\ne0$ assez petit : minimum local strict.
> - En $(-1,0)$ : $f=2$, $r=-6$, $s=0$, $t=2$ :
> $f(-1+h_1,h_2)=2-3h_1^2+h_2^2+\lVert h\rVert^2\varepsilon(h)$. Sur $h=(h_1,0)$ : signe $<0$ ; sur $h=(0,h_2)$ : signe $>0$. $f(x,y)-f(-1,0)$ **change de signe** aussi près qu'on veut de $(-1,0)$ : pas d'extremum.

## 🔗 Liens

- **Voir aussi** : [[taylor-young-ordre-2|Formule de Taylor-Young à l'ordre 2]], [[matrice-hessienne|Matrice hessienne]], [[gradient|Gradient]]
