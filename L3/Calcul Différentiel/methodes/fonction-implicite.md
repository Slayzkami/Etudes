---
aliases:
  - "Méthode : étudier une fonction implicite (existence, dérivée, DL)"
  - "fonction implicite"
  - "y = φ(x) près de (a,b)"
  - "DL d'une fonction implicite"
  - "φ'(a)"
tags:
  - cd
  - cd/methode
  - cd/chapitre-05
---

# 🛠️ Méthode : étudier une fonction implicite (existence, dérivée, DL)

*Méthode* · Chapitre : [[05-inversion-locale-fonctions-implicites|5 – Inversion locale et fonctions implicites]] · Méthodes 5.4 et 5.5 du cours · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette – existence
> 1. **Poser** $f(x,y)=\dots$ (tout d'un côté, « $=0$ »). Justifier que $f$ est $\mathcal C^k$ (polynôme, exponentielle : $\mathcal C^\infty$).
> 2. **Vérifier** $f(a,b)=0$.
> 3. **Calculer** $\partial_yf(a,b)$ (dérivée par rapport à la variable à exprimer) et vérifier $\ne0$.
> 4. **Conclure** : « par le théorème des fonctions implicites, il existe un intervalle ouvert $I\ni a$, un voisinage $V$ de $(a,b)$ et $\varphi:I\to\mathbb R$ de classe $\mathcal C^k$ tels que, pour $(x,y)\in V$, $f(x,y)=0\iff y=\varphi(x)$ ; de plus $\varphi(a)=b$. »

> [!ABSTRACT] Recette – dérivées et DL
> On part de $f(x,\varphi(x))=0$ sur $I$.
> - **$\varphi'(a)$** : $\varphi'(a)=-\dfrac{\partial_xf(a,b)}{\partial_yf(a,b)}$.
> - **$\varphi''(a)$** : dériver une seconde fois, $\partial^2_{xx}f+2\varphi'\partial^2_{xy}f+(\varphi')^2\partial^2_{yy}f+\varphi''\partial_yf=0$, évaluer en $a$.
> - **DL** : $\varphi(a+h)=b+\varphi'(a)h+\frac{\varphi''(a)}2h^2+o(h^2)$. Ou poser $\varphi(a+h)=b+c_1h+c_2h^2+o(h^2)$, remplacer dans $f(a+h,\varphi(a+h))=0$ et identifier.
> - **Tangente** à la courbe en $(a,b)$ : $y=b+\varphi'(a)(x-a)$.

> [!EXAMPLE] Rédaction modèle
> $f(x,y)=x^3+y^3-3xy-1$ près de $(0,1)$. $f$ est polynomiale donc $\mathcal C^\infty$. $f(0,1)=0+1-0-1=0$. $\partial_yf=3y^2-3x$, $\partial_yf(0,1)=3\ne0$. Par le théorème des fonctions implicites, il existe $I\ni0$ et $\varphi:I\to\mathbb R$ de classe $\mathcal C^\infty$ avec $\varphi(0)=1$ et, près de $(0,1)$, $f(x,y)=0\iff y=\varphi(x)$.
> $\partial_xf=3x^2-3y$, $\partial_xf(0,1)=-3$, donc $\varphi'(0)=-\frac{-3}{3}=1$. Tangente : $y=1+x$.

> [!WARNING] Pièges
> - Oublier de vérifier $f(a,b)=0$.
> - Dériver par rapport à la mauvaise variable.
> - Le signe **moins**.

## 🔗 Liens

- **Voir aussi** : [[fonctions-implicites-une-variable|Théorème des fonctions implicites (une variable)]], [[fonctions-implicites|Théorème des fonctions implicites (cas général)]], [[taylor-young-ordre-2|Formule de Taylor-Young à l'ordre 2]]
