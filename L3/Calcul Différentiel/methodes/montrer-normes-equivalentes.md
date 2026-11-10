---
aliases:
  - "Méthode : montrer que deux normes sont (ou ne sont pas) équivalentes"
  - "normes équivalentes ou non"
  - "comparer deux normes"
tags:
  - cd
  - cd/methode
  - cd/chapitre-01
---

# 🛠️ Méthode : montrer que deux normes sont (ou ne sont pas) équivalentes

*Méthode* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Méthode 1.2 du cours · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> - **Dimension finie** : toutes les normes sont équivalentes (Th. 1.13). Une phrase suffit.
> - **Pour montrer l'équivalence** : établir $\alpha N_1(x)\le N_2(x)\le\beta N_1(x)$ en majorant terme à terme ($\max\le\sum\le n\max$).
> - **Pour montrer la non-équivalence** : trouver une suite $u_n\ne0$ telle que $\dfrac{N_2(u_n)}{N_1(u_n)}\to+\infty$ (ou $\to0$).

> [!EXAMPLE] Rédaction modèle
> Sur $E=\mathcal C([0,1])$, $u_n(t)=t^n$. $\lVert u_n\rVert_\infty=1$ et $\lVert u_n\rVert_1=\int_0^1t^n\,\mathrm dt=\frac1{n+1}$.
> Supposons qu'il existe $\beta>0$ tel que $\lVert f\rVert_\infty\le\beta\lVert f\rVert_1$ pour tout $f\in E$. Alors $1\le\frac\beta{n+1}$ pour tout $n$, ce qui est faux pour $n$ grand. Donc les normes ne sont pas équivalentes.

> [!WARNING] Piège
> « $\mathcal C([0,1])$ » est de dimension **infinie** : le Th. 1.13 ne s'applique pas.

## 🔗 Liens

- **Voir aussi** : [[normes-equivalentes|Normes équivalentes]], [[equivalence-normes-dimension-finie|Équivalence des normes en dimension finie]]
