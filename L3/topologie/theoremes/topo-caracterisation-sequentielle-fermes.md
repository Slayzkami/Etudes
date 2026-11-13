---
aliases:
  - "Caractérisation séquentielle des fermés"
  - "caractérisation séquentielle"
  - "fermé par les suites"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-02
---

# ⭐ Caractérisation séquentielle des fermés

*Théorème* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Th. 2.12 du cours (poly : Th. 2.3) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> $A\subset E$ est fermé si et seulement si **toute suite d'éléments de $A$ qui converge dans $E$ a sa limite dans $A$**.

> [!SUCCESS]- Démonstration
> ($\Rightarrow$) $A$ fermé, $x_n\in A$, $x_n\to\ell$. Si $\ell\notin A$, comme $A^c$ est ouvert, $B(\ell,\varepsilon)\subset A^c$ ; or $x_n\in B(\ell,\varepsilon)$ pour $n$ grand : absurde.
> ($\Leftarrow$) Si $A^c$ n'est pas ouvert, il existe $x\in A^c$ tel que pour tout $n\ge1$, $B(x,\frac1n)\cap A\neq\emptyset$ : on choisit $x_n$ dedans. $x_n\in A$, $x_n\to x$, donc $x\in A$ : absurde.

> [!EXAMPLE] Exemple
> Le graphe $\{(x,\sin x)\}$ est fermé : $(x_n,\sin x_n)\to(a,b)\Rightarrow x_n\to a$, $\sin x_n\to\sin a$, donc $b=\sin a$.

> [!TIP] Réflexes
> - **Fermé** : « soit $(x_n)$ une suite de $A$ qui converge vers $\ell$ ; montrons $\ell\in A$ ».
> - **Pas fermé** : une suite **de $A$** qui converge vers un point **hors de $A$**.
> - **Pas ouvert** : une suite **hors de $A$** qui converge vers un point **de $A$** ($A^c$ pas fermé).

## 🔗 Liens

- **S'appuie sur** : [[topo-ferme|Fermé]], [[topo-suite-convergente|Suite convergente]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-caracterisation-adherence|Caractérisations de l'adhérence]], [[topo-ferme-dans-compact|Un fermé dans un compact est compact]]
- **Méthodes** : [[topo-montrer-ouvert-ferme|Méthode : montrer qu'une partie EST ouverte ou fermée]], [[topo-montrer-pas-ouvert-pas-ferme|Méthode : montrer qu'une partie N'EST PAS ouverte / PAS fermée]], [[topo-comparer-distances|Méthode : comparer deux distances]]
- **Voir aussi** : —
