---
aliases:
  - "Méthode : montrer qu'une application est (ou n'est pas) continue"
  - "prouver la continuité"
  - "non continue en (0,0)"
tags:
  - cd
  - cd/methode
  - cd/chapitre-01
---

# 🛠️ Méthode : montrer qu'une application est (ou n'est pas) continue

*Méthode* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Méthode 1.3 du cours · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> - **Par opérations** : sommes, produits, quotients (dénominateur non nul), composées de fonctions continues ; composante par composante à l'arrivée.
> - **Par une majoration** : $\lVert f(x)-f(a)\rVert\le(\text{quelque chose qui tend vers }0\text{ quand }x\to a)$.
> - **Pour réfuter** : une suite (ou un chemin) $x_n\to a$ avec $f(x_n)\not\to f(a)$.

> [!EXAMPLE] Majoration en $(0,0)$
> $f(x,y)=\dfrac{x^2y}{x^2+y^2}$, $f(0,0)=0$. Pour $(x,y)\ne(0,0)$ : $x^2\le x^2+y^2$, donc $\lvert f(x,y)-0\rvert\le\abs y\le\lVert (x,y)\rVert_\infty\to0$. $f$ est continue en $(0,0)$.

> [!EXAMPLE] Réfutation
> $f(x,y)=\dfrac{xy}{x^2+y^2}$, $f(0,0)=0$ : $f(\frac1n,\frac1n)=\frac12\not\to0=f(0,0)$ alors que $(\frac1n,\frac1n)\to(0,0)$. Non continue en $(0,0)$.

> [!WARNING] Piège
> Tester seulement les axes ($f(x,0)$, $f(0,y)$) ne prouve rien.

## 🔗 Liens

- **Voir aussi** : [[continuite|Continuité en un point]], [[continuite-et-composantes|Continuité et composantes]], [[etudier-en-un-point-particulier|Étudier une fonction en un point particulier (souvent (0,0))]]
