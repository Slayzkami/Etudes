---
aliases:
  - "Méthode : montrer qu'un groupe est cyclique (ou ne l'est pas), trouver ses générateurs"
  - "montrer cyclique"
  - "montrer non cyclique"
  - "trouver les générateurs"
tags:
  - gac
  - gac/methode
  - gac/chapitre-02
---

# 🛠️ Méthode : montrer qu'un groupe est cyclique (ou ne l'est pas), trouver ses générateurs

*Méthode* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · [[index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> **Montrer que $G$ (fini, d'ordre $n$) est cyclique** : exhiber **un** élément $a$ d'ordre $n$. Alors $\langle a\rangle$ a $n$ éléments, donc $\langle a\rangle=G$.
> Autres arguments : $G$ d'ordre **premier** ([[groupe-ordre-premier]]) ; $G\simeq\mathbb Z/n\mathbb Z$ ; $\mathbb Z/m\mathbb Z\times\mathbb Z/n\mathbb Z$ avec $\operatorname{pgcd}(m,n)=1$ ([[lemme-chinois]]).
>
> **Montrer que $G$ n'est pas cyclique** (au choix) :
> - $G$ n'est pas abélien (cyclique ⟹ abélien) ;
> - **aucun** élément n'est d'ordre $n$ : calculer tous les ordres, ou trouver $m<n$ tel que $x^m=e$ pour tout $x$.
>
> **Générateurs de $\mathbb Z/n\mathbb Z$** : les $\bar k$ avec $\operatorname{pgcd}(n,k)=1$ ([[ordre-dans-znz]]).
> **Générateurs de $\langle a\rangle$ avec $o(a)=n$** : les $a^k$ avec $\operatorname{pgcd}(n,k)=1$.

> [!EXAMPLE] Rédactions modèles
> - $\mathbb Z/2\mathbb Z\times\mathbb Z/3\mathbb Z$ est cyclique : $o(\bar1,\bar1)=\operatorname{ppcm}(2,3)=6$ = ordre du groupe.
> - $\mathbb Z/2\mathbb Z\times\mathbb Z/2\mathbb Z$ ne l'est pas : $2x=0$ pour tout $x$, donc aucun élément d'ordre 4.
> - $\mathfrak S_3$ ne l'est pas : il n'est pas abélien.
> - $\mathbb U_n$ est cyclique : engendré par $e^{2i\pi/n}$, d'ordre $n$.
> - Générateurs de $\mathbb Z/12\mathbb Z$ : $\bar1,\bar5,\bar7,\overline{11}$.

> [!WARNING] Piège
> « $G$ est abélien donc cyclique » est **faux** (Klein). Abélien ne dit rien sur l'existence d'un générateur → [[groupe-abelien]].

## 🔗 Liens

- **S'appuie sur** : [[groupe-monogene-cyclique|Groupe monogène, groupe cyclique]], [[ordre-element|Ordre d'un élément]], [[structure-groupes-monogenes|Structure des groupes monogènes]]
- **Voir aussi** : [[calculer-ordre]], [[montrer-non-isomorphes]], [[vrai-faux-classiques]]
- **Corrigés** : [[exercices-types-corriges#1. Ordres et sous-groupes de Z/18Z|ex. 1 c)]], [[exercices-types-corriges#9. Groupe d'ordre premier|ex. 9]], [[exercices-types-corriges#11. Ordres dans un produit|ex. 11]]
