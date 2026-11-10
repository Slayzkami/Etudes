---
aliases:
  - "Méthode : étudier les points critiques d'une fonction de R²"
  - "points critiques et nature"
  - "extrema locaux"
  - "tableau r s t"
tags:
  - cd
  - cd/methode
  - cd/chapitre-04
---

# 🛠️ Méthode : étudier les points critiques d'une fonction de R²

*Méthode* · Chapitre : [[04-differentielles-ordre-superieur|4 – Différentielles d'ordre supérieur]] · Méthode 4.2 du cours · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> 1. **Régularité** : $f$ est $\mathcal C^2$ sur l'ouvert $U$ (polynôme, fonctions usuelles).
> 2. **Points critiques** : résoudre le système $\partial_xf=0$, $\partial_yf=0$.
> 3. **Dérivées secondes** : $r=\partial^2_{xx}f$, $s=\partial^2_{xy}f$, $t=\partial^2_{yy}f$ en chaque point critique.
> 4. **Conclure avec $rt-s^2$** (Cor. 4.25) : $>0$ et $r>0$ : min local strict ; $>0$ et $r<0$ : max local strict ; $<0$ : point-selle.
> 5. **Si $rt-s^2=0$** : étudier directement le signe de $f(a+h)-f(a)$ (le long de droites, de courbes).
> 6. **Global ?** Question séparée → [[extremum-global]].

> [!TIP] Résoudre le système sans se tromper (mon point faible)
> - **Factoriser** chaque équation : un produit est nul ssi l'un des facteurs est nul.
> - Traiter les cas **un par un** (« cas 1 : $x=0$… ; cas 2 : $y=x^2$… »), et dans chaque cas **reporter dans l'autre équation**.
> - **Vérifier** chaque point trouvé dans les **deux** équations.

> [!EXAMPLE] Rédaction modèle (Écrit 2024-2025, ex. 2)
> $f(x,y)=3xy-x^3-y^3$, polynomiale donc $\mathcal C^2$ sur $\mathbb R^2$.
> $\partial_xf=3y-3x^2=0\iff y=x^2$ ; $\partial_yf=3x-3y^2=0\iff x=y^2$. En reportant : $x=x^4$, soit $x(x^3-1)=0$, donc $x=0$ (alors $y=0$) ou $x=1$ (alors $y=1$). Points critiques : $(0,0)$ et $(1,1)$ (vérifiés dans les deux équations).
> $r=-6x$, $s=3$, $t=-6y$.
>
> | point | $r$ | $s$ | $t$ | $rt-s^2$ | nature |
> |---|---|---|---|---|---|
> | $(0,0)$ | $0$ | $3$ | $0$ | $-9<0$ | point-selle |
> | $(1,1)$ | $-6$ | $3$ | $-6$ | $27>0$, $r<0$ | maximum local strict |

> [!EXAMPLE] Cas $rt-s^2=0$
> $f(x,y)=x^2+y^4$ en $(0,0)$ : $r=2$, $s=t=0$. Mais $f(x,y)\ge0=f(0,0)$ : minimum (global).
> $f(x,y)=x^2+y^3$ en $(0,0)$ : $f(0,y)=y^3$ change de signe : pas d'extremum.

## 🔗 Liens

- **Voir aussi** : [[point-critique|Point critique]], [[critere-rt-s2|Critère rt − s² (dimension 2)]], [[critere-c2|Critère C2]], [[matrice-hessienne|Matrice hessienne]], [[taylor-young-ordre-2|Formule de Taylor-Young à l'ordre 2]], [[extremum-local|Extremum local, extremum global]]
