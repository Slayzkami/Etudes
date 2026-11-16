---
aliases:
  - "Mes erreurs à ne plus faire CD"
  - "pièges personnels calcul différentiel"
  - "erreurs CD"
tags:
  - cd
  - cd/revision
---

# 🚨 Mes erreurs à ne plus faire

Les erreurs que j'ai réellement faites en m'entraînant (test diagnostique, sujets d'entraînement, partiels blancs avant l'Écrit 1), avec la bonne version et un moyen de contrôle. À relire **juste avant l'épreuve**. À compléter après chaque séance. · [[cd-plan-de-revision|↩ Plan de révision]] · [[cd-index-definitions|↩ Index]]

> [!WARNING] 1. Dériver la formule pour avoir les dérivées partielles en $(0,0)$
> ❌ « $\partial_xf(x,y)=\dots$ donc $\partial_xf(0,0)=\dots$ » alors que la formule n'est valable que pour $(x,y)\ne(0,0)$.
> ✅ En un point où $f$ est définie à part : **la limite**. $\dfrac{\partial f}{\partial x}(0,0)=\lim_{t\to0}\dfrac{f(t,0)-f(0,0)}t$.
> **Contrôle** : ai-je écrit un quotient avec $t$ ? Si non, c'est faux.
> → [[etudier-en-un-point-particulier]], [[derivee-partielle]]

> [!WARNING] 2. Écrire la jacobienne transposée
> ❌ Mettre les dérivées de $f_1$ dans la première **colonne**.
> ✅ **Ligne $i$ = composante $f_i$, colonne $j$ = variable $x_j$.** Pour $f:\mathbb R^n\to\mathbb R^p$ : $p$ lignes, $n$ colonnes.
> **Contrôle** : la première ligne ne contient que des dérivées de $f_1$ ; $J_f(a)\,h$ doit pouvoir se calculer ($h$ a $n$ coordonnées).
> → [[matrice-jacobienne]], [[calculer-jacobienne]]

> [!WARNING] 3. Les valeurs numériques : $e^0=0$
> ❌ « $e^0=0$ »
> ✅ $e^0=1$, $\cos0=1$, $\sin0=0$, $\ln1=0$, $\cos\pi=-1$, $\sin\frac\pi2=1$.
> **Contrôle** : relire chaque valeur remplacée dans une jacobienne, une par une.

> [!WARNING] 4. « $L$ est linéaire, donc différentiable » (ou « donc continue »)
> ❌ Oublier la continuité.
> ✅ « $L$ est linéaire, **et continue car $E$ est de dimension finie** (Th. 1.44) » ou « car $\lVert L(h)\rVert\le C\lVert h\rVert$ (Th. 1.43) ». Alors seulement : $DL_a=L$.
> **Contrôle** : le mot « continue » et sa justification sont-ils sur la copie ?
> → [[differentielles-de-reference]], [[continuite-application-lineaire]]

> [!WARNING] 5. Norme d'opérateur : oublier d'« atteindre »
> ❌ « $\lVert u(x)\rVert\le7\lVert x\rVert$ donc $\tn u=7$ »
> ✅ La majoration donne $\tn u\le7$. Il faut **un vecteur** $x_0$ avec $\lVert u(x_0)\rVert=7\lVert x_0\rVert$ pour avoir $\tn u\ge7$.
> **Contrôle** : deux paragraphes sur la copie, « Majoration » et « Atteinte ».
> → [[calculer-norme-operateur]]

> [!WARNING] 6. Ne pas savoir les énoncés de cours mot pour mot
> ❌ IAF sans le segment, différentiabilité sans « linéaire continue », Taylor-Young sans le reste.
> ✅ Les énoncés avec **toutes** les hypothèses : IAF = « $f$ différentiable sur $U$ ouvert, $[a,b]\subset U$, $\lvert\!\lvert\!\lvert Df_x\rvert\!\rvert\!\rvert\le M$ sur $[a,b]$ ». Lipschitzienne = ouvert **convexe**.
> **Contrôle** : [[cd-fiche-definitions]] et [[cd-fiche-theoremes]], méthode « lire, fermer, réécrire, comparer ».
> → [[iaf]], [[iaf-sur-un-convexe]], [[differentiabilite]], [[taylor-young-ordre-2]]

> [!WARNING] 7. Résoudre le système des points critiques trop vite
> ❌ Simplifier par $x$ sans traiter le cas $x=0$ ; oublier un cas ; ne pas reporter dans l'autre équation.
> ✅ **Factoriser**, puis traiter les cas **un par un** ; dans chaque cas, reporter dans l'autre équation ; **vérifier** chaque point dans les deux équations.
> **Contrôle** : chaque point critique annoncé annule-t-il $\partial_xf$ **et** $\partial_yf$ ?
> → [[etudier-points-critiques]]

## 👀 Pièges voisins à surveiller (classiques, pas encore relevés sur mes copies)

> [!WARNING] 8. Développer $(A+H)^2$ comme des nombres
> ❌ « $(A+H)^2=A^2+2AH+H^2$ »
> ✅ $(A+H)^2=A^2+AH+HA+H^2$ : les matrices ne commutent pas.
> → [[differentielle-sur-les-matrices]]

> [!WARNING] 9. Dérivée directionnelle : donner un nombre
> ❌ Répondre par un réel pour $f:\mathbb R^2\to\mathbb R^2$.
> ✅ La dérivée en $a$ dans la direction $v$ est $Df_a(v)=J_f(a)\,v$ : un **vecteur** de l'espace d'arrivée.
> → [[calculer-derivee-directionnelle]]

> [!TIP] Mes 6 réflexes de contrôle
> 1. Point « à part » ⟹ quotient avec $t$.
> 2. Jacobienne : compter lignes et colonnes.
> 3. « Linéaire » ⟹ j'écris aussi « continue car… ».
> 4. $\tn u$ ⟹ majorer **et** atteindre.
> 5. Lipschitzienne ⟹ j'écris « ouvert convexe ».
> 6. Points critiques ⟹ je vérifie chaque point dans les deux équations.

## 📝 À compléter au fil des séances

| Date | Erreur (version fausse) | Version juste | Comment la contrôler |
|---|---|---|---|
| 14/11 (TD6 ex. 1.1) | Domaine de $f(x,y)=e^x\ln(1+y)$ : « $]-1,+\infty[$ », puis « $\mathbb R_+\times]-1,+\infty[$ » | $U=\mathbb R\times\,]-1,+\infty[$ : une fonction de 2 variables est définie sur une partie de $\mathbb R^2$, et $e^x$ est défini pour tout $x$ | Tester un point précis : $(5,0)$, $(-3,0)$ sont-ils dans mon $U$ ? $f$ y est-elle définie ? |
| 14/11 (TD6 ex. 1.1) | « $e^x\ln(1+y)$ est $\mathcal C^2$ par composition » | C'est un **produit** de deux fonctions $\mathcal C^\infty$ | Regarder l'opération entre les morceaux : $\times$ (produit) ou $g(u(x))$ (composition) |
| 14/11 (TD6 ex. 1.1) | $\partial_yf(0,0)=\dfrac{e^0}{1}=e$ (récidive de l'erreur n° 3) | $e^0=1$, donc $\partial_yf(0,0)=1$ | Relire chaque valeur remplacée une par une |
| 14/11 (TD6 ex. 1.1) | Ne pas connaître la formule de Taylor-Young à l'ordre 2 | $f(a+h)=f(a)+\partial_xf\,h_1+\partial_yf\,h_2+\frac12(rh_1^2+2sh_1h_2+th_2^2)+\lVert h\rVert^2\varepsilon(h)$ | La réécrire de mémoire chaque jour jusqu'à l'épreuve → [[taylor-young-ordre-2]] |
| 14/11 (TD6 ex. 1.1) | Factoriser le DL : $h_2+h_1h_2-\frac12h_2^2=h_2(1+h_1-h_2)$ (faux) | Ne pas factoriser une formule de Taylor ; garder $h_2+h_1h_2-\frac12h_2^2$ | Redévelopper toute factorisation ; comparer avec les DL usuels ($e^x\approx1+x$, $\ln(1+y)\approx y-\frac{y^2}2$) |
| 15/11 (TD6 ex. 1.2) | Dériver $\cos u$ et garder $\cos u$ (toutes les dérivées secondes fausses) | $\partial(\cos u)=-\sin u\cdot\partial u$ | Après chaque dérivation, la fonction doit avoir changé : $\sin\to\cos\to-\sin\to-\cos$ |
| 15/11 (TD6 ex. 1.2) | $\partial_z(\cos u)=-2z\sin u$ avec $u=2x+y-z^2$ | $-\sin u\cdot(-2z)=+2z\sin u$ | Compter les « moins » : deux « moins » qui se multiplient donnent « plus » |
| 15/11 (TD6 ex. 1.2) | $\partial_z(-2z\cos u)$ : premier terme écrit avec $\sin u$ | $(vw)'=v'w+vw'$ : $v'w=-2\cos u$ ($w$ **non dérivé**) | Écrire $v$, $w$, $v'$, $w'$ séparément avant d'assembler |
| 15/11 (TD6 ex. 1.2) | $\frac12\times(-2)\,h_3^2=+2h_3^2$ | $\frac12\times(-2)=-1$, donc $-h_3^2$ | Vérifier avec un DL en une variable : $\sin(2\pi+t)\approx t$, avec $t=2h_1+h_2-h_3^2$ |
| 15/11 (TD6 ex. 2) | $\varphi'(x)=-1-e^x/(1+e^{\varphi(x)})$ (parenthèses manquantes) | $\varphi'(x)=-\dfrac{1+e^x}{1+e^{\varphi(x)}}$ | Relire la formule « comme une machine » : que calcule-t-on en premier ? |
| 15/11 (TD6 ex. 2) | $\varphi'''(0)=-\frac25$, puis $-\frac23$ (termes oubliés, puis fraction inversée) | Dériver chaque produit en 2 termes : 6 termes au total ; $3+2\varphi'''(0)=0\Rightarrow\varphi'''(0)=-\frac32$ | Compter les termes avant d'évaluer ; le coefficient de $\varphi'''$ en $0$ est $e^0+1=2$, donc le dénominateur doit être $2$ |
| 15/11 (TD6 ex. 2) | Coefficient de $x^3$ : $\frac{-3/2}{6}=-\frac12$ | $\frac{\varphi'''(0)}{6}=-\frac{3}{2}\times\frac16=-\frac14$ | Écrire la division comme un produit par $\frac16$ |
| 15/11 (TD6 ex. 3) | $e^x-y$ au lieu de $e^{x-y}$ ; « somme » au lieu de « composée » ; conclusion du TFI sans $I$, sans l'équivalence, sans $\varphi(0)=0$ | Écrire $e^{x-y}$ ; $e^{x-y}$ est l'exponentielle d'un polynôme ; conclusion complète (intervalle, voisinage, équivalence, classe, $\varphi(0)$) | Relire la conclusion modèle de [[fonction-implicite]] et cocher chaque élément |
| 15/11 (TD6 ex. 3) | Parenthèses oubliées pour la 2e fois : $e^{x-\varphi}-1/(1+e^{x-\varphi})$ | $\dfrac{e^{x-\varphi}-1}{1+e^{x-\varphi}}$ ; mieux : évaluer directement la relation dérivée en $0$ | Dès qu'on tape « / », mettre le numérateur et le dénominateur entre parenthèses |
| 15/11 (TD6 ex. 2-3) | Donner seulement le résultat ($\varphi''(0)=-1$, $\frac12$, « $\frac14$ ») sans le calcul | Écrire la relation dérivée, puis la valeur en $0$, puis conclure | Si le résultat est dans l'énoncé (« montrer que »), seule la justification rapporte des points |
| 15/11 (TD6 ex. 4) | Évaluer $F$ en $(0,0,0)$ au lieu du point de l'énoncé $(0,1,1)$ | Toujours évaluer au point donné | Recopier le point en haut du brouillon avant de calculer |
| 15/11 (TD6 ex. 4) | « $F$ est $\mathcal C^\infty$ par composition d'exponentielle » alors que $F$ contient $\sin$ et $\cos$ | « composées de $\sin$, $\cos$ et de polynômes » | Nommer les fonctions réellement présentes |
| 15/11 (TD6 ex. 4) | $\cos0=0$ (même famille que $e^0=0$) ; terme $y\cos(xy)$ oublié dans la valeur | $\cos0=1$ ; évaluer **chaque** terme | Écrire la valeur de chaque terme séparément avant de sommer |
| 15/11 (TD6 ex. 4) | Dérivée de $\cos(xz)$ en $x$ : $-z\sin(xy)$ | $-z\sin(xz)$ : on garde l'argument de départ | Le sinus obtenu doit avoir le même argument que le cosinus dérivé |
| 16/11 (contrôle blanc 1) | IAF énoncée sans l'hypothèse « $[a,b]\subset U$ », et avec « dérivée bornée en valeur absolue » | $f$ différentiable sur l'ouvert $U$, $[a,b]\subset U$, $\tnorm{Df_x}\le M$ sur $[a,b]$ $\Rightarrow$ $\lVert f(b)-f(a)\rVert\le M\lVert b-a\rVert$ | Les 3 hypothèses de [[iaf]] : différentiable sur un ouvert, segment inclus, $\tnorm{Df}$ majorée |
| 16/11 (contrôle blanc 1) | « $\Omega$ convexe » écrit mais jamais utilisé | « Soient $a,b\in\Omega$ ; $\Omega$ est convexe donc $[a,b]\subset\Omega$ » | Chaque hypothèse de l'énoncé doit servir quelque part dans la preuve |
| 16/11 (contrôle blanc 1) | Système des points critiques non résolu : « par la résolution du système, on obtient… » | $y=\frac2x$, puis $x^4-5x^2+4=(x^2-1)(x^2-4)=0$ | Un résultat sans calcul = 0 point ; écrire la résolution |
| 16/11 (contrôle blanc 1) | Critère $rt-s^2$ inversé : « $r>0$ : maximum », « $r<0$ : minimum » | $rt-s^2>0$ et $r>0$ : **minimum** ; $r<0$ : **maximum** | $r>0$ comme $x\mapsto x^2$ (dérivée seconde $>0$, cuvette) : minimum |
| 16/11 (contrôle blanc 1) | « $\mathcal C^\infty$ sur l'ouvert $\mathbb R$ » pour une fonction de 2 variables ; question 5 laissée vide | « l'ouvert $\mathbb R^2$ » ; pas de minimum global car $f(x,0)=x^3-15x\to-\infty$ | Tester $f$ sur un axe quand $x\to\pm\infty$ |

## 🔗 Liens

- [[cd-exercices-types-corriges]] · [[cd-vrai-faux-classiques]] · [[cd-reconnaitre-exercice]]
