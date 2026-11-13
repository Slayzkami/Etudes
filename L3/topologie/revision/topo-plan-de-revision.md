---
aliases:
  - "Plan de révision topologie"
  - "planning examen topologie"
  - "révision topo"
tags:
  - topologie
  - topo/revision
---

# 📅 Plan de révision – examen du mercredi 18 novembre

**Épreuve** : 1 h 30, sans document. **Programme** : tout le cours magistral (chapitres 1 à 3 : espaces métriques, topologie, compacité). · [[L3/topologie/README|↩ Fiche matière]] · [[topo-index-definitions|↩ Index]]

> [!TIP] La méthode pour chaque case : **lire, fermer, réécrire de mémoire, comparer**
> 1. **Lire** la fiche ou la correction (2 fois, en comprenant chaque ligne).
> 2. **Fermer** : cacher l'écran ou la feuille.
> 3. **Réécrire de mémoire** sur papier, en entier, avec les quantificateurs.
> 4. **Comparer** ligne par ligne ; ce qui manque ou est faux va dans [[topo-mes-erreurs]], et on recommence la case le lendemain.
> Une case n'est cochée que si la réécriture est **juste du premier coup**.

> [!IMPORTANT] Ce qui tombe (analyse de 4 sujets : écrits 2022-23 et 2025-26, interros 2025-26 et 2026-27)
> | Priorité | Type d'exercice | Fréquence | Fiches |
> |---|---|---|---|
> | **1** | Une partie de $\mathbb R$ ou $\mathbb R^2$ : ouvert ? fermé ? adhérence, intérieur | 3 sujets sur 4 (5 exercices) | [[topo-montrer-pas-ouvert-pas-ferme]], [[topo-calculer-interieur-adherence-frontiere]] |
> | **2** | Question de cours : boule fermée fermée, $\overline{B(a,r)}\subset\bar B(a,r)$, voisinage $\iff$ boule | 2 sur 4 (4 questions) | [[topo-boule-fermee-fermee]], [[topo-voisinages-et-boules]] |
> | **3** | Distances : discrète, $\min(1,d)$, $\delta\le kd$, métriquement ⟹ mêmes fermés | 4 sur 4 | [[topo-montrer-distance]], [[topo-comparer-distances]], [[topo-distance-discrete]] |
> | **4** | Adhérence / intérieur et opérations ($\cap$, $\cup$, complémentaire) | 2 sur 4 | [[topo-caracterisation-adherence]], [[topo-complementaire-interieur-adherence]] |
> | **5** | $\{f=g\}$ fermé, $\{f\neq g\}$ ouvert (image réciproque) | 2 sur 4 | [[topo-montrer-ouvert-ferme]] |
> | **6** | $A+B$ (compact + fermé, compact + compact, contre-exemple) | 2 sur 4 | [[topo-somme-a-plus-b]] |
> | **7** | Compacité de $\{0\}\cup\{\frac1n\}$, fermé borné, bornes atteintes | 1 sur 4 (mais programme complet cette fois) | [[topo-montrer-compact]] |
> | **8** | Distance induite, ouverts relatifs | 1 sur 4 | [[topo-distance-induite-ouverts-relatifs]] |
>
> Toutes les annales sont rédigées dans [[topo-exercices-types-corriges]].

## Vendredi 13 (soir) – rien
- [x] Organisation du dossier (fait). Dormir.

## Samedi 14 – les bases qui rapportent le plus
- [ ] Définitions avec quantificateurs : ouvert, fermé, voisinage, intérieur, adhérence, frontière ([[topo-fiche-definitions]], chapitre 2) — lire, fermer, réécrire
- [ ] Les 2 tableaux « pas ouvert / pas fermé » et « adhérence = deux inclusions » → [[topo-montrer-pas-ouvert-pas-ferme]], [[topo-calculer-interieur-adherence-frontiere]]
- [ ] Refaire seul : [[topo-exercices-types-corriges#5. Une partie de R – ouvert, fermé, adhérence, intérieur|ex. 5]] puis ses variantes ($[1,2[\cup\{5\}$, $\mathbb Z$, $\{\frac1n\}$)
- [ ] Refaire seul : [[topo-exercices-types-corriges#6. Une suite qui tend vers 0 (écrit 2025-26)|ex. 6]] et [[topo-exercices-types-corriges#7. La parabole (interro 2025-26)|ex. 7]]
- [ ] Relire [[topo-mes-erreurs]]

## Dimanche 15 – questions de cours + continuité
- [ ] Par cœur (lire, fermer, réécrire) : [[topo-boule-ouverte-ouverte]], [[topo-boule-fermee-fermee]] (2 versions), [[topo-caracterisation-sequentielle-fermes]], [[topo-voisinages-et-boules]]
- [ ] $\overline{B(a,r)}\subset\bar B(a,r)$ et distance discrète : [[topo-exercices-types-corriges#2. Adhérence de la boule ouverte et distance discrète|ex. 2]]
- [ ] Image réciproque : [[topo-continuite-globale]] puis [[topo-exercices-types-corriges#4. Les ensembles {f = g} et {f ≠ g}|ex. 4]] et [[topo-exercices-types-corriges#16. Ouverts et fermés de R²|ex. 16]]
- [ ] Opérations sur adhérence/intérieur : [[topo-exercices-types-corriges#14. Adhérence et intérieur d'une intersection, d'une réunion (écrit 2025-26)|ex. 14]], [[topo-exercices-types-corriges#12. Interro 2026-27 – exercices|ex. 12 (ex. 2)]]
- [ ] Continuité en $(0,0)$ et U.C. : [[topo-exercices-types-corriges#17. Continuité en (0,0)|ex. 17]], [[topo-exercices-types-corriges#18. Uniforme continuité de x²|ex. 18]]

## Lundi 16 – distances + compacité
- [ ] $\min(1,d)$ en entier (distance + boules) : [[topo-exercices-types-corriges#9. Interro 2025-26 – la distance min(1, d)|ex. 9]]
- [ ] $\delta\le kd$ et métriquement ⟹ mêmes fermés : [[topo-exercices-types-corriges#10. Une distance plus petite qu'une autre (écrit 2025-26)|ex. 10]], [[topo-exercices-types-corriges#11. Interro 2026-27 – questions de cours|ex. 11 (Q2, Q5)]]
- [ ] Distance induite : [[topo-exercices-types-corriges#8. Distance induite sur une bande trouée|ex. 8]]
- [ ] Compacité, définitions et théorèmes : [[topo-espace-compact]], [[topo-bolzano-weierstrass]], [[topo-compact-complet-borne]], [[topo-borel-lebesgue]], [[topo-bornes-atteintes]], [[topo-heine]] (énoncés par cœur via [[topo-fiche-theoremes]])
- [ ] $\{0\}\cup\{\frac1n\}$ compact et $A+B$ : [[topo-exercices-types-corriges#13. Un compact de R (interro 2025-26)|ex. 13]], [[topo-exercices-types-corriges#3. La somme A + B|ex. 3]], [[topo-exercices-types-corriges#19. Compact de R² et maximum|ex. 19]]
- [ ] Les Vrai/Faux en cachant la colonne de droite → [[topo-vrai-faux-classiques]]

## Mardi 17 (veille) – conditions réelles
- [ ] **Sujet blanc, 1 h 30, sans document, sans téléphone** (demandé à Claude dans le chat)
- [ ] Correction notée, erreurs ajoutées à [[topo-mes-erreurs]]
- [ ] Fiche d'une page « pièges et réflexes »
- [ ] Coucher tôt : pas de nouvel exercice après 21 h

## Mercredi 18 – examen
- [ ] Relire uniquement : [[topo-mes-erreurs]], la fiche « pièges et réflexes », [[topo-fiche-definitions]] (chapitre 2)

> [!ABSTRACT] Stratégie pendant l'épreuve
> - Lire tout le sujet (5 min) ; commencer par l'exercice le plus familier (souvent « partie de $\mathbb R^2$ »).
> - **Ne jamais laisser une question vide** : écrire au moins la définition, ou la méthode (« soit $(x_n)$ une suite de $A$ qui converge vers $\ell$ ; montrons $\ell\in A$ »).
> - Adhérence : **deux inclusions**. Fermé : **suites** ou **image réciproque**. Réunion de fermés : **finie** seulement.
> - Si un énoncé semble faux, le dire et montrer ce qui est vrai (interro 2026-27, ex. 1).
> - Bloqué plus de 10 min : passer à la suite, revenir à la fin.
> - Garder 10 minutes pour relire : $n\in\mathbb N^*$ ? $n\to+\infty$ ? conclusion encadrée ?
