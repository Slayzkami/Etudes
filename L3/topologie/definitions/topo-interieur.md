---
aliases:
  - "Intérieur"
  - "intérieur"
  - "Int A"
  - "point intérieur"
  - "Å"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-02
---

# 📘 Intérieur

*Définition* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Déf. 2.18 du cours (poly : Déf. 2.4) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> L'**intérieur** de $A$ est la réunion de tous les ouverts contenus dans $A$ :
> $$\operatorname{Int}A=\mathring A=\bigcup\{O\ \text{ouvert}\mid O\subset A\}.$$
> C'est le **plus grand ouvert contenu dans $A$**.

> [!IMPORTANT] À retenir
> - $x\in\operatorname{Int}A\iff\exists r>0,\ B(x,r)\subset A$ (Prop. 2.19) → [[topo-caracterisation-interieur]].
> - Par les suites : $x\notin\operatorname{Int}A\iff$ il existe une suite de $A^c$ qui tend vers $x$.
> - $\operatorname{Int}A\subset A$ ; $A$ ouvert $\iff\operatorname{Int}A=A$ ; $(\operatorname{Int}A)^c=\overline{A^c}$.

> [!EXAMPLE] Exemples
> $\operatorname{Int}[0,1[=]0,1[$ ; $\operatorname{Int}\mathbb Q=\emptyset$ ; $\operatorname{Int}\{a\}=\emptyset$ ; $\operatorname{Int}\mathbb Z=\emptyset$ ; intérieur d'une courbe ($y=x^2$) dans $\mathbb R^2$ : $\emptyset$.

> [!WARNING] Pièges
> - Pour justifier qu'un point n'est **pas** intérieur, il faut une suite **hors de $A$** qui tend vers **ce point** (pas recopier les points d'un autre exemple — mon erreur sur $[1,2[\cup\{5\}$).
> - $\operatorname{Int}A\cup\operatorname{Int}B\subsetneq\operatorname{Int}(A\cup B)$ possible : $A=[0,1]$, $B=[1,2]$.

## 🔗 Liens

- **S'appuie sur** : [[topo-ouvert|Ouvert]]
- **Utilisé par (définitions)** : [[topo-frontiere|Frontière]]
- **Utilisé par (théorèmes)** : [[topo-caracterisation-interieur|Caractérisation et propriétés de l'intérieur]], [[topo-complementaire-interieur-adherence|Intérieur et adhérence échangés par complémentaire]]
- **Méthodes** : [[topo-calculer-interieur-adherence-frontiere|Méthode : calculer intérieur, adhérence, frontière]]
- **Voir aussi** : [[topo-adherence|Adhérence]], [[topo-frontiere|Frontière]]
