---
aliases:
  - "Normes équivalentes"
  - "normes équivalentes"
  - "équivalence des normes"
tags:
  - cd
  - cd/definition
  - cd/chapitre-01
---

# 📘 Normes équivalentes

*Définition* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Déf. 1.10 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> Deux normes $N_1$ et $N_2$ sur $E$ sont **équivalentes** s'il existe $\alpha>0$ et $\beta>0$ tels que
> $$\forall x\in E,\qquad \alpha N_1(x)\le N_2(x)\le\beta N_1(x).$$

> [!IMPORTANT] Ce que cela préserve (Prop. 1.11)
> Deux normes équivalentes définissent les mêmes suites convergentes (mêmes limites), les mêmes ouverts et fermés, les mêmes applications continues, les mêmes parties bornées, les mêmes suites de Cauchy.

> [!EXAMPLE] Dans $\mathbb K^n$ (Ex. 1.12)
> $\lVert x\rVert_\infty\le\lVert x\rVert_2\le\lVert x\rVert_1\le n\,\lVert x\rVert_\infty$.

> [!EXAMPLE] Contre-exemple en dimension infinie (Ex. 1.14)
> Sur $\mathcal C([0,1])$, $\lVert \cdot\rVert_1$ et $\lVert \cdot\rVert_\infty$ ne sont **pas** équivalentes : pour $u_n(t)=t^n$, $\lVert u_n\rVert_\infty=1$ et $\lVert u_n\rVert_1=\frac1{n+1}$, donc $\dfrac{\lVert u_n\rVert_\infty}{\lVert u_n\rVert_1}=n+1\to+\infty$.

> [!WARNING] Piège
> Les constantes $\alpha,\beta$ ne dépendent **pas** de $x$, et il faut les **deux** inégalités.

## 🔗 Liens

- **S'appuie sur** : [[norme|Norme, espace vectoriel normé]]
- **Utilisé par (théorèmes)** : [[equivalence-normes-dimension-finie|Équivalence des normes en dimension finie]]
- **Méthodes** : [[montrer-normes-equivalentes|Montrer que deux normes sont (ou ne sont pas) équivalentes]]
