---
aliases:
  - "Vrai/Faux classiques CD"
  - "vrai faux calcul différentiel"
  - "peut-on affirmer que"
tags:
  - cd
  - cd/revision
---

# ✅ Vrai/Faux classiques (avec justification)

· [[cd-plan-de-revision|↩ Plan de révision]] · [[cd-index-definitions|↩ Index]] · Contre-exemples : [[exemples-et-contre-exemples]]

> [!ABSTRACT] Règle
> **Vrai** ⟹ citer le théorème (ou une preuve courte). **Faux** ⟹ **un** contre-exemple explicite et vérifié.
> Mode d'emploi : cacher les colonnes de droite, répondre à l'écrit, comparer.

| n° | Affirmation | Réponse | Idée |
|---|---|---|---|
| 1 | Toute application linéaire entre e.v.n. est continue | **Faux** | $f\mapsto f(1)$ pour $\lVert \cdot\rVert_1$ sur $\mathcal C([0,1])$ |
| 2 | Toute application linéaire de $\mathbb R^n$ dans un e.v.n. est continue | **Vrai** | Th. 1.44 |
| 3 | Sur $\mathcal C([0,1])$, $\lVert \cdot\rVert_1$ et $\lVert \cdot\rVert_\infty$ sont équivalentes | **Faux** | $u_n(t)=t^n$ |
| 4 | Si $\lVert f(u)\rVert\le5\lVert u\rVert$ pour tout $u$ ($f$ linéaire), alors $\tn f=5$ | **Faux** | seulement $\tn f\le5$ |
| 5 | Une application lipschitzienne est continue | **Vrai** | Prop. 1.34 |
| 6 | Si $f$ a des dérivées partielles en $a$, elle est continue en $a$ | **Faux** | $\frac{xy}{x^2+y^2}$ |
| 7 | Si $f$ est différentiable en $a$, elle est continue en $a$ | **Vrai** | Prop. 2.18 |
| 8 | Si $f$ est dérivable en $a$ dans toutes les directions, elle est différentiable en $a$ | **Faux** | $\frac{x^2y}{x^2+y^2}$ |
| 9 | La différentielle d'une application linéaire continue $\varphi$ en $a$ est $\varphi$ | **Vrai** | Ex. 2.16 |
| 10 | La différentielle d'une application bilinéaire continue $B$ est $B$ | **Faux** | $B(h_1,a_2)+B(a_1,h_2)$ |
| 11 | $D(g\circ f)_a=Dg_a\circ Df_a$ | **Faux** | c'est $Dg_{f(a)}$ |
| 12 | Si les dérivées partielles de $f$ sont continues sur $U$, $f$ est différentiable sur $U$ | **Vrai** | Cor. 3.16 |
| 13 | $f:[a,b]\to\mathbb R^2$ continue, dérivable sur $]a,b[$ : il existe $c$ avec $f(b)-f(a)=(b-a)f'(c)$ | **Faux** | $(\cos t,\sin t)$ sur $[0,2\pi]$ |
| 14 | Si $Df_x=0$ sur un ouvert $U$, alors $f$ est constante sur $U$ | **Faux** | $U$ doit être connexe |
| 15 | Si $\lvert\!\lvert\!\lvert Df_x\rvert\!\rvert\!\rvert\le M$ sur un ouvert convexe, $f$ est $M$-lipschitzienne | **Vrai** | Cor. 3.13 |
| 16 | Toute boule est convexe | **Vrai** | Ex. 3.5 |
| 17 | Un point critique est un extremum local | **Faux** | $x^2-y^2$ |
| 18 | Un extremum local d'une fonction différentiable sur un ouvert est un point critique | **Vrai** | Prop. 4.20 |
| 19 | Si $rt-s^2=0$ en un point critique, il n'y a pas d'extremum | **Faux** | $x^2+y^4$ |
| 20 | Si $f$ est $\mathcal C^2$, sa hessienne est symétrique | **Vrai** | Schwarz |
| 21 | Une bijection $\mathcal C^1$ est un difféomorphisme | **Faux** | $x\mapsto x^3$ |
| 22 | Si $\det J_f(x)\ne0$ pour tout $x$, alors $f$ est injective | **Faux** | $(e^x\cos y,e^x\sin y)$ |
| 23 | Si $f(a,b)=0$ et $\partial_yf(a,b)=0$, on ne peut **jamais** écrire $y=\varphi(x)$ près de $(a,b)$ | **Faux** | $f(x,y)=y^3-x$ : $y=\sqrt[3]x$ (le théorème ne s'applique pas, c'est tout) |

## ✍️ Justifications rédigées

> [!SUCCESS]- 1. Linéaire ⟹ continue : faux
> Soit $E=\mathcal C([0,1])$ muni de $\lVert f\rVert_1=\int_0^1\abs f$ et $\delta:f\mapsto f(1)$, linéaire. Pour $u_n(t)=t^n$ : $\delta(u_n)=1$ et $\lVert u_n\rVert_1=\frac1{n+1}$. Si $\delta$ était continue, il existerait $C$ avec $1\le\frac C{n+1}$ pour tout $n$ : absurde. → [[application-lineaire-continue]]

> [!SUCCESS]- 4. Une majoration ne donne pas la norme : faux
> $f:\mathbb R\to\mathbb R$, $f(u)=u$ vérifie $\lvert f(u)\rvert\le5\abs u$, mais $\tn f=1$. La majoration donne seulement $\tn f\le5$ (Prop. 1.50 (ii)) ; pour l'égalité il faut atteindre la constante. → [[calculer-norme-operateur]]

> [!SUCCESS]- 6. Dérivées partielles ⟹ continue : faux
> $f(x,y)=\frac{xy}{x^2+y^2}$ si $(x,y)\ne(0,0)$, $f(0,0)=0$. $\frac{f(t,0)-f(0,0)}t=0$ et $\frac{f(0,t)-f(0,0)}t=0$ : les deux dérivées partielles en $(0,0)$ existent et valent $0$. Mais $f(\frac1n,\frac1n)=\frac12\not\to0=f(0,0)$ : $f$ n'est pas continue en $(0,0)$. → [[derivee-partielle]]

> [!SUCCESS]- 7. Différentiable ⟹ continue : vrai
> $\lVert f(x)-f(a)\rVert\le\lvert\!\lvert\!\lvert Df_a\rvert\!\rvert\!\rvert\lVert x-a\rVert+\lVert x-a\rVert\lVert \varepsilon(x)\rVert\to0$ quand $x\to a$. → [[differentiable-implique-continue]]

> [!SUCCESS]- 8. Toutes les dérivées directionnelles ⟹ différentiable : faux
> $f(x,y)=\frac{x^2y}{x^2+y^2}$, $f(0,0)=0$. Pour $v=(v_1,v_2)\ne0$ et $t\ne0$ : $\frac{f(tv)-f(0)}t=\frac{v_1^2v_2}{v_1^2+v_2^2}$, donc $f'_v(0)=\frac{v_1^2v_2}{v_1^2+v_2^2}$ existe pour tout $v$. Mais $f'_{(1,0)}(0)=0$, $f'_{(0,1)}(0)=0$ et $f'_{(1,1)}(0)=\frac12\ne0+0$ : $v\mapsto f'_v(0)$ n'est pas linéaire, donc ne peut pas être $Df_{(0,0)}$ (Prop. 2.9). → [[montrer-non-differentiable]]

> [!SUCCESS]- 10. Différentielle d'une bilinéaire : faux
> Pour $B(x,y)=xy$ sur $\mathbb R\times\mathbb R$ : $DB_{(a_1,a_2)}(h_1,h_2)=h_1a_2+a_1h_2$, qui n'est pas $B(h_1,h_2)=h_1h_2$. → [[differentielles-de-reference]]

> [!SUCCESS]- 13. Égalité des accroissements finis vectorielle : faux
> $f(t)=(\cos t,\sin t)$ sur $[0,2\pi]$ : $f(2\pi)-f(0)=(0,0)$, mais $f'(c)=(-\sin c,\cos c)$ n'est jamais nul ($\sin$ et $\cos$ ne s'annulent pas en même temps). On a seulement l'inégalité : $\lVert f(b)-f(a)\rVert\le M(b-a)$. → [[taf]], [[iaf]]

> [!SUCCESS]- 14. $Df=0$ ⟹ constante : faux sans connexité
> $U=\mathbb R^*$ (ouvert, non connexe), $f(x)=1$ si $x>0$, $f(x)=-1$ si $x<0$. $f$ est dérivable de dérivée nulle sur $U$, non constante. Vrai si $U$ est connexe (Th. 3.25). → [[differentielle-nulle]]

> [!SUCCESS]- 16. Toute boule est convexe : vrai
> Soient $a,b\in B(x_0,r)$ et $t\in[0,1]$. $\lVert a+t(b-a)-x_0\rVert=\lVert (1-t)(a-x_0)+t(b-x_0)\rVert\le(1-t)\lVert a-x_0\rVert+t\lVert b-x_0\rVert<(1-t)r+tr=r$. → [[segment-et-convexe]]

> [!SUCCESS]- 17. Point critique ⟹ extremum : faux
> $f(x,y)=x^2-y^2$ : $\nabla f(0,0)=0$, mais $f(x,0)=x^2>0$ et $f(0,y)=-y^2<0$ aussi près qu'on veut de $(0,0)$. → [[point-critique]]

> [!SUCCESS]- 19. $rt-s^2=0$ : on ne peut rien dire
> $f(x,y)=x^2+y^4$ : en $(0,0)$, $r=2$, $s=t=0$, $rt-s^2=0$, et pourtant $f\ge0=f(0,0)$ : minimum global. → [[critere-rt-s2]]

> [!SUCCESS]- 21. Bijection $\mathcal C^1$ ⟹ difféomorphisme : faux
> $f(x)=x^3$ est bijective et $\mathcal C^1$ de $\mathbb R$ sur $\mathbb R$. Si $f^{-1}$ était dérivable en $0=f(0)$, on aurait $(f^{-1})'(0)\cdot f'(0)=1$ (règle de la chaîne), or $f'(0)=0$. → [[diffeomorphisme]]

> [!SUCCESS]- 22. Jacobien non nul ⟹ injective : faux
> $f(x,y)=(e^x\cos y,e^x\sin y)$ : $\det J_f=e^{2x}\ne0$ partout, mais $f(0,0)=f(0,2\pi)$. → [[inversion-globale]]

## 🔗 Liens
- [[exemples-et-contre-exemples]] · [[cd-fiche-theoremes]] · [[cd-mes-erreurs]]
