---
aliases:
  - "Linéaire au départ d'une dimension finie : continue"
  - "Théorème 1.44"
  - "départ de dimension finie"
  - "linéaire en dimension finie donc continue"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-01
---

# ⭐ Linéaire au départ d'une dimension finie : continue

*Théorème* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Th. 1.44 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> Si $E$ est de **dimension finie**, toute application linéaire $f:E\to F$ est continue.

> [!SUCCESS]- Démonstration
> Soit $(e_1,\dots,e_n)$ une base de $E$ et $\lVert u\rVert_\infty=\max_i\lvert u_i\rvert$ pour $u=\sum_iu_ie_i$. Alors
> $$\lVert f(u)\rVert_F=\Big\|\sum_iu_if(e_i)\Big\|_F\le\sum_i\lvert u_i\rvert\,\lVert f(e_i)\rVert_F\le\Big(\sum_i\lVert f(e_i)\rVert_F\Big)\lVert u\rVert_\infty.$$
> Toutes les normes de $E$ étant équivalentes (Th. 1.13), $\lVert u\rVert_\infty\le\beta\lVert u\rVert_E$ : on a (iv) du Th. 1.43. $\blacksquare$

> [!TIP] Phrase à écrire sur la copie
> « $L$ est linéaire et $E$ est de dimension finie, donc $L$ est continue (Théorème 1.44). »

> [!WARNING] Piège
> C'est la dimension de l'espace de **départ** qui compte. En dimension infinie c'est faux → [[application-lineaire-continue]].

## 🔗 Liens

- **S'appuie sur** : [[caracterisation-lineaires-continues|Caractérisations des applications linéaires continues]], [[equivalence-normes-dimension-finie|Équivalence des normes en dimension finie]]
- **Méthodes** : [[continuite-application-lineaire|Continuité d'une application linéaire]], [[differentiabilite-par-definition|Montrer la différentiabilité par la définition]], [[differentielle-sur-les-matrices|Calculer une différentielle sur les matrices]]
