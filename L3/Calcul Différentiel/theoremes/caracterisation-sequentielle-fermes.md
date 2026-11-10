---
aliases:
  - "Caractérisation séquentielle des fermés"
  - "fermé par les suites"
  - "fermé séquentiellement"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-01
---

# ⭐ Caractérisation séquentielle des fermés

*Théorème* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Th. 1.24 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> $A\subset E$ est fermé si et seulement si toute suite d'éléments de $A$ qui converge dans $E$ a sa limite dans $A$.

> [!SUCCESS]- Démonstration
> ($\Rightarrow$) Soit $A$ fermé, $x_n\in A$, $x_n\to\ell$. Si $\ell\notin A$, comme $E\setminus A$ est ouvert il existe $r>0$ avec $B(\ell,r)\cap A=\emptyset$. Or $\lVert x_n-\ell\rVert<r$ pour $n$ grand, donc $x_n\in B(\ell,r)\cap A$ : contradiction.
> ($\Leftarrow$) Par contraposée : si $A$ n'est pas fermé, il existe $\ell\notin A$ tel que pour tout $n\ge1$, $B(\ell,\frac1n)\cap A\ne\emptyset$. On choisit $x_n$ dans cette intersection : $x_n\in A$, $x_n\to\ell\notin A$. $\blacksquare$

## 🔗 Liens

- **S'appuie sur** : [[ouvert-ferme|Ouvert, fermé]], [[suite-convergente|Suite convergente]]
- **Méthodes** : [[montrer-ouvert-ferme|Montrer qu'une partie est ouverte ou fermée]]
