---
aliases:
  - "Boules et sphères"
  - "boule ouverte"
  - "boule fermée"
  - "sphère"
  - "B(a,r)"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-01
---

# 📘 Boules et sphères

*Définition* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Déf. 1.13 du cours (poly : Déf. 1.4) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> Soit $(E,d)$ un espace métrique, $a\in E$ et $r>0$.
> - **Boule ouverte** : $B(a,r)=\{x\in E\mid d(a,x)<r\}$ ;
> - **Boule fermée** : $\bar B(a,r)=\{x\in E\mid d(a,x)\le r\}$ ;
> - **Sphère** : $S(a,r)=\{x\in E\mid d(a,x)=r\}$.

> [!IMPORTANT] À retenir
> - $a\in B(a,r)\subset\bar B(a,r)$ ; $\bar B(a,r)=B(a,r)\sqcup S(a,r)$ → [[topo-proprietes-boules]].
> - Une boule ouverte **est un ouvert** ([[topo-boule-ouverte-ouverte]]) ; une boule fermée **est un fermé** ([[topo-boule-fermee-fermee]]).
> - Dans un sous-espace : $B_F(a,r)=B_E(a,r)\cap F$ → [[topo-boules-sous-espace]].

> [!EXAMPLE] Exemples
> - Dans $F=[0,1]$ : $B_F(0,\tfrac12)=[0,\tfrac12[$ (le centre est toujours dans la boule).
> - Distance discrète : $B(a,r)=\{a\}$ si $r\le1$, $E$ si $r>1$.

> [!WARNING] Pièges
> - $\overline{B(a,r)}=\bar B(a,r)$ est vrai dans un **e.v.n.**, faux en général (distance discrète).
> - $\operatorname{diam}B(a,r)\le2r$, avec égalité seulement dans un e.v.n. non nul.

## 🔗 Liens

- **S'appuie sur** : [[topo-distance|Distance, espace métrique]]
- **Utilisé par (définitions)** : [[topo-ouvert|Ouvert]], [[topo-partie-bornee-diametre|Partie bornée, diamètre]], [[topo-suite-bornee|Suite bornée]]
- **Utilisé par (théorèmes)** : [[topo-proprietes-boules|Premières propriétés des boules]], [[topo-boule-fermee-fermee|Une boule fermée est un fermé]], [[topo-boule-ouverte-ouverte|Une boule ouverte est un ouvert]]
- **Méthodes** : [[topo-determiner-boule|Méthode : déterminer et dessiner une boule]]
- **Voir aussi** : —
