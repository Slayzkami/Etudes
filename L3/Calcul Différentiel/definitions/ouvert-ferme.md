---
aliases:
  - "Ouvert, fermé"
  - "ouvert"
  - "fermé"
  - "partie ouverte"
  - "partie fermée"
tags:
  - cd
  - cd/definition
  - cd/chapitre-01
---

# 📘 Ouvert, fermé

*Définition* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Déf. 1.20 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> Soit $(E,\lVert \cdot\rVert)$ un e.v.n. et $A\subset E$.
> - $A$ est un **ouvert** si $A=\emptyset$ ou si $\forall x\in A,\ \exists r>0,\ B(x,r)\subset A$.
> - $A$ est un **fermé** si son complémentaire $E\setminus A$ est ouvert.

> [!TIP] En clair – pourquoi des ouverts en calcul différentiel ?
> Si $U$ est ouvert et $a\in U$, alors $a+h\in U$ dès que $\lVert h\rVert$ est assez petit : on peut bouger autour de $a$ dans **toutes** les directions. C'est ce qu'il faut pour écrire $f(a+h)$ et faire tendre $h$ vers $0$.

> [!EXAMPLE] Exemples
> - Une boule ouverte est un ouvert ; une boule fermée est un fermé (Prop. 1.21).
> - $\{g<c\}$ est ouvert, $\{g\le c\}$ et $\{g=c\}$ sont fermés si $g:E\to\mathbb R$ est continue.
> - $[0,1[$ n'est ni ouvert ni fermé dans $\mathbb R$.

> [!WARNING] Pièges
> - « Pas ouvert » ne veut pas dire « fermé ».
> - Intersection **infinie** d'ouverts : pas forcément ouverte ($\bigcap_n\,]-\frac1n,\frac1n[=\{0\}$) → [[stabilite-ouverts-fermes]].

## 🔗 Liens

- **S'appuie sur** : [[boules-spheres|Boules et sphères]]
- **Utilisé par (définitions)** : [[voisinage|Voisinage]], [[differentiabilite|Différentiabilité en un point, différentielle]], [[partie-connexe|Partie connexe]], [[extremum-local|Extremum local, extremum global]]
- **Utilisé par (théorèmes)** : [[stabilite-ouverts-fermes|Stabilité des ouverts et des fermés]], [[caracterisation-sequentielle-fermes|Caractérisation séquentielle des fermés]]
- **Méthodes** : [[montrer-ouvert-ferme|Montrer qu'une partie est ouverte ou fermée]]
