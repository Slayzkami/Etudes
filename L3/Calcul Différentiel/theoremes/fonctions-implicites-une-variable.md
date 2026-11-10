---
aliases:
  - "Théorème des fonctions implicites (une variable)"
  - "TFI"
  - "fonctions implicites dans R²"
  - "y = φ(x)"
  - "Théorème 5.15"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-05
---

# ⭐ Théorème des fonctions implicites (une variable)

*Théorème* · Chapitre : [[05-inversion-locale-fonctions-implicites|5 – Inversion locale et fonctions implicites]] · Th. 5.15 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> Soit $f:U\to\mathbb R$ de classe $\mathcal C^k$ ($k\ge1$) sur un ouvert $U\subset\mathbb R^2$, et $(a,b)\in U$ tel que
> $$f(a,b)=0\qquad\text{et}\qquad\frac{\partial f}{\partial y}(a,b)\ne0.$$
> Alors il existe un voisinage ouvert $V$ de $(a,b)$ inclus dans $U$, un intervalle $I=\,]a-\varepsilon,a+\varepsilon[$ et $\varphi:I\to\mathbb R$ de classe $\mathcal C^k$ tels que
> $$\big[(x,y)\in V\text{ et }f(x,y)=0\big]\iff\big[x\in I\text{ et }y=\varphi(x)\big].$$
> De plus $\varphi(a)=b$ et $f(x,\varphi(x))=0$ pour tout $x\in I$.

> [!IMPORTANT] Dérivée de $\varphi$ (Rem. 5.16)
> En dérivant $f(x,\varphi(x))=0$ : $\partial_xf(x,\varphi(x))+\varphi'(x)\,\partial_yf(x,\varphi(x))=0$, donc
> $$\varphi'(x)=-\frac{\partial_xf(x,\varphi(x))}{\partial_yf(x,\varphi(x))},\qquad\varphi'(a)=-\frac{\partial_xf(a,b)}{\partial_yf(a,b)}.$$

> [!SUCCESS]- Idée de la démonstration
> On applique l'[[inversion-locale]] à $\Phi(x,y)=(x,f(x,y))$ : $J_\Phi(a,b)=\begin{pmatrix}1&0\\ \partial_xf&\partial_yf\end{pmatrix}$ a pour déterminant $\partial_yf(a,b)\ne0$. La réciproque locale s'écrit $\Phi^{-1}(x,z)=(x,\psi(x,z))$, et $f(x,y)=0\iff\Phi(x,y)=(x,0)\iff y=\psi(x,0)=:\varphi(x)$. $\blacksquare$

> [!EXAMPLE] Le cercle (Ex. 5.17)
> $f(x,y)=x^2+y^2-1$. En $(0,1)$ : $\partial_yf=2\ne0$, $y=\sqrt{1-x^2}$. En $(1,0)$ : $\partial_yf=0$, on ne peut pas exprimer $y$ en fonction de $x$ (mais $x$ en fonction de $y$, oui : $\partial_xf=2\ne0$).

> [!WARNING] Pièges
> - Vérifier que le point est **sur la courbe** : $f(a,b)=0$.
> - On dérive par rapport à la variable qu'on veut **exprimer** ($y$).
> - Ne pas oublier le signe **moins** dans $\varphi'$.

## 🔗 Liens

- **S'appuie sur** : [[inversion-locale|Théorème d'inversion locale]], [[derivee-partielle|Dérivée partielle]]
- **Utilisé par (théorèmes)** : [[fonctions-implicites|Théorème des fonctions implicites (cas général)]]
- **Méthodes** : [[fonction-implicite|Étudier une fonction implicite (existence, dérivée, DL)]]
