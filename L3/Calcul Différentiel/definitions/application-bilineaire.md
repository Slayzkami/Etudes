---
aliases:
  - "Application bilinéaire (continue)"
  - "bilinéaire"
  - "bilinéaire continue"
tags:
  - cd
  - cd/definition
  - cd/chapitre-01
---

# 📘 Application bilinéaire (continue)

*Définition* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Déf. 1.52 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> Soient $E_1,E_2,F$ des e.v.n. $B:E_1\times E_2\to F$ est **bilinéaire** si elle est linéaire par rapport à chaque variable, l'autre étant fixée :
> $$B(u+\lambda u',v)=B(u,v)+\lambda B(u',v),\qquad B(u,v+\lambda v')=B(u,v)+\lambda B(u,v').$$

> [!IMPORTANT] Continuité (Prop. 1.53, 1.55)
> $B$ bilinéaire est continue $\iff$ $\exists C\ge0,\ \forall(u,v),\ \lVert B(u,v)\rVert\le C\,\lVert u\rVert\,\lVert v\rVert$. En dimension finie, toute application bilinéaire est continue → [[caracterisation-bilineaires-continues]].

> [!EXAMPLE] Exemples (Ex. 1.54)
> Le produit de réels $(x,y)\mapsto xy$ ; le produit matriciel $(X,Y)\mapsto XY$ ; $(\lambda,x)\mapsto\lambda x$ ; $(f,g)\mapsto fg$ sur $\mathcal C([0,1])$ avec $\lVert \cdot\rVert_\infty$.

> [!WARNING] Piège
> Une application bilinéaire n'est **pas** linéaire sur $E_1\times E_2$ : $B(2u,2v)=4B(u,v)$. Sa différentielle n'est donc pas elle-même → [[differentielles-de-reference]].

## 🔗 Liens

- **S'appuie sur** : [[application-lineaire-continue|Application linéaire continue, espace Lc(E,F)]]
- **Utilisé par (définitions)** : [[differentielle-seconde|Différentielle seconde, classe C2]]
- **Utilisé par (théorèmes)** : [[caracterisation-bilineaires-continues|Caractérisation des applications bilinéaires continues]], [[differentielles-de-reference|Différentielles de référence : constante, linéaire, bilinéaire]]
