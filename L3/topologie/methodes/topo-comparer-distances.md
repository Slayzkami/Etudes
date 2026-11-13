---
aliases:
  - "Méthode : comparer deux distances"
  - "distances équivalentes"
  - "δ ≤ kd"
tags:
  - topologie
  - topo/methode
  - topo/chapitre-02
---

# 🛠️ Méthode : comparer deux distances

*Méthode* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · § 2.10–2.11 du cours · [[topo-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> - **Si $\delta\le k\,d$** : $B_d(a,\frac rk)\subset B_\delta(a,r)$, donc tout ouvert (et tout fermé) de $\delta$ est un ouvert (fermé) de $d$.
> - **Topologiquement équivalentes** : mêmes suites convergentes ($d(x_n,a)\to0\iff\delta(x_n,a)\to0$), ou critère des boules, ou $\mathrm{id}$ bicontinue.
> - **Métriquement équivalentes** : trouver $\alpha,\beta>0$ avec $\alpha d\le\delta\le\beta d$.
> - **Pas métriquement équivalentes** : une partie bornée pour l'une et pas pour l'autre ; ou $\frac{\delta(x_n,y_n)}{d(x_n,y_n)}\to+\infty$ (ou $\to0$).
> - **Pas topologiquement équivalentes** : une suite qui converge pour l'une et pas pour l'autre.

> [!EXAMPLE] Rédaction modèle (comme sur la copie)
> *Écrit 2025-26, ex. 1.3* : « Sur $E=[0,1]$ avec $\delta(x,y)=|x-y|$, soit $d$ la distance discrète. Pour $x\neq y$ : $\delta(x,y)\le1=d(x,y)$ ; donc $\delta\le1\cdot d$. Le singleton $\{0\}=B_d(0,\frac12)$ est ouvert pour $d$ mais pas pour $\delta$ : $\frac1n\notin\{0\}$ et $\frac1n\to0$. »
>
> *Interro 2026-27, Q5* : « Si $\alpha d\le\tilde d$ et $F$ est $d$-fermé : soit $x_n\in F$ avec $\tilde d(x_n,x)\to0$ ; alors $d(x_n,x)\le\frac1\alpha\tilde d(x_n,x)\to0$, donc $x\in F$. $F$ est $\tilde d$-fermé. Par symétrie, mêmes fermés, donc mêmes ouverts : topologiquement équivalentes. »

## 🔗 Liens

- **S'appuie sur** : [[topo-critere-des-boules|Critère des boules (distances topologiquement équivalentes)]], [[topo-metriquement-implique-topologiquement|Métriquement équivalentes ⇒ topologiquement équivalentes]], [[topo-caracterisation-sequentielle-fermes|Caractérisation séquentielle des fermés]]
- **Méthodes voisines** : —
- **Corrigés** : [[topo-exercices-types-corriges#10. Une distance plus petite qu'une autre (écrit 2025-26)|ex. 10]]
- **Voir aussi** : —
