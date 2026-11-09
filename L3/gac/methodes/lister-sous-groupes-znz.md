---
aliases:
  - "Méthode : lister les sous-groupes de Z/nZ (treillis)"
  - "sous-groupes de Z/nZ"
  - "treillis"
  - "diagramme des inclusions"
tags:
  - gac
  - gac/methode
  - gac/chapitre-02
---

# 🛠️ Méthode : lister les sous-groupes de Z/nZ (treillis)

*Méthode* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · [[index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> Les sous-groupes de $\mathbb Z/n\mathbb Z$ sont les $\langle\bar d\rangle=d\mathbb Z/n\mathbb Z$ pour $d$ **diviseur positif de $n$**, et $\langle\bar d\rangle$ a $n/d$ éléments.
>
> **Justification avec le cours** : si $H\le\mathbb Z/n\mathbb Z$, $p^{-1}(H)$ est un sous-groupe de $\mathbb Z$ ([[noyau-et-image|image réciproque]]) contenant $n\mathbb Z=p^{-1}(\{\bar0\})$, donc $=d\mathbb Z$ ([[sous-groupes-de-z]]) avec $d\mid n$, et $H=p(d\mathbb Z)=\langle\bar d\rangle$.
>
> **Treillis** : $\langle\bar a\rangle\subset\langle\bar b\rangle\iff b\mid a$ (pour $a,b\mid n$). On dessine les diviseurs, du plus grand ($\{\bar0\}$, en bas) au plus petit ($\langle\bar1\rangle$, en haut).

> [!EXAMPLE] $\mathbb Z/12\mathbb Z$ (diviseurs 1, 2, 3, 4, 6, 12)
> $\langle\bar1\rangle$ (12), $\langle\bar2\rangle=\{\bar0,\bar2,\bar4,\bar6,\bar8,\overline{10}\}$ (6), $\langle\bar3\rangle=\{\bar0,\bar3,\bar6,\bar9\}$ (4), $\langle\bar4\rangle=\{\bar0,\bar4,\bar8\}$ (3), $\langle\bar6\rangle=\{\bar0,\bar6\}$ (2), $\{\bar0\}$ (1).

> [!EXAMPLE] $\mathbb Z/18\mathbb Z$ (sujet 2025)
> Diviseurs 1, 2, 3, 6, 9, 18 : $\langle\bar1\rangle$ (18), $\langle\bar2\rangle$ (9), $\langle\bar3\rangle$ (6), $\langle\bar6\rangle$ (3), $\langle\bar9\rangle$ (2), $\{\bar0\}$ (1).
> Inclusions : $\{\bar0\}\subset\langle\bar9\rangle\subset\langle\bar3\rangle$, $\{\bar0\}\subset\langle\bar6\rangle\subset\langle\bar3\rangle$ et $\langle\bar6\rangle\subset\langle\bar2\rangle$, puis $\langle\bar2\rangle,\langle\bar3\rangle\subset\langle\bar1\rangle$.

## 🔗 Liens

- **Utilisé par (théorèmes)** : [[sous-groupes-de-z|Sous-groupes de (Z,+)]]
- **Voir aussi** : [[intersection-sous-groupes|Intersection et réunion de sous-groupes]]
