---
aliases:
  - "Caractérisations de l'adhérence"
  - "x ∈ Ā"
  - "point adhérent par les suites"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-02
---

# ⭐ Caractérisations de l'adhérence

*Théorème* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Prop. 2.23 et 2.24 du cours (poly : Prop. 2.7, 2.8) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Pour $x\in E$, sont équivalentes :
> (i) $x\in\bar A$ ; (ii) $\forall r>0,\ B(x,r)\cap A\neq\emptyset$ ; (iii) il existe une suite $(x_n)$ de $A$ qui converge vers $x$.
> De plus, $A$ est fermé $\iff\bar A=A$.

> [!SUCCESS]- Démonstration
> (i)⇒(ii) Si $B(x,r)\cap A=\emptyset$, $F=B(x,r)^c$ est un fermé contenant $A$, donc $\bar A\subset F$, et $x\notin F$.
> (ii)⇒(iii) On choisit $x_n\in B(x,\frac1n)\cap A$ : $d(x_n,x)<\frac1n\to0$.
> (iii)⇒(i) $(x_n)$ est dans le fermé $\bar A$, donc sa limite aussi (caractérisation séquentielle).

> [!TIP] Réflexes
> - $A\subset B\Rightarrow\bar A\subset\bar B$.
> - $\overline{A\cup B}=\bar A\cup\bar B$ ; $\overline{A\cap B}\subset\bar A\cap\bar B$, stricte pour $A=\mathbb Q$, $B=\mathbb R\setminus\mathbb Q$ (écrit 2025-26).
> - $x\in\bar A\iff d(x,A)=0$.

## 🔗 Liens

- **S'appuie sur** : [[topo-adherence|Adhérence]], [[topo-caracterisation-sequentielle-fermes|Caractérisation séquentielle des fermés]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : —
- **Méthodes** : [[topo-calculer-interieur-adherence-frontiere|Méthode : calculer intérieur, adhérence, frontière]]
- **Voir aussi** : —
