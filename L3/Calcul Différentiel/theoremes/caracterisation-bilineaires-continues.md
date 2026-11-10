---
aliases:
  - "Caractérisation des applications bilinéaires continues"
  - "bilinéaire continue ssi"
  - "||B(u,v)|| ≤ C||u|| ||v||"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-01
---

# ⭐ Caractérisation des applications bilinéaires continues

*Théorème* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Prop. 1.53 et 1.55 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Proposition
> Soit $B:E_1\times E_2\to F$ bilinéaire. $B$ est continue si et seulement si
> $$\exists C\ge0,\ \forall(u,v)\in E_1\times E_2,\qquad \lVert B(u,v)\rVert_F\le C\,\lVert u\rVert_{E_1}\lVert v\rVert_{E_2}.$$
> Si $E_1$ et $E_2$ sont de dimension finie, toute application bilinéaire est continue (Prop. 1.55).

> [!SUCCESS]- Démonstration (sens ⇐, astuce d'ajout-retrait)
> $B(u,v)-B(a,b)=B(u-a,v)+B(a,v-b)$, donc
> $\lVert B(u,v)-B(a,b)\rVert\le C\lVert u-a\rVert\lVert v\rVert+C\lVert a\rVert\lVert v-b\rVert\to0$ quand $(u,v)\to(a,b)$ (car $\lVert v\rVert$ reste borné). $\blacksquare$

> [!TIP] L'astuce à retenir
> **Ajouter et retrancher** un terme mixte : $B(u,v)-B(a,b)=B(u-a,v)+B(a,v-b)$. Elle resservira pour montrer qu'une application est $\mathcal C^1$ → [[montrer-classe-c1]].

## 🔗 Liens

- **S'appuie sur** : [[application-bilineaire|Application bilinéaire (continue)]]
- **Utilisé par (théorèmes)** : [[differentielles-de-reference|Différentielles de référence : constante, linéaire, bilinéaire]]
- **Méthodes** : [[montrer-classe-c1|Montrer qu'une application est de classe C1 (ou C2)]]
