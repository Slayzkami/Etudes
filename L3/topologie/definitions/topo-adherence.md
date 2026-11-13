---
aliases:
  - "Adhérence"
  - "adhérence"
  - "fermeture"
  - "point adhérent"
  - "Ā"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-02
---

# 📘 Adhérence

*Définition* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Déf. 2.22 du cours (poly : Déf. 2.5) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> L'**adhérence** de $A$ est l'intersection de tous les fermés contenant $A$ :
> $$\bar A=\bigcap\{F\ \text{fermé}\mid F\supset A\}.$$
> C'est le **plus petit fermé contenant $A$**.

> [!IMPORTANT] À retenir
> - $x\in\bar A\iff\forall r>0,\ B(x,r)\cap A\neq\emptyset\iff\exists(x_n)\in A^{\mathbb N},\ x_n\to x\iff d(x,A)=0$ → [[topo-caracterisation-adherence]].
> - $A\subset\bar A$ ; $A$ fermé $\iff\bar A=A$ ; $(\bar A)^c=\operatorname{Int}(A^c)$.
> - **Pour calculer $\bar A$ : deux inclusions** — (1) chaque point ajouté est limite d'une suite de $A$ ; (2) le candidat est **fermé et contient $A$**.

> [!EXAMPLE] Exemples
> $\overline{]0,1]\cup\{2\}}=[0,1]\cup\{2\}$ ; $\bar{\mathbb Q}=\mathbb R$ ; $\overline{\{\frac1n\}}=\{\frac1n\}\cup\{0\}$ ; $\overline{\{e^{-n}\}}=\{e^{-n}\}\cup\{0\}$ ; dans un e.v.n. $\overline{B(a,r)}=\bar B(a,r)$.

> [!WARNING] Pièges
> - L'adhérence n'est **pas** le complémentaire : on a toujours $A\subset\bar A$ (mon erreur).
> - Oublier l'inclusion $\bar A\subset F$ (« $F$ fermé contenant $A$ ») : la moitié des points (interro 2025-26).
> - $\overline{A\cap B}\subsetneq\bar A\cap\bar B$ possible : $A=\mathbb Q$, $B=\mathbb R\setminus\mathbb Q$.

## 🔗 Liens

- **S'appuie sur** : [[topo-ferme|Fermé]]
- **Utilisé par (définitions)** : [[topo-distance-a-une-partie|Distance d'un point à une partie, entre deux parties]], [[topo-frontiere|Frontière]], [[topo-partie-dense|Partie dense]]
- **Utilisé par (théorèmes)** : [[topo-caracterisation-adherence|Caractérisations de l'adhérence]], [[topo-complementaire-interieur-adherence|Intérieur et adhérence échangés par complémentaire]]
- **Méthodes** : [[topo-calculer-interieur-adherence-frontiere|Méthode : calculer intérieur, adhérence, frontière]]
- **Voir aussi** : [[topo-interieur|Intérieur]], [[topo-frontiere|Frontière]], [[topo-partie-dense|Partie dense]]
