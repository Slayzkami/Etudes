---
aliases:
  - "Distance, espace métrique"
  - "distance"
  - "métrique"
  - "espace métrique"
  - "M1 M2 M3"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-01
---

# 📘 Distance, espace métrique

*Définition* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Déf. 1.1 du cours (poly : Déf. 1.1) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> Soit $E$ un ensemble non vide. Une **distance** sur $E$ est une application $d:E\times E\to\mathbb R_+$ telle que :
> - **(M1) séparation** : $\forall x,y\in E,\ d(x,y)=0\iff x=y$ ;
> - **(M2) symétrie** : $\forall x,y\in E,\ d(x,y)=d(y,x)$ ;
> - **(M3) inégalité triangulaire** : $\forall x,y,z\in E,\ d(x,y)\le d(x,z)+d(z,y)$.
>
> Un **espace métrique** est un couple $(E,d)$, avec $E\neq\emptyset$ et $d$ une distance sur $E$.

> [!IMPORTANT] À retenir
> - La **positivité** fait partie de la définition ($d$ est à valeurs dans $\mathbb R_+$).
> - Toute partie non vide $F\subset E$, munie de la restriction de $d$, est encore un espace métrique ([[topo-distance-induite|distance induite]]).
> - Seconde inégalité triangulaire : $|d(x,z)-d(z,y)|\le d(x,y)$ → [[topo-seconde-inegalite-triangulaire]].

> [!EXAMPLE] Exemples
> - $\mathbb R$ avec $|x-y|$ ; $\mathbb R^n$ avec $d_1,d_2,d_\infty$ (→ [[topo-normes-usuelles]]).
> - La [[topo-distance-discrete|distance discrète]] sur n'importe quel ensemble.
> - $\min(1,d)$, $\lambda d$ ($\lambda>0$), $d_1+d_2$, $|f(x)-f(y)|$ avec $f$ injective → [[topo-montrer-distance]].
> - Exemple d'espace métrique $E\subset\mathbb R^3$, $E\neq\mathbb R^3$ (interro 2026-27) : la boule unité de $\mathbb R^3$ avec la distance induite par $d_2$.

> [!WARNING] Pièges
> - $d(x,y)=(x-y)^3$ n'est **pas** une distance : $d(0,1)=-1<0$ (Piège 1.1).
> - $\min(|x-x'|,|y-y'|)$ sur $\mathbb R^2$ n'est pas une distance : séparation fausse (TD 1.6).

## 🔗 Liens

- **S'appuie sur** : —
- **Utilisé par (définitions)** : [[topo-application-lipschitzienne|Application lipschitzienne]], [[topo-boules-spheres|Boules et sphères]], [[topo-continuite|Continuité en un point]], [[topo-distance-associee-norme|Distance associée à une norme]], [[topo-distance-a-une-partie|Distance d'un point à une partie, entre deux parties]], [[topo-distance-discrete|Distance discrète]], [[topo-distance-induite|Distance induite, sous-espace métrique]], [[topo-distance-produit|Distance produit]], [[topo-distances-metriquement-equivalentes|Distances métriquement équivalentes]], [[topo-isometrie|Isométrie]], [[topo-partie-bornee-diametre|Partie bornée, diamètre]], [[topo-suite-convergente|Suite convergente]]
- **Utilisé par (théorèmes)** : [[topo-inegalite-triangulaire-generalisee|Inégalité triangulaire généralisée]], [[topo-seconde-inegalite-triangulaire|Seconde inégalité triangulaire]]
- **Méthodes** : [[topo-montrer-distance|Méthode : montrer qu'une application est une distance]]
- **Voir aussi** : [[topo-norme|Norme, espace vectoriel normé]], [[topo-distance-associee-norme|Distance associée à une norme]]
