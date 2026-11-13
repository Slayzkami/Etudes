---
aliases:
  - "Métriquement équivalentes ⇒ topologiquement équivalentes"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-02
---

# ⭐ Métriquement équivalentes ⇒ topologiquement équivalentes

*Théorème* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Prop. 2.61, Ex. 2.62, Rem. 2.63 du cours (poly : Prop. 2.15, Ex. 2.7, Rem. 2.7) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Deux distances métriquement équivalentes sont topologiquement équivalentes. La **réciproque est fausse**.

> [!SUCCESS]- Démonstration
> Si $d_2\le\beta d_1$ : $B_{d_1}(a,\frac r\beta)\subset B_{d_2}(a,r)$. Si $\alpha d_1\le d_2$ : $B_{d_2}(a,\alpha r)\subset B_{d_1}(a,r)$. On conclut par le critère des boules.
>
> *Version suites (interro 2026-27, Q5)* : $F$ fermé pour $d$, $x_n\in F$, $x_n\to x$ pour $\tilde d$. Alors $d(x_n,x)\le\frac1\alpha\tilde d(x_n,x)\to0$, donc $x\in F$. Par symétrie, mêmes fermés, donc mêmes ouverts.

> [!EXAMPLE] Exemple
> Sur $[0,+\infty[$ : $|x-y|$ et $|x^2-y^2|$ sont topologiquement équivalentes (mêmes suites convergentes) mais $\frac{d_2(n+1,n)}{d_1(n+1,n)}=2n+1\to+\infty$.

## 🔗 Liens

- **S'appuie sur** : [[topo-distances-metriquement-equivalentes|Distances métriquement équivalentes]], [[topo-critere-des-boules|Critère des boules (distances topologiquement équivalentes)]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : —
- **Méthodes** : [[topo-comparer-distances|Méthode : comparer deux distances]]
- **Voir aussi** : —
