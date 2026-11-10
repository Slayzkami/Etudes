---
aliases:
  - "Norme, espace vectoriel normé"
  - "norme"
  - "e.v.n."
  - "evn"
  - "espace vectoriel normé"
  - "N1 N2 N3"
tags:
  - cd
  - cd/definition
  - cd/chapitre-01
---

# 📘 Norme, espace vectoriel normé

*Définition* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Déf. 1.1 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> Soit $E$ un espace vectoriel sur $\mathbb K$ ($\mathbb R$ ou $\mathbb C$). Une **norme** sur $E$ est une application $N:E\to\mathbb R_+$ vérifiant :
> - **(N1) séparation** : $\forall x\in E,\ N(x)=0\iff x=0_E$ ;
> - **(N2) homogénéité** : $\forall\lambda\in\mathbb K,\ \forall x\in E,\ N(\lambda x)=\lvert \lambda\rvert\,N(x)$ ;
> - **(N3) inégalité triangulaire** : $\forall (x,y)\in E^2,\ N(x+y)\le N(x)+N(y)$.
>
> Un espace vectoriel muni d'une norme est un **espace vectoriel normé** (e.v.n.). On note souvent $\lVert x\rVert$ au lieu de $N(x)$.

> [!TIP] En clair
> Une norme mesure la « taille » d'un vecteur. La **distance** associée est $d(x,y)=\lVert x-y\rVert$ (Déf. 1.3).

> [!EXAMPLE] Les trois normes usuelles de $\mathbb K^n$ (Ex. 1.4)
> Pour $x=(x_1,\dots,x_n)$ :
> - $\lVert x\rVert_1=\lvert x_1\rvert+\dots+\lvert x_n\rvert$ ;
> - $\lVert x\rVert_2=\sqrt{\lvert x_1\rvert^2+\dots+\lvert x_n\rvert^2}$ ;
> - $\lVert x\rVert_\infty=\max_{1\le i\le n}\lvert x_i\rvert$.
>
> Sur $\mathcal C([a,b])$ (Ex. 1.5) : $\lVert f\rVert_\infty=\sup_{[a,b]}\lvert f\rvert$, $\lVert f\rVert_1=\int_a^b\lvert f\rvert$, $\lVert f\rVert_2=\big(\int_a^b f^2\big)^{1/2}$.

> [!WARNING] Pièges
> - (N1) est une **équivalence** : il faut montrer $N(x)=0\Rightarrow x=0$ (le sens difficile) **et** $N(0)=0$.
> - (N2) : c'est $\lvert \lambda\rvert$, pas $\lambda$. Tester avec $\lambda=-1$.
> - Ne pas oublier de dire que $N(x)$ est bien défini et $\ge0$.

## 🔗 Liens

- **Utilisé par (définitions)** : [[boules-spheres|Boules et sphères]], [[norme-produit|Norme produit]], [[normes-equivalentes|Normes équivalentes]], [[suite-convergente|Suite convergente]], [[continuite|Continuité en un point]], [[application-lipschitzienne|Application lipschitzienne]], [[petit-o|Petit o]], [[segment-et-convexe|Segment, partie convexe]]
- **Utilisé par (théorèmes)** : [[seconde-inegalite-triangulaire|Seconde inégalité triangulaire]]
- **Méthodes** : [[montrer-norme|Montrer qu'une application est une norme]]
