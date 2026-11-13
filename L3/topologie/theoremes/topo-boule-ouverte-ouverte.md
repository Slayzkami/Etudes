---
aliases:
  - "Une boule ouverte est un ouvert"
  - "boule ouverte est ouverte"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-02
---

# ⭐ Une boule ouverte est un ouvert

*Théorème* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Prop. 2.5 du cours (poly : Prop. 2.1) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Dans un espace métrique, toute boule ouverte $B(a,\rho)$ est un ouvert.

> [!SUCCESS]- Démonstration
> Soit $x\in B(a,\rho)$ ; on pose $r=\rho-d(a,x)>0$ (« ce qui reste jusqu'au bord »). Si $y\in B(x,r)$ :
> $$d(a,y)\le d(a,x)+d(x,y)<d(a,x)+r=\rho,$$
> donc $y\in B(a,\rho)$. Ainsi $B(x,r)\subset B(a,\rho)$ : la boule est ouverte.

> [!TIP] Réflexes
> 3 mots pour la retenir : **$r$ = ce qui reste**, **inégalité triangulaire**, **$<\rho$**. Question de cours classique.

## 🔗 Liens

- **S'appuie sur** : [[topo-boules-spheres|Boules et sphères]], [[topo-ouvert|Ouvert]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-ouverts-reunions-de-boules|Un ouvert est une réunion de boules ouvertes]], [[topo-voisinages-et-boules|Voisinages et boules]]
- **Méthodes** : —
- **Corrigés** : [[topo-exercices-types-corriges#1. Une boule fermée est fermée|ex. 1]]
- **Voir aussi** : —
