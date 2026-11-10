---
aliases:
  - "Méthode : montrer la différentiabilité par la définition"
  - "différentiable par la définition"
  - "développer f(a+h)"
tags:
  - cd
  - cd/methode
  - cd/chapitre-02
---

# 🛠️ Méthode : montrer la différentiabilité par la définition

*Méthode* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Méthode 2.2 du cours · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> 1. **Développer** $f(a+h)-f(a)$.
> 2. **Repérer la partie linéaire en $h$** : c'est le candidat $L(h)$. Tout le reste est $r(h)$.
> 3. **$L$ est linéaire continue** : dimension finie (Th. 1.44) ou $\lVert L(h)\rVert\le C\lVert h\rVert$.
> 4. **Majorer le reste** : montrer $\dfrac{\lVert r(h)\rVert}{\lVert h\rVert}\to0$ (souvent $\lVert r(h)\rVert\le C\lVert h\rVert^2$).
> 5. **Conclure** : $f$ est différentiable en $a$ et $Df_a=L$.

> [!TIP] Rédaction type
> « Soit $a\in U$. Pour $h\in E$ tel que $a+h\in U$ : $f(a+h)-f(a)=L(h)+r(h)$ avec $L(h)=\dots$ et $r(h)=\dots$. L'application $L$ est linéaire, et continue car […]. De plus $\lVert r(h)\rVert\le C\lVert h\rVert^2$, donc $\frac{\lVert r(h)\rVert}{\lVert h\rVert}\le C\lVert h\rVert\to0$ quand $h\to0$. Par définition, $f$ est différentiable en $a$ et $Df_a(h)=\dots$ »

> [!EXAMPLE] Exemple
> $f(x,y)=x^2y$ en $a=(a_1,a_2)$ : $f(a+h)=(a_1+h_1)^2(a_2+h_2)=a_1^2a_2+\underbrace{2a_1a_2h_1+a_1^2h_2}_{L(h)}+\underbrace{a_2h_1^2+2a_1h_1h_2+h_1^2h_2}_{r(h)}$.
> Avec $\lVert h\rVert_\infty\le1$ : $\lvert r(h)\rvert\le(\lvert a_2\rvert+2\lvert a_1\rvert+1)\lVert h\rVert_\infty^2$.

> [!WARNING] Pièges
> - Trier par **nombre de $h$** : 0 $h$ = $f(a)$ ; 1 $h$ = $L(h)$ ; 2 $h$ ou plus = reste.
> - Ne pas oublier de dire que $L$ est **continue**.

## 🔗 Liens

- **Voir aussi** : [[differentiabilite|Différentiabilité en un point, différentielle]], [[petit-o|Petit o]], [[differentielle-et-derivees-directionnelles|Différentielle et dérivées directionnelles]], [[lineaire-en-dimension-finie|Linéaire au départ d'une dimension finie : continue]]
