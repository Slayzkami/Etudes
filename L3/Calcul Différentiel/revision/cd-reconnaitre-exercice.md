---
aliases:
  - "Reconnaître le type d'exercice CD"
  - "quelle méthode utiliser en calcul différentiel"
  - "types d'exercices CD"
tags:
  - cd
  - cd/revision
---

# 🧭 Reconnaître le type d'exercice

« L'énoncé dit ça → je sors cette méthode → je commence par cette phrase. » · [[cd-plan-de-revision|↩ Plan de révision]] · [[cd-index-definitions|↩ Index]]

## 1 – Normes et applications linéaires continues

| L'énoncé demande… | Méthode | Première phrase sur la copie | Corrigé |
|---|---|---|---|
| Montrer que $N$ est une norme | [[montrer-norme]] | « $N$ est bien définie et positive. Séparation : soit $x$ tel que $N(x)=0$… » | [[cd-exercices-types-corriges#1. Montrer qu'une application est une norme\|ex. 1]] |
| Montrer que deux normes sont / ne sont pas équivalentes | [[montrer-normes-equivalentes]] | « $E$ est de dimension finie, donc… » ou « Posons $u_n(t)=t^n$… » | [[cd-exercices-types-corriges#2. Normes non équivalentes, forme linéaire non continue\|ex. 2]] |
| Justifier l'existence de $C$ tel que $\lVert \varphi(x)\rVert\le C\lVert x\rVert$ | [[continuite-application-lineaire]] | « $\varphi$ est linéaire et $E$ est de dimension finie, donc $\varphi$ est continue (Th. 1.44) ; par le Th. 1.43… » | [[cd-exercices-types-corriges#1. Montrer qu'une application est une norme\|ex. 1 c)]] |
| Cette application linéaire est-elle continue ? | [[continuite-application-lineaire]] | « $L$ est linéaire. Pour tout $u$, $\lVert L(u)\rVert\le\dots$ » | [[cd-exercices-types-corriges#2. Normes non équivalentes, forme linéaire non continue\|ex. 2 c)]] |
| Calculer $\lvert\!\lvert\!\lvert u\rvert\!\rvert\!\rvert$ | [[calculer-norme-operateur]] | « Majoration : soit $x\in E$… » puis « Atteinte : pour $x_0=\dots$ » | [[cd-exercices-types-corriges#3. Norme d'opérateur d'une matrice\|ex. 3]] |
| Montrer qu'une partie est ouverte / fermée | [[montrer-ouvert-ferme]] | « $g$ est continue et $U=\{g>0\}$… » | [[cd-exercices-types-corriges#9. Classe C1, gradient, plan tangent\|ex. 9 a)]] |

## 2 – Différentiabilité

| L'énoncé demande… | Méthode | Première phrase sur la copie | Corrigé |
|---|---|---|---|
| Montrer que $f:\mathbb R^n\to\mathbb R^p$ est différentiable, calculer sa jacobienne | [[calculer-jacobienne]] | « Les composantes de $f$ admettent des dérivées partielles continues sur $\mathbb R^n$, donc… » | [[cd-exercices-types-corriges#4. Jacobienne, différentielle, dérivée directionnelle\|ex. 4]] |
| Calculer la dérivée de $f$ en $a$ dans la direction $v$ | [[calculer-derivee-directionnelle]] | « $f$ est différentiable en $a$, donc cette dérivée vaut $Df_a(v)=J_f(a)v$ (Prop. 2.9). » | [[cd-exercices-types-corriges#4. Jacobienne, différentielle, dérivée directionnelle\|ex. 4 b)]] |
| « En utilisant la définition », montrer que $f$ est différentiable | [[differentiabilite-par-definition]] | « Soient $a,h\in E$. $f(a+h)-f(a)=\dots$ » | [[cd-exercices-types-corriges#5. Différentielle de X³ et de tr(X³)\|ex. 5]] |
| « Développer $f(A+H)$ » (matrices) | [[differentielle-sur-les-matrices]] | « En développant sans commuter : $f(A+H)=\dots$ » | [[cd-exercices-types-corriges#6. Différentielle de XMX, deux méthodes\|ex. 6]], [[cd-exercices-types-corriges#7. Différentielle de tr(X tX) et d'une composée\|ex. 7]] |
| « En remarquant que $f=p\circ q$ » / différentielle d'une composée | [[appliquer-regle-de-la-chaine]] | « $q$ est linéaire continue donc… ; $p$ est bilinéaire continue donc… ; par la règle de la chaîne… » | [[cd-exercices-types-corriges#6. Différentielle de XMX, deux méthodes\|ex. 6 b)]] |
| $f$ définie à part en $(0,0)$ : continue ? dérivées partielles ? différentiable ? | [[etudier-en-un-point-particulier]] | « Pour $t\ne0$, $\frac{f(t,0)-f(0,0)}t=\dots$ » | [[cd-exercices-types-corriges#8. Étude en (0,0)\|ex. 8]] |
| Montrer que $f$ n'est pas différentiable en $a$ | [[montrer-non-differentiable]] | « Supposons $f$ différentiable en $a$. Alors… » | [[cd-exercices-types-corriges#8. Étude en (0,0)\|ex. 8 c)]] |
| Montrer que $f$ est $\mathcal C^1$ ; gradient ; plan tangent | [[montrer-classe-c1]] | « Les dérivées partielles existent et sont continues sur $U$ : … » | [[cd-exercices-types-corriges#9. Classe C1, gradient, plan tangent\|ex. 9]] |

## 3 – Accroissements finis

| L'énoncé demande… | Méthode | Première phrase sur la copie | Corrigé |
|---|---|---|---|
| Montrer $\lvert\!\lvert\!\lvert Df_x\rvert\!\rvert\!\rvert\le M$ | [[utiliser-iaf]] | « Pour tout $h$ : $\lVert Df_x(h)\rVert\le\dots\le M\lVert h\rVert$, donc… » | [[cd-exercices-types-corriges#10. Majorer la différentielle, lipschitzienne\|ex. 10 b)]] |
| Montrer que $f$ est $M$-lipschitzienne | [[utiliser-iaf]] | « $\mathbb R^n$ est un ouvert convexe, $f$ y est différentiable et $\lvert\!\lvert\!\lvert Df_x\rvert\!\rvert\!\rvert\le M$ ; par le Cor. 3.13… » | [[cd-exercices-types-corriges#10. Majorer la différentielle, lipschitzienne\|ex. 10 c)]] |
| Montrer que $f$ est constante | [[montrer-constante]] | « $Df_x=0$ pour tout $x$ et $U$ est un ouvert connexe, donc… (Th. 3.25) » | — |

## 4 – Ordre 2 et extrema

| L'énoncé demande… | Méthode | Première phrase sur la copie | Corrigé |
|---|---|---|---|
| Justifier $\mathcal C^2$, gradient, hessienne | [[calculer-differentielle-seconde]] | « $f$ est polynomiale, donc $\mathcal C^\infty$… » | [[cd-exercices-types-corriges#11. Points critiques et Taylor-Young\|ex. 11 a)]] |
| Points critiques et nature | [[etudier-points-critiques]] | « $(x,y)$ est critique ssi $\partial_xf(x,y)=0$ et $\partial_yf(x,y)=0$, c'est-à-dire… » | [[cd-exercices-types-corriges#12. Points critiques, système à résoudre\|ex. 12]] |
| $rt-s^2=0$ | [[etudier-points-critiques]] | « Le critère ne conclut pas ; étudions le signe de $f(a+h)-f(a)$. » | [[cd-exercices-types-corriges#13. Le cas rt − s² = 0\|ex. 13]] |
| Écrire Taylor-Young à l'ordre 2 en $a$ ; signe de $f(x,y)-f(a)$ | [[ecrire-taylor-young]] | « $f$ est $\mathcal C^2$ donc deux fois différentiable en $a$ ; pour $h=(h_1,h_2)$… » | [[cd-exercices-types-corriges#11. Points critiques et Taylor-Young\|ex. 11 c)]] |
| L'extremum est-il global ? | [[extremum-global]] | « $f(x,0)=\dots\to-\infty$, donc… » | [[cd-exercices-types-corriges#12. Points critiques, système à résoudre\|ex. 12]] |

## 5 – Inversion locale et fonctions implicites

| L'énoncé demande… | Méthode | Première phrase sur la copie | Corrigé |
|---|---|---|---|
| Montrer que $f$ est un difféomorphisme local en $a$ | [[montrer-diffeomorphisme]] | « $f$ est $\mathcal C^1$ de $\mathbb R^n$ dans $\mathbb R^n$ et $\det J_f(a)=\dots\ne0$ ; par le théorème d'inversion locale… » | [[cd-exercices-types-corriges#14. Difféomorphisme local, pas global\|ex. 14]] |
| Montrer que $f$ est un difféomorphisme de $U$ sur $V$ | [[montrer-diffeomorphisme]] | « $f$ est $\mathcal C^1$, $\det J_f\ne0$ sur $U$ ; montrons que $f$ est injective… » | [[cd-exercices-types-corriges#14. Difféomorphisme local, pas global\|ex. 14 b)]] |
| Jacobienne de $f^{-1}$ | [[montrer-diffeomorphisme]] | « $J_{f^{-1}}(f(a))=[J_f(a)]^{-1}$ » | [[cd-exercices-types-corriges#14. Difféomorphisme local, pas global\|ex. 14 c)]] |
| « La relation $f(x,y)=0$ définit $y$ comme fonction de $x$ près de $(a,b)$ » | [[fonction-implicite]] | « $f$ est $\mathcal C^\infty$, $f(a,b)=0$ et $\partial_yf(a,b)=\dots\ne0$ ; par le théorème des fonctions implicites… » | [[cd-exercices-types-corriges#15. Fonction implicite\|ex. 15]] |
| $\varphi'(a)$, tangente, DL de $\varphi$ | [[fonction-implicite]] | « $\varphi'(a)=-\frac{\partial_xf(a,b)}{\partial_yf(a,b)}$ » | [[cd-exercices-types-corriges#15. Fonction implicite\|ex. 15 b)]] |

## Question de cours / Vrai-Faux

| L'énoncé demande… | Où réviser |
|---|---|
| « Donner la définition de… » | [[cd-fiche-definitions]] |
| « Énoncer… » | [[cd-fiche-theoremes]] |
| « Montrer que différentiable ⟹ continue » | [[differentiable-implique-continue]] |
| « Montrer que $Df_a(v)$ est la dérivée dans la direction $v$ » | [[differentielle-et-derivees-directionnelles]] |
| « Peut-on affirmer que… ? » | [[cd-vrai-faux-classiques]], [[exemples-et-contre-exemples]] |
