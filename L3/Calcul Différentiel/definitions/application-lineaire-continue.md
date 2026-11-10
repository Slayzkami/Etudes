---
aliases:
  - "Application linéaire continue, espace Lc(E,F)"
  - "Lc(E,F)"
  - "linéaire continue"
  - "forme linéaire continue"
tags:
  - cd
  - cd/definition
  - cd/chapitre-01
---

# 📘 Application linéaire continue, espace Lc(E,F)

*Définition* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · § 1.9 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> On note $\mathcal L_c(E,F)$ l'espace vectoriel des applications **linéaires et continues** de $E$ dans $F$. Une application linéaire $f:E\to F$ est continue si et seulement si
> $$\exists C\ge0,\ \forall u\in E,\qquad \lVert f(u)\rVert_F\le C\,\lVert u\rVert_E$$
> ([[caracterisation-lineaires-continues|Théorème 1.43]]).

> [!IMPORTANT] Dimension finie
> Si $E$ est de dimension finie, **toute** application linéaire $f:E\to F$ est continue ([[lineaire-en-dimension-finie|Th. 1.44]]).

> [!EXAMPLE] Exemples et contre-exemples
> - Continue (Ex. 1.45) : $I:(\mathcal C([0,1]),\lVert \cdot\rVert_\infty)\to\mathbb R$, $I(f)=\int_0^1 f$, car $\lvert I(f)\rvert\le\lVert f\rVert_\infty$.
> - **Non** continue (Ex. 1.46) : $\delta_1:f\mapsto f(1)$ sur $(\mathcal C([0,1]),\lVert \cdot\rVert_1)$ : $u_n(t)=t^n$ donne $\delta_1(u_n)=1$ et $\lVert u_n\rVert_1=\frac1{n+1}\to0$.
> - **Non** continue (Ex. 1.47) : la dérivation $f\mapsto f'$ pour $\lVert \cdot\rVert_\infty$ ($u_n(t)=t^n$ : $\lVert u_n\rVert_\infty=1$, $\lVert u_n'\rVert_\infty=n$).

> [!WARNING] Piège
> « Linéaire donc continue » est **faux** en dimension infinie. Il faut toujours une phrase : « $E$ est de dimension finie » ou « $\lVert f(u)\rVert\le C\lVert u\rVert$ ».

## 🔗 Liens

- **S'appuie sur** : [[continuite|Continuité en un point]]
- **Utilisé par (définitions)** : [[norme-operateur|Norme d'opérateur]], [[application-bilineaire|Application bilinéaire (continue)]], [[differentiabilite|Différentiabilité en un point, différentielle]]
- **Utilisé par (théorèmes)** : [[caracterisation-lineaires-continues|Caractérisations des applications linéaires continues]]
- **Méthodes** : [[continuite-application-lineaire|Continuité d'une application linéaire]]
