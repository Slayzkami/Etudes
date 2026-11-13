---
aliases:
  - "Méthode : ouverts et fermés d'un sous-espace (distance induite)"
  - "ouvert relatif"
  - "fermé relatif"
  - "sous-espace métrique"
tags:
  - topologie
  - topo/methode
  - topo/chapitre-02
---

# 🛠️ Méthode : ouverts et fermés d'un sous-espace (distance induite)

*Méthode* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Prop. 1.20 et preuve de la Prop. 3.9 du cours · [[topo-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> Dans $(F,d_F)$ avec $F\subset E$ :
> 1. **Boules** : $B_F(a,r)=B_E(a,r)\cap F$.
> 2. **Ouvert de $F$** : pour tout $x\in V$, trouver $r>0$ avec $B_E(x,r)\cap F\subset V$ ; ou écrire $V=O\cap F$ avec $O$ ouvert de $E$ ; ou $V=B_F(a,r)$.
> 3. **Fermé de $F$** : par les suites **dans $F$** (la limite est supposée dans $F$) ; ou complémentaire **dans $F$** ouvert de $F$.
> 4. Une partie **ouverte et fermée** de $F$ : un « morceau » séparé du reste.

> [!EXAMPLE] Rédaction modèle (comme sur la copie)
> *$I=[0,1[\cup]2,3]$, montrer que $[0,1[$ est ouvert et fermé dans $I$.*
> « $[0,1[=B_I(\frac12,1)$ ($=]-\frac12,\frac32[\cap I$) est une boule ouverte de $I$, donc un ouvert de $I$. Son complémentaire dans $I$ est $]2,3]=B_I(\frac52,1)$, ouvert de $I$ ; donc $[0,1[$ est aussi fermé dans $I$. »

> [!WARNING] Pièges
> - Dans un sous-espace, la limite d'une suite doit être prise **dans $F$** : $(\frac1n,y)\to(0,y)\notin I$ ne contredit pas « fermé dans $I$ ».
> - « Ouvert dans $F$ » ne veut pas dire « ouvert dans $E$ ».

## 🔗 Liens

- **S'appuie sur** : [[topo-distance-induite|Distance induite, sous-espace métrique]], [[topo-boules-sous-espace|Boules d'un sous-espace métrique]]
- **Méthodes voisines** : —
- **Corrigés** : [[topo-exercices-types-corriges#8. Distance induite sur une bande trouée|ex. 8]]
- **Voir aussi** : —
