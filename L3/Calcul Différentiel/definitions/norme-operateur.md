---
aliases:
  - "Norme d'opérateur"
  - "norme triple"
  - "norme subordonnée"
  - "norme d'une application linéaire continue"
  - "|||f|||"
tags:
  - cd
  - cd/definition
  - cd/chapitre-01
---

# 📘 Norme d'opérateur

*Définition* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Déf. 1.48 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> Pour $f\in\mathcal L_c(E,F)$, on pose
> $$\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert=\sup_{\lVert u\rVert_E\le1}\lVert f(u)\rVert_F.$$
> Ce sup est fini (Th. 1.43 (iii)), et $(\mathcal L_c(E,F),\lvert\!\lvert\!\lvert \cdot\rvert\!\rvert\!\rvert)$ est un e.v.n. (Prop. 1.49).

> [!IMPORTANT] Formules équivalentes (Prop. 1.50)
> $$\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert=\sup_{u\ne0}\frac{\lVert f(u)\rVert_F}{\lVert u\rVert_E}=\sup_{\lVert u\rVert=1}\lVert f(u)\rVert_F,\qquad \forall u\in E,\ \lVert f(u)\rVert_F\le\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert\,\lVert u\rVert_E.$$
> $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert$ est la **plus petite** constante $C$ telle que $\lVert f(u)\rVert\le C\lVert u\rVert$ pour tout $u$ → [[caracterisations-norme-operateur]].

> [!TIP] En clair
> $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert$ est le plus grand facteur par lequel $f$ peut « agrandir » un vecteur.

> [!WARNING] Pièges
> - $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert$ dépend des normes choisies au départ **et** à l'arrivée.
> - Majorer $\lVert f(u)\rVert\le C\lVert u\rVert$ donne seulement $\lvert\!\lvert\!\lvert f\rvert\!\rvert\!\rvert\le C$. Pour l'égalité il faut **atteindre** $C$ → [[calculer-norme-operateur]].

## 🔗 Liens

- **S'appuie sur** : [[application-lineaire-continue|Application linéaire continue, espace Lc(E,F)]]
- **Utilisé par (définitions)** : [[classe-c1|Application de classe C1]]
- **Utilisé par (théorèmes)** : [[caracterisations-norme-operateur|Caractérisations de la norme d'opérateur]], [[norme-composee|Norme d'une composée]], [[espaces-de-banach-usuels|Espaces de Banach usuels]], [[iaf|Inégalité des accroissements finis (IAF)]]
- **Méthodes** : [[calculer-norme-operateur|Calculer une norme d'opérateur]]
