---
aliases:
  - "Morphisme de groupes"
  - "morphisme"
  - "homomorphisme"
  - "endomorphisme"
  - "isomorphisme"
  - "automorphisme"
tags:
  - gac
  - gac/definition
  - gac/chapitre-01
---

# 📘 Morphisme de groupes

*Définition* · Chapitre : [[01-definitions-generales|I – Définitions générales]] · § I.3 du cours · [[index-definitions|↩ Index]]

> [!NOTE] Définition
> Soient $(G,\star)$, $(G',\star')$ deux [[groupe|groupes]]. $f:G\to G'$ est un **(homo)morphisme** si
> $$\forall x,y\in G,\qquad f(x\star y)=f(x)\star'f(y).$$
> - **endomorphisme** : $G=G'$ ;
> - **isomorphisme** : morphisme bijectif ;
> - **automorphisme** : endomorphisme bijectif.

> [!TIP] En clair
> Calculer puis appliquer $f$, ou appliquer $f$ puis calculer : même résultat. Attention aux lois : $e^{x+y}=e^xe^y$ (une somme devient un produit).

> [!IMPORTANT] Conséquences
> $f(1)=1$, $f(x^{-1})=f(x)^{-1}$, $f(x^n)=f(x)^n$ → [[proprietes-morphismes]].
> Composée et réciproque d'isomorphismes : isomorphismes.

> [!EXAMPLE] Exemples
> | morphisme | noyau | image |
> |---|---|---|
> | $\mathbb Z\to\mathbb Z/n\mathbb Z,\ k\mapsto\bar k$ | $n\mathbb Z$ | $\mathbb Z/n\mathbb Z$ |
> | $(\mathbb C^*,\times)\to(\mathbb R_+^*,\times),\ z\mapsto\lvert z\rvert$ | $\mathbb U$ | $\mathbb R_+^*$ |
> | $(\mathbb R,+)\to(\mathbb U,\times),\ \theta\mapsto e^{i\theta}$ | $2\pi\mathbb Z$ | $\mathbb U$ |
> | $\det:GL_n(\mathbb R)\to\mathbb R^*$ | $SL_n(\mathbb R)$ | $\mathbb R^*$ |
> | $(\mathbb R,+)\to(\mathbb R_+^*,\times),\ x\mapsto e^x$ | $\{0\}$ | $\mathbb R_+^*$ (isomorphisme) |

## 🔗 Liens

- **S'appuie sur** : [[groupe|Groupe]]
- **Utilisé par (définitions)** : [[application-induite|Application induite et décomposition canonique]], [[automorphismes|Automorphismes et automorphismes intérieurs]], [[groupes-isomorphes|Groupes isomorphes]], [[image-noyau|Image, noyau, image réciproque]]
- **Utilisé par (théorèmes)** : [[proprietes-morphismes|Propriétés des morphismes]]
- **Méthodes** : [[identifier-quotient|Méthode : identifier un groupe quotient G/H]]
- **Voir aussi** : [[premier-theoreme-isomorphisme|Premier théorème d'isomorphisme]], [[endomorphismes-de-z|Méthode : morphismes de source Z (endomorphismes de (Z,+))]]
- **Méthode** : [[montrer-morphisme|étudier un morphisme (noyau, image, injectif, surjectif)]]
