---
aliases:
  - "Méthode : montrer qu'une partie N'EST PAS ouverte / PAS fermée"
  - "pas ouvert"
  - "pas fermé"
  - "ni ouvert ni fermé"
  - "contre-exemple par une suite"
tags:
  - topologie
  - topo/methode
  - topo/chapitre-02
---

# 🛠️ Méthode : montrer qu'une partie N'EST PAS ouverte / PAS fermée

*Méthode* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Méthode 2.1 (point 5) du cours · [[topo-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> | Pour montrer que… | on exhibe… |
> |---|---|
> | $A$ **n'est pas fermé** | une suite **de $A$** qui converge vers un point **hors de $A$** |
> | $A$ **n'est pas ouvert** | une suite **hors de $A$** qui converge vers un point **de $A$** (donc $A^c$ n'est pas fermé) |
>
> Version boules pour « pas ouvert » : un point $a\in A$ tel que pour tout $r>0$, $B(a,r)$ contient un point hors de $A$ (prendre $a+\frac r2$, ou $(a,b-\frac r2)$…).
> Où chercher : **aux bords** de $A$ (inégalités larges/strictes, points exclus, bord d'un disque).

> [!EXAMPLE] Rédaction modèle (comme sur la copie)
> *$A=]0,1]\cup\{2\}$.*
> « **Pas ouvert.** Pour $n\in\mathbb N^*$, $y_n=2+\frac1n\notin A$ car $2<y_n\le3$, et $y_n\to2\in A$. Une suite hors de $A$ converge vers un point de $A$ : $A^c$ n'est pas fermé, donc $A$ n'est pas ouvert.
> **Pas fermé.** Pour $n\in\mathbb N^*$, $x_n=\frac1n\in A$ car $0<x_n\le1$, et $x_n\to0\notin A$. Une suite de $A$ converge vers un point hors de $A$ : $A$ n'est pas fermé (caractérisation séquentielle). »

> [!WARNING] Pièges
> - Vérifier **le signe** : pour sortir d'un demi-disque $\{y\ge0\}$, il faut $(0,-\frac1n)$, pas $(0,\frac1n)$ (mon erreur).
> - Comparer **la bonne quantité** : pour $X=\{y=x^2\}$ et $v_n=(1,1+\frac1n)$, on vérifie $1+\frac1n\neq1^2$ (comparer $y$ à $x^2$), pas $(1+\frac1n)^2\neq1$ (mon erreur, interro 2025-26).
> - Écrire $n\in\mathbb N^*$ (sinon $\frac1n$ n'existe pas) et $n\to+\infty$ (pas $x\to+\infty$).
> - « Pas ouvert » ne prouve pas « fermé ».

## 🔗 Liens

- **S'appuie sur** : [[topo-caracterisation-sequentielle-fermes|Caractérisation séquentielle des fermés]], [[topo-ouvert|Ouvert]], [[topo-ferme|Fermé]]
- **Méthodes voisines** : [[topo-montrer-ouvert-ferme|Méthode : montrer qu'une partie EST ouverte ou fermée]], [[topo-calculer-interieur-adherence-frontiere|Méthode : calculer intérieur, adhérence, frontière]]
- **Corrigés** : [[topo-exercices-types-corriges#5. Une partie de R – ouvert, fermé, adhérence, intérieur|ex. 5]], [[topo-exercices-types-corriges#7. La parabole (interro 2025-26)|ex. 7]]
- **Voir aussi** : [[topo-montrer-ouvert-ferme|Méthode : montrer qu'une partie EST ouverte ou fermée]], [[topo-calculer-interieur-adherence-frontiere|Méthode : calculer intérieur, adhérence, frontière]]
