---
aliases:
  - "Boules d'un sous-espace métrique"
  - "B_F(a,r) = B_E(a,r) ∩ F"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-01
---

# ⭐ Boules d'un sous-espace métrique

*Théorème* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Prop. 1.20 du cours (poly : Rem. 1.3) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Pour $a\in F$ et $r>0$ : $B_F(a,r)=B_E(a,r)\cap F$ et $\bar B_F(a,r)=\bar B_E(a,r)\cap F$.

> [!SUCCESS]- Démonstration
> $x\in B_F(a,r)\iff x\in F$ et $d(a,x)<r\iff x\in B_E(a,r)\cap F$.

> [!EXAMPLE] Exemple
> - $F=[0,1]$ : $B_F(0,\frac12)=]-\frac12,\frac12[\cap[0,1]=[0,\frac12[$.
> - Écrit 2025-26 : $I=([-1,0[\cup]0,1])\times\mathbb R$, $A=(1,0)$ : $B_I(A,1)=\{(x,y)\mid(x-1)^2+y^2<1,\ 0<x\le1\}$ (demi-disque ouvert, bord vertical $x=1$ compris).

## 🔗 Liens

- **S'appuie sur** : [[topo-distance-induite|Distance induite, sous-espace métrique]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : —
- **Méthodes** : [[topo-determiner-boule|Méthode : déterminer et dessiner une boule]], [[topo-distance-induite-ouverts-relatifs|Méthode : ouverts et fermés d'un sous-espace (distance induite)]]
- **Voir aussi** : —
