---
aliases:
  - "Classes à gauche et à droite modulo un sous-groupe"
  - "classe à gauche"
  - "classe à droite"
  - "xH"
  - "Hx"
  - "G/H"
  - "relation associée à H"
tags:
  - gac
  - gac/definition
  - gac/chapitre-03
---

# 📘 Classes à gauche et à droite modulo un sous-groupe

*Définition* · Chapitre : [[03-groupes-quotients|III – Groupes quotients]] · § III.3 du cours · [[index-definitions|↩ Index]]

> [!NOTE] Définitions
> Soit $H$ un [[sous-groupe]] de $G$.
> - La relation $x\mathcal R y\iff x^{-1}y\in H$ est une [[relation-equivalence|relation d'équivalence]] [[relation-compatible|compatible à gauche]] ; la classe de $1$ est $H$.
> - **Classe à gauche** de $x$ : $xH=\{xh\mid h\in H\}$ (c'est la classe de $x$ pour $\mathcal R$).
> - **Classe à droite** : $Hx=\{hx\mid h\in H\}$ (classes de $x\mathcal R y\iff yx^{-1}\in H$, compatible à droite).
> - $G/H$ = ensemble des classes à gauche.

> [!IMPORTANT] Théorème
> Une relation d'équivalence est compatible à gauche avec la loi de $G$ $\iff$ elle est de la forme $x^{-1}y\in H$ pour un sous-groupe $H$ (unique : la classe de $1$).

> [!TIP] Utile
> $xH=yH\iff x^{-1}y\in H$ ; $\mathrm{Card}(xH)=\mathrm{Card}(H)$ (bijection $h\mapsto xh$) ; les classes forment une partition → [[lagrange]].

> [!EXAMPLE] Exemple dans $\mathfrak S_3$, $H=\{e,\tau_1\}$
> Classes à gauche : $\{e,\tau_1\}$, $\{\gamma,\tau_2\}$, $\{\gamma^2,\tau_3\}$. Mais $\gamma H=\{\gamma,\tau_2\}\neq H\gamma=\{\gamma,\tau_3\}$ : $H$ n'est pas distingué.

## 🔗 Liens

- **S'appuie sur** : [[sous-groupe|Sous-groupe]], [[relation-equivalence|Relation d'équivalence]]
- **Utilisé par (définitions)** : [[congruence-modulo-sous-groupe|Congruence modulo un sous-groupe]], [[indice|Indice d'un sous-groupe]]
- **Utilisé par (théorèmes)** : [[relations-compatibles-groupe|Relations compatibles avec la loi d'un groupe]], [[lagrange|Théorème de Lagrange]]
