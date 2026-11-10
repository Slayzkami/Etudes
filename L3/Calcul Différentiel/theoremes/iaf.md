---
aliases:
  - "Inégalité des accroissements finis (IAF)"
  - "IAF"
  - "inégalité des accroissements finis"
  - "Théorème 3.11"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-03
---

# ⭐ Inégalité des accroissements finis (IAF)

*Théorème* · Chapitre : [[03-accroissements-finis|3 – Accroissements finis]] · Th. 3.8, 3.9 et 3.11 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème (cas général, Th. 3.11)
> Soient $E,F$ des e.v.n., $U\subset E$ un ouvert et $f:U\to F$ différentiable sur $U$. Soient $a,b\in U$ tels que **$[a,b]\subset U$**. S'il existe $M\ge0$ tel que $\lvert\!\lvert\!\lvert Df_x\rvert\!\rvert\!\rvert\le M$ pour tout $x\in[a,b]$, alors
> $$\lVert f(b)-f(a)\rVert_F\le M\,\lVert b-a\rVert_E.$$

> [!NOTE] Les trois hypothèses à écrire
> 1. $f$ différentiable sur l'ouvert $U$ ;
> 2. le segment $[a,b]$ est inclus dans $U$ ;
> 3. $\lvert\!\lvert\!\lvert Df_x\rvert\!\rvert\!\rvert\le M$ sur le segment.

> [!SUCCESS]- Démonstration (à partir du Th. 3.9)
> Th. 3.9 (démontré dans le cours rédigé) : si $g:I\to F$ est continue sur $[0,1]$, dérivable sur $]0,1[$ avec $\lVert g'(t)\rVert\le M'$, alors $\lVert g(1)-g(0)\rVert\le M'$.
> On l'applique à $g(t)=f(a+t(b-a))$ : $g'(t)=Df_{a+t(b-a)}(b-a)$, donc $\lVert g'(t)\rVert\le\lvert\!\lvert\!\lvert Df_{a+t(b-a)}\rvert\!\rvert\!\rvert\,\lVert b-a\rVert\le M\lVert b-a\rVert$. D'où $\lVert f(b)-f(a)\rVert=\lVert g(1)-g(0)\rVert\le M\lVert b-a\rVert$. $\blacksquare$

> [!TIP] Versions en une variable
> Th. 3.8 : $f:[a,b]\to\mathbb R$ continue, dérivable sur $]a,b[$, $\lvert f'\rvert\le M$ $\Rightarrow$ $\lvert f(b)-f(a)\rvert\le M(b-a)$.

> [!WARNING] Pièges
> - Oublier que le **segment** doit être dans $U$.
> - $M$ majore la **norme d'opérateur** de $Df_x$, pas $\lVert Df_x(h)\rVert$ pour un $h$.

## 🔗 Liens

- **S'appuie sur** : [[differentiabilite|Différentiabilité en un point, différentielle]], [[norme-operateur|Norme d'opérateur]], [[segment-et-convexe|Segment, partie convexe]]
- **Utilisé par (théorèmes)** : [[iaf-sur-un-convexe|IAF sur un convexe : différentielle bornée implique lipschitzienne]], [[critere-c1|Critère C1 par les dérivées partielles]], [[inversion-locale|Théorème d'inversion locale]]
- **Méthodes** : [[utiliser-iaf|Utiliser l'inégalité des accroissements finis (montrer lipschitzienne)]]
