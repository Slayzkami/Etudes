---
aliases:
  - "Continuité globale : image réciproque"
  - "image réciproque"
  - "f^{-1}(ouvert)"
  - "continuité et ouverts"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-02
---

# ⭐ Continuité globale : image réciproque

*Théorème* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Th. 2.34 du cours (poly : Th. 2.7) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Sont équivalentes :
> (i) $f$ est continue sur $E$ ;
> (ii) l'image réciproque de **tout ouvert** de $F$ est un ouvert de $E$ ;
> (iii) l'image réciproque de **tout fermé** de $F$ est un fermé de $E$.

> [!SUCCESS]- Démonstration
> (i)⇒(ii) $O$ ouvert de $F$, $a\in f^{-1}(O)$ : $O$ est voisinage de $f(a)$, donc $f^{-1}(O)$ est voisinage de $a$ ; il est voisinage de chacun de ses points : ouvert.
> (ii)⇒(i) $f^{-1}(B(f(a),\varepsilon))$ est un ouvert contenant $a$, donc contient $B(a,\delta)$.
> (ii)⇔(iii) $f^{-1}(B^c)=(f^{-1}(B))^c$.
>
> *Version suites de (iii), à savoir aussi* : $B$ fermé, $x_n\in f^{-1}(B)$, $x_n\to x$ ; alors $f(x_n)\to f(x)$ et $f(x_n)\in B$ fermé, donc $f(x)\in B$.

> [!TIP] Réflexes
> **Outil n°1** : $\{f>0\}=f^{-1}(]0,+\infty[)$ ouvert ; $\{f\ge0\}$, $\{f=0\}$ fermés. Inégalités **strictes** → ouvert ; **larges ou égalités** → fermé.
> $\{f=g\}=(f-g)^{-1}(\{0\})$ fermé et $\{f\neq g\}$ ouvert (écrits 2022-23 et 2025-26).

> [!WARNING] Pièges
> - L'**image directe** ne conserve rien : $x^2$ envoie $]-1,1[$ sur $[0,1[$ ; $\exp(\mathbb R)=]0,+\infty[$.
> - La fonction doit être définie et continue sur **tout l'espace** ($\mathbb R$ ou $\mathbb R^2$), pas seulement sur la partie étudiée (mon erreur sur $]0,+\infty[$).

## 🔗 Liens

- **S'appuie sur** : [[topo-continuite|Continuité en un point]], [[topo-ouvert|Ouvert]], [[topo-ferme|Fermé]], [[topo-caracterisations-continuite-point|Caractérisations de la continuité en un point]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : —
- **Méthodes** : [[topo-montrer-ouvert-ferme|Méthode : montrer qu'une partie EST ouverte ou fermée]]
- **Voir aussi** : —
