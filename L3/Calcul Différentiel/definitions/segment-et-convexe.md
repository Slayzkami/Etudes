---
aliases:
  - "Segment, partie convexe"
  - "segment"
  - "convexe"
  - "partie convexe"
  - "[a,b]"
tags:
  - cd
  - cd/definition
  - cd/chapitre-03
---

# 📘 Segment, partie convexe

*Définition* · Chapitre : [[03-accroissements-finis|3 – Accroissements finis]] · Déf. 3.3 et 3.4 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> - Pour $a,b\in E$, le **segment** $[a,b]$ est $\{a+t(b-a)\ :\ t\in[0,1]\}$ ; le segment ouvert est $]a,b[=\{a+t(b-a)\ :\ t\in\,]0,1[\}$.
> - Une partie $C\subset E$ est **convexe** si, pour tous $a,b\in C$, le segment $[a,b]$ est inclus dans $C$.

> [!EXAMPLE] Exemples (Ex. 3.5)
> Les boules (ouvertes ou fermées), les sous-espaces vectoriels, $E$ tout entier, un produit de convexes, un demi-plan sont convexes.
> Preuve pour une boule : si $\lVert a-x_0\rVert<r$ et $\lVert b-x_0\rVert<r$, alors pour $t\in[0,1]$,
> $\lVert a+t(b-a)-x_0\rVert=\lVert (1-t)(a-x_0)+t(b-x_0)\rVert\le(1-t)\lVert a-x_0\rVert+t\lVert b-x_0\rVert<r$.

> [!EXAMPLE] Contre-exemple
> $\mathbb R^2\setminus\{(0,0)\}$ n'est pas convexe : le segment de $(-1,0)$ à $(1,0)$ passe par l'origine.

> [!TIP] Où ça sert
> L'[[iaf]] demande que le segment $[a,b]$ soit dans $U$ : c'est automatique si $U$ est convexe → [[iaf-sur-un-convexe]].

## 🔗 Liens

- **S'appuie sur** : [[norme|Norme, espace vectoriel normé]]
- **Utilisé par (théorèmes)** : [[taf|Théorème des accroissements finis (TAF)]], [[iaf|Inégalité des accroissements finis (IAF)]], [[iaf-sur-un-convexe|IAF sur un convexe : différentielle bornée implique lipschitzienne]], [[convexe-implique-connexe|Tout convexe est connexe]]
