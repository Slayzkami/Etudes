---
aliases:
  - "Ordre d'un élément"
  - "ordre d'un élément"
  - "o(x)"
  - "ordre infini"
  - "ordre fini"
tags:
  - gac
  - gac/definition
  - gac/chapitre-02
---

# 📘 Ordre d'un élément

*Définition* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · § II.6 du cours · [[index-definitions|↩ Index]]

> [!NOTE] Définition
> $o(x)$ est le **plus petit entier $m\ge1$ tel que $x^m=1$**, s'il existe ; sinon $x$ est **d'ordre infini**.
> (Additif : plus petit $m\ge1$ tel que $mx=0$.)

> [!IMPORTANT] Le morphisme $\varphi:\mathbb Z\to\langle x\rangle,\ n\mapsto x^n$
> - **Cas 1** ($\mathrm{Ker}\,\varphi=\{0\}$) : ordre infini ; $x^n=x^{n'}\iff n=n'$ ; $\langle x\rangle\simeq\mathbb Z$.
> - **Cas 2** ($\mathrm{Ker}\,\varphi=m\mathbb Z$, $m\ge1$) : $o(x)=m$ et
>   - $x^n=1\iff m\mid n$ ; $x^n=x^{n'}\iff n\equiv n'\pmod m$ ;
>   - $\langle x\rangle=\{1,x,\dots,x^{m-1}\}$ (éléments distincts), donc **$o(x)=\mathrm{Card}\,\langle x\rangle$** ;
>   - $\langle x\rangle\simeq\mathbb Z/m\mathbb Z$.

> [!EXAMPLE] Exemples
> - Dans $\mathbb C^*$ : $o(i)=4$, $2$ est d'ordre infini, $o(-1)=2$.
> - Dans $\mathbb Z/12\mathbb Z$ : $o(\bar2)=6$, $o(\bar3)=4$, $o(\bar4)=3$, $o(\bar6)=2$, $o(\bar1)=o(\bar5)=12$ → [[ordre-dans-znz]].
> - Dans $\mathfrak S_3$ : $o(\tau_i)=2$, $o(\gamma)=3$.

> [!WARNING] Pièges
> - $x^N=1$ donne seulement $o(x)\mid N$, pas $o(x)=N$.
> - Un morphisme **injectif** conserve l'ordre ; un morphisme quelconque, **non** (le morphisme trivial envoie tout sur $1$) → [[vrai-faux-classiques]].

## 🔗 Liens

- **S'appuie sur** : [[puissances-multiples|Puissances et multiples]], [[sous-groupe-engendre|Sous-groupe engendré par une partie]], [[sous-groupes-de-z|Sous-groupes de (Z,+)]]
- **Utilisé par (définitions)** : [[groupe-monogene-cyclique|Groupe monogène, groupe cyclique]]
- **Utilisé par (théorèmes)** : [[ordre-dans-znz|Ordre d'un élément de Z/nZ]], [[structure-groupes-monogenes|Structure des groupes monogènes]], [[lagrange|Théorème de Lagrange]]
- **Voir aussi** : [[calculer-ordre|Méthode : calculer l'ordre d'un élément]]
- **Base** : [[calculer-dans-znz|Méthode : calculer dans Z/nZ (la base)]] · **Pièges** : [[mes-erreurs|Mes erreurs à ne plus faire]]
