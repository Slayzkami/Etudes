---
aliases:
  - "Méthode : calculer dans Z/nZ (la base)"
  - "calcul modulo n"
  - "horloge"
  - "calcul dans Z/nZ"
tags:
  - gac
  - gac/methode
  - gac/chapitre-02
---

# 🛠️ Méthode : calculer dans Z/nZ (la base)

*Méthode* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · [[index-definitions|↩ Index]]

> [!TIP] L'image à garder en tête : l'horloge
> $\mathbb Z/12\mathbb Z$, c'est une horloge à 12 heures : quand on dépasse 12, on **repart de 0**.
> Il est 9 h, on ajoute 5 h : il est 14 h, c'est-à-dire 2 h. On écrit $\bar9+\bar5=\overline{14}=\bar2$.
> $\mathbb Z/n\mathbb Z$, c'est la même chose avec une horloge à $n$ heures.

> [!NOTE] Ce que veut dire la barre
> $\bar k$ est la [[classe-equivalence|classe]] de $k$ modulo $n$ : tous les entiers qui ont le même reste que $k$ dans la division par $n$.
> $$\bar a=\bar b\ \text{dans}\ \mathbb Z/n\mathbb Z\iff n\mid a-b.$$
> En particulier **$\bar k=\bar0\iff n\mid k$**.
> $\mathbb Z/n\mathbb Z=\{\bar0,\bar1,\dots,\overline{n-1}\}$ a exactement $n$ éléments.

> [!ABSTRACT] Recette
> 1. **Additionner** : on additionne les entiers, puis on **réduit** (on retire $n$ autant de fois qu'il faut pour revenir entre $0$ et $n-1$).
> 2. **Neutre** : $\bar0$.
> 3. **Opposé** de $\bar k$ : c'est $\overline{n-k}$ (ce qu'il manque pour arriver à $n$), car $\bar k+\overline{n-k}=\bar n=\bar0$.
> 4. **Multiple** $m\cdot\bar k$ : c'est $\bar k+\dots+\bar k$ ($m$ fois) $=\overline{mk}$, puis on réduit.
> 5. **Sous-groupe engendré** $\langle\bar k\rangle$ : on écrit $\bar k,\ 2\bar k,\ 3\bar k,\dots$ et **on ne s'arrête que lorsqu'on retombe sur $\bar0$**.
> 6. **Ordre** $o(\bar k)$ : le numéro du premier multiple qui vaut $\bar0$ ; c'est aussi le nombre d'éléments de $\langle\bar k\rangle$.

> [!EXAMPLE] Rédaction modèle dans $\mathbb Z/12\mathbb Z$
> - $\bar9+\bar5=\overline{14}=\bar2$ (car $14-12=2$).
> - $\bar7+\overline{11}=\overline{18}=\bar6$ (car $18-12=6$).
> - L'opposé de $\bar8$ est $\bar4$, car $\bar8+\bar4=\overline{12}=\bar0$.
> - L'opposé de $\bar5$ est $\bar7$ ; l'opposé de $\bar6$ est $\bar6$ lui-même ($\bar6+\bar6=\overline{12}=\bar0$).

> [!EXAMPLE] Rédaction modèle dans $\mathbb Z/18\mathbb Z$ : $\langle\overline{12}\rangle$ et $o(\overline{12})$
> $1\cdot\overline{12}=\overline{12}$
> $2\cdot\overline{12}=\overline{24}=\bar6$ (car $24-18=6$)
> $3\cdot\overline{12}=\overline{36}=\bar0$ (car $36=2\times18$)
> On est retombé sur $\bar0$ au 3ᵉ pas : $o(\overline{12})=3$ et $\langle\overline{12}\rangle=\{\bar0,\bar6,\overline{12}\}$.
> Vérification par la formule : $\operatorname{pgcd}(18,12)=6$, donc $o(\overline{12})=18/6=3$ → [[ordre-dans-znz]].

> [!WARNING] Pièges
> - Le multiple se calcule avec **l'élément**, pas avec son ordre : $2\cdot\overline{12}=\overline{24}$, et non « $2\times3$ ».
> - Toujours réduire : $\overline{36}$ n'est pas « un nouveau nombre », c'est $\bar0$ dans $\mathbb Z/18\mathbb Z$.
> - Écrire les barres et préciser **dans quel groupe** on calcule : « $\bar8+\bar4=\bar0$ dans $\mathbb Z/12\mathbb Z$ », pas « $8+4=12=0$ ».
> - Une égalité par étape : $\operatorname{pgcd}(18,15)=3$, **donc** $o(\overline{15})=18/3=6$. Jamais « $=3=6$ ».

## 🔗 Liens

- **S'appuie sur** : [[classe-equivalence|Classe d'équivalence]], [[groupe-quotient|Groupe quotient]], [[puissances-multiples|Puissances et multiples]]
- **Suite logique** : [[calculer-ordre|Méthode : calculer l'ordre d'un élément]], [[lister-sous-groupes-znz|Méthode : lister les sous-groupes de Z/nZ]]
- **Voir aussi** : [[ordre-element|Ordre d'un élément]], [[sous-groupe-engendre|Sous-groupe engendré]], [[mes-erreurs|Mes erreurs à ne plus faire]]
