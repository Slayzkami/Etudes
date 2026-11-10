---
aliases:
  - "Norme produit"
  - "espace produit"
  - "produit d'e.v.n."
  - "norme sur E1×E2"
tags:
  - cd
  - cd/definition
  - cd/chapitre-01
---

# 📘 Norme produit

*Définition* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Prop. 1.8 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> Soient $(E_1,N_1),\dots,(E_p,N_p)$ des e.v.n. et $E=E_1\times\dots\times E_p$. Pour $x=(x_1,\dots,x_p)\in E$ on pose
> $$N(x)=\max_{1\le i\le p}N_i(x_i).$$
> $N$ est une norme sur $E$ : c'est la **norme produit**.

> [!IMPORTANT] Autres normes sur le produit (Prop. 1.9)
> $N'(x)=\sum_i N_i(x_i)$ et $N''(x)=\big(\sum_i N_i(x_i)^2\big)^{1/2}$ sont aussi des normes, et $N\le N''\le N'\le p\,N$ : les trois sont [[normes-equivalentes|équivalentes]].

> [!TIP] En clair
> Dans un produit, « être petit » = « chaque composante est petite ». Une suite converge dans $E$ si et seulement si chaque composante converge (Prop. 1.19).

## 🔗 Liens

- **S'appuie sur** : [[norme|Norme, espace vectoriel normé]]
- **Utilisé par (définitions)** : [[differentielle-partielle|Différentielle partielle]]
- **Utilisé par (théorèmes)** : [[continuite-et-composantes|Continuité et composantes]], [[differentiabilite-par-composantes|Différentiabilité par composantes]]
