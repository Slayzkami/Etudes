---
aliases:
  - "Méthode : montrer qu'une application n'est pas différentiable en a"
  - "non différentiable"
  - "réfuter la différentiabilité"
tags:
  - cd
  - cd/methode
  - cd/chapitre-02
---

# 🛠️ Méthode : montrer qu'une application n'est pas différentiable en a

*Méthode* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Méthode 2.5 du cours · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette (dans cet ordre)
> 1. **Non continue** en $a$ $\Rightarrow$ non différentiable (contraposée de la Prop. 2.18).
> 2. **Une dérivée directionnelle n'existe pas** (limites différentes en $0^+$ et $0^-$) : contraposée de la Prop. 2.9.
> 3. **$v\mapsto f'_v(0)$ n'est pas linéaire** : elle ne peut pas être $Df_a$.
> 4. **Le seul candidat ne convient pas** : $L$ est imposée par les dérivées partielles ; on trouve un chemin $h\to0$ où $\dfrac{\lvert f(a+h)-f(a)-L(h)\rvert}{\lVert h\rVert}\not\to0$.

> [!TIP] Rédaction type (par l'absurde)
> « Supposons $f$ différentiable en $a$. D'après la Prop. 2.9, pour tout $v$, $\lim_{t\to0}\frac{f(a+tv)-f(a)}t$ existe et vaut $Df_a(v)$. Or pour $v=\dots$ ce quotient tend vers … en $0^+$ et vers … en $0^-$. Contradiction. »

> [!EXAMPLE] Exemples
> - $f(x,y)=\abs x$ en $(0,0)$, $v=(1,0)$ : $\frac{\abs t}t\to\pm1$.
> - $f(x,y)=\frac{x^2y}{x^2+y^2}$, $f(0,0)=0$ : $\partial_xf(0,0)=\partial_yf(0,0)=0$, donc $L=0$ ; mais $\frac{\lvert f(t,t)\rvert}{\lVert (t,t)\rVert_\infty}=\frac{\abs t/2}{\abs t}=\frac12\not\to0$.

## 🔗 Liens

- **Voir aussi** : [[differentiable-implique-continue|Différentiable implique continue]], [[differentielle-et-derivees-directionnelles|Différentielle et dérivées directionnelles]], [[differentiabilite|Différentiabilité en un point, différentielle]], [[etudier-en-un-point-particulier|Étudier une fonction en un point particulier (souvent (0,0))]]
