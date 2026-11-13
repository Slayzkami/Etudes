---
aliases:
  - "Une boule fermée est un fermé"
  - "boule fermée est fermée"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-02
---

# ⭐ Une boule fermée est un fermé

*Théorème* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Prop. 2.6 du cours (poly : Prop. 2.2) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Dans un espace métrique, toute boule fermée $\bar B(a,\rho)$ est un fermé.

> [!SUCCESS]- Démonstration
> **Par le complémentaire (cours).** Soit $x\notin\bar B(a,\rho)$ : $d(a,x)>\rho$. On pose $r=d(a,x)-\rho>0$. Si $y\in B(x,r)$, la seconde inégalité triangulaire donne
> $d(a,y)\ge d(a,x)-d(x,y)>d(a,x)-r=\rho$, donc $y\notin\bar B(a,\rho)$. Ainsi $B(x,r)\cap\bar B(a,\rho)=\emptyset$ : le complémentaire est ouvert.
>
> **Par les suites.** Soit $x_n\in\bar B(a,\rho)$ avec $x_n\to x$. Alors $d(a,x)\le d(a,x_n)+d(x_n,x)\le\rho+d(x_n,x)$ ; quand $n\to+\infty$, $d(a,x)\le\rho$. Donc $x\in\bar B(a,\rho)$ ([[topo-caracterisation-sequentielle-fermes|caractérisation séquentielle]]).

> [!TIP] Réflexes
> Tombée à l'écrit 2022-23 **et** à l'interro 2026-27 : à savoir rédiger sans hésiter (les deux versions).

## 🔗 Liens

- **S'appuie sur** : [[topo-boules-spheres|Boules et sphères]], [[topo-ferme|Fermé]], [[topo-seconde-inegalite-triangulaire|Seconde inégalité triangulaire]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-exemples-fermes|Singletons, parties finies et sphères sont fermés]]
- **Méthodes** : —
- **Corrigés** : [[topo-exercices-types-corriges#1. Une boule fermée est fermée|ex. 1]]
- **Voir aussi** : —
