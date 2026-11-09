---
aliases:
  - "Méthode : déterminer les classes modulo un sous-groupe, l'indice et le quotient"
  - "déterminer les classes"
  - "calculer l'indice"
  - "écrire G/H"
tags:
  - gac
  - gac/methode
  - gac/chapitre-03
---

# 🛠️ Méthode : déterminer les classes modulo un sous-groupe, l'indice et le quotient

*Méthode* · Chapitre : [[03-groupes-quotients|III – Groupes quotients]] · [[index-definitions|↩ Index]]

> [!ABSTRACT] Recette (groupe fini)
> 1. Écrire les éléments de $H$ et calculer l'[[indice]] : $[G:H]=[G]/[H]$. C'est **le nombre de classes** à trouver.
> 2. Première classe : $H$ lui-même (classe du neutre).
> 3. Prendre un élément $x$ **pas encore rangé** ; sa classe est $xH=\{xh,\ h\in H\}$ (additif : $x+H$).
> 4. Recommencer jusqu'à avoir rangé tout le monde. **Contrôle** : toutes les classes ont $[H]$ éléments, elles sont disjointes.
> 5. Si $H\lhd G$ (toujours vrai si $G$ abélien) : $G/H$ est un groupe d'ordre $[G:H]$, avec $(xH)(yH)=xyH$. Pour le reconnaître : ordre premier ⟹ cyclique ; sinon calculer l'ordre d'une classe, ou utiliser [[identifier-quotient]].
>
> **Rappel** : $xH=yH\iff x^{-1}y\in H$ (additif : $y-x\in H$).

> [!EXAMPLE] Rédaction modèle : $G=\mathbb Z/12\mathbb Z$, $H=\langle\bar4\rangle=\{\bar0,\bar4,\bar8\}$
> $[G:H]=12/3=4$ classes :
> $H=\{\bar0,\bar4,\bar8\}$, $\bar1+H=\{\bar1,\bar5,\bar9\}$, $\bar2+H=\{\bar2,\bar6,\overline{10}\}$, $\bar3+H=\{\bar3,\bar7,\overline{11}\}$.
> $G$ est abélien donc $H\lhd G$ et $G/H$ est un groupe d'ordre 4. La classe $\bar1+H$ est d'ordre 4 ($k(\bar1+H)=\bar k+H=H\iff4\mid k$), donc $G/H$ est cyclique : $G/H\simeq\mathbb Z/4\mathbb Z$.

> [!WARNING] Pièges
> - Les éléments de $G/H$ sont des **paquets** (les classes), pas des éléments de $G$.
> - Si $G$ n'est pas abélien, classes à gauche $xH$ et à droite $Hx$ peuvent différer ; elles coïncident toutes ssi $H\lhd G$ → [[montrer-distingue]].

## 🔗 Liens

- **S'appuie sur** : [[classes-modulo-sous-groupe|Classes à gauche et à droite]], [[indice|Indice]], [[groupe-quotient|Groupe quotient]], [[lagrange|Théorème de Lagrange]]
- **Voir aussi** : [[identifier-quotient]], [[utiliser-lagrange]], [[montrer-relation-equivalence]]
- **Corrigés** : [[exercices-types-corriges#12. Classes, indice et quotient|ex. 12]]
