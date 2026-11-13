---
aliases:
  - "Ouvert"
  - "ouvert"
  - "partie ouverte"
  - "ensemble ouvert"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-02
---

# 📘 Ouvert

*Définition* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Déf. 2.1 du cours (poly : Déf. 2.1) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> Une partie $A\subset E$ est un **ouvert** de $E$ si $A=\emptyset$ ou si
> $$\forall x\in A,\ \exists r>0,\ B(x,r)\subset A.$$

> [!IMPORTANT] À retenir
> - Réunion **quelconque** et intersection **finie** d'ouverts : ouvert → [[topo-stabilite-ouverts]].
> - Une boule ouverte est ouverte ([[topo-boule-ouverte-ouverte]]) ; un ouvert est une réunion de boules ouvertes.
> - $A$ ouvert $\iff$ $\operatorname{Int}A=A$ $\iff$ $A$ est voisinage de chacun de ses points.
> - **Par les suites** : $A$ ouvert $\iff$ $A^c$ fermé $\iff$ aucune suite de $A^c$ ne converge vers un point de $A$.
> - Le plus rapide : $A=f^{-1}(O)$ avec $f$ continue et $O$ ouvert → [[topo-continuite-globale]].

> [!EXAMPLE] Exemples
> $]a,b[$ ; $\{y>0\}\subset\mathbb R^2$ ; $\{x^2+y^2<1\}$ ; $\{f\neq g\}$ si $f,g$ continues ; pour la distance discrète, **toutes** les parties.

> [!WARNING] Pièges
> - « Pas ouvert » ne veut pas dire « fermé » : $[0,1[$ n'est ni l'un ni l'autre ; $\emptyset$, $E$ sont les deux.
> - $\bigcap_n]-\tfrac1n,\tfrac1n[=\{0\}$ : une intersection **infinie** d'ouverts n'est pas forcément ouverte.
> - L'**image directe** d'un ouvert par une application continue n'est pas forcément ouverte ($x^2$ envoie $]-1,1[$ sur $[0,1[$).

## 🔗 Liens

- **S'appuie sur** : [[topo-boules-spheres|Boules et sphères]]
- **Utilisé par (définitions)** : [[topo-distances-topologiquement-equivalentes|Distances topologiquement équivalentes]], [[topo-ferme|Fermé]], [[topo-interieur|Intérieur]], [[topo-recouvrement|Recouvrement]], [[topo-voisinage|Voisinage]]
- **Utilisé par (théorèmes)** : [[topo-continuite-globale|Continuité globale : image réciproque]], [[topo-stabilite-ouverts|Stabilité des ouverts]], [[topo-boule-ouverte-ouverte|Une boule ouverte est un ouvert]]
- **Méthodes** : [[topo-montrer-ouvert-ferme|Méthode : montrer qu'une partie EST ouverte ou fermée]], [[topo-montrer-pas-ouvert-pas-ferme|Méthode : montrer qu'une partie N'EST PAS ouverte / PAS fermée]]
- **Voir aussi** : [[topo-ferme|Fermé]]
