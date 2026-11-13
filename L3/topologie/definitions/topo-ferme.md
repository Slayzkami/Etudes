---
aliases:
  - "Fermé"
  - "fermé"
  - "partie fermée"
  - "ensemble fermé"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-02
---

# 📘 Fermé

*Définition* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Déf. 2.2 du cours (poly : Déf. 2.2) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> Une partie $A\subset E$ est un **fermé** de $E$ si son complémentaire $A^c=E\setminus A$ est un ouvert, c'est-à-dire
> $$\forall x\notin A,\ \exists r>0,\ B(x,r)\cap A=\emptyset.$$

> [!IMPORTANT] À retenir
> - **Caractérisation séquentielle** : $A$ fermé $\iff$ toute suite de $A$ qui converge dans $E$ a sa limite dans $A$ → [[topo-caracterisation-sequentielle-fermes]].
> - Intersection **quelconque** et réunion **finie** de fermés : fermé → [[topo-stabilite-fermes]].
> - Boules fermées, sphères, singletons, parties finies sont fermés.
> - $A$ fermé $\iff\bar A=A\iff\operatorname{Fr}A\subset A$.

> [!EXAMPLE] Exemples
> $[a,b]$ ; $\mathbb Z$ ; $\{0\}\cup\{\frac1n\}$ ; $\{f=g\}$, $\{f\le g\}$ si $f,g$ continues ; un graphe $\{(x,f(x))\}$ avec $f$ continue.

> [!WARNING] Pièges
> - Une réunion **infinie** de fermés n'est pas forcément fermée : $\{\frac1n,\ n\ge1\}=\bigcup_n\{\frac1n\}$ n'est pas fermé ($\frac1n\to0$), $\bigcup_n[\frac1n,1]=]0,1]$ (mon erreur, interro 2025-26).
> - L'image directe d'un fermé n'est pas forcément fermée : $\exp(\mathbb R)=]0,+\infty[$.

## 🔗 Liens

- **S'appuie sur** : [[topo-ouvert|Ouvert]]
- **Utilisé par (définitions)** : [[topo-adherence|Adhérence]]
- **Utilisé par (théorèmes)** : [[topo-caracterisation-sequentielle-fermes|Caractérisation séquentielle des fermés]], [[topo-continuite-globale|Continuité globale : image réciproque]], [[topo-stabilite-fermes|Stabilité des fermés]], [[topo-boule-fermee-fermee|Une boule fermée est un fermé]]
- **Méthodes** : [[topo-montrer-ouvert-ferme|Méthode : montrer qu'une partie EST ouverte ou fermée]], [[topo-montrer-pas-ouvert-pas-ferme|Méthode : montrer qu'une partie N'EST PAS ouverte / PAS fermée]]
- **Voir aussi** : [[topo-adherence|Adhérence]]
