---
aliases:
  - "Méthode : la somme A + B"
  - "A+B"
  - "somme de Minkowski"
tags:
  - topologie
  - topo/methode
  - topo/chapitre-03
---

# 🛠️ Méthode : la somme A + B

*Méthode* · Chapitre : [[03-espaces-metriques-compacts|3 – Espaces métriques compacts]] · Écrit 2022-23 et interro 2025-26 (utilise Th. 3.11, Prop. 3.24, 3.27) · [[topo-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> $A+B=\{x+y\mid x\in A,\ y\in B\}$ dans $\mathbb R^n$.
> | Hypothèses | Conclusion | Argument |
> |---|---|---|
> | $A$ compact, $B$ fermé | $A+B$ **fermé** | suites : extraire dans $A$, puis $b=z-a\in B$ car $B$ fermé |
> | $A$, $B$ compacts | $A+B$ **compact** | $A+B=s(A\times B)$, $s(x,y)=x+y$ continue |
> | $A$ **ouvert**, $B$ quelconque | $A+B$ **ouvert** | $A+B=\bigcup_{b\in B}(A+b)$, et chaque translaté $A+b$ est ouvert |
> | $A$, $B$ seulement fermés | **pas forcément fermé** | $A=\mathbb N$, $B=\{-n+\frac1n\mid n\ge2\}$ |

> [!EXAMPLE] Rédaction modèle (comme sur la copie)
> *$A$ compact, $B$ fermé.* « Soit $z_k=a_k+b_k$ ($a_k\in A$, $b_k\in B$) une suite de $A+B$ qui converge vers $z$. $A$ étant compact, il existe $\varphi$ strictement croissante et $a\in A$ avec $a_{\varphi(k)}\to a$. Alors $b_{\varphi(k)}=z_{\varphi(k)}-a_{\varphi(k)}\to z-a$, et $B$ est fermé, donc $z-a\in B$. Ainsi $z=a+(z-a)\in A+B$ : $A+B$ est fermé. »

> [!TIP] Astuces
> Contre-exemple « fermés » : $\frac1n=n+(-n+\frac1n)\in A+B$ tend vers $0$, et $0\notin A+B$ car $m-n+\frac1n=0$ forcerait $\frac1n=n-m\in\mathbb Z$.
> Pourquoi $A$, $B$ fermés : deux éléments distincts sont à distance $\ge1$, donc une suite convergente est stationnaire.

## 🔗 Liens

- **S'appuie sur** : [[topo-bolzano-weierstrass|Caractérisation séquentielle des compacts (Bolzano–Weierstrass)]], [[topo-image-continue-compact|Image continue d'un compact ; bijection continue sur un compact]], [[topo-produit-de-compacts|Produit de compacts]], [[topo-stabilite-ouverts|Stabilité des ouverts]]
- **Méthodes voisines** : —
- **Corrigés** : [[topo-exercices-types-corriges#3. La somme A + B|ex. 3]]
- **Voir aussi** : —
