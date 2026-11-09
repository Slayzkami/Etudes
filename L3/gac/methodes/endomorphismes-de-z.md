---
aliases:
  - "Méthode : morphismes de source Z (endomorphismes de (Z,+))"
  - "endomorphismes de Z"
  - "Hom(Z,G)"
  - "morphismes de Z"
tags:
  - gac
  - gac/methode
  - gac/chapitre-02
---

# 🛠️ Méthode : morphismes de source Z (endomorphismes de (Z,+))

*Méthode* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · [[index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> Un morphisme $f:(\mathbb Z,+)\to G$ est **déterminé par $f(1)$** : $f(n)=n\,f(1)$ (propriété $f(x^n)=f(x)^n$ en additif).
> Réciproquement, pour tout $a\in G$, $n\mapsto na$ est un morphisme ($(n+m)a=na+ma$).

> [!EXAMPLE] Endomorphismes de $(\mathbb Z,+)$ (sujet 2025, ex. 4)
> Ce sont exactement les $f_a:n\mapsto an$, $a\in\mathbb Z$.
> - Si $f$ est un endomorphisme, posons $a=f(1)$ : $f(n)=nf(1)=an$ ([[proprietes-morphismes]]).
> - Réciproquement $f_a(n+m)=an+am=f_a(n)+f_a(m)$.
> - Bonus : automorphismes : $f_a$ bijective $\iff a=\pm1$ ; donc $\mathrm{Aut}(\mathbb Z)=\{\mathrm{id},-\mathrm{id}\}$.

> [!EXAMPLE] Morphismes de $\mathbb Z/n\mathbb Z$ dans un groupe
> $f$ est déterminé par $a=f(\bar1)$, et il faut $na=0$ (car $n\bar1=\bar0$). Ex. : $\mathrm{Aut}(\mathbb Z/4\mathbb Z)=\{\mathrm{id},-\mathrm{id}\}\simeq\mathbb Z/2\mathbb Z$.

## 🔗 Liens

- **Utilisé par (théorèmes)** : [[proprietes-morphismes|Propriétés des morphismes]], [[sous-groupes-de-z|Sous-groupes de (Z,+)]]
- **Voir aussi** : [[morphisme-de-groupes|Morphisme de groupes]]
