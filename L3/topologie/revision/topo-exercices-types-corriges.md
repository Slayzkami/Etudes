---
aliases:
  - "Exercices types corrigés topologie"
  - "corrections modèles topo"
  - "annales corrigées topologie"
tags:
  - topologie
  - topo/revision
---

# ✍️ Exercices types corrigés (rédactions modèles)

Les exercices qui reviennent dans les sujets (écrits 2022-23 et 2025-26, interros 2025-26 et 2026-27), rédigés comme sur une copie. **Mode d'emploi** : lire l'énoncé, chercher sur brouillon (5 à 10 min), puis seulement déplier la correction et comparer ligne par ligne. · [[topo-plan-de-revision|↩ Plan de révision]] · [[topo-index-definitions|↩ Index]]

> [!NOTE] Sommaire
> 1. [[#1. Une boule fermée est fermée]] *(écrit 2022-23, interro 2026-27)*
> 2. [[#2. Adhérence de la boule ouverte et distance discrète]] *(écrit 2022-23)*
> 3. [[#3. La somme A + B]] *(écrit 2022-23, interro 2025-26)*
> 4. [[#4. Les ensembles {f = g} et {f ≠ g}]] *(écrit 2022-23, écrit 2025-26)*
> 5. [[#5. Une partie de R – ouvert, fermé, adhérence, intérieur]]
> 6. [[#6. Une suite qui tend vers 0 (écrit 2025-26)]]
> 7. [[#7. La parabole (interro 2025-26)]]
> 8. [[#8. Distance induite sur une bande trouée]] *(écrit 2025-26)*
> 9. [[#9. Interro 2025-26 – la distance min(1, d)]]
> 10. [[#10. Une distance plus petite qu'une autre (écrit 2025-26)]]
> 11. [[#11. Interro 2026-27 – questions de cours]]
> 12. [[#12. Interro 2026-27 – exercices]]
> 13. [[#13. Un compact de R (interro 2025-26)]]
> 14. [[#14. Adhérence et intérieur d'une intersection, d'une réunion (écrit 2025-26)]]
> 15. [[#15. Distance à une partie et à un compact]] *(TD 2.13, § 3.8.2)*
> 16. [[#16. Ouverts et fermés de R²]] *(TD 2.18)*
> 17. [[#17. Continuité en (0,0)]] *(TD, Ex. 2.51)*
> 18. [[#18. Uniforme continuité de x²]]
> 19. [[#19. Compact de R² et maximum]]
> 20. [[#20. Une norme sur R² et sa boule unité]] *(TD 1.10)*
>
> Pour savoir quelle méthode sortir face à un énoncé : [[topo-reconnaitre-exercice]].

---

## 1. Une boule fermée est fermée

**Énoncé.** Soit $(X,d)$ un espace métrique, $x\in X$ et $r>0$. Montrer que $\bar B(x,r)=\{y\in X\mid d(y,x)\le r\}$ est une partie fermée de $X$.

Méthodes : [[topo-montrer-ouvert-ferme]] · Cours : [[topo-boule-fermee-fermee]].

> [!SUCCESS]- Correction (par les suites)
> Soit $(y_n)$ une suite de $\bar B(x,r)$ qui converge vers $y\in X$. Pour tout $n$, par l'inégalité triangulaire,
> $$d(x,y)\le d(x,y_n)+d(y_n,y)\le r+d(y_n,y).$$
> Quand $n\to+\infty$, $d(y_n,y)\to0$, donc $d(x,y)\le r$, c'est-à-dire $y\in\bar B(x,r)$.
> Toute suite de $\bar B(x,r)$ qui converge a sa limite dans $\bar B(x,r)$ : par la caractérisation séquentielle des fermés, **$\bar B(x,r)$ est fermée**.

> [!SUCCESS]- Correction (par le complémentaire, version du cours)
> Soit $z\notin\bar B(x,r)$ : $d(x,z)>r$. Posons $\rho=d(x,z)-r>0$. Si $y\in B(z,\rho)$, la seconde inégalité triangulaire donne
> $$d(x,y)\ge d(x,z)-d(z,y)>d(x,z)-\rho=r,$$
> donc $y\notin\bar B(x,r)$. Ainsi $B(z,\rho)\subset\bar B(x,r)^c$ : le complémentaire est ouvert, **$\bar B(x,r)$ est fermée**.

---

## 2. Adhérence de la boule ouverte et distance discrète

**Énoncé (écrit 2022-23, ex. 1).** Soit $(X,d)$ un espace métrique.
1. Montrer que $\overline{B(x,r)}\subset\bar B(x,r)$.
2. Donner un exemple où l'inclusion est une égalité.
3. On suppose que $X$ a au moins deux éléments et que $d$ est la distance discrète. (a) Montrer que toutes les parties de $X$ sont ouvertes et fermées. (b) Vérifier que l'inclusion peut être stricte.

Cours : [[topo-adherence]], [[topo-distance-discrete]].

> [!SUCCESS]- Correction
> **1.** $\bar B(x,r)$ est un fermé ([[#1. Une boule fermée est fermée|ex. 1]]) qui contient $B(x,r)$. Or $\overline{B(x,r)}$ est le plus petit fermé contenant $B(x,r)$, donc $\overline{B(x,r)}\subset\bar B(x,r)$.
>
> **2.** Dans $\mathbb R$ : $\overline{]x-r,x+r[}=[x-r,x+r]$. Plus généralement, dans un e.v.n., si $\|y-x\|=r$, la suite $y_n=x+(1-\frac1n)(y-x)$ vérifie $\|y_n-x\|=(1-\frac1n)r<r$ et $\|y_n-y\|=\frac rn\to0$ : $y\in\overline{B(x,r)}$.
>
> **3.(a)** Soit $A\subset X$ et $a\in A$ : $B(a,\frac12)=\{a\}\subset A$. Donc $A$ est ouvert. Son complémentaire, qui est aussi une partie de $X$, est ouvert : $A$ est fermé.
>
> **3.(b)** Soient $a\neq b$ dans $X$. $B(a,1)=\{y\mid d(a,y)<1\}=\{a\}$, qui est fermé (3.a), donc $\overline{B(a,1)}=\{a\}$. Mais $\bar B(a,1)=\{y\mid d(a,y)\le1\}=X\ni b$. Donc $\overline{B(a,1)}=\{a\}\subsetneq X=\bar B(a,1)$.

---

## 3. La somme A + B

**Énoncé.** Dans $\mathbb R^n$, $A+B=\{x+y\mid x\in A,\ y\in B\}$.
1. Si $A$ est compact et $B$ fermé, $A+B$ est fermé.
2. Si $A$ et $B$ sont compacts, $A+B$ est compact.
3. Donner deux fermés dont la somme n'est pas fermée.
4. (Écrit 2022-23) Si $A$ et $B$ sont ouverts, que dire de $A+B$ ?

Méthode : [[topo-somme-a-plus-b]].

> [!SUCCESS]- Correction
> **1.** Soit $z_k=a_k+b_k$ ($a_k\in A$, $b_k\in B$) une suite de $A+B$ qui converge vers $z$. Comme $A$ est compact, il existe $\varphi$ strictement croissante et $a\in A$ avec $a_{\varphi(k)}\to a$. Alors $b_{\varphi(k)}=z_{\varphi(k)}-a_{\varphi(k)}\to z-a$. Comme $B$ est fermé, $z-a\in B$. Donc $z=a+(z-a)\in A+B$ : **$A+B$ est fermé**.
>
> **2.** $A\times B$ est compact (produit de compacts) et $s:(x,y)\mapsto x+y$ est continue. Donc $A+B=s(A\times B)$ est compact (image continue d'un compact).
>
> **3.** Dans $\mathbb R$ : $A=\mathbb N$ et $B=\{-n+\frac1n\mid n\ge2\}$.
> – *$A$ et $B$ sont fermés* : deux éléments distincts de $A$ sont à distance $\ge1$ ; pour $B$, si $m>n\ge2$, $(-n+\frac1n)-(-m+\frac1m)=(m-n)+\frac1n-\frac1m\ge1$. Une suite convergente de $A$ (ou de $B$) est de Cauchy, donc ses termes finissent par être à distance $<1$, donc égaux : elle est stationnaire et sa limite est dans l'ensemble.
> – *$\frac1n\in A+B$* : $\frac1n=n+(-n+\frac1n)$ pour $n\ge2$, et $\frac1n\to0$.
> – *$0\notin A+B$* : si $0=m+(-n+\frac1n)$ avec $m\in\mathbb N$, $n\ge2$, alors $\frac1n=n-m\in\mathbb Z$, impossible car $0<\frac1n<1$.
> Donc **$A+B$ n'est pas fermé**.
>
> **4.** Si $A$ est ouvert, $A+B$ est **ouvert** (même si $B$ est quelconque) : $A+B=\bigcup_{b\in B}(A+b)$, et chaque translaté $A+b$ est ouvert (si $a\in A$ et $B(a,r)\subset A$, alors $B(a+b,r)=B(a,r)+b\subset A+b$). Une réunion d'ouverts est ouverte.

---

## 4. Les ensembles {f = g} et {f ≠ g}

**Énoncé.** (Écrit 2022-23) $X,Y$ espaces métriques, $f,g:X\to Y$ continues. Que dire de $E=\{x\in X\mid f(x)=g(x)\}$ ? (Écrit 2025-26) $f,g:E\to\mathbb R$ continues : $A=\{x\mid f(x)\neq g(x)\}$ est-il ouvert ? fermé ?

Méthode : [[topo-montrer-ouvert-ferme]] · Cours : [[topo-continuite-globale]].

> [!SUCCESS]- Correction
> **$E=\{f=g\}$ est fermé** (cas général, à valeurs dans $Y$ métrique). Soit $(x_n)$ une suite de $E$ qui converge vers $x\in X$. Par continuité, $f(x_n)\to f(x)$ et $g(x_n)\to g(x)$. Or $f(x_n)=g(x_n)$ pour tout $n$ : par unicité de la limite dans $Y$, $f(x)=g(x)$, donc $x\in E$. Par la caractérisation séquentielle, $E$ est fermé.
>
> **Cas réel.** $h=f-g$ est continue, $\{f=g\}=h^{-1}(\{0\})$ est fermé et $\{f\neq g\}=h^{-1}(\mathbb R\setminus\{0\})$ est **ouvert** (image réciproque d'un ouvert). C'est aussi le complémentaire du fermé $\{f=g\}$.
> En général $\{f\neq g\}$ **n'est pas fermé** : $f(x)=x$, $g=0$ sur $\mathbb R$ donnent $\mathbb R^*$, non fermé ($\frac1n\to0$).

---

## 5. Une partie de R – ouvert, fermé, adhérence, intérieur

**Énoncé.** Pour $A=]0,1]\cup\{2\}$ dans $(\mathbb R,|\cdot|)$ : ouvert ? fermé ? adhérence, intérieur, frontière.

Méthodes : [[topo-montrer-pas-ouvert-pas-ferme]], [[topo-calculer-interieur-adherence-frontiere]].

> [!SUCCESS]- Correction
> **Pas ouvert.** Pour $n\in\mathbb N^*$, $y_n=2+\frac1n\notin A$ (car $2<y_n\le3$) et $y_n\to2\in A$. Une suite hors de $A$ converge vers un point de $A$ : $A^c$ n'est pas fermé, donc **$A$ n'est pas ouvert**.
> **Pas fermé.** Pour $n\in\mathbb N^*$, $x_n=\frac1n\in A$ (car $0<x_n\le1$) et $x_n\to0\notin A$ : **$A$ n'est pas fermé**.
> **Adhérence.** $0=\lim x_n$ avec $x_n\in A$, donc $A\cup\{0\}=[0,1]\cup\{2\}\subset\bar A$. Inversement, $[0,1]\cup\{2\}$ est fermé (réunion **finie** de fermés) et contient $A$, donc $\bar A\subset[0,1]\cup\{2\}$. Ainsi **$\bar A=[0,1]\cup\{2\}$**.
> **Intérieur.** $]0,1[$ est ouvert et contenu dans $A$, donc $]0,1[\subset\operatorname{Int}A$. Les autres points de $A$ sont $1$ et $2$ : $1=\lim(1+\frac1{n+1})$ avec $1+\frac1{n+1}\in]1,2[$, hors de $A$ ; $2=\lim(2+\frac1n)$ avec $2+\frac1n\notin A$. Ils ne sont pas intérieurs. **$\operatorname{Int}A=]0,1[$**.
> **Frontière.** $\operatorname{Fr}A=\bar A\setminus\operatorname{Int}A=\{0,1,2\}$.

> [!TIP] Variantes à refaire seul
> $[1,2[\cup\{5\}$ (adh. $[1,2]\cup\{5\}$, int. $]1,2[$, fr. $\{1,2,5\}$) ; $]0,+\infty[$ (ouvert, adh. $[0,+\infty[$, fr. $\{0\}$) ; $\mathbb Z$ (fermé, int. $\emptyset$, fr. $\mathbb Z$) ; $\mathbb Q$ (adh. $\mathbb R$, int. $\emptyset$).

---

## 6. Une suite qui tend vers 0 (écrit 2025-26)

**Énoncé.** $A=\{e^{-n}\mid n\in\mathbb N\}$ dans $(\mathbb R,|\cdot|)$ : ouvert ? fermé ? adhérence et intérieur.

> [!SUCCESS]- Correction
> **Pas ouvert.** $1=e^0\in A$, et $1+\frac1k\notin A$ (car $A\subset]0,1]$) tend vers $1$.
> **Pas fermé.** $e^{-n}\in A$ et $e^{-n}\to0\notin A$ (car $e^{-n}>0$).
> **Adhérence : $\bar A=A\cup\{0\}$.** ($\supset$) $0=\lim e^{-n}$. ($\subset$) $A\cup\{0\}$ est fermé : son complémentaire
> $$]-\infty,0[\ \cup\ ]1,+\infty[\ \cup\ \bigcup_{n\ge0}\,]e^{-(n+1)},e^{-n}[$$
> est une réunion d'ouverts (un réel de $]0,1[$ qui n'est pas un $e^{-n}$ est strictement entre deux termes consécutifs, car $(e^{-n})$ décroît vers $0$). Il contient $A$, donc $\bar A\subset A\cup\{0\}$.
> **Intérieur : $\emptyset$.** Soit $a=e^{-n}\in A$. Si $n\ge1$, les réels $z_k=e^{-n}+\frac1k\big(e^{-(n-1)}-e^{-n}\big)$ ($k\ge2$) sont strictement entre les deux termes consécutifs $e^{-n}$ et $e^{-(n-1)}$, donc hors de $A$, et $z_k\to e^{-n}$. Si $n=0$, $1+\frac1k\notin A$ tend vers $1$. Aucun point de $A$ n'est intérieur.

---

## 7. La parabole (interro 2025-26)

**Énoncé.** $X=\{(x,y)\in\mathbb R^2\mid x>0,\ y=x^2\}$. 1. $X$ n'est ni ouvert ni fermé. 2. Adhérence et intérieur.

Méthodes : [[topo-montrer-pas-ouvert-pas-ferme]], [[topo-calculer-interieur-adherence-frontiere]].

> [!SUCCESS]- Correction
> Toutes les normes de $\mathbb R^2$ sont équivalentes : on prend la distance euclidienne.
> **Pas fermé.** $u_n=(\frac1n,\frac1{n^2})\in X$ (car $\frac1n>0$ et $\frac1{n^2}=(\frac1n)^2$), et $u_n\to(0,0)\notin X$ (on n'a pas $0>0$).
> **Pas ouvert.** $v_n=(1,1+\frac1n)\notin X$ car $1+\frac1n\neq1=1^2$ ; et $v_n\to(1,1)\in X$. Le complémentaire n'est pas fermé.
> **Adhérence : $\bar X=F=\{(x,y)\mid x\ge0,\ y=x^2\}$.** ($F\subset\bar X$) $F=X\cup\{(0,0)\}$ et $(0,0)=\lim u_n$. ($\bar X\subset F$) $g(x,y)=y-x^2$ et $h(x,y)=x$ sont continues ; $F=g^{-1}(\{0\})\cap h^{-1}([0,+\infty[)$ est une intersection de fermés : fermé, et il contient $X$.
> **Intérieur : $\emptyset$.** Tout $p=(a,a^2)\in X$ est limite de $p_n=(a,a^2+\frac1n)\notin X$ ; si $B(p,r)\subset X$, on aurait $p_n\in X$ pour $n$ grand : absurde.

---

## 8. Distance induite sur une bande trouée

**Énoncé (écrit 2025-26, ex. 2).** Dans $\mathbb R^2$, $I=([-1,0[\cup]0,1])\times\mathbb R$.
1. $I$ n'est ni ouvert ni fermé. 2. Adhérence et intérieur. 3. On munit $I$ de la distance induite. (a) Expliciter $B_I(A,1)$, $A=(1,0)$. (b) $[-1,0[\times\mathbb R$ est un fermé de $I$. (c) $]0,1]\times\mathbb R$ est un ouvert de $I$. (d) Une partie propre non vide de $I$ ouverte et fermée dans $I$.

Méthode : [[topo-distance-induite-ouverts-relatifs]].

> [!SUCCESS]- Correction
> **1.** *Pas ouvert* : $(1,0)\in I$, et $(1+\frac1n,0)\notin I$ tend vers $(1,0)$. *Pas fermé* : $(\frac1n,0)\in I$ tend vers $(0,0)\notin I$.
> **2.** *Adhérence* $[-1,1]\times\mathbb R$ : fermé (image réciproque de $[-1,1]$ par $(x,y)\mapsto x$) contenant $I$ ; et $(0,y)=\lim(\frac1n,y)$, $(\pm1,y)\in I$. *Intérieur* $(]-1,0[\cup]0,1[)\times\mathbb R$ : ouvert contenu dans $I$ ; les points $(\pm1,y)$ sont limites de $(\pm(1+\frac1n),y)\notin I$.
> **3.(a)** $B_I(A,1)=B(A,1)\cap I=\{(x,y)\mid(x-1)^2+y^2<1\}\cap I$. Dans le disque, $0<x<2$ ; avec $x\le1$ : $B_I(A,1)=\{(x,y)\mid(x-1)^2+y^2<1,\ 0<x\le1\}$, un demi-disque ouvert dont le bord vertical $\{x=1\}$ est inclus.
> **3.(b)** Soit $(x_n,y_n)\in[-1,0[\times\mathbb R$ qui converge vers $(a,b)\in I$. Alors $x_n\to a$ avec $x_n<0$, donc $a\le0$ ; comme $(a,b)\in I$, $a\neq0$, donc $a\in[-1,0[$. La limite est dans $[-1,0[\times\mathbb R$ : c'est un fermé de $I$.
> **3.(c)** $]0,1]\times\mathbb R$ est le complémentaire dans $I$ du fermé de $I$ précédent : c'est un ouvert de $I$. (Ou : pour $p=(x,y)$ avec $x\in]0,1]$, $B_I(p,x)\subset]0,1]\times\mathbb R$.)
> **3.(d)** $J=[-1,0[\times\mathbb R$ : fermé de $I$ par (b), et ouvert de $I$ car son complémentaire $]0,1]\times\mathbb R$ est fermé de $I$ (même raisonnement que (b)).

---

## 9. Interro 2025-26 – la distance min(1, d)

**Énoncé.** $\delta(x,y)=\inf(1,d(x,y))$. 1. $\delta$ est une distance. 2. $E=\mathbb R^2$, $d=d_2$ : boules ouvertes et fermées de $(\mathbb R^2,\delta)$.

Méthodes : [[topo-montrer-distance]], [[topo-determiner-boule]].

> [!SUCCESS]- Correction
> **1.** *Séparation* : $\delta\ge0$ ; si $\delta(x,y)=0$, comme $1\neq0$, $d(x,y)=0$ donc $x=y$ ; $\delta(x,x)=0$. *Symétrie* : héritée de $d$. *Inégalité triangulaire* : si $d(x,y)\ge1$ ou $d(y,z)\ge1$, $\delta(x,y)+\delta(y,z)\ge1\ge\delta(x,z)$ ; sinon $\delta(x,y)+\delta(y,z)=d(x,y)+d(y,z)\ge d(x,z)\ge\delta(x,z)$.
> **2.** On utilise $\min(1,t)<r\iff(1<r$ ou $t<r)$.
> – $r\le1$ : $B_\delta(a,r)=B_2(a,r)$ (disque ouvert) ; $r>1$ : $B_\delta(a,r)=\mathbb R^2$.
> – $r<1$ : $\bar B_\delta(a,r)=\bar B_2(a,r)$ (disque fermé) ; $r\ge1$ : $\bar B_\delta(a,r)=\mathbb R^2$.
> **Complément (TD 2.12)** : $\delta$ et $d$ ont les mêmes boules de rayon $\le1$, donc sont topologiquement équivalentes (critère des boules) ; pas métriquement équivalentes car $\mathbb R^2$ est borné pour $\delta$ et pas pour $d_2$.

---

## 10. Une distance plus petite qu'une autre (écrit 2025-26)

**Énoncé.** $(E,d)$ métrique, $\delta$ distance avec $\delta\le k\,d$ ($k>0$). 1. Toute boule de $\delta$ contient une boule de $d$ (même centre). 2. Tout ouvert de $\delta$ est un ouvert de $d$ ; et les fermés ? 3. Sur $E=[0,1]$ avec $\delta$ usuelle, trouver $d$ vérifiant l'hypothèse et un ouvert de $d$ qui n'est pas un ouvert de $\delta$.

Méthode : [[topo-comparer-distances]].

> [!SUCCESS]- Correction
> **1.** Si $d(a,x)<\frac rk$, alors $\delta(a,x)\le k\,d(a,x)<r$ : $B_d(a,\frac rk)\subset B_\delta(a,r)$. Idem avec $\le$ pour les boules fermées.
> **2.** Soit $O$ un ouvert de $\delta$ et $a\in O$ : il existe $r>0$ avec $B_\delta(a,r)\subset O$, donc $B_d(a,\frac rk)\subset O$ : $O$ est un ouvert de $d$. Si $F$ est un fermé de $\delta$, $F^c$ est un ouvert de $\delta$, donc de $d$ : **$F$ est un fermé de $d$**.
> **3.** $d$ = distance discrète sur $[0,1]$. Pour $x\neq y$, $\delta(x,y)=|x-y|\le1=d(x,y)$ : hypothèse vérifiée avec $k=1$. $\{0\}=B_d(0,\frac12)$ est ouvert pour $d$, mais pas pour $\delta$ : $\frac1n\notin\{0\}$ et $\frac1n\to0$.

---

## 11. Interro 2026-27 – questions de cours

**Énoncé.** 1. Un espace métrique $E\subset\mathbb R^3$, $E\neq\mathbb R^3$. 2. Existe-t-il une norme $N$ sur $\mathbb R^2$ dont la distance discrète serait la distance associée ? 3. Toute boule fermée est fermée. 4. $V$ voisinage de $a$ $\iff\exists r>0,\ B(a,r)\subset V$. 5. Si $\tilde d$ est métriquement équivalente à $d$, tout fermé de $(E,d)$ est un fermé de $(E,\tilde d)$ ; que peut-on en déduire ?

> [!SUCCESS]- Correction
> **1.** $E=\{x\in\mathbb R^3\mid\|x\|_2<1\}$ avec la distance induite $d(x,y)=\|x-y\|_2$ : c'est un espace métrique (restriction d'une distance), et $(2,0,0)\notin E$.
> **2. Non.** Si $N(x-y)=d(x,y)$ (distance discrète), pour $x=(1,0)$ : $N(x)=1$ et $N(\frac x2)=1$ (car $\frac x2\neq0$). Mais (N2) impose $N(\frac x2)=\frac12N(x)=\frac12$ : contradiction.
> **3.** Voir [[#1. Une boule fermée est fermée|ex. 1]].
> **4.** Par définition, $V$ est un voisinage de $a$ s'il existe un ouvert $O$ avec $a\in O\subset V$. ($\Rightarrow$) $O$ est ouvert et $a\in O$ : il existe $r>0$ avec $B(a,r)\subset O\subset V$. ($\Leftarrow$) $B(a,r)$ est un ouvert (boule ouverte) qui contient $a$ et est contenu dans $V$.
> **5.** $\alpha d\le\tilde d\le\beta d$. Soit $F$ fermé pour $d$ et $(x_n)$ une suite de $F$ qui converge vers $x$ pour $\tilde d$. Alors $d(x_n,x)\le\frac1\alpha\tilde d(x_n,x)\to0$ : $x_n\to x$ pour $d$, donc $x\in F$. $F$ est fermé pour $\tilde d$. **Déduction** : comme $\frac1\beta\tilde d\le d\le\frac1\alpha\tilde d$, les rôles sont symétriques : mêmes fermés, donc (complémentaires) mêmes ouverts : $d$ et $\tilde d$ sont **topologiquement équivalentes**.

---

## 12. Interro 2026-27 – exercices

**Énoncé.**
- *Ex. 1.* $X=\{(x,y)\mid x+y>0,\ y=e^{x^2}\}$ : « montrer » que $X$ n'est ni ouvert ni fermé ; adhérence et intérieur.
- *Ex. 2.* $(X,d)$ métrique, $Y\subset X$ : $\operatorname{int}(X\setminus Y)=X\setminus\bar Y$ ; en déduire $\overline{X\setminus Y}=X\setminus\operatorname{int}Y$.
- *Ex. 3.* $X=\{(0,e^{-n})\mid n\in\mathbb N^*\}\subset\mathbb R^2$ : ouvert ? fermé ? intérieur, adhérence.

> [!SUCCESS]- Correction de l'ex. 1 (attention : énoncé erroné)
> La condition $x+y>0$ est **toujours vraie** sur la courbe : $e^t\ge1+t$ donne $e^{x^2}\ge1+x^2$, et $1+x^2-|x|=(|x|-\frac12)^2+\frac34>0$, donc $e^{x^2}>|x|\ge-x$. Ainsi $X=\{y=e^{x^2}\}$ est le graphe entier.
> **$X$ est fermé** : $X=h^{-1}(\{0\})$ avec $h(x,y)=y-e^{x^2}$ continue. **Pas ouvert** : $(0,1+\frac1n)\notin X$ tend vers $(0,1)\in X$.
> **$\bar X=X$** (fermé) ; **$\operatorname{Int}X=\emptyset$** : $(a,e^{a^2}+\frac1n)\notin X$ tend vers $(a,e^{a^2})$.
> Sur la copie : signaler que l'énoncé ne peut pas être démontré, et montrer ce qui est vrai.

> [!SUCCESS]- Correction de l'ex. 2
> **($\supset$)** $X\setminus\bar Y$ est ouvert (complémentaire d'un fermé) et contenu dans $X\setminus Y$ (car $Y\subset\bar Y$). Comme $\operatorname{int}(X\setminus Y)$ est le plus grand ouvert contenu dans $X\setminus Y$ : $X\setminus\bar Y\subset\operatorname{int}(X\setminus Y)$.
> **($\subset$)** $F=X\setminus\operatorname{int}(X\setminus Y)$ est fermé (complémentaire d'un ouvert) et contient $Y$ (car $\operatorname{int}(X\setminus Y)\subset X\setminus Y$). Comme $\bar Y$ est le plus petit fermé contenant $Y$ : $\bar Y\subset F$, c'est-à-dire $\operatorname{int}(X\setminus Y)\subset X\setminus\bar Y$.
> **Déduction.** On applique le résultat à $Z=X\setminus Y$ : $X\setminus Z=Y$, donc $\operatorname{int}Y=X\setminus\overline{X\setminus Y}$. En passant au complémentaire : $\overline{X\setminus Y}=X\setminus\operatorname{int}Y$.

> [!SUCCESS]- Correction de l'ex. 3
> **Pas ouvert** : $(\frac1k,e^{-1})\notin X$ (abscisse non nulle) tend vers $(0,e^{-1})\in X$. **Pas fermé** : $(0,e^{-n})\in X$ tend vers $(0,0)\notin X$.
> **Intérieur** $\emptyset$ : $(0,e^{-n})=\lim_k(\frac1k,e^{-n})$ avec $(\frac1k,e^{-n})\notin X$.
> **Adhérence** $X\cup\{(0,0)\}$. ($\supset$) $(0,0)=\lim(0,e^{-n})$. ($\subset$) $C=\{e^{-n}\mid n\ge1\}\cup\{0\}$ est fermé dans $\mathbb R$ (complémentaire réunion d'intervalles ouverts) ; si $(0,b_k)\in X\cup\{(0,0)\}$ converge vers $(a,b)$, alors $a=0$ et $b_k\to b$ avec $b_k\in C$, donc $b\in C$. $X\cup\{(0,0)\}$ est fermé et contient $X$.

---

## 13. Un compact de R (interro 2025-26)

**Énoncé.** $X=\{\frac1n\mid n\in\mathbb N^*\}\cup\{0\}$ muni de la distance induite. 1. $X$ est compact. 2. En déduire qu'un compact de $\mathbb R$ n'est pas forcément une réunion finie d'intervalles fermés.

Méthode : [[topo-montrer-compact]].

> [!SUCCESS]- Correction
> **1.** *Borné* : $X\subset[0,1]$. *Fermé* : $\mathbb R\setminus X=]-\infty,0[\cup]1,+\infty[\cup\bigcup_{n\ge1}]\frac1{n+1},\frac1n[$ est une réunion d'ouverts. Fermé et borné dans $\mathbb R$ : $X$ est une partie compacte de $\mathbb R$ (Borel–Lebesgue), donc $(X,d)$ est un espace compact.
> *(Autre preuve, Ex. 3.10 : une suite convergente et sa limite forment un compact.)*
> **2.** Supposons $X=I_1\cup\dots\cup I_p$, $I_k$ intervalles fermés. Si un $I_k$ contenait deux points $a<b$ de $X$ : $b\neq0$ donc $b=\frac1m$, et $a\le\frac1{m+1}$ ; alors $]\frac1{m+1},\frac1m[\subset[a,b]\subset I_k\subset X$, alors que cet intervalle ne contient aucun point de $X$ : absurde. Chaque $I_k$ est un singleton, donc $X$ serait fini : contradiction, $X$ est infini.

> [!WARNING] Erreur à ne pas faire
> « $X=\bigcup_n\{\frac1n\}\cup\{0\}$ est une réunion de fermés, donc fermé » : **faux**, la réunion est infinie (→ [[topo-mes-erreurs]]).

---

## 14. Adhérence et intérieur d'une intersection, d'une réunion (écrit 2025-26)

**Énoncé.** Montrer $\overline{A\cap B}\subset\bar A\cap\bar B$ ; exemple d'inclusion stricte. Que dire de $\operatorname{Int}(A\cup B)$ ? Exemple.

> [!SUCCESS]- Correction
> **Adhérence.** $A\cap B\subset A\subset\bar A$, fermé, donc $\overline{A\cap B}\subset\bar A$ (plus petit fermé) ; de même $\subset\bar B$. Stricte : $A=\mathbb Q$, $B=\mathbb R\setminus\mathbb Q$ : $\overline{A\cap B}=\overline{\emptyset}=\emptyset$ et $\bar A\cap\bar B=\mathbb R$.
> **Intérieur.** $\operatorname{Int}A$ est un ouvert contenu dans $A\subset A\cup B$, donc $\operatorname{Int}A\subset\operatorname{Int}(A\cup B)$ ; de même pour $B$ : $\operatorname{Int}A\cup\operatorname{Int}B\subset\operatorname{Int}(A\cup B)$. Stricte : $A=[0,1]$, $B=[1,2]$ : $1\in\operatorname{Int}(A\cup B)=]0,2[$ mais $1\notin]0,1[\cup]1,2[$.
> **À savoir aussi** : $\overline{A\cup B}=\bar A\cup\bar B$ (réunion **finie** de fermés) et $\operatorname{Int}(A\cap B)=\operatorname{Int}A\cap\operatorname{Int}B$ (intersection **finie** d'ouverts).

---

## 15. Distance à une partie et à un compact

**Énoncé.** 1. $|d(x,A)-d(y,A)|\le d(x,y)$. 2. $d(x,A)=0\iff x\in\bar A$. 3. $K$ compact, $F$ fermé, $K\cap F=\emptyset$ $\Rightarrow d(K,F)>0$ ; faux avec $K$ seulement fermé.

Cours : [[topo-distance-a-une-partie]], [[topo-bornes-atteintes]].

> [!SUCCESS]- Correction
> **1.** Pour $a\in A$ : $d(x,A)\le d(x,a)\le d(x,y)+d(y,a)$ ; en passant à l'inf sur $a$ : $d(x,A)\le d(x,y)+d(y,A)$. On échange $x$ et $y$. Donc $x\mapsto d(x,A)$ est 1-lipschitzienne, donc continue.
> **2.** $d(x,A)=0\iff\forall r>0,\ \exists a\in A,\ d(x,a)<r\iff\forall r>0,\ B(x,r)\cap A\neq\emptyset\iff x\in\bar A$.
> **3.** $g(k)=d(k,F)$ est continue sur le compact $K$ : elle atteint son minimum en $k_1$. $k_1\notin F=\bar F$, donc $d(k_1,F)>0$, et $d(K,F)=\inf_kd(k,F)=d(k_1,F)>0$. Contre-exemple : $A=\{n\mid n\ge2\}$ et $B=\{n+\frac1n\mid n\ge2\}$ fermés disjoints avec $d(n,n+\frac1n)=\frac1n\to0$.

---

## 16. Ouverts et fermés de R²

**Énoncé (TD 2.18).** Ouverts ? fermés ? $A=\{-1<x<1,\ -1<y<1\}$, $C=\{-1\le x\le1\}$, $D=\{x^2+y^2\neq1\}$, $E=\{x^2-y^2\le1\}$.

> [!SUCCESS]- Correction
> - $A=\pi_1^{-1}(]-1,1[)\cap\pi_2^{-1}(]-1,1[)$ **ouvert** ; pas fermé : $(1-\frac1n,0)\in A\to(1,0)\notin A$.
> - $C=\pi_1^{-1}([-1,1])$ **fermé** ; pas ouvert : $(1+\frac1n,0)\notin C\to(1,0)\in C$.
> - $D=\varphi^{-1}(\mathbb R\setminus\{1\})$, $\varphi=x^2+y^2$ : **ouvert** ; pas fermé : $(1-\frac1n,0)\in D\to(1,0)\notin D$.
> - $E=\psi^{-1}(]-\infty,1])$, $\psi=x^2-y^2$ : **fermé** ; pas ouvert : $(1+\frac1n,0)\notin E\to(1,0)\in E$.

---

## 17. Continuité en (0,0)

**Énoncé.** Continuité en $(0,0)$ de $f=\frac{xy}{x^2+y^2}$, $g=\frac{x^2y}{x^2+y^2}$ (prolongées par $0$).

Méthode : [[topo-continuite-deux-variables]].

> [!SUCCESS]- Correction
> **$f$** : $(\frac1n,\frac1n)\to(0,0)$ mais $f(\frac1n,\frac1n)=\frac12\not\to0$ : **pas continue** (alors que $f(x,0)=f(0,y)=0$ : applications partielles continues).
> **$g$** : $x^2\le x^2+y^2$ donne $|g(x,y)|\le|y|\le\|(x,y)\|_2\to0$ : **continue** en $(0,0)$ ; ailleurs, quotient de polynômes à dénominateur non nul.

---

## 18. Uniforme continuité de x²

**Énoncé.** $u(x)=x^2$. 1. $u$ n'est pas U.C. sur $\mathbb R$. 2. $u$ est U.C. sur $[-a,a]$ (deux façons).

Méthode : [[topo-uniforme-continuite]].

> [!SUCCESS]- Correction
> **1.** $x_n=n$, $y_n=n+\frac1n$ : $|x_n-y_n|=\frac1n\to0$ mais $|u(y_n)-u(x_n)|=2+\frac1{n^2}\ge2$. La définition échoue pour $\varepsilon=2$.
> **2.** $[-a,a]$ est compact (fermé borné de $\mathbb R$) et $u$ continue : U.C. par **Heine**. Directement : $|x^2-y^2|=|x+y||x-y|\le2a|x-y|$ : $u$ est $2a$-lipschitzienne, donc U.C.

---

## 19. Compact de R² et maximum

**Énoncé.** $K=\{(x,y)\mid|x|+|y|\le1\}$. 1. $K$ est compact. 2. $f(x,y)=xy$ atteint ses bornes ; calculer $\max_Kf$.

Méthodes : [[topo-montrer-compact]], [[topo-exploiter-compacite]].

> [!SUCCESS]- Correction
> **1.** $K=\|\cdot\|_1^{-1}([0,1])$ est fermé ($\|\cdot\|_1$ continue) et borné ($\|\cdot\|_\infty\le\|\cdot\|_1\le1$) : compact (fermé borné de $\mathbb R^2$).
> **2.** $f$ est continue (polynomiale) sur le compact $K$ : bornée et atteint ses bornes. Sur $K$ : $(|x|-|y|)^2\ge0$ donne $4|x||y|\le(|x|+|y|)^2\le1$, donc $xy\le\frac14$, avec égalité en $(\frac12,\frac12)\in K$. $\max_Kf=\frac14$ (et $\min_Kf=-\frac14$ en $(\frac12,-\frac12)$).

---

## 20. Une norme sur R² et sa boule unité

**Énoncé (TD 1.10).** $N(x,y)=\max(|x+y|,|x-2y|)$ : norme ? boule unité fermée ?

Méthodes : [[topo-montrer-norme]], [[topo-determiner-boule]].

> [!SUCCESS]- Correction
> Avec $A=\begin{pmatrix}1&1\\1&-2\end{pmatrix}$ ($\det A=-3\neq0$), $N(v)=\|Av\|_\infty$ : (N1) par injectivité de $A$, (N2) et (N3) par linéarité et propriétés de $\|\cdot\|_\infty$.
> $\bar B_N(0,1)=\{|x+y|\le1\}\cap\{|x-2y|\le1\}$ : parallélogramme de sommets $(1,0)$, $(\frac13,\frac23)$, $(-1,0)$, $(-\frac13,-\frac23)$ (intersections des droites $x+y=\pm1$ et $x-2y=\pm1$).
