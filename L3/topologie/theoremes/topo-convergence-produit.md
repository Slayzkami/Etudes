---
aliases:
  - "Convergence dans un produit"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-01
---

# ⭐ Convergence dans un produit

*Théorème* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Prop. 1.32 du cours (poly : Prop. 1.6) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Dans $E=E_1\times\dots\times E_p$ muni de la distance produit : $x^{(n)}\to\ell\iff$ pour tout $i$, $x^{(n)}_i\to\ell_i$ dans $E_i$.

> [!SUCCESS]- Démonstration
> $d(x^{(n)},\ell)=\max_id_i(x_i^{(n)},\ell_i)$ : chaque terme est entre $0$ et le max ; et un max d'un nombre **fini** de suites tendant vers $0$ tend vers $0$.

> [!TIP] Réflexes
> Dans $\mathbb R^2$ : $(x_n,y_n)\to(a,b)\iff x_n\to a$ et $y_n\to b$. Indispensable pour les graphes et les parties de $\mathbb R^2$.

## 🔗 Liens

- **S'appuie sur** : [[topo-distance-produit|Distance produit]], [[topo-suite-convergente|Suite convergente]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-continuite-composantes|Continuité dans un produit]], [[topo-produit-de-compacts|Produit de compacts]]
- **Méthodes** : [[topo-etudier-convergence-suite|Méthode : montrer qu'une suite converge (ou non)]]
- **Voir aussi** : —
