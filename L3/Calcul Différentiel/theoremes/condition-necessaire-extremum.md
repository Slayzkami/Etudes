---
aliases:
  - "Condition nécessaire d'extremum (ordre 1)"
  - "Proposition 4.20"
  - "extremum donc point critique"
  - "Fermat"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-04
---

# ⭐ Condition nécessaire d'extremum (ordre 1)

*Théorème* · Chapitre : [[04-differentielles-ordre-superieur|4 – Différentielles d'ordre supérieur]] · Prop. 4.20 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Proposition
> Soit $U$ un **ouvert** de $E$ et $f:U\to\mathbb R$ différentiable en $a$. Si $f$ admet un extremum local en $a$, alors $a$ est un point critique : $Df_a=0$.

> [!SUCCESS]- Démonstration
> Soit $v\in E$ et $g(t)=f(a+tv)$, définie pour $\abs t$ petit ($U$ ouvert). $g$ est dérivable en $0$ avec $g'(0)=Df_a(v)$ (Prop. 2.9) et admet un extremum local en $0$. D'après le résultat en une variable, $g'(0)=0$. Donc $Df_a(v)=0$ pour tout $v$. $\blacksquare$

> [!WARNING] Pièges
> - Réciproque fausse : $x^2-y^2$ en $(0,0)$, $x^3$ en $0$.
> - Faux si $U$ n'est pas ouvert (extremum au bord).

## 🔗 Liens

- **S'appuie sur** : [[extremum-local|Extremum local, extremum global]], [[point-critique|Point critique]], [[differentielle-et-derivees-directionnelles|Différentielle et dérivées directionnelles]]
- **Utilisé par (théorèmes)** : [[extrema-et-hessienne|Extrema et différentielle seconde]]
- **Méthodes** : [[extremum-global|Montrer l'existence d'un extremum global]]
