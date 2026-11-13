---
aliases:
  - "Méthode : déterminer et dessiner une boule"
  - "calculer une boule"
  - "dessiner une boule unité"
tags:
  - topologie
  - topo/methode
  - topo/chapitre-01
---

# 🛠️ Méthode : déterminer et dessiner une boule

*Méthode* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Méthode 1.3 du cours · [[topo-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> 1. Écrire l'inégalité $d(a,x)<r$ avec la formule de $d$.
> 2. La résoudre, en **distinguant des cas selon $r$** : comparer $r$ aux valeurs seuils ($1$ pour la distance discrète ou pour $\min(1,d)$…).
> 3. Dans $\mathbb R^2$ : repérer les droites « forme linéaire $=\pm r$ » ; $\max(|\varphi_1|,|\varphi_2|)\le1$ ou $|\varphi_1|+|\varphi_2|\le1$ donnent un parallélogramme.
> 4. Dans un sous-espace $F$ : $B_F(a,r)=B_E(a,r)\cap F$.
>
> Outil : $\min(a,b)<r\iff(a<r$ ou $b<r)$ ; $\min(a,b)\le r\iff(a\le r$ ou $b\le r)$.

> [!EXAMPLE] Rédaction modèle (comme sur la copie)
> *Boules de $\delta=\min(1,d_2)$ sur $\mathbb R^2$.* « Soient $a\in\mathbb R^2$, $r>0$. On a $\delta(a,x)<r\iff(1<r$ ou $d_2(a,x)<r)$.
> – Si $r\le1$ : $1<r$ est faux, donc $B_\delta(a,r)=B_2(a,r)$, le disque ouvert euclidien.
> – Si $r>1$ : $\delta\le1<r$ toujours, donc $B_\delta(a,r)=\mathbb R^2$.
> De même avec $\le$ : $\bar B_\delta(a,r)=\bar B_2(a,r)$ si $r<1$, et $\mathbb R^2$ si $r\ge1$. »

> [!WARNING] Pièges
> - Cas limite $r=1$ : la boule ouverte est le disque, la boule **fermée** est tout $\mathbb R^2$.
> - Le centre est **toujours** dans la boule : $B_{[0,1]}(0,\frac12)=[0,\frac12[$.

## 🔗 Liens

- **S'appuie sur** : [[topo-boules-spheres|Boules et sphères]], [[topo-boules-sous-espace|Boules d'un sous-espace métrique]]
- **Méthodes voisines** : [[topo-montrer-norme|Méthode : montrer qu'une application est une norme]]
- **Voir aussi** : —
