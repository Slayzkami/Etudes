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
|  |  |  |  |

## 🔗 Liens

- [[cd-exercices-types-corriges]] · [[cd-vrai-faux-classiques]] · [[cd-reconnaitre-exercice]]
