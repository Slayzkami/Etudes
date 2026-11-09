---
aliases:
  - "Propriétés des morphismes"
  - "f(1)=1"
  - "f(x^-1)"
  - "composée de morphismes"
  - "réciproque d'un isomorphisme"
tags:
  - gac
  - gac/theoreme
  - gac/chapitre-01
---

# ⭐ Propriétés des morphismes

*Théorème* · Chapitre : [[01-definitions-generales|I – Définitions générales]] · § I.3 du cours · [[index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Si $f:G\to G'$ est un [[morphisme-de-groupes|morphisme]] :
> 1. $f(1_G)=1_{G'}$ ; 2. $f(x^{-1})=f(x)^{-1}$ ; 3. $\forall n\in\mathbb Z,\ f(x^n)=f(x)^n$.
>
> La composée de deux morphismes (isomorphismes) est un morphisme (isomorphisme) ; la réciproque d'un isomorphisme est un isomorphisme.

> [!SUCCESS]- Démonstration
> 1. $f(1)=f(1\cdot1)=f(1)f(1)$, on simplifie par $f(1)$.
> 2. $f(x)f(x^{-1})=f(1)=1$ et de même à gauche ; unicité de l'inverse.
> 3. Récurrence pour $n\ge0$, puis 2. pour $n<0$.
> - Réciproque : avec $x=f^{-1}(x')$, $y=f^{-1}(y')$, $f(xy)=x'y'$ donc $f^{-1}(x'y')=xy$.

> [!TIP] Application : morphismes de source $\mathbb Z$ ou $\mathbb Z/n\mathbb Z$
> Un morphisme $f$ de source $\mathbb Z$ est déterminé par $f(1)$ : $f(n)=nf(1)$ → [[endomorphismes-de-z]].

## 🔗 Liens

- **S'appuie sur** : [[morphisme-de-groupes|Morphisme de groupes]]
- **Utilisé par (théorèmes)** : [[noyau-et-image|Noyau distingué, image sous-groupe, injectivité]]
- **Méthodes** : [[endomorphismes-de-z|Méthode : morphismes de source Z (endomorphismes de (Z,+))]]
- **Voir aussi** : [[image-noyau|Image, noyau, image réciproque]]
