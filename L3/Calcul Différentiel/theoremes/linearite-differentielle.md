---
aliases:
  - "Linéarité de la différentielle"
  - "Théorème 2.19"
  - "différentielle d'une somme"
  - "D(αf+βg)"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-02
---

# ⭐ Linéarité de la différentielle

*Théorème* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Th. 2.19 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> Si $f,g:U\to F$ sont différentiables en $a$, alors pour tous $\alpha,\beta\in\mathbb K$, $\alpha f+\beta g$ est différentiable en $a$ et
> $$D(\alpha f+\beta g)_a=\alpha\,Df_a+\beta\,Dg_a.$$

> [!SUCCESS]- Démonstration
> $(\alpha f+\beta g)(a+h)-(\alpha f+\beta g)(a)=\alpha Df_a(h)+\beta Dg_a(h)+\alpha\,o(h)+\beta\,o(h)$. L'application $\alpha Df_a+\beta Dg_a$ est linéaire continue, et $\alpha\,o(h)+\beta\,o(h)=o(h)$ (Lemme 2.2). $\blacksquare$

> [!WARNING] Piège
> $f$ et $g$ doivent être à valeurs dans le **même** espace $F$. Pour une fonction à valeurs dans un produit, c'est la [[differentiabilite-par-composantes]] qu'on utilise.

## 🔗 Liens

- **S'appuie sur** : [[differentiabilite|Différentiabilité en un point, différentielle]]
- **Méthodes** : [[differentiabilite-par-theoremes|Montrer la différentiabilité par les théorèmes généraux]]
