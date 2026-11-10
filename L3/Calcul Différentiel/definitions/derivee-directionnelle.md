---
aliases:
  - "Dérivée directionnelle"
  - "dérivée selon un vecteur"
  - "dérivée dans la direction v"
  - "f'_v(0)"
tags:
  - cd
  - cd/definition
  - cd/chapitre-02
---

# 📘 Dérivée directionnelle

*Définition* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Déf. 2.8 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> Soit $v\in E$. $f$ est **dérivable en $a$ dans la direction $v$** si la fonction d'une variable réelle $f_v:t\mapsto f(a+tv)$, définie au voisinage de $0$, est dérivable en $0$. On note
> $$f_v'(0)=\lim_{t\to0}\frac{f(a+tv)-f(a)}{t}\ \in F.$$

> [!IMPORTANT] Lien avec la différentielle (Prop. 2.9)
> Si $f$ est différentiable en $a$, alors $f$ est dérivable en $a$ dans **toutes** les directions et $f_v'(0)=Df_a(v)$ → [[differentielle-et-derivees-directionnelles]].

> [!EXAMPLE] Calcul type (Écrit 2025-2026)
> $f(x,y)=(\cos(x+2y),\sin(2x+y))$, dérivée en $(\pi/2,0)$ dans la direction $(1,1)$ : c'est $J_f(\pi/2,0)\binom11$.

> [!WARNING] Piège
> La réciproque est **fausse** : $f$ peut avoir des dérivées dans toutes les directions sans être différentiable, ni même continue (Rem. 2.10, Ex. 2.11).

## 🔗 Liens

- **S'appuie sur** : [[differentiabilite|Différentiabilité en un point, différentielle]]
- **Utilisé par (définitions)** : [[derivee-partielle|Dérivée partielle]]
- **Utilisé par (théorèmes)** : [[differentielle-et-derivees-directionnelles|Différentielle et dérivées directionnelles]]
- **Méthodes** : [[calculer-derivee-directionnelle|Calculer une dérivée directionnelle]]
