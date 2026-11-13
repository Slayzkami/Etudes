---
aliases:
  - "Équivalence des normes en dimension finie"
  - "dimension finie"
  - "toutes les normes sont équivalentes"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-03
---

# ⭐ Équivalence des normes en dimension finie

*Théorème* · Chapitre : [[03-espaces-metriques-compacts|3 – Espaces métriques compacts]] · Th. 2.67 = Th. 3.34 et Cor. 3.35 du cours (poly : Th. 2.10) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Sur un espace vectoriel de **dimension finie**, toutes les normes sont équivalentes. Conséquences : les compacts sont les fermés bornés, l'espace est complet, toute application linéaire est continue.

> [!SUCCESS]- Démonstration
> On compare $N$ à $N_\infty(u)=\max|u_i|$ (coordonnées dans une base).
> 1. $N(u)\le\sum|u_i|N(e_i)\le\beta N_\infty(u)$.
> 2. Donc $N$ est $\beta$-lipschitzienne pour $N_\infty$, donc continue.
> 3. La sphère $S=\{N_\infty=1\}$ est fermée bornée, donc **compacte**.
> 4. $N$ atteint son minimum $\alpha=N(u_0)>0$ sur $S$ ; pour $u\neq0$, $N(\frac{u}{N_\infty(u)})\ge\alpha$, d'où $N\ge\alpha N_\infty$.

> [!WARNING] Pièges
> **Faux en dimension infinie** : sur $C([a,b])$, $f_n=(\frac{x-a}{b-a})^n$ donne $\frac{\|f_n\|_\infty}{\|f_n\|_1}=\frac{n+1}{b-a}\to+\infty$ (Rem. 2.68).

## 🔗 Liens

- **S'appuie sur** : [[topo-normes-equivalentes-encadrement|Normes équivalentes : caractérisation par encadrement]], [[topo-bornes-atteintes|Une fonction continue sur un compact est bornée et atteint ses bornes]], [[topo-borel-lebesgue|Borel–Lebesgue : compacts de R et de R^n]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : —
- **Méthodes** : [[topo-montrer-normes-equivalentes|Méthode : normes équivalentes ou non]]
- **Voir aussi** : —
