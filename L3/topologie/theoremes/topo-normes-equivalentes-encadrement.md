---
aliases:
  - "Normes équivalentes : caractérisation par encadrement"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-02
---

# ⭐ Normes équivalentes : caractérisation par encadrement

*Théorème* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Prop. 2.65 et Ex. 2.66 du cours (poly : Prop. 2.16, Ex. 2.8) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> $N_1$ et $N_2$ sont équivalentes $\iff\exists\alpha,\beta>0,\ \forall x\in E,\ \alpha N_1(x)\le N_2(x)\le\beta N_1(x)$.
> Dans $\mathbb R^n$ : $\|x\|_\infty\le\|x\|_2\le\|x\|_1\le n\|x\|_\infty$.

> [!SUCCESS]- Démonstration
> ($\Leftarrow$) L'encadrement donne $\alpha d_1\le d_2\le\beta d_1$. ($\Rightarrow$) $\mathrm{id}$ est continue en $0$ : il existe $\eta>0$ avec $N_1(y)<\eta\Rightarrow N_2(y)<1$. Pour $x\neq0$, $y=\frac{\eta}{2N_1(x)}x$ vérifie $N_1(y)=\frac\eta2<\eta$, donc $N_2(x)\le\frac2\eta N_1(x)$ (**astuce d'homogénéité**).

## 🔗 Liens

- **S'appuie sur** : [[topo-normes-equivalentes|Normes équivalentes]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-equivalence-normes-dimension-finie|Équivalence des normes en dimension finie]]
- **Méthodes** : [[topo-montrer-normes-equivalentes|Méthode : normes équivalentes ou non]]
- **Voir aussi** : —
