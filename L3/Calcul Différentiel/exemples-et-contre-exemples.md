---
aliases:
  - "Exemples et contre-exemples classiques"
  - "catalogue d'exemples CD"
  - "contre-exemples calcul différentiel"
tags:
  - cd
  - cd/exemples
---

# 🧩 Exemples et contre-exemples classiques

Les exemples qui reviennent partout (cours, TD, sujets) et les contre-exemples à sortir dans un Vrai/Faux. · [[cd-index-definitions|↩ Index]]

## Espaces à connaître

| Espace | Dimension | Normes usuelles | À retenir |
|---|---|---|---|
| $\mathbb R^n$ | $n$ | $\lVert \cdot\rVert_1,\lVert \cdot\rVert_2,\lVert \cdot\rVert_\infty$ | toutes équivalentes → [[equivalence-normes-dimension-finie]] |
| $\mathcal M_n(\mathbb R)$ | $n^2$ | une norme avec $\lVert XY\rVert\le\lVert X\rVert\lVert Y\rVert$ | toute application linéaire y est continue → [[differentielle-sur-les-matrices]] |
| $\mathbb R_n[X]$ | $n+1$ | — | dimension finie |
| $\mathcal C([0,1])$ | **infinie** | $\lVert \cdot\rVert_\infty$ (Banach), $\lVert \cdot\rVert_1$ (pas Banach) | normes **non** équivalentes → [[normes-equivalentes]] |
| $\mathcal L_c(E,F)$ | — | $\lvert\!\lvert\!\lvert \cdot\rvert\!\rvert\!\rvert$ | Banach si $F$ l'est → [[espaces-de-banach-usuels]] |

## Différentielles à connaître par cœur

| Application | Différentielle | Référence |
|---|---|---|
| constante | $Df_a=0$ | [[differentielles-de-reference]] |
| $\varphi$ linéaire continue | $D\varphi_a(h)=\varphi(h)$ | [[differentielles-de-reference]] |
| $B$ bilinéaire continue | $DB_{(a_1,a_2)}(h_1,h_2)=B(h_1,a_2)+B(a_1,h_2)$ | [[differentielles-de-reference]] |
| $x\mapsto\lVert x\rVert_2^2$ sur $\mathbb R^n$ | $Df_a(h)=2(a_1h_1+\dots+a_nh_n)$ | [[differentiabilite-par-definition]] |
| $X\mapsto X^2$ | $AH+HA$ | [[differentiabilite]] |
| $X\mapsto X^3$ | $A^2H+AHA+HA^2$ | [[differentielle-sur-les-matrices]] |
| $X\mapsto XMX$ | $HMA+AMH$ | [[appliquer-regle-de-la-chaine]] |
| $X\mapsto\mathrm{tr}(X\,{}^t\!X)$ | $2\,\mathrm{tr}(A\,{}^t\!H)$ | [[differentielle-sur-les-matrices]] |
| $\varphi\circ u$ ($\varphi$ d'une variable) | $\varphi'(u(a))\,Du_a(h)$ | [[regle-de-la-chaine]] |
| polaires $(\rho,\theta)\mapsto(\rho\cos\theta,\rho\sin\theta)$ | $J=\begin{pmatrix}\cos\theta&-\rho\sin\theta\\ \sin\theta&\rho\cos\theta\end{pmatrix}$, $\det=\rho$ | [[matrice-jacobienne]] |

## Contre-exemples

| Ce qu'on croit | Contre-exemple | Voir |
|---|---|---|
| Linéaire ⟹ continue | $f\mapsto f(1)$ sur $(\mathcal C([0,1]),\lVert \cdot\rVert_1)$ ; la dérivation pour $\lVert \cdot\rVert_\infty$ ; suite $u_n(t)=t^n$ | [[application-lineaire-continue]] |
| Toutes les normes sont équivalentes | $\lVert \cdot\rVert_1$ et $\lVert \cdot\rVert_\infty$ sur $\mathcal C([0,1])$, avec $u_n(t)=t^n$ | [[normes-equivalentes]] |
| Intersection d'ouverts ⟹ ouvert | $\bigcap_n\,]-\frac1n,\frac1n[=\{0\}$ | [[stabilite-ouverts-fermes]] |
| Continue ⟹ uniformément continue | $x\mapsto x^2$ sur $\mathbb R$ | [[continuite-uniforme]] |
| Applications partielles continues ⟹ continue | $\frac{xy}{x^2+y^2}$ en $(0,0)$ | [[continuite]] |
| Dérivées partielles en $a$ ⟹ continue en $a$ | $\frac{xy}{x^2+y^2}$, $f(0,0)=0$ : $\partial_xf(0,0)=\partial_yf(0,0)=0$ mais $f(t,t)=\frac12$ | [[derivee-partielle]] |
| Dérivées dans toutes les directions ⟹ différentiable | $\frac{x^2y}{x^2+y^2}$, $f(0,0)=0$ : continue, toutes les dérivées directionnelles existent, non différentiable | [[montrer-non-differentiable]] |
| Continue ⟹ différentiable | $(x,y)\mapsto\abs x$ en $(0,0)$ ; une norme en $0$ | [[montrer-non-differentiable]] |
| Différentiable ⟹ $\mathcal C^1$ | $x^2\sin\frac1x$ (prolongée par $0$) : dérivable en $0$, dérivée non continue | [[classe-c1]] |
| Égalité des accroissements finis à valeurs dans $\mathbb R^2$ | $t\mapsto(\cos t,\sin t)$ sur $[0,2\pi]$ | [[taf]] |
| $Df=0$ ⟹ constante | $f=\pm1$ sur les deux moitiés de $\mathbb R^*$ (ouvert non connexe) | [[differentielle-nulle]] |
| Connexe ⟹ convexe | $\mathbb R^2\setminus\{(0,0)\}$ | [[convexe-implique-connexe]] |
| Dérivées croisées toujours égales | $xy\frac{x^2-y^2}{x^2+y^2}$ en $(0,0)$ | [[theoreme-de-schwarz]] |
| Point critique ⟹ extremum | $x^2-y^2$ en $(0,0)$ (point-selle) ; $x^3$ en $0$ | [[point-critique]] |
| $rt-s^2=0$ ⟹ pas d'extremum | $x^2+y^4$ (minimum) contre $x^2+y^3$ (pas d'extremum), en $(0,0)$ | [[critere-rt-s2]] |
| Extremum local ⟹ global | $x^3-3x+y^2$ en $(1,0)$ | [[extremum-global]] |
| Bijection $\mathcal C^1$ ⟹ difféomorphisme | $x\mapsto x^3$ sur $\mathbb R$ | [[diffeomorphisme]] |
| Jacobien non nul partout ⟹ injective | $(x,y)\mapsto(e^x\cos y,e^x\sin y)$ | [[inversion-locale]] |
| On peut toujours écrire $y=\varphi(x)$ | cercle $x^2+y^2=1$ en $(1,0)$ : $\partial_yf=0$ | [[fonctions-implicites-une-variable]] |

## 🔗 Liens
- [[cd-vrai-faux-classiques]] · [[cd-fiche-theoremes]] · [[cd-mes-erreurs]]
