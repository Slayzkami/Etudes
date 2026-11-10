---
aliases:
  - "Méthode : étudier une fonction en un point particulier (souvent (0,0))"
  - "étude en (0,0)"
  - "continuité dérivées partielles différentiabilité en (0,0)"
  - "fonction définie par morceaux"
tags:
  - cd
  - cd/methode
  - cd/chapitre-02
---

# 🛠️ Méthode : étudier une fonction en un point particulier (souvent (0,0))

*Méthode* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Méthode 3.4 du cours · [[cd-index-definitions|↩ Index]]

Situation : $f(x,y)=\dfrac{\text{numérateur}}{\text{dénominateur}}$ si $(x,y)\ne(0,0)$ et $f(0,0)=0$.

> [!ABSTRACT] Recette
> 1. **Ailleurs qu'en $(0,0)$** : $f$ est $\mathcal C^1$ (quotient de fonctions $\mathcal C^1$ dont le dénominateur ne s'annule pas).
> 2. **Continuité en $(0,0)$** : majorer $\lvert f(x,y)-f(0,0)\rvert$ par quelque chose qui tend vers $0$, ou réfuter avec un chemin $(t,t)$, $(t,t^2)$…
> 3. **Dérivées partielles en $(0,0)$ : par la limite.**
> $$\frac{\partial f}{\partial x}(0,0)=\lim_{t\to0}\frac{f(t,0)-f(0,0)}t,\qquad\frac{\partial f}{\partial y}(0,0)=\lim_{t\to0}\frac{f(0,t)-f(0,0)}t.$$
> 4. **Différentiabilité en $(0,0)$** : le seul candidat est $L(h)=\partial_xf(0,0)h_1+\partial_yf(0,0)h_2$. Étudier
> $$\frac{\lvert f(h_1,h_2)-f(0,0)-L(h)\rvert}{\lVert h\rVert}\xrightarrow[h\to0]{?}0.$$
> Si oui (majoration) : différentiable. Si non (un chemin) : pas différentiable.
> 5. **$\mathcal C^1$ ?** Calculer $\partial_xf(x,y)$ pour $(x,y)\ne(0,0)$ et regarder si elle tend vers $\partial_xf(0,0)$.

> [!EXAMPLE] Rédaction modèle
> $f(x,y)=\dfrac{x^3}{x^2+y^2}$, $f(0,0)=0$.
> - $\lvert f(x,y)\rvert\le\abs x\to0$ : continue en $(0,0)$.
> - $\frac{f(t,0)-0}t=\frac{t}{t}=1\to1$ : $\partial_xf(0,0)=1$. $\frac{f(0,t)-0}t=0$ : $\partial_yf(0,0)=0$.
> - Candidat $L(h)=h_1$. $f(h)-L(h)=\frac{h_1^3}{h_1^2+h_2^2}-h_1=\frac{-h_1h_2^2}{h_1^2+h_2^2}$. Sur le chemin $h=(t,t)$, $t>0$ : $\frac{\lvert -t/2\rvert}{\lVert (t,t)\rVert_\infty}=\frac12\not\to0$. Donc $f$ n'est **pas** différentiable en $(0,0)$.

> [!WARNING] Pièges (mes erreurs n° 1)
> - Dériver la **formule** pour obtenir $\partial_xf(0,0)$ : interdit, la formule n'est pas valable en $(0,0)$.
> - « Les dérivées partielles existent donc $f$ est différentiable » : faux.
> - Oublier $-f(0,0)$ et $-L(h)$ dans le quotient.

## 🔗 Liens

- **Voir aussi** : [[derivee-partielle|Dérivée partielle]], [[differentiabilite|Différentiabilité en un point, différentielle]], [[montrer-continue|Montrer qu'une application est (ou n'est pas) continue]], [[montrer-non-differentiable|Montrer qu'une application n'est pas différentiable en a]], [[critere-c1|Critère C1 par les dérivées partielles]]
