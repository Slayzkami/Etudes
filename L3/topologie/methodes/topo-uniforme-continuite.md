---
aliases:
  - "Méthode : montrer (ou réfuter) l'uniforme continuité"
  - "uniformément continue ou non"
tags:
  - topologie
  - topo/methode
  - topo/chapitre-02
---

# 🛠️ Méthode : montrer (ou réfuter) l'uniforme continuité

*Méthode* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Méthode 2.4 du cours · [[topo-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> - **Oui** : inégalité lipschitzienne $d(f(x),f(y))\le k\,d(x,y)$ (souvent via $|f'|\le k$), ou **Heine** sur un compact.
> - **Non** : deux suites $(x_n),(y_n)$ avec $d(x_n,y_n)\to0$ mais $d(f(x_n),f(y_n))\ge\varepsilon>0$.

> [!EXAMPLE] Rédaction modèle (comme sur la copie)
> « $u(x)=x^2$ n'est pas U.C. sur $\mathbb R$ : avec $x_n=n$, $y_n=n+\frac1n$, $|x_n-y_n|=\frac1n\to0$ mais $|u(y_n)-u(x_n)|=2+\frac1{n^2}\ge2$. Sur $[-a,a]$ (compact), $u$ est continue donc U.C. par Heine ; directement, $|x^2-y^2|=|x+y||x-y|\le2a|x-y|$. »

## 🔗 Liens

- **S'appuie sur** : [[topo-hierarchie-lipschitz-uc-continue|Lipschitzienne ⇒ uniformément continue ⇒ continue]], [[topo-heine|Théorème de Heine]]
- **Méthodes voisines** : —
- **Voir aussi** : —
