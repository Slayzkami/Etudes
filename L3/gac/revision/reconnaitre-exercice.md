---
aliases:
  - "Reconnaître le type d'exercice"
  - "quelle méthode utiliser"
  - "types d'exercices"
tags:
  - gac
  - gac/revision
---

# 🧭 Reconnaître le type d'exercice

« L'énoncé dit ça → je sors cette méthode → je commence par cette phrase. » · [[plan-de-revision|↩ Plan de révision]] · [[index-definitions|↩ Index]]

## Rappels – relations d'équivalence

| L'énoncé demande… | Méthode | Première phrase sur la copie | Corrigé |
|---|---|---|---|
| Montrer que $\mathcal R$ est une relation d'équivalence | [[montrer-relation-equivalence]] | « Réflexivité : soit $x\in E$… » | [[exercices-types-corriges#6. Relation d'équivalence associée à une application|ex. 6]] |
| Décrire la classe de $x$, le quotient | [[montrer-relation-equivalence]] | « $\bar x=\{y\in E\mid y\mathcal Rx\}=\dots$ » | [[exercices-types-corriges#6. Relation d'équivalence associée à une application|ex. 6]] |
| La relation est-elle compatible avec la loi ? | [[montrer-relation-equivalence]] | « Soient $x\mathcal Ry$ et $x'\mathcal Ry'$… » | — |

## I – Groupes et morphismes

| L'énoncé demande… | Méthode | Première phrase sur la copie | Corrigé |
|---|---|---|---|
| Montrer que $(G,\star)$ est un groupe (loi bizarre) | [[montrer-groupe]] | « Loi interne : soient $a,b\in G$… » | [[exercices-types-corriges#4. Loi exotique a ⋆ b = a + b + ab|ex. 4]] |
| Montrer qu'un groupe est abélien | calcul : $xy=yx$ | « Soient $x,y\in G$… » | [[exercices-types-corriges#15. Groupe où tout élément vérifie x² = e|ex. 15]] |
| Montrer que $f$ est un morphisme / un isomorphisme | [[montrer-morphisme]] | « Soient $x,y\in G$. $f(xy)=\dots$ » | [[exercices-types-corriges#10. Étudier un morphisme|ex. 10]], [[exercices-types-corriges#16. Automorphismes intérieurs|ex. 16]] |
| Trouver **tous** les morphismes de $\mathbb Z$ ou $\mathbb Z/n\mathbb Z$ vers… | [[endomorphismes-de-z]] | « Analyse : posons $a=f(1)$… » | [[exercices-types-corriges#5. Endomorphismes de (Z, +)|ex. 5]], [[exercices-types-corriges#18. Morphismes de Z/4Z dans Z/6Z|ex. 18]] |
| Ces deux groupes sont-ils isomorphes ? | [[montrer-non-isomorphes]] (si non) ; exhiber un isomorphisme (si oui) | « Un isomorphisme conserve… » | [[exercices-types-corriges#11. Ordres dans un produit|ex. 11]] |
| Vrai ou faux ? | [[vrai-faux-classiques]] | « Faux. Contre-exemple : … » / « Vrai. En effet… » | [[vrai-faux-classiques#✍️ Justifications rédigées (comme sur la copie)\|rédactions]] |

## II – Sous-groupes, ordres

| L'énoncé demande… | Méthode | Première phrase sur la copie | Corrigé |
|---|---|---|---|
| Calculer dans $\mathbb Z/n\mathbb Z$ | [[calculer-dans-znz]] | « Dans $\mathbb Z/n\mathbb Z$ : … » | — |
| Montrer que $H$ est un sous-groupe | [[montrer-sous-groupe]] | « $e\in H$ car… Soient $x,y\in H$, montrons $xy^{-1}\in H$. » | [[exercices-types-corriges#7. Montrer qu'une partie est un sous-groupe|ex. 7]], [[exercices-types-corriges#13. Centre et sous-groupe distingué|ex. 13]] |
| $H\cup K$, $H\cap K$ sont-ils des sous-groupes ? | [[intersection-sous-groupes]] | « $x\in H\cup K$, $y\in H\cup K$ mais $x+y\notin$… » | [[exercices-types-corriges#2. Réunion de deux sous-groupes|ex. 2]], [[exercices-types-corriges#19. Intersection et somme de sous-groupes de Z|ex. 19]] |
| Ordre d'un élément | [[calculer-ordre]] | « $\operatorname{pgcd}(n,k)=\dots$, donc $o(\bar k)=n/\dots$ » | [[exercices-types-corriges#1. Ordres et sous-groupes de Z/18Z|ex. 1]], [[exercices-types-corriges#11. Ordres dans un produit|ex. 11]], [[exercices-types-corriges#17. Ordre de l'inverse et d'un conjugué|ex. 17]] |
| Sous-groupe engendré $\langle x\rangle$ | [[calculer-dans-znz]] | « $1x=\dots$, $2x=\dots$ jusqu'au neutre » | [[exercices-types-corriges#1. Ordres et sous-groupes de Z/18Z|ex. 1]] |
| Tous les sous-groupes de $\mathbb Z/n\mathbb Z$, diagramme | [[lister-sous-groupes-znz]] | « Les diviseurs de $n$ sont… » | [[exercices-types-corriges#1. Ordres et sous-groupes de Z/18Z|ex. 1]] |
| Tous les sous-groupes d'un petit groupe | [[utiliser-lagrange]] | « Par Lagrange, les ordres possibles sont… » | [[exercices-types-corriges#14. Sous-groupes de S3|ex. 14]] |
| Le groupe est-il cyclique ? Générateurs ? | [[montrer-cyclique]] | « $o(a)=[G]$ donc $\langle a\rangle=G$ » | [[exercices-types-corriges#1. Ordres et sous-groupes de Z/18Z|ex. 1]], [[exercices-types-corriges#9. Groupe d'ordre premier|ex. 9]] |
| Noyau, image, injectif, surjectif | [[montrer-morphisme]] | « $x\in\mathrm{Ker}\,f\iff f(x)=e'\iff\dots$ » | [[exercices-types-corriges#3. Morphisme Z/18Z → Z/6Z et quotient|ex. 3]], [[exercices-types-corriges#10. Étudier un morphisme|ex. 10]] |
| $H$ est-il distingué ? | [[montrer-distingue]] | « Soient $g\in G$, $h\in H$ : $g^{-1}hg=\dots$ » | [[exercices-types-corriges#13. Centre et sous-groupe distingué|ex. 13]], [[exercices-types-corriges#14. Sous-groupes de S3|ex. 14]] |

## III – Quotients

| L'énoncé demande… | Méthode | Première phrase sur la copie | Corrigé |
|---|---|---|---|
| $f$ définie sur un quotient est-elle bien définie ? | [[morphisme-sur-quotient]] | « Soient $x,y$ tels que $\bar x=\bar y$. Alors… » | [[exercices-types-corriges#3. Morphisme Z/18Z → Z/6Z et quotient|ex. 3]], [[exercices-types-corriges#18. Morphismes de Z/4Z dans Z/6Z|ex. 18]] |
| Écrire les classes, calculer l'indice | [[classes-et-indice]] | « $[G:H]=[G]/[H]=\dots$ classes » | [[exercices-types-corriges#12. Classes, indice et quotient|ex. 12]] |
| « Montrer que $G/H\simeq\dots$ », « en déduire un isomorphisme » | [[identifier-quotient]] | « Soit $f:G\to\dots$ ; $\mathrm{Ker}\,f=H$… » | [[exercices-types-corriges#3. Morphisme Z/18Z → Z/6Z et quotient|ex. 3]], [[exercices-types-corriges#8. Identifier un quotient|ex. 8]], [[exercices-types-corriges#12. Classes, indice et quotient|ex. 12]] |
| Ordres possibles, « peut-il exister… ? » (groupe fini) | [[utiliser-lagrange]] | « D'après le théorème de Lagrange… » | [[exercices-types-corriges#9. Groupe d'ordre premier|ex. 9]], [[exercices-types-corriges#14. Sous-groupes de S3|ex. 14]] |

> [!TIP] Les mots de l'énoncé qui doivent faire tilt
> - « **bien définie** » → indépendance du représentant.
> - « **en déduire** un isomorphisme » → premier théorème d'isomorphisme avec le morphisme de la question d'avant.
> - « **déterminer tous** les… » → analyse (ce que ça doit être) puis synthèse (ça marche).
> - « groupe **fini** », « d'ordre $n$ » → Lagrange.
> - « **justifier** » → preuve si vrai, contre-exemple chiffré si faux.

## 🔗 Liens

- [[exercices-types-corriges]] · [[vrai-faux-classiques]] · [[mes-erreurs]] · [[fiche-definitions]] · [[fiche-theoremes]]
