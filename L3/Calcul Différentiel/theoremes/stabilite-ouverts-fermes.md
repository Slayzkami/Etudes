---
aliases:
  - "Stabilité des ouverts et des fermés"
  - "réunion d'ouverts"
  - "intersection de fermés"
  - "O1 O2 O3"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-01
---

# ⭐ Stabilité des ouverts et des fermés

*Théorème* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Th. 1.22 et 1.23 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> - **(O1)** $E$ et $\emptyset$ sont ouverts. **(O2)** Une réunion **quelconque** d'ouverts est un ouvert. **(O3)** Une intersection **finie** d'ouverts est un ouvert.
> - **(F1)** $E$ et $\emptyset$ sont fermés. **(F2)** Une intersection **quelconque** de fermés est un fermé. **(F3)** Une réunion **finie** de fermés est un fermé.

> [!SUCCESS]- Démonstration
> **(O2)** Si $x\in\bigcup_iO_i$, alors $x\in O_{i_0}$ pour un $i_0$ ; il existe $r>0$ avec $B(x,r)\subset O_{i_0}\subset\bigcup_iO_i$.
> **(O3)** Si $x\in O_1\cap\dots\cap O_m$, il existe $r_k>0$ avec $B(x,r_k)\subset O_k$. On pose $r=\min(r_1,\dots,r_m)>0$ (minimum d'un nombre **fini** de réels $>0$) : $B(x,r)\subset O_1\cap\dots\cap O_m$.
> **(F2), (F3)** : passer au complémentaire. $\blacksquare$

> [!EXAMPLE] Contre-exemples
> $\bigcap_{n\ge1}\,]-\frac1n,\frac1n[=\{0\}$ n'est pas ouvert ; $\bigcup_{n\ge1}[\frac1n,1]=\,]0,1]$ n'est pas fermé.

## 🔗 Liens

- **S'appuie sur** : [[ouvert-ferme|Ouvert, fermé]]
- **Méthodes** : [[montrer-ouvert-ferme|Montrer qu'une partie est ouverte ou fermée]]
