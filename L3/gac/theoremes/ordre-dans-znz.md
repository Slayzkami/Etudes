---
aliases:
  - "Ordre d'un élément de Z/nZ"
  - "n/pgcd(n,k)"
  - "ordre dans Z/nZ"
  - "générateurs de Z/nZ"
tags:
  - gac
  - gac/theoreme
  - gac/chapitre-02
---

# ⭐ Ordre d'un élément de Z/nZ

*Théorème* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · § II.6 du cours · [[index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Dans $(\mathbb Z/n\mathbb Z,+)$ : $\displaystyle o(\bar k)=\frac{n}{\operatorname{pgcd}(n,k)}$. En particulier $\bar k$ engendre $\mathbb Z/n\mathbb Z\iff\operatorname{pgcd}(n,k)=1$.

> [!SUCCESS]- Démonstration
> $d=\operatorname{pgcd}(n,k)$, $n=dn'$, $k=dk'$, $\operatorname{pgcd}(n',k')=1$. $m\bar k=\bar0\iff n\mid mk\iff n'\mid mk'\iff n'\mid m$ (Gauss). Le plus petit $m\ge1$ est $n'$.

> [!EXAMPLE] $\mathbb Z/12\mathbb Z$ et $\mathbb Z/18\mathbb Z$
> | $\mathbb Z/12$ | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 |
> |---|---|---|---|---|---|---|---|---|---|---|---|---|
> | ordre | 1 | 12 | 6 | 4 | 3 | 12 | 2 | 12 | 3 | 4 | 6 | 12 |
>
> $\mathbb Z/6\mathbb Z$ : $o(\bar0)=1$, $o(\bar1)=o(\bar5)=6$, $o(\bar2)=o(\bar4)=3$, $o(\bar3)=2$.

## 🔗 Liens

- **S'appuie sur** : [[ordre-element|Ordre d'un élément]]
- **Méthodes** : [[calculer-ordre|Méthode : calculer l'ordre d'un élément]]
- **Voir aussi** : [[lister-sous-groupes-znz|Méthode : lister les sous-groupes de Z/nZ (treillis)]]
