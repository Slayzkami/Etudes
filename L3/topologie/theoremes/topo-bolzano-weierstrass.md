---
aliases:
  - "Caractérisation séquentielle des compacts (Bolzano–Weierstrass)"
  - "Bolzano-Weierstrass"
  - "compact par les suites"
  - "valeur d'adhérence"
  - "lemme de Lebesgue"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-03
---

# ⭐ Caractérisation séquentielle des compacts (Bolzano–Weierstrass)

*Théorème* · Chapitre : [[03-espaces-metriques-compacts|3 – Espaces métriques compacts]] · Th. 3.11 et Lemme 3.12 du cours (poly : Th. 3.1, Lemme 3.1) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Un espace métrique $(E,d)$ est compact **si et seulement si** de toute suite de $E$ on peut extraire une sous-suite convergente **dans $E$**.

> [!SUCCESS]- Démonstration
> ($\Rightarrow$) $F_n=\overline{\{x_k\mid k\ge n\}}$ : fermés non vides décroissants, donc il existe $\ell\in\bigcap F_n$ ; on construit $n_1<n_2<\dots$ avec $d(x_{n_k},\ell)<\frac1k$.
> ($\Leftarrow$) *Lemme de Lebesgue* : il existe $r>0$ tel que toute boule $B(x,r)$ soit dans un des $O_i$. On choisit $x_1,x_2,\dots$ hors des ouverts déjà pris ; si le procédé ne s'arrêtait pas, $d(x_n,x_m)\ge r$ pour $n\neq m$ et aucune sous-suite ne convergerait.

> [!TIP] Réflexes
> C'est **l'outil de travail** : « soit $(x_n)$ une suite de $K$ ; par compacité, il existe $\varphi$ strictement croissante et $\ell\in K$ tels que $x_{\varphi(n)}\to\ell$ ».

> [!WARNING] Pièges
> La limite doit être **dans la partie** : $1-\frac1n\to1\notin[0,1[$ (Piège 3.3).

## 🔗 Liens

- **S'appuie sur** : [[topo-espace-compact|Espace compact]], [[topo-suite-extraite|Suite extraite]], [[topo-version-fermes-compacite|Compacité : version « fermés » et fermés emboîtés]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-bolzano-weierstrass-dans-r|Bolzano–Weierstrass dans R ; les segments sont compacts]], [[topo-image-continue-compact|Image continue d'un compact ; bijection continue sur un compact]], [[topo-produit-de-compacts|Produit de compacts]], [[topo-heine|Théorème de Heine]], [[topo-compact-complet-borne|Un compact est complet et borné ; une partie compacte est fermée et bornée]], [[topo-ferme-dans-compact|Un fermé dans un compact est compact]]
- **Méthodes** : [[topo-montrer-compact|Méthode : montrer qu'une partie est compacte]], [[topo-exploiter-compacite|Méthode : exploiter la compacité]], [[topo-montrer-non-compact|Méthode : montrer qu'une partie n'est pas compacte]], [[topo-somme-a-plus-b|Méthode : la somme A + B]]
- **Voir aussi** : —
