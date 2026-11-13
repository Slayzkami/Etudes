---
aliases:
  - "Espace compact"
  - "compact"
  - "compacité"
  - "Borel-Lebesgue (définition)"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-03
---

# 📘 Espace compact

*Définition* · Chapitre : [[03-espaces-metriques-compacts|3 – Espaces métriques compacts]] · Déf. 3.3 du cours (poly : Déf. 3.2) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> $(E,d)$ est **compact** si de tout recouvrement ouvert de $E$ on peut extraire un sous-recouvrement fini :
> $$\forall(O_i)_{i\in I}\ \text{ouverts},\ E\subset\bigcup_{i\in I}O_i\ \Rightarrow\ \exists i_1,\dots,i_n\in I,\ E\subset O_{i_1}\cup\dots\cup O_{i_n}.$$

> [!IMPORTANT] À retenir
> - **Caractérisation séquentielle (Bolzano–Weierstrass, Th. 3.11)** : $E$ compact $\iff$ toute suite de $E$ admet une sous-suite qui converge **dans $E$** → [[topo-bolzano-weierstrass]]. C'est elle qu'on utilise en pratique.
> - Compact $\Rightarrow$ complet et borné ; dans $\mathbb R^n$ : compact $\iff$ fermé et borné → [[topo-borel-lebesgue]].

> [!EXAMPLE] Exemples
> Compacts : $[a,b]$, un ensemble fini, $\{0\}\cup\{\frac1n\}$, la sphère unité de $\mathbb R^n$. Non compacts : $\mathbb R$, $]0,1[$, $[0,1[$, $\mathbb N$ discret.

> [!WARNING] Pièges
> - « Fermé borné » est un **théorème** (vrai dans $\mathbb R^n$), pas la définition (mon erreur au bilan) ; faux en général (Piège 3.1).
> - Trouver **un** recouvrement fini ne prouve rien : il faut que **tout** recouvrement ouvert en ait un (Piège 3.2).

## 🔗 Liens

- **S'appuie sur** : [[topo-recouvrement|Recouvrement]]
- **Utilisé par (définitions)** : [[topo-partie-compacte|Partie compacte]]
- **Utilisé par (théorèmes)** : [[topo-bolzano-weierstrass|Caractérisation séquentielle des compacts (Bolzano–Weierstrass)]], [[topo-version-fermes-compacite|Compacité : version « fermés » et fermés emboîtés]], [[topo-riesz|Théorème de Riesz]]
- **Méthodes** : [[topo-montrer-compact|Méthode : montrer qu'une partie est compacte]], [[topo-montrer-non-compact|Méthode : montrer qu'une partie n'est pas compacte]]
- **Voir aussi** : [[topo-partie-compacte|Partie compacte]]
