---
aliases:
  - "Différentielle de la réciproque"
  - "Proposition 5.4"
  - "D(f^-1)"
  - "jacobienne de la réciproque"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-05
---

# ⭐ Différentielle de la réciproque

*Théorème* · Chapitre : [[05-inversion-locale-fonctions-implicites|5 – Inversion locale et fonctions implicites]] · Prop. 5.4 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Proposition
> Si $f:U\to V$ est un difféomorphisme, alors pour tout $a\in U$, $Df_a$ est un isomorphisme de $E$ sur $F$ et
> $$D(f^{-1})_{f(a)}=(Df_a)^{-1}.$$
> En particulier $\dim E=\dim F$. En dimension finie : $J_{f^{-1}}(f(a))=[J_f(a)]^{-1}$.

> [!SUCCESS]- Démonstration
> $f^{-1}\circ f=\mathrm{id}_U$ et $f\circ f^{-1}=\mathrm{id}_V$. On différentie par la règle de la chaîne ($D(\mathrm{id})=\mathrm{id}$) :
> $D(f^{-1})_{f(a)}\circ Df_a=\mathrm{id}_E$ et $Df_a\circ D(f^{-1})_{f(a)}=\mathrm{id}_F$.
> Donc $Df_a$ est bijective, d'inverse $D(f^{-1})_{f(a)}$, qui est linéaire continue. $\blacksquare$

> [!TIP] Conséquence
> En un point où $\det J_f(a)=0$, $f$ n'est **pas** un difféomorphisme local.

> [!WARNING] Piège
> $J_{f^{-1}}$ se calcule **au point $f(a)$** et vaut l'inverse de $J_f$ **au point $a$**.

## 🔗 Liens

- **S'appuie sur** : [[diffeomorphisme|Difféomorphisme, difféomorphisme local]], [[regle-de-la-chaine|Règle de la chaîne (différentielle d'une composée)]]
- **Utilisé par (théorèmes)** : [[inversion-locale|Théorème d'inversion locale]]
- **Méthodes** : [[montrer-diffeomorphisme|Montrer qu'une application est un difféomorphisme (local ou global)]]
