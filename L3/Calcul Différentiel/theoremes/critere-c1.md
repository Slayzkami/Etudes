---
aliases:
  - "Critère C1 par les dérivées partielles"
  - "Théorème 3.15"
  - "Corollaire 3.16"
  - "dérivées partielles continues donc C1"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-03
---

# ⭐ Critère C1 par les dérivées partielles

*Théorème* · Chapitre : [[03-accroissements-finis|3 – Accroissements finis]] · Th. 3.15, Cor. 3.16 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> Soit $E=E_1\times\dots\times E_n$, $U\subset E$ ouvert, $f:U\to F$. $f$ est de classe $\mathcal C^1$ sur $U$ si et seulement si, pour tout $j$, $\partial_jf(x)$ existe en tout point $x\in U$ et $x\mapsto\partial_jf(x)$ est continue sur $U$.
>
> **Cas $E=\mathbb R^n$ (Cor. 3.16)** : $f$ est $\mathcal C^1$ sur $U$ $\iff$ les dérivées partielles $\dfrac{\partial f}{\partial x_j}$ existent en tout point de $U$ et sont **continues sur $U$**.

> [!SUCCESS]- Idée de la démonstration ($n=2$)
> On écrit $f(a+h)-f(a)=[f(a_1+h_1,a_2+h_2)-f(a_1,a_2+h_2)]+[f(a_1,a_2+h_2)-f(a_1,a_2)]$. Le second crochet vaut $\partial_2f(a)(h_2)+o(h_2)$ par définition. Pour le premier, on applique l'IAF à $x_1\mapsto f(x_1,a_2+h_2)-\partial_1f(a)(x_1)$, dont la différentielle $\partial_1f(x_1,a_2+h_2)-\partial_1f(a)$ est petite par **continuité** de $\partial_1f$. On obtient $f(a+h)-f(a)=\partial_1f(a)(h_1)+\partial_2f(a)(h_2)+o(h)$. $\blacksquare$

> [!TIP] Le point important
> C'est le moyen le plus rapide de prouver qu'une fonction de $\mathbb R^n$ est **différentiable** : dérivées partielles continues $\Rightarrow$ $\mathcal C^1$ $\Rightarrow$ différentiable.

> [!WARNING] Pièges
> - Il faut la **continuité** des dérivées partielles, pas seulement leur existence.
> - Si les dérivées partielles ne sont pas continues en un point, on ne peut **rien conclure** : $f$ peut quand même y être différentiable → [[etudier-en-un-point-particulier]].

## 🔗 Liens

- **S'appuie sur** : [[classe-c1|Application de classe C1]], [[derivee-partielle|Dérivée partielle]], [[differentielle-partielle|Différentielle partielle]], [[iaf|Inégalité des accroissements finis (IAF)]]
- **Utilisé par (théorèmes)** : [[critere-c2|Critère C2]]
- **Méthodes** : [[differentiabilite-par-theoremes|Montrer la différentiabilité par les théorèmes généraux]], [[calculer-jacobienne|Calculer une jacobienne et une différentielle sur R^n]], [[etudier-en-un-point-particulier|Étudier une fonction en un point particulier (souvent (0,0))]], [[montrer-classe-c1|Montrer qu'une application est de classe C1 (ou C2)]]
