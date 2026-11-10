---
aliases:
  - "Difféomorphisme, difféomorphisme local"
  - "difféomorphisme"
  - "C1-difféomorphisme"
  - "difféo local"
  - "difféomorphisme global"
tags:
  - cd
  - cd/definition
  - cd/chapitre-05
---

# 📘 Difféomorphisme, difféomorphisme local

*Définition* · Chapitre : [[05-inversion-locale-fonctions-implicites|5 – Inversion locale et fonctions implicites]] · Déf. 5.1 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> Soient $E,F$ deux e.v.n., $U$ un ouvert de $E$, $V$ un ouvert de $F$ et $f:U\to V$.
> 1. $f$ est un **difféomorphisme de classe $\mathcal C^1$** de $U$ sur $V$ si
>    - (a) $f$ est une **bijection** de $U$ sur $V$ ;
>    - (b) $f$ est de classe $\mathcal C^1$ sur $U$ ;
>    - (c) sa réciproque $f^{-1}$ est de classe $\mathcal C^1$ sur $V$.
> 2. Soit $a\in U$. $f$ est un **difféomorphisme local en $a$** s'il existe un voisinage ouvert $U'\subset U$ de $a$ et un voisinage ouvert $V'\subset V$ de $f(a)$ tels que $f$ soit un difféomorphisme de $U'$ sur $V'$.

> [!EXAMPLE] Exemples
> - Une application linéaire bijective de $\mathbb R^n$ dans $\mathbb R^n$.
> - Coordonnées polaires (Ex. 5.2) : $P(\rho,\theta)=(\rho\cos\theta,\rho\sin\theta)$ de $]0,+\infty[\times]-\pi,\pi[$ sur $\mathbb R^2\setminus(\,]-\infty,0]\times\{0\})$.

> [!EXAMPLE] Contre-exemple
> $x\mapsto x^3$ est une bijection $\mathcal C^1$ de $\mathbb R$ sur $\mathbb R$, mais sa réciproque $y\mapsto\sqrt[3]{y}$ n'est pas dérivable en $0$ : ce n'est **pas** un difféomorphisme (et $f'(0)=0$).

> [!WARNING] Pièges
> - Bijective et $\mathcal C^1$ ne suffit pas : il faut aussi $f^{-1}$ de classe $\mathcal C^1$.
> - Difféomorphisme local en tout point $\not\Rightarrow$ difféomorphisme global : il manque l'**injectivité** → [[inversion-globale]].

## 🔗 Liens

- **S'appuie sur** : [[classe-c1|Application de classe C1]]
- **Utilisé par (théorèmes)** : [[differentielle-de-la-reciproque|Différentielle de la réciproque]], [[inversion-locale|Théorème d'inversion locale]], [[inversion-globale|Théorème d'inversion globale]]
- **Méthodes** : [[montrer-diffeomorphisme|Montrer qu'une application est un difféomorphisme (local ou global)]]
