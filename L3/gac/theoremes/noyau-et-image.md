---
aliases:
  - "Noyau distingué, image sous-groupe, injectivité"
  - "Ker distingué"
  - "injectif ssi noyau trivial"
tags:
  - gac
  - gac/theoreme
  - gac/chapitre-02
---

# ⭐ Noyau distingué, image sous-groupe, injectivité

*Théorème* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · § II.5 du cours · [[index-definitions|↩ Index]]

> [!IMPORTANT] Énoncés
> Soit $f:G\to G'$ un morphisme, $H\le G$, $H'\le G'$.
> 1. $f(H)$ est un sous-groupe de $G'$ ; $f^{-1}(H')$ est un sous-groupe de $G$, distingué si $H'\lhd G'$.
> 2. **$\mathrm{Ker} f$ est un sous-groupe distingué de $G$** ; $\mathrm{Im} f$ est un sous-groupe de $G'$.
> 3. **$f$ injectif $\iff\mathrm{Ker} f=\{1_G\}$.**

> [!SUCCESS]- Démonstration de 2 (directe, à savoir par cœur)
> - $f(1)=1$ donc $1\in\mathrm{Ker} f$.
> - $x,y\in\mathrm{Ker} f$ : $f(xy^{-1})=f(x)f(y)^{-1}=1\cdot1=1$.
> - $g\in G$, $x\in\mathrm{Ker} f$ : $f(g^{-1}xg)=f(g)^{-1}f(x)f(g)=f(g)^{-1}f(g)=1$.

> [!SUCCESS]- Démonstration de 3
> ($\Rightarrow$) $f(x)=1=f(1)\Rightarrow x=1$. ($\Leftarrow$) $f(x)=f(y)\Rightarrow f(x^{-1}y)=1\Rightarrow x^{-1}y=1$.

> [!WARNING] Piège
> $f(H)$ distingué dans $f(G)$ si $H\lhd G$, mais **pas forcément dans $G'$** (TD1 ex. 7).

## 🔗 Liens

- **S'appuie sur** : [[image-noyau|Image, noyau, image réciproque]], [[sous-groupe-distingue|Sous-groupe distingué]], [[proprietes-morphismes|Propriétés des morphismes]]
- **Utilisé par (théorèmes)** : [[premier-theoreme-isomorphisme|Premier théorème d'isomorphisme]]
- **Méthodes** : [[lister-sous-groupes-znz|Méthode : lister les sous-groupes de Z/nZ (treillis)]], [[montrer-sous-groupe|Méthode : montrer qu'une partie est un sous-groupe]]
