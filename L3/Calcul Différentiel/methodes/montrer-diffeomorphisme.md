---
aliases:
  - "Méthode : montrer qu'une application est un difféomorphisme (local ou global)"
  - "difféomorphisme local en a"
  - "difféomorphisme de U sur V"
  - "jacobienne de la réciproque"
tags:
  - cd
  - cd/methode
  - cd/chapitre-05
---

# 🛠️ Méthode : montrer qu'une application est un difféomorphisme (local ou global)

*Méthode* · Chapitre : [[05-inversion-locale-fonctions-implicites|5 – Inversion locale et fonctions implicites]] · Méthodes 5.1, 5.2, 5.3, 5.6 du cours · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette – local en $a$
> 1. $f$ est $\mathcal C^1$ sur un ouvert contenant $a$.
> 2. $f$ va de $\mathbb R^n$ dans $\mathbb R^n$ (jacobienne carrée).
> 3. $\det J_f(a)\ne0$.
> 4. « Par le théorème d'inversion locale, $f$ est un difféomorphisme local en $a$. »

> [!ABSTRACT] Recette – global de $U$ sur $f(U)$
> 1. $U$ ouvert, $f$ de classe $\mathcal C^1$ sur $U$.
> 2. $\det J_f(x)\ne0$ pour **tout** $x\in U$.
> 3. **Injectivité** : résoudre $f(x)=f(x')$, ou résoudre $f(x)=y$ (au plus une solution), ou stricte monotonie en dimension 1.
> 4. Conclure par le Cor. 5.13. Pour avoir « sur $V$ » : montrer $f(U)=V$.

> [!ABSTRACT] Jacobienne de la réciproque
> $J_{f^{-1}}(f(a))=[J_f(a)]^{-1}$, avec en dimension 2 : $\begin{pmatrix}\alpha&\beta\\ \gamma&\delta\end{pmatrix}^{-1}=\dfrac1{\alpha\delta-\beta\gamma}\begin{pmatrix}\delta&-\beta\\-\gamma&\alpha\end{pmatrix}$.

> [!EXAMPLE] Rédaction modèle
> $f(x,y)=(x+y,\ xy)$ en $a=(2,1)$. $f$ est polynomiale donc $\mathcal C^1$ sur $\mathbb R^2$. $J_f(x,y)=\begin{pmatrix}1&1\\ y&x\end{pmatrix}$, $\det J_f(2,1)=2-1=1\ne0$. Par le théorème d'inversion locale, $f$ est un difféomorphisme local en $(2,1)$, et
> $J_{f^{-1}}(3,2)=\begin{pmatrix}1&1\\1&2\end{pmatrix}^{-1}=\begin{pmatrix}2&-1\\-1&1\end{pmatrix}$.
> En revanche $\det J_f(x,y)=x-y=0$ sur la droite $y=x$ : $f$ n'y est pas un difféomorphisme local ; et $f(x,y)=f(y,x)$ : $f$ n'est pas injective sur $\mathbb R^2$.

> [!TIP] Résoudre une équation près d'une solution connue (Méthode 5.6)
> Pour montrer que $\Phi(X)=A$ a une solution pour $A$ proche de $A_0=\Phi(X_0)$ : $\Phi$ est $\mathcal C^1$, $D\Phi_{X_0}$ est injective donc bijective (dimension finie) ; par inversion locale, $\Phi$ est bijective d'un ouvert $U\ni X_0$ sur un ouvert $V\ni A_0$, qui contient une boule $B(A_0,\alpha)$.

> [!WARNING] Pièges
> - Jacobien non nul partout $\not\Rightarrow$ injective.
> - $f:\mathbb R^2\to\mathbb R^3$ : le théorème ne s'applique pas.

## 🔗 Liens

- **Voir aussi** : [[inversion-locale|Théorème d'inversion locale]], [[inversion-globale|Théorème d'inversion globale]], [[differentielle-de-la-reciproque|Différentielle de la réciproque]], [[diffeomorphisme|Difféomorphisme, difféomorphisme local]], [[matrice-jacobienne|Matrice jacobienne]]
