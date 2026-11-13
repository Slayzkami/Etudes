---
aliases:
  - "Reconnaître le type d'exercice topologie"
  - "quelle méthode utiliser topo"
tags:
  - topologie
  - topo/revision
---

# 🧭 Reconnaître le type d'exercice

« L'énoncé demande ça → je sors cette méthode → je commence par cette phrase. » · [[topo-plan-de-revision|↩ Plan de révision]] · [[topo-index-definitions|↩ Index]]

## Chapitre 1 – distances, normes, boules

| L'énoncé demande… | Méthode | Première phrase sur la copie | Corrigé |
|---|---|---|---|
| Montrer que $d$ est une distance | [[topo-montrer-distance\|distance]] | « Séparation : $d\ge0$ ; si $d(x,y)=0$, alors… » | [[topo-exercices-types-corriges#9. Interro 2025-26 – la distance min(1, d)\|ex. 9]] |
| Montrer que $N$ est une norme | [[topo-montrer-norme\|norme]] | « (N2) : soit $\lambda\in\mathbb R$, $N(\lambda x)=\dots$ » | [[topo-exercices-types-corriges#20. Une norme sur R² et sa boule unité\|ex. 20]] |
| Déterminer / dessiner une boule | [[topo-determiner-boule\|boule]] | « Soit $r>0$. $x\in B(a,r)\iff d(a,x)<r\iff\dots$ ; distinguons $r\le1$ et $r>1$. » | [[topo-exercices-types-corriges#9. Interro 2025-26 – la distance min(1, d)\|ex. 9]] |
| Donner un espace métrique $E\subset\mathbb R^3$, $E\neq\mathbb R^3$ | [[topo-distance-induite\|distance induite]] | « $E=\bar B(0,1)$ muni de la distance induite par $d_2$… » | [[topo-exercices-types-corriges#11. Interro 2026-27 – questions de cours\|ex. 11]] |
| La distance discrète vient-elle d'une norme ? | [[topo-distance-et-norme\|(P1)]] | « Non : pour $x\neq0$, $N(x)=1$ et $N(\frac x2)=1\neq\frac12N(x)$. » | [[topo-exercices-types-corriges#11. Interro 2026-27 – questions de cours\|ex. 11]] |

## Chapitre 2 – ouverts, fermés, adhérence, continuité

| L'énoncé demande… | Méthode | Première phrase sur la copie | Corrigé |
|---|---|---|---|
| $A$ n'est **pas fermé** | [[topo-montrer-pas-ouvert-pas-ferme\|suites]] | « Pour $n\in\mathbb N^*$, $x_n=\dots\in A$ car… et $x_n\to\ell\notin A$. » | [[topo-exercices-types-corriges#5. Une partie de R – ouvert, fermé, adhérence, intérieur\|ex. 5]] |
| $A$ n'est **pas ouvert** | [[topo-montrer-pas-ouvert-pas-ferme\|suites]] | « Pour $n\in\mathbb N^*$, $y_n=\dots\notin A$ car… et $y_n\to a\in A$. » | [[topo-exercices-types-corriges#7. La parabole (interro 2025-26)\|ex. 7]] |
| $A$ **est** ouvert / fermé (dans $\mathbb R^2$) | [[topo-montrer-ouvert-ferme\|image réciproque]] | « L'application $g:\mathbb R^2\to\mathbb R$, $g(x,y)=\dots$ est continue, et $A=g^{-1}(\dots)$. » | [[topo-exercices-types-corriges#16. Ouverts et fermés de R²\|ex. 16]] |
| $A$ **est** fermé (cas abstrait) | [[topo-caracterisation-sequentielle-fermes\|suites]] | « Soit $(x_n)$ une suite de $A$ qui converge vers $\ell\in E$ ; montrons $\ell\in A$. » | [[topo-exercices-types-corriges#1. Une boule fermée est fermée\|ex. 1]] |
| Boule fermée fermée ; boule ouverte ouverte | [[topo-boule-fermee-fermee\|cours]] | « Soit $(y_n)$ une suite de $\bar B(x,r)$ qui converge vers $y$… » | [[topo-exercices-types-corriges#1. Une boule fermée est fermée\|ex. 1]] |
| Adhérence de $A$ | [[topo-calculer-interieur-adherence-frontiere\|deux inclusions]] | « Montrons $\bar A=F$. ($\supset$) … est limite de … ; ($\subset$) $F$ est fermé et contient $A$. » | [[topo-exercices-types-corriges#7. La parabole (interro 2025-26)\|ex. 7]] |
| Intérieur de $A$ | [[topo-calculer-interieur-adherence-frontiere\|deux inclusions]] | « $U$ est ouvert et contenu dans $A$, donc $U\subset\operatorname{Int}A$. Les autres points… » | [[topo-exercices-types-corriges#5. Une partie de R – ouvert, fermé, adhérence, intérieur\|ex. 5]] |
| $\overline{A\cap B}$, $\operatorname{Int}(A\cup B)$, $\operatorname{int}(X\setminus Y)$ | [[topo-caracterisation-adherence\|plus petit fermé / plus grand ouvert]] | « $\bar A\cap\bar B$ est un fermé contenant $A\cap B$, donc… » | [[topo-exercices-types-corriges#14. Adhérence et intérieur d'une intersection, d'une réunion (écrit 2025-26)\|ex. 14]], [[topo-exercices-types-corriges#12. Interro 2026-27 – exercices\|ex. 12]] |
| $V$ voisinage $\iff$ boule | [[topo-voisinages-et-boules\|cours]] | « Par définition, $V$ est un voisinage de $a$ s'il existe un ouvert $O$… » | [[topo-exercices-types-corriges#11. Interro 2026-27 – questions de cours\|ex. 11]] |
| $\{f=g\}$, $\{f\neq g\}$, $\{f\le g\}$ | [[topo-montrer-ouvert-ferme\|image réciproque]] | « $h=f-g$ est continue et $\{f=g\}=h^{-1}(\{0\})$… » | [[topo-exercices-types-corriges#4. Les ensembles {f = g} et {f ≠ g}\|ex. 4]] |
| Distance induite, « ouvert de $I$ » | [[topo-distance-induite-ouverts-relatifs\|sous-espace]] | « $B_I(a,r)=B(a,r)\cap I=\dots$ » | [[topo-exercices-types-corriges#8. Distance induite sur une bande trouée\|ex. 8]] |
| $f$ continue en $(0,0)$ ? | [[topo-continuite-deux-variables\|majorer / suite]] | « Pour $(x,y)\neq(0,0)$, $\lvert f(x,y)\rvert\le\dots\to0$. » ou « $(\frac1n,\frac1n)\to(0,0)$ mais… » | [[topo-exercices-types-corriges#17. Continuité en (0,0)\|ex. 17]] |
| $f$ uniformément continue ? | [[topo-uniforme-continuite\|lipschitz / Heine / deux suites]] | « Soient $x_n=n$, $y_n=n+\frac1n$… » | [[topo-exercices-types-corriges#18. Uniforme continuité de x²\|ex. 18]] |
| $\delta\le kd$ ; distances équivalentes ? | [[topo-comparer-distances\|boules / suites / bornés]] | « Si $d(a,x)<\frac rk$, alors $\delta(a,x)\le k\,d(a,x)<r$… » | [[topo-exercices-types-corriges#10. Une distance plus petite qu'une autre (écrit 2025-26)\|ex. 10]] |
| Normes équivalentes ? | [[topo-montrer-normes-equivalentes\|encadrement]] | « En dimension finie, toutes les normes sont équivalentes. » ou « Soit $f_n=\dots$ » | — |

## Chapitre 3 – compacité

| L'énoncé demande… | Méthode | Première phrase sur la copie | Corrigé |
|---|---|---|---|
| $K\subset\mathbb R^n$ est compact | [[topo-montrer-compact\|fermé + borné]] | « $K$ est borné car $\dots\le M$. $K$ est fermé car… Fermé borné de $\mathbb R^n$ : compact. » | [[topo-exercices-types-corriges#13. Un compact de R (interro 2025-26)\|ex. 13]], [[topo-exercices-types-corriges#19. Compact de R² et maximum\|ex. 19]] |
| $K$ (abstrait) est compact | [[topo-bolzano-weierstrass\|suites]] | « Soit $(x_n)$ une suite de $K$ ; montrons qu'elle a une sous-suite convergente dans $K$. » | [[topo-exercices-types-corriges#3. La somme A + B\|ex. 3]] |
| $K$ n'est pas compact | [[topo-montrer-non-compact\|non borné / non fermé]] | « $K$ n'est pas borné : … » ou « $x_n\in K$ et $x_n\to\ell\notin K$… » | — |
| Une fonction atteint son max / min | [[topo-exploiter-compacite\|bornes atteintes]] | « $f$ est continue sur le compact $K$, donc bornée et atteint ses bornes. » | [[topo-exercices-types-corriges#19. Compact de R² et maximum\|ex. 19]] |
| $A+B$ fermé / compact | [[topo-somme-a-plus-b\|A + B]] | « Soit $z_k=a_k+b_k$ une suite de $A+B$ qui converge vers $z$… » | [[topo-exercices-types-corriges#3. La somme A + B\|ex. 3]] |
| Partie compacte ⟹ fermée et bornée | [[topo-compact-complet-borne\|cours]] | « Soit $(x_n)$ une suite de $K$ qui converge vers $x$ ; par compacité… » | — |
| $d(K,F)>0$, minoration stricte | [[topo-exploiter-compacite\|bornes atteintes]] | « $k\mapsto d(k,F)$ est continue sur le compact $K$… » | [[topo-exercices-types-corriges#15. Distance à une partie et à un compact\|ex. 15]] |
| Vrai ou faux ? | [[topo-vrai-faux-classiques\|vrai/faux]] | « Faux. Contre-exemple : … » / « Vrai. En effet… » | [[topo-vrai-faux-classiques]] |
