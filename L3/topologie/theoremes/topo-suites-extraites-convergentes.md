---
aliases:
  - "Suites extraites d'une suite convergente"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-01
---

# ⭐ Suites extraites d'une suite convergente

*Théorème* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Prop. 1.28 (et Lemme 1.27) du cours (poly : Prop. 1.4) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Si $x_n\to\ell$, toute suite extraite $(x_{\varphi(n)})$ converge vers $\ell$. (Lemme : $\varphi$ strictement croissante $\Rightarrow\varphi(n)\ge n$.)

> [!SUCCESS]- Démonstration
> Soit $\varepsilon>0$ et $N$ tel que $d(x_n,\ell)<\varepsilon$ pour $n\ge N$. Si $n\ge N$, alors $\varphi(n)\ge n\ge N$, donc $d(x_{\varphi(n)},\ell)<\varepsilon$.

> [!TIP] Réflexes
> Pour montrer qu'une suite **diverge** : deux sous-suites de limites différentes ($(-1)^n$).

## 🔗 Liens

- **S'appuie sur** : [[topo-suite-extraite|Suite extraite]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-convergente-cauchy|Suites de Cauchy : convergente ⇒ Cauchy ; Cauchy + sous-suite convergente ⇒ convergente]]
- **Méthodes** : [[topo-etudier-convergence-suite|Méthode : montrer qu'une suite converge (ou non)]]
- **Voir aussi** : —
