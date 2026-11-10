---
aliases:
  - "Exercices types corrigés CD"
  - "corrections modèles calcul différentiel"
  - "exercices du partiel CD"
tags:
  - cd
  - cd/revision
---

# ✍️ Exercices types corrigés (rédactions modèles)

Les exercices qui reviennent dans les sujets, rédigés comme sur une copie. **Mode d'emploi** : lire l'énoncé, chercher sur brouillon, puis seulement déplier la correction et comparer ligne par ligne. · [[cd-plan-de-revision|↩ Plan de révision]] · [[cd-index-definitions|↩ Index]]

> [!NOTE] Sommaire
> 1. [[#1. Montrer qu'une application est une norme]]
> 2. [[#2. Normes non équivalentes, forme linéaire non continue]]
> 3. [[#3. Norme d'opérateur d'une matrice]]
> 4. [[#4. Jacobienne, différentielle, dérivée directionnelle]]
> 5. [[#5. Différentielle de X³ et de tr(X³)]]
> 6. [[#6. Différentielle de XMX, deux méthodes]]
> 7. [[#7. Différentielle de tr(X tX) et d'une composée]]
> 8. [[#8. Étude en (0,0)]]
> 9. [[#9. Classe C1, gradient, plan tangent]]
> 10. [[#10. Majorer la différentielle, lipschitzienne]]
> 11. [[#11. Points critiques et Taylor-Young]]
> 12. [[#12. Points critiques, système à résoudre]]
> 13. [[#13. Le cas rt − s² = 0]]
> 14. [[#14. Difféomorphisme local, pas global]]
> 15. [[#15. Fonction implicite]]
>
> Pour savoir quelle méthode sortir face à un énoncé : [[cd-reconnaitre-exercice]].

---

## 1. Montrer qu'une application est une norme

**Énoncé** (Écrit 2024-2025). Sur $E=\mathcal M_n(\mathbb R)$, on pose $N(X)=n\max_{1\le i,j\le n}\lvert x_{ij}\rvert$.
a) Montrer que $N$ est une norme sur $E$.
b) Montrer que $N(XY)\le N(X)N(Y)$ pour tous $X,Y\in E$.
c) Justifier l'existence de $c>0$ tel que $\lvert \mathrm{tr}(X)\rvert\le c\,N(X)$ pour tout $X$.

Méthodes : [[montrer-norme]], [[continuite-application-lineaire]].

> [!SUCCESS]- Correction a)
> $N(X)$ est le maximum d'un nombre fini de réels positifs : $N$ est bien définie, à valeurs dans $\mathbb R_+$.
> **Séparation.** Si $N(X)=0$, alors $\max_{i,j}\lvert x_{ij}\rvert=0$, donc $x_{ij}=0$ pour tous $i,j$ : $X=0$. Réciproquement $N(0)=0$.
> **Homogénéité.** Soit $\lambda\in\mathbb R$. $N(\lambda X)=n\max_{i,j}\lvert \lambda x_{ij}\rvert=n\abs\lambda\max_{i,j}\lvert x_{ij}\rvert=\abs\lambda N(X)$.
> **Inégalité triangulaire.** Pour tous $i,j$ : $\lvert x_{ij}+y_{ij}\rvert\le\lvert x_{ij}\rvert+\lvert y_{ij}\rvert\le\frac1nN(X)+\frac1nN(Y)$. Le majorant ne dépend pas de $(i,j)$, donc $\max_{i,j}\lvert x_{ij}+y_{ij}\rvert\le\frac1n(N(X)+N(Y))$, soit $N(X+Y)\le N(X)+N(Y)$.
> Donc $N$ est une norme sur $E$.

> [!SUCCESS]- Correction b)
> Le coefficient $(i,j)$ de $XY$ est $\sum_{k=1}^nx_{ik}y_{kj}$. Donc
> $$\Big|\sum_{k=1}^nx_{ik}y_{kj}\Big|\le\sum_{k=1}^n\lvert x_{ik}\rvert\lvert y_{kj}\rvert\le\sum_{k=1}^n\frac{N(X)}n\cdot\frac{N(Y)}n=\frac{N(X)N(Y)}n.$$
> En prenant le max sur $(i,j)$ puis en multipliant par $n$ : $N(XY)\le N(X)N(Y)$.

> [!SUCCESS]- Correction c)
> $\mathrm{tr}:E\to\mathbb R$ est linéaire et $E$ est de dimension finie ($n^2$), donc $\mathrm{tr}$ est continue ([[lineaire-en-dimension-finie|Th. 1.44]]). D'après le [[caracterisation-lineaires-continues|Th. 1.43]] (iv), il existe $c\ge0$ tel que $\lvert \mathrm{tr}(X)\rvert\le c\,N(X)$ pour tout $X$ ; quitte à remplacer $c$ par $c+1$, $c>0$.
> (Calcul direct : $\lvert \mathrm{tr}(X)\rvert\le\sum_i\lvert x_{ii}\rvert\le n\max\lvert x_{ij}\rvert=N(X)$, donc $c=1$ convient.)

---

## 2. Normes non équivalentes, forme linéaire non continue

**Énoncé.** Soit $E=\mathcal C([0,1],\mathbb R)$, $\lVert f\rVert_\infty=\sup_{[0,1]}\abs f$ et $\lVert f\rVert_1=\int_0^1\lvert f(t)\rvert\,\mathrm dt$.
a) Montrer que $\lVert f\rVert_1\le\lVert f\rVert_\infty$ pour tout $f\in E$.
b) Montrer que $\lVert \cdot\rVert_1$ et $\lVert \cdot\rVert_\infty$ ne sont pas équivalentes.
c) L'application $\delta:f\mapsto f(1)$ est-elle continue sur $(E,\lVert \cdot\rVert_\infty)$ ? sur $(E,\lVert \cdot\rVert_1)$ ?

Méthodes : [[montrer-normes-equivalentes]], [[continuite-application-lineaire]].

> [!SUCCESS]- Correction a)
> Pour tout $t\in[0,1]$, $\lvert f(t)\rvert\le\lVert f\rVert_\infty$. En intégrant sur $[0,1]$ : $\lVert f\rVert_1\le\int_0^1\lVert f\rVert_\infty\,\mathrm dt=\lVert f\rVert_\infty$.

> [!SUCCESS]- Correction b)
> Pour $n\in\mathbb N$, soit $u_n(t)=t^n$. Alors $\lVert u_n\rVert_\infty=1$ et $\lVert u_n\rVert_1=\int_0^1t^n\,\mathrm dt=\frac1{n+1}$.
> Supposons les normes équivalentes : il existe $\beta>0$ tel que $\lVert f\rVert_\infty\le\beta\lVert f\rVert_1$ pour tout $f\in E$. Avec $f=u_n$ : $1\le\frac\beta{n+1}$, soit $n+1\le\beta$ pour tout $n$ : absurde. Donc les normes ne sont pas équivalentes.

> [!SUCCESS]- Correction c)
> $\delta$ est linéaire : $\delta(f+\lambda g)=f(1)+\lambda g(1)=\delta(f)+\lambda\delta(g)$.
> **Pour $\lVert \cdot\rVert_\infty$.** $\lvert \delta(f)\rvert=\lvert f(1)\rvert\le\lVert f\rVert_\infty$ : par le Th. 1.43 (iv), $\delta$ est continue (et $\tn\delta\le1$ ; la fonction constante $1$ donne $\tn\delta=1$).
> **Pour $\lVert \cdot\rVert_1$.** Si $\delta$ était continue, il existerait $C\ge0$ avec $\lvert f(1)\rvert\le C\lVert f\rVert_1$ pour tout $f$. Avec $u_n$ : $1\le\frac C{n+1}$ pour tout $n$ : absurde. Donc $\delta$ n'est pas continue.

---

## 3. Norme d'opérateur d'une matrice

**Énoncé.** Soit $u:\mathbb R^2\to\mathbb R^2$, $u(x,y)=(x-2y,\ 3x+4y)$.
a) Justifier que $u$ est linéaire continue.
b) Calculer $\tn u$ quand $\mathbb R^2$ est muni de $\lVert \cdot\rVert_\infty$ au départ et à l'arrivée.
c) Même question avec $\lVert \cdot\rVert_1$.

Méthode : [[calculer-norme-operateur]].

> [!SUCCESS]- Correction a)
> $u$ est linéaire (ses composantes sont des combinaisons linéaires de $x$ et $y$) et $\mathbb R^2$ est de dimension finie : $u$ est continue (Th. 1.44).

> [!SUCCESS]- Correction b)
> **Majoration.** Soit $(x,y)\in\mathbb R^2$, $m=\lVert (x,y)\rVert_\infty=\max(\abs x,\abs y)$.
> $\lvert x-2y\rvert\le\abs x+2\abs y\le3m$ et $\lvert 3x+4y\rvert\le3\abs x+4\abs y\le7m$.
> Donc $\lVert u(x,y)\rVert_\infty\le7\,\lVert (x,y)\rVert_\infty$, d'où $\tn u\le7$ (Prop. 1.50 (ii)).
> **Atteinte.** Pour $v=(1,1)$ : $\lVert v\rVert_\infty=1$ et $u(v)=(-1,7)$, $\lVert u(v)\rVert_\infty=7$. Donc $\tn u\ge7$.
> **Conclusion.** $\tn u=7$ (la plus grosse ligne : $\abs3+\abs4$).

> [!SUCCESS]- Correction c)
> **Majoration.** $\lVert u(x,y)\rVert_1=\lvert x-2y\rvert+\lvert 3x+4y\rvert\le\abs x+2\abs y+3\abs x+4\abs y=4\abs x+6\abs y\le6(\abs x+\abs y)=6\lVert (x,y)\rVert_1$. Donc $\tn u\le6$.
> **Atteinte.** Pour $v=(0,1)$ : $\lVert v\rVert_1=1$ et $u(v)=(-2,4)$, $\lVert u(v)\rVert_1=6$. Donc $\tn u\ge6$.
> **Conclusion.** $\tn u=6$ (la plus grosse colonne : $\lvert -2\rvert+\abs4$).

---

## 4. Jacobienne, différentielle, dérivée directionnelle

**Énoncé** (Écrit 2024-2025). Soit $f:\mathbb R^2\to\mathbb R^2$, $f(x,y)=\Big(\dfrac{\cos x-\sin y}2,\ \dfrac{\sin x-\cos y}2\Big)$.
a) Montrer que $f$ est différentiable en tout point et calculer sa matrice jacobienne.
b) Calculer la dérivée de $f$ en $(0,0)$ dans la direction $(1,1)$.

Méthodes : [[calculer-jacobienne]], [[calculer-derivee-directionnelle]].

> [!SUCCESS]- Correction a)
> Les composantes $f_1(x,y)=\frac{\cos x-\sin y}2$ et $f_2(x,y)=\frac{\sin x-\cos y}2$ admettent en tout point des dérivées partielles
> $\partial_xf_1=-\frac{\sin x}2$, $\partial_yf_1=-\frac{\cos y}2$, $\partial_xf_2=\frac{\cos x}2$, $\partial_yf_2=\frac{\sin y}2$,
> qui sont continues sur $\mathbb R^2$. Donc $f_1,f_2$ sont $\mathcal C^1$ (Cor. 3.16), donc différentiables, et $f$ est différentiable sur $\mathbb R^2$ (Prop. 2.33). Sa jacobienne (ligne = composante, colonne = variable) est
> $$J_f(x,y)=\frac12\begin{pmatrix}-\sin x&-\cos y\\ \cos x&\sin y\end{pmatrix}.$$

> [!SUCCESS]- Correction b)
> $f$ est différentiable en $(0,0)$, donc elle y est dérivable dans la direction $v=(1,1)$ et cette dérivée vaut $Df_{(0,0)}(v)=J_f(0,0)\,v$ (Prop. 2.9). Or $J_f(0,0)=\frac12\begin{pmatrix}0&-1\\1&0\end{pmatrix}$, donc
> $$Df_{(0,0)}(1,1)=\frac12\begin{pmatrix}0&-1\\1&0\end{pmatrix}\binom11=\binom{-1/2}{1/2}.$$

---

## 5. Différentielle de X³ et de tr(X³)

**Énoncé** (Écrit 2022-2023). $E=\mathcal M_n(\mathbb R)$ muni d'une norme vérifiant $\lVert AB\rVert\le\lVert A\rVert\lVert B\rVert$. On pose $f(X)=X^3$ et $g(X)=\mathrm{tr}(X^3)$.
a) Par la définition, montrer que $f$ est différentiable en tout $A\in E$ et donner $Df_A$.
b) Montrer que $g$ est différentiable en tout $A$ et donner $Dg_A$.

Méthodes : [[differentielle-sur-les-matrices]], [[appliquer-regle-de-la-chaine]].

> [!SUCCESS]- Correction a)
> Soient $A,H\in E$. En développant **sans commuter** :
> $$(A+H)^3=A^3+\underbrace{A^2H+AHA+HA^2}_{L(H)}+\underbrace{AH^2+HAH+H^2A+H^3}_{r(H)}.$$
> - $L$ est linéaire en $H$ ; $E$ est de dimension finie, donc $L$ est continue (Th. 1.44).
> - $\lVert r(H)\rVert\le\lVert A\rVert\lVert H\rVert^2+\lVert H\rVert\lVert A\rVert\lVert H\rVert+\lVert H\rVert^2\lVert A\rVert+\lVert H\rVert^3=3\lVert A\rVert\lVert H\rVert^2+\lVert H\rVert^3$. Donc pour $H\ne0$ : $\dfrac{\lVert r(H)\rVert}{\lVert H\rVert}\le3\lVert A\rVert\lVert H\rVert+\lVert H\rVert^2\xrightarrow[H\to0]{}0$.
>
> Par définition, $f$ est différentiable en $A$ et $Df_A(H)=A^2H+AHA+HA^2$.

> [!SUCCESS]- Correction b)
> $g=\mathrm{tr}\circ f$. $\mathrm{tr}$ est linéaire, continue car $E$ est de dimension finie ; elle est donc différentiable et $D(\mathrm{tr})_B=\mathrm{tr}$ pour tout $B$ (Ex. 2.16). $f$ est différentiable en $A$ (question a). Par la règle de la chaîne (Th. 2.20), $g$ est différentiable en $A$ et
> $$Dg_A(H)=\mathrm{tr}\big(Df_A(H)\big)=\mathrm{tr}(A^2H)+\mathrm{tr}(AHA)+\mathrm{tr}(HA^2)=3\,\mathrm{tr}(A^2H),$$
> car $\mathrm{tr}(XY)=\mathrm{tr}(YX)$ donne $\mathrm{tr}(AHA)=\mathrm{tr}(A^2H)=\mathrm{tr}(HA^2)$.

---

## 6. Différentielle de XMX, deux méthodes

**Énoncé** (Écrit 2025-2026). Même cadre. On fixe $M\in E$ et $f(X)=XMX$.
a) Développer $f(A+H)$ ; en déduire que $f$ est différentiable en tout $A$ et donner $Df_A(H)$.
b) Retrouver ce résultat avec $f=p\circ q$, $p(X,Y)=XY$, $q(X)=(X,MX)$.

> [!SUCCESS]- Correction a)
> $f(A+H)=(A+H)M(A+H)=AMA+\underbrace{AMH+HMA}_{L(H)}+\underbrace{HMH}_{r(H)}$.
> $L$ est linéaire en $H$, continue (dimension finie). $\lVert r(H)\rVert\le\lVert M\rVert\lVert H\rVert^2$, donc $\frac{\lVert r(H)\rVert}{\lVert H\rVert}\le\lVert M\rVert\lVert H\rVert\to0$.
> Donc $f$ est différentiable en $A$ et $Df_A(H)=AMH+HMA$.

> [!SUCCESS]- Correction b)
> - $q:E\to E\times E$ est linéaire, continue (dimension finie) : différentiable, $Dq_A(H)=q(H)=(H,MH)$.
> - $p:E\times E\to E$ est bilinéaire, continue car $\lVert XY\rVert\le\lVert X\rVert\lVert Y\rVert$ : différentiable, $Dp_{(A,B)}(H,K)=HB+AK$ (Ex. 2.17).
> - Règle de la chaîne (Th. 2.20) : $f=p\circ q$ est différentiable en $A$ et
> $$Df_A(H)=Dp_{q(A)}\big(Dq_A(H)\big)=Dp_{(A,MA)}(H,MH)=H(MA)+A(MH)=HMA+AMH.$$
> On retrouve le résultat de a).

---

## 7. Différentielle de tr(X tX) et d'une composée

**Énoncé** (Écrit 2024-2025). $E=\mathcal M_n(\mathbb R)$. On rappelle que $\mathrm{tr}(B\,{}^t\!A)=\mathrm{tr}(A\,{}^t\!B)$.
a) $f(X)=\mathrm{tr}(X\,{}^t\!X)$. Développer $f(A+H)$, montrer que $f$ est différentiable et donner $Df_A(H)$.
b) $g(X)=\exp(-\mathrm{tr}(X\,{}^t\!X))$. Montrer que $g$ est différentiable et donner $Dg_A(H)$.

> [!SUCCESS]- Correction a)
> $f(A+H)=\mathrm{tr}\big((A+H)({}^t\!A+{}^t\!H)\big)=\mathrm{tr}(A\,{}^t\!A)+\mathrm{tr}(A\,{}^t\!H)+\mathrm{tr}(H\,{}^t\!A)+\mathrm{tr}(H\,{}^t\!H)$.
> Par le rappel, $\mathrm{tr}(H\,{}^t\!A)=\mathrm{tr}(A\,{}^t\!H)$. Donc $f(A+H)=f(A)+L(H)+r(H)$ avec
> $L(H)=2\,\mathrm{tr}(A\,{}^t\!H)$ et $r(H)=\mathrm{tr}(H\,{}^t\!H)$.
> - $L$ est linéaire en $H$, continue (dimension finie).
> - $H\mapsto{}^t\!H$ est linéaire continue : $\lVert {}^t\!H\rVert\le c_1\lVert H\rVert$ ; et $\lvert \mathrm{tr}(X)\rvert\le c\lVert X\rVert$. Donc $\lvert r(H)\rvert\le c\,\lVert H\rVert\,\lVert {}^t\!H\rVert\le c\,c_1\lVert H\rVert^2$, et $\frac{\lvert r(H)\rvert}{\lVert H\rVert}\to0$.
>
> Donc $f$ est différentiable en $A$ et $Df_A(H)=2\,\mathrm{tr}(A\,{}^t\!H)$.

> [!SUCCESS]- Correction b)
> $g=\varphi\circ f$ avec $\varphi(s)=e^{-s}$, dérivable sur $\mathbb R$ : $D\varphi_s(k)=\varphi'(s)\,k=-e^{-s}k$. $f$ est différentiable en $A$. Par la règle de la chaîne :
> $$Dg_A(H)=\varphi'(f(A))\,Df_A(H)=-2\,e^{-\mathrm{tr}(A\,{}^t\!A)}\,\mathrm{tr}(A\,{}^t\!H).$$

---

## 8. Étude en (0,0)

**Énoncé.** On pose $f(x,y)=\dfrac{xy^2}{x^2+y^2}$ et $g(x,y)=\dfrac{x^2y^2}{x^2+y^2}$ pour $(x,y)\ne(0,0)$, et $f(0,0)=g(0,0)=0$.
a) $f$ est-elle continue en $(0,0)$ ?
b) Calculer les dérivées partielles de $f$ en $(0,0)$.
c) $f$ est-elle différentiable en $(0,0)$ ?
d) Mêmes questions pour $g$.

Méthode : [[etudier-en-un-point-particulier]].

> [!SUCCESS]- Correction a)
> Pour $(x,y)\ne(0,0)$ : $y^2\le x^2+y^2$, donc $\lvert f(x,y)-f(0,0)\rvert=\abs x\dfrac{y^2}{x^2+y^2}\le\abs x\le\lVert (x,y)\rVert_\infty\xrightarrow[(x,y)\to(0,0)]{}0$.
> Donc $f$ est continue en $(0,0)$.

> [!SUCCESS]- Correction b)
> **Par la limite** (la formule n'est pas valable en $(0,0)$). Pour $t\ne0$ :
> $\dfrac{f(t,0)-f(0,0)}t=\dfrac{0-0}t=0\to0$, donc $\dfrac{\partial f}{\partial x}(0,0)=0$.
> $\dfrac{f(0,t)-f(0,0)}t=\dfrac{0-0}t=0\to0$, donc $\dfrac{\partial f}{\partial y}(0,0)=0$.

> [!SUCCESS]- Correction c)
> Si $f$ était différentiable en $(0,0)$, on aurait $Df_{(0,0)}(h)=h_1\partial_xf(0,0)+h_2\partial_yf(0,0)=0$ (Cor. 2.32), donc
> $\dfrac{\lvert f(h)-f(0,0)-0\rvert}{\lVert h\rVert_\infty}\to0$ quand $h\to0$. Or pour $h=(t,t)$, $t>0$ : $f(t,t)=\dfrac{t^3}{2t^2}=\dfrac t2$ et $\lVert h\rVert_\infty=t$, donc le quotient vaut $\frac12$, qui ne tend pas vers $0$. Contradiction : $f$ n'est **pas** différentiable en $(0,0)$.

> [!SUCCESS]- Correction d)
> $g(t,0)=g(0,t)=0$, donc $\partial_xg(0,0)=\partial_yg(0,0)=0$ : le seul candidat est $L=0$.
> Pour $h=(h_1,h_2)\ne(0,0)$ : $h_2^2\le h_1^2+h_2^2$, donc $\lvert g(h)-g(0,0)-L(h)\rvert=h_1^2\dfrac{h_2^2}{h_1^2+h_2^2}\le h_1^2\le\lVert h\rVert_\infty^2$, et
> $\dfrac{\lvert g(h)-g(0,0)-L(h)\rvert}{\lVert h\rVert_\infty}\le\lVert h\rVert_\infty\to0$.
> $L=0$ est linéaire continue : $g$ est différentiable en $(0,0)$ et $Dg_{(0,0)}=0$. En particulier $g$ est continue en $(0,0)$.

---

## 9. Classe C1, gradient, plan tangent

**Énoncé** (Écrit 2022-2023). $f(x,y)=x(\ln x)^2+y^2$.
a) Domaine de définition $U$ ; montrer que $U$ est ouvert.
b) Montrer que $f$ est $\mathcal C^1$ sur $U$ et calculer son gradient.
c) Équation du plan tangent à la surface $z=f(x,y)$ au point $(1,1,1)$.

> [!SUCCESS]- Correction a)
> $\ln x$ est défini pour $x>0$ : $U=\{(x,y)\in\mathbb R^2\mid x>0\}$. L'application $\pi_1:(x,y)\mapsto x$ est continue (linéaire en dimension finie) et $U=\{\pi_1>0\}$ : $U$ est ouvert.

> [!SUCCESS]- Correction b)
> En tout point de $U$ : $\dfrac{\partial f}{\partial x}(x,y)=(\ln x)^2+x\cdot2\ln x\cdot\dfrac1x=(\ln x)^2+2\ln x$ et $\dfrac{\partial f}{\partial y}(x,y)=2y$.
> Ces deux fonctions sont continues sur $U$, donc $f$ est $\mathcal C^1$ sur $U$ (Cor. 3.16) et
> $\nabla f(x,y)=\begin{pmatrix}(\ln x)^2+2\ln x\\2y\end{pmatrix}$.

> [!SUCCESS]- Correction c)
> $f(1,1)=1\cdot0+1=1$ (le point est bien sur la surface), $\nabla f(1,1)=\binom02$ (car $\ln1=0$).
> Plan tangent : $z=f(1,1)+\partial_xf(1,1)(x-1)+\partial_yf(1,1)(y-1)=1+2(y-1)$, soit $z=2y-1$.

---

## 10. Majorer la différentielle, lipschitzienne

**Énoncé** (Écrit 2025-2026). $\mathbb R^2$ est muni de $\lVert (x,y)\rVert_1=\abs x+\abs y$. Soit $f(x,y)=(\cos(x+2y),\sin(2x+y))$.
a) Montrer que $f$ est différentiable et calculer $J_f(x,y)$.
b) Montrer que $\lVert Df_{(x,y)}(h)\rVert_1\le3\lVert h\rVert_1$, puis $\lvert\!\lvert\!\lvert Df_{(x,y)}\rvert\!\rvert\!\rvert\le3$.
c) Montrer que $f$ est $3$-lipschitzienne sur $\mathbb R^2$.

Méthode : [[utiliser-iaf]].

> [!SUCCESS]- Correction a)
> Les composantes sont des composées de fonctions $\mathcal C^1$ : $f$ est $\mathcal C^1$, donc différentiable sur $\mathbb R^2$, et
> $$J_f(x,y)=\begin{pmatrix}-\sin(x+2y)&-2\sin(x+2y)\\2\cos(2x+y)&\cos(2x+y)\end{pmatrix}.$$

> [!SUCCESS]- Correction b)
> $Df_{(x,y)}(h)=J_f(x,y)h=\big(-\sin(x+2y)(h_1+2h_2),\ \cos(2x+y)(2h_1+h_2)\big)$. Comme $\lvert \sin\rvert\le1$ et $\lvert \cos\rvert\le1$ :
> $$\lVert Df_{(x,y)}(h)\rVert_1\le\lvert h_1+2h_2\rvert+\lvert 2h_1+h_2\rvert\le\lvert h_1\rvert+2\lvert h_2\rvert+2\lvert h_1\rvert+\lvert h_2\rvert=3\lVert h\rVert_1.$$
> $3$ est une constante $C$ telle que $\lVert Df_{(x,y)}(h)\rVert_1\le C\lVert h\rVert_1$ pour tout $h$ ; or $\lvert\!\lvert\!\lvert Df_{(x,y)}\rvert\!\rvert\!\rvert$ est la plus petite (Prop. 1.50 (ii)). Donc $\lvert\!\lvert\!\lvert Df_{(x,y)}\rvert\!\rvert\!\rvert\le3$.

> [!SUCCESS]- Correction c)
> $\mathbb R^2$ est un ouvert **convexe**, $f$ y est différentiable et $\lvert\!\lvert\!\lvert Df_x\rvert\!\rvert\!\rvert\le3$ pour tout $x\in\mathbb R^2$. D'après le Corollaire 3.13 (IAF sur un convexe), pour tous $a,b\in\mathbb R^2$ : $\lVert f(b)-f(a)\rVert_1\le3\lVert b-a\rVert_1$. Donc $f$ est $3$-lipschitzienne.

---

## 11. Points critiques et Taylor-Young

**Énoncé** (Écrit 2025-2026). $f(x,y)=x^3-3x+y^2$.
a) Justifier que $f$ est $\mathcal C^2$ ; donner son gradient et sa hessienne.
b) Points critiques et nature.
c) Écrire Taylor-Young à l'ordre 2 en $(1,0)$ et en $(-1,0)$ ; signe de $f(x,y)-f(\pm1,0)$ près de ces points.

Méthodes : [[etudier-points-critiques]], [[ecrire-taylor-young]].

> [!SUCCESS]- Correction a)
> $f$ est polynomiale, donc $\mathcal C^\infty$, en particulier $\mathcal C^2$ sur $\mathbb R^2$.
> $\nabla f(x,y)=\binom{3x^2-3}{2y}$, $H_f(x,y)=\begin{pmatrix}6x&0\\0&2\end{pmatrix}$.

> [!SUCCESS]- Correction b)
> $(x,y)$ est critique $\iff3x^2-3=0$ et $2y=0\iff x=\pm1$ et $y=0$. Points critiques : $(1,0)$ et $(-1,0)$.
>
> | point | $r$ | $s$ | $t$ | $rt-s^2$ | nature |
> |---|---|---|---|---|---|
> | $(1,0)$ | $6$ | $0$ | $2$ | $12>0$, $r>0$ | minimum local strict |
> | $(-1,0)$ | $-6$ | $0$ | $2$ | $-12<0$ | point-selle (pas d'extremum) |
>
> (Corollaire 4.25.)

> [!SUCCESS]- Correction c)
> **En $(1,0)$** : $f(1,0)=-2$, $Df_{(1,0)}=0$. Pour $h=(h_1,h_2)$ :
> $$f(1+h_1,h_2)=-2+\tfrac12(6h_1^2+2h_2^2)+\lVert h\rVert^2\varepsilon(h)=-2+3h_1^2+h_2^2+\lVert h\rVert^2\varepsilon(h),\quad\varepsilon(h)\to0.$$
> Avec la norme euclidienne, $3h_1^2+h_2^2\ge h_1^2+h_2^2=\lVert h\rVert^2$, donc $f(1+h_1,h_2)-f(1,0)\ge\lVert h\rVert^2(1+\varepsilon(h))>0$ pour $h\ne0$ assez petit : $f(x,y)-f(1,0)>0$ près de $(1,0)$.
> **En $(-1,0)$** : $f(-1,0)=2$, $Df_{(-1,0)}=0$ :
> $$f(-1+h_1,h_2)=2-3h_1^2+h_2^2+\lVert h\rVert^2\varepsilon(h).$$
> Pour $h=(h_1,0)$ : $f-2=h_1^2(-3+\varepsilon(h))<0$ pour $h_1\ne0$ petit. Pour $h=(0,h_2)$ : $f-2=h_2^2(1+\varepsilon(h))>0$. Donc $f(x,y)-f(-1,0)$ **n'a pas de signe constant** près de $(-1,0)$.

---

## 12. Points critiques, système à résoudre

**Énoncé** (Écrit 2024-2025). $f(x,y)=3xy-x^3-y^3$. Déterminer les points critiques de $f$ et leur nature.

> [!SUCCESS]- Correction
> $f$ est polynomiale donc $\mathcal C^2$ sur $\mathbb R^2$.
> **Points critiques.** $\partial_xf=3y-3x^2$ et $\partial_yf=3x-3y^2$.
> $$\begin{cases}3y-3x^2=0\\3x-3y^2=0\end{cases}\iff\begin{cases}y=x^2\\x=y^2\end{cases}$$
> En reportant la première dans la seconde : $x=x^4$, soit $x(x^3-1)=0$, donc $x=0$ ou $x=1$.
> - Si $x=0$ : $y=x^2=0$. Vérification : $3\cdot0-0=0$ ✔ et $0-0=0$ ✔.
> - Si $x=1$ : $y=1$. Vérification : $3-3=0$ ✔ et $3-3=0$ ✔.
>
> Points critiques : $(0,0)$ et $(1,1)$.
> **Nature.** $r=\partial^2_{xx}f=-6x$, $s=\partial^2_{xy}f=3$, $t=\partial^2_{yy}f=-6y$.
>
> | point | $r$ | $s$ | $t$ | $rt-s^2$ | nature |
> |---|---|---|---|---|---|
> | $(0,0)$ | $0$ | $3$ | $0$ | $-9<0$ | point-selle |
> | $(1,1)$ | $-6$ | $3$ | $-6$ | $27>0$, $r<0$ | maximum local strict, $f(1,1)=1$ |
>
> Ce maximum n'est pas global : $f(x,0)=-x^3\to+\infty$ quand $x\to-\infty$.

---

## 13. Le cas rt − s² = 0

**Énoncé.** $f(x,y)=x^4+y^4-2(x-y)^2$. Déterminer les points critiques de $f$ et leur nature.

> [!SUCCESS]- Correction
> $f$ est polynomiale donc $\mathcal C^2$.
> **Points critiques.** $\partial_xf=4x^3-4(x-y)$, $\partial_yf=4y^3+4(x-y)$.
> En **additionnant** les deux équations : $4x^3+4y^3=0$, donc $y^3=-x^3$, soit $y=-x$.
> En reportant dans la première : $4x^3-8x=0$, soit $4x(x^2-2)=0$ : $x=0$, $x=\sqrt2$ ou $x=-\sqrt2$.
> Points critiques : $(0,0)$, $(\sqrt2,-\sqrt2)$, $(-\sqrt2,\sqrt2)$ (on vérifie chacun dans les deux équations).
> **Dérivées secondes.** $r=12x^2-4$, $s=4$, $t=12y^2-4$.
> - En $(\pm\sqrt2,\mp\sqrt2)$ : $r=t=20$, $s=4$, $rt-s^2=384>0$ et $r>0$ : minimum local strict, de valeur $4+4-2(2\sqrt2)^2=-8$.
> - En $(0,0)$ : $r=t=-4$, $s=4$, $rt-s^2=0$ : **le critère ne conclut pas**. On étudie directement $f(h)-f(0,0)=f(h)$ :
>   - sur la droite $y=x$ : $f(x,x)=2x^4>0$ pour $x\ne0$ ;
>   - sur la droite $y=0$ : $f(x,0)=x^4-2x^2=x^2(x^2-2)<0$ pour $0<\abs x<\sqrt2$.
>
>   $f$ prend des valeurs $>0$ et $<0$ aussi près qu'on veut de $(0,0)$ : pas d'extremum en $(0,0)$.

---

## 14. Difféomorphisme local, pas global

**Énoncé.** $f:\mathbb R^2\to\mathbb R^2$, $f(x,y)=(e^x\cos y,\ e^x\sin y)$.
a) Montrer que $f$ est un difféomorphisme local en tout point de $\mathbb R^2$.
b) $f$ est-elle un difféomorphisme de $\mathbb R^2$ sur $f(\mathbb R^2)$ ?
c) Calculer la jacobienne de la réciproque locale de $f$ au point $f(0,0)=(1,0)$.

Méthode : [[montrer-diffeomorphisme]].

> [!SUCCESS]- Correction a)
> Les composantes de $f$ sont des produits de fonctions usuelles $\mathcal C^\infty$ : $f$ est $\mathcal C^1$ sur l'ouvert $\mathbb R^2$, à valeurs dans $\mathbb R^2$.
> $$J_f(x,y)=\begin{pmatrix}e^x\cos y&-e^x\sin y\\e^x\sin y&e^x\cos y\end{pmatrix},\qquad\det J_f(x,y)=e^{2x}(\cos^2y+\sin^2y)=e^{2x}\ne0.$$
> Par le théorème d'inversion locale, $f$ est un difféomorphisme local en tout point $(x,y)\in\mathbb R^2$.

> [!SUCCESS]- Correction b)
> Non : $f(0,0)=(1,0)=f(0,2\pi)$, donc $f$ n'est pas injective sur $\mathbb R^2$, donc pas bijective sur son image. (Le théorème d'inversion globale demande l'injectivité.)

> [!SUCCESS]- Correction c)
> $J_f(0,0)=\begin{pmatrix}1&0\\0&1\end{pmatrix}$, donc $J_{f^{-1}}(1,0)=[J_f(0,0)]^{-1}=\begin{pmatrix}1&0\\0&1\end{pmatrix}$ (Prop. 5.4).

---

## 15. Fonction implicite

**Énoncé.** Soit $f(x,y)=x^3+y^3-3xy-1$.
a) Montrer que la relation $f(x,y)=0$ définit, au voisinage de $(0,1)$, $y$ comme fonction $\varphi$ de $x$, de classe $\mathcal C^\infty$.
b) Calculer $\varphi'(0)$ et l'équation de la tangente à la courbe $f(x,y)=0$ en $(0,1)$.
c) Calculer $\varphi''(0)$ et donner le développement limité de $\varphi$ à l'ordre 2 en $0$.

Méthode : [[fonction-implicite]].

> [!SUCCESS]- Correction a)
> $f$ est polynomiale, donc $\mathcal C^\infty$ sur l'ouvert $\mathbb R^2$.
> $f(0,1)=0+1-0-1=0$.
> $\dfrac{\partial f}{\partial y}(x,y)=3y^2-3x$, donc $\dfrac{\partial f}{\partial y}(0,1)=3\ne0$.
> Par le théorème des fonctions implicites (Th. 5.15), il existe un intervalle ouvert $I$ contenant $0$, un voisinage ouvert $V$ de $(0,1)$ et $\varphi:I\to\mathbb R$ de classe $\mathcal C^\infty$ tels que, pour $(x,y)\in V$ : $f(x,y)=0\iff y=\varphi(x)$. De plus $\varphi(0)=1$.

> [!SUCCESS]- Correction b)
> $\dfrac{\partial f}{\partial x}(x,y)=3x^2-3y$, donc $\dfrac{\partial f}{\partial x}(0,1)=-3$.
> $\varphi'(0)=-\dfrac{\partial_xf(0,1)}{\partial_yf(0,1)}=-\dfrac{-3}3=1$.
> Tangente en $(0,1)$ : $y=\varphi(0)+\varphi'(0)(x-0)$, soit $y=1+x$.

> [!SUCCESS]- Correction c)
> Pour tout $x\in I$ : $f(x,\varphi(x))=0$. On dérive deux fois par rapport à $x$ :
> $$\partial^2_{xx}f+2\varphi'\,\partial^2_{xy}f+(\varphi')^2\,\partial^2_{yy}f+\varphi''\,\partial_yf=0\quad\text{en }(x,\varphi(x)).$$
> Or $\partial^2_{xx}f=6x$, $\partial^2_{xy}f=-3$, $\partial^2_{yy}f=6y$. En $x=0$ (point $(0,1)$, $\varphi'(0)=1$) :
> $0+2\cdot1\cdot(-3)+1\cdot6+3\varphi''(0)=0$, donc $\varphi''(0)=0$.
> Par Taylor-Young : $\varphi(x)=\varphi(0)+\varphi'(0)x+\frac{\varphi''(0)}2x^2+o(x^2)=1+x+o(x^2)$.
> (Vérification : $f(x,1+x)=x^3+(1+x)^3-3x(1+x)-1=2x^3$, bien négligeable devant $x^2$.)
