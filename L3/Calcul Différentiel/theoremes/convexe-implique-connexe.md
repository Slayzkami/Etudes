---
aliases:
  - "Tout convexe est connexe"
  - "Proposition 3.22"
  - "convexe donc connexe"
  - "ouvert et fermé dans un connexe"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-03
---

# ⭐ Tout convexe est connexe

*Théorème* · Chapitre : [[03-accroissements-finis|3 – Accroissements finis]] · Prop. 3.21 et 3.22 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Propositions
> - (Prop. 3.21) Si $X$ est connexe, les seules parties de $X$ à la fois ouvertes et fermées dans $X$ sont $X$ et $\emptyset$.
> - (Prop. 3.22) Dans un e.v.n., toute partie convexe est connexe.

> [!SUCCESS]- Démonstration
> **3.21.** Si $A$ est ouvert et fermé dans $X$, alors $U_1=A$ et $U_2=X\setminus A$ sont deux ouverts disjoints de réunion $X$ : l'un des deux est vide.
> **3.22 (idée).** Si $C$ convexe s'écrivait $U_1\cup U_2$ (ouverts de $C$ disjoints non vides), on prendrait $a\in U_1$, $b\in U_2$ : le segment $[a,b]\subset C$ serait coupé en deux ouverts disjoints non vides, donc $[0,1]$ aussi (via $t\mapsto a+t(b-a)$ continue). Impossible car $[0,1]$ est connexe. $\blacksquare$

> [!EXAMPLE] Réciproque fausse (Ex. 3.24)
> $\mathbb R^2\setminus\{(0,0)\}$ est connexe (on relie deux points par un chemin qui contourne l'origine) mais pas convexe.

## 🔗 Liens

- **S'appuie sur** : [[partie-connexe|Partie connexe]], [[segment-et-convexe|Segment, partie convexe]]
- **Méthodes** : [[montrer-constante|Montrer qu'une application est constante]]
