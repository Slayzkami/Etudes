---
aliases:
  - "Norme, espace vectoriel normé"
  - "norme"
  - "e.v.n."
  - "espace vectoriel normé"
  - "N1 N2 N3"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-01
---

# 📘 Norme, espace vectoriel normé

*Définition* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Déf. 1.5 du cours (poly : Déf. 1.2) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> Soit $E$ un espace vectoriel sur $\mathbb K=\mathbb R$ ou $\mathbb C$. Une **norme** est une application $N:E\to\mathbb R_+$ telle que :
> - **(N1)** $\forall x\in E,\ N(x)=0\iff x=0_E$ ;
> - **(N2)** $\forall\lambda\in\mathbb K,\ \forall x\in E,\ N(\lambda x)=|\lambda|\,N(x)$ ;
> - **(N3)** $\forall x,y\in E,\ N(x+y)\le N(x)+N(y)$.
>
> $(E,N)$ est un **espace vectoriel normé** (e.v.n.) ; on note souvent $\|x\|$.

> [!IMPORTANT] À retenir
> - Seconde inégalité triangulaire : $|N(x)-N(y)|\le N(x-y)$ → [[topo-seconde-inegalite-triangulaire]].
> - Toute norme donne une distance $d(x,y)=N(x-y)$ → [[topo-distance-associee-norme]].

> [!EXAMPLE] Exemples
> $\|\cdot\|_1,\|\cdot\|_2,\|\cdot\|_\infty$ sur $\mathbb K^n$ et sur $C([a,b])$ → [[topo-normes-usuelles]] ; $N(v)=\|Av\|_\infty$ avec $A$ inversible (TD 1.10).

> [!WARNING] Pièges
> - $x\mapsto\|x\|^2$ n'est pas une norme : $\|2x\|^2=4\|x\|^2$ (tester (N2) en premier).
> - Sur un espace de fonctions, (N1) utilise la **continuité** (une fonction nulle sauf en un point a une intégrale nulle).

## 🔗 Liens

- **S'appuie sur** : —
- **Utilisé par (définitions)** : [[topo-distance-associee-norme|Distance associée à une norme]], [[topo-norme-operateur|Norme d'une application linéaire continue]], [[topo-normes-usuelles|Normes usuelles de K^n et de C([a,b])]], [[topo-normes-equivalentes|Normes équivalentes]]
- **Utilisé par (théorèmes)** : [[topo-applications-lineaires-continues|Continuité d'une application linéaire]], [[topo-seconde-inegalite-triangulaire|Seconde inégalité triangulaire]]
- **Méthodes** : [[topo-montrer-norme|Méthode : montrer qu'une application est une norme]]
- **Voir aussi** : [[topo-distance|Distance, espace métrique]]
