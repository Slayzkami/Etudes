---
aliases:
  - "Méthode : montrer qu'une application est une norme"
  - "prouver que N est une norme"
  - "vérifier N1 N2 N3"
tags:
  - cd
  - cd/methode
  - cd/chapitre-01
---

# 🛠️ Méthode : montrer qu'une application est une norme

*Méthode* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> 0. **Bien définie et positive** : dire pourquoi $N(x)$ existe (max d'un nombre fini de termes, sup d'une fonction continue sur un segment…) et que $N(x)\ge0$.
> 1. **Séparation** : supposer $N(x)=0$ et en déduire $x=0$. (Et $N(0)=0$.)
> 2. **Homogénéité** : calculer $N(\lambda x)$ et sortir $\abs\lambda$.
> 3. **Inégalité triangulaire** : partir de l'inégalité triangulaire sur $\lvert \cdot\rvert$ (ou sur une norme connue), **terme par terme**, puis passer au max / à la somme.

> [!EXAMPLE] Rédaction modèle : $N(X)=n\max_{i,j}\lvert x_{ij}\rvert$ sur $\mathcal M_n(\mathbb R)$ (Écrit 2024-2025)
> - $N(X)$ est le max d'un nombre fini de réels $\ge0$ : bien défini, $\ge0$.
> - **Séparation.** Si $N(X)=0$ alors $\max_{i,j}\lvert x_{ij}\rvert=0$, donc $\lvert x_{ij}\rvert=0$ pour tous $i,j$ : $X=0$.
> - **Homogénéité.** $N(\lambda X)=n\max\lvert \lambda x_{ij}\rvert=n\abs\lambda\max\lvert x_{ij}\rvert=\abs\lambda N(X)$.
> - **Inégalité triangulaire.** Pour tous $i,j$ : $\lvert x_{ij}+y_{ij}\rvert\le\lvert x_{ij}\rvert+\lvert y_{ij}\rvert\le\max\lvert x_{kl}\rvert+\max\lvert y_{kl}\rvert$. Le membre de droite ne dépend pas de $(i,j)$, donc il majore le max : $N(X+Y)\le N(X)+N(Y)$.
> - **Sous-multiplicativité.** $\lvert (XY)_{ij}\rvert=\lvert \sum_kx_{ik}y_{kj}\rvert\le\sum_{k=1}^n\lvert x_{ik}\rvert\lvert y_{kj}\rvert\le n\max\lvert x_{kl}\rvert\max\lvert y_{kl}\rvert$. En multipliant par $n$ : $N(XY)\le N(X)N(Y)$.

> [!WARNING] Pièges
> - Pour le max : majorer **chaque terme** par une quantité indépendante de l'indice, **puis** prendre le max.
> - Séparation avec une intégrale : « $\int_a^b\abs f=0$ et $\abs f$ continue positive $\Rightarrow f=0$ » (il faut la continuité).

## 🔗 Liens

- **Voir aussi** : [[norme|Norme, espace vectoriel normé]], [[seconde-inegalite-triangulaire|Seconde inégalité triangulaire]]
