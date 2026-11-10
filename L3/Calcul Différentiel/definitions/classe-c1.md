---
aliases:
  - "Application de classe C1"
  - "C1"
  - "continûment différentiable"
  - "classe C^1"
  - "différentiable sur un ouvert"
tags:
  - cd
  - cd/definition
  - cd/chapitre-02
---

# 📘 Application de classe C1

*Définition* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Déf. 2.12, 2.13 et 3.14 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> - $f$ est **différentiable sur $U$** si elle l'est en tout point de $U$. Sa différentielle est alors l'application $Df:U\to\mathcal L_c(E,F)$, $a\mapsto Df_a$.
> - $f$ est **de classe $\mathcal C^1$ sur $U$** si $f$ est différentiable sur $U$ et si $Df:U\to(\mathcal L_c(E,F),\lvert\!\lvert\!\lvert \cdot\rvert\!\rvert\!\rvert)$ est continue, c'est-à-dire
> $$\forall a\in U,\qquad \lvert\!\lvert\!\lvert Df_x-Df_a\rvert\!\rvert\!\rvert\xrightarrow[x\to a]{}0.$$

> [!IMPORTANT] En pratique sur $\mathbb R^n$ (Cor. 3.16)
> $f:U\subset\mathbb R^n\to F$ est $\mathcal C^1$ $\iff$ toutes les dérivées partielles existent en tout point de $U$ et sont **continues sur $U$** → [[critere-c1]].

> [!WARNING] Pièges
> - $\mathcal C^1\Rightarrow$ différentiable $\Rightarrow$ continue. Aucune réciproque.
> - La continuité de $Df$ se mesure avec la norme d'opérateur, pas « pour chaque $h$ ».

## 🔗 Liens

- **S'appuie sur** : [[differentiabilite|Différentiabilité en un point, différentielle]], [[norme-operateur|Norme d'opérateur]]
- **Utilisé par (définitions)** : [[differentielle-seconde|Différentielle seconde, classe C2]], [[diffeomorphisme|Difféomorphisme, difféomorphisme local]]
- **Utilisé par (théorèmes)** : [[critere-c1|Critère C1 par les dérivées partielles]]
- **Méthodes** : [[montrer-classe-c1|Montrer qu'une application est de classe C1 (ou C2)]]
