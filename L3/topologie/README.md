---
aliases:
  - "Topologie"
  - "Topo"
  - "Topologie des espaces métriques"
tags:
  - topologie
---

# 🎓 Topologie

**Prof :** N. Igbida  
**Année / semestre :** Licence 3 de mathématiques, semestre 5 (2026–2027), FST Limoges  
**Évaluation :** interro écrite du 9 novembre 2026 (faite) · **examen du mercredi 18 novembre 2026** (1 h 30, sans document, tout le cours magistral : chapitres 1 à 3)

## 📅 Dates importantes
| Date | Quoi |
|---|---|
| Lundi 9 novembre 2026 | Interro écrite (faite) |
| **Mercredi 18 novembre 2026** | **Examen (1 h 30, sans document)** |

## 🚀 Par où commencer
1. 📅 [[topo-plan-de-revision|Plan de révision]] : le programme jour par jour, à cocher (méthode « lire, fermer, réécrire de mémoire, comparer »).
2. 📘 [[topo-fiche-definitions|Toutes les définitions sur une page]], puis ⭐ [[topo-fiche-theoremes|tous les énoncés]].
3. 🛠️ Les deux méthodes qui tombent à chaque fois : [[topo-montrer-pas-ouvert-pas-ferme|pas ouvert / pas fermé]] et [[topo-calculer-interieur-adherence-frontiere|adhérence et intérieur]].
4. 🧭 [[topo-reconnaitre-exercice|Reconnaître le type d'exercice]] : quelle méthode sortir face à quel énoncé.
5. ✍️ [[topo-exercices-types-corriges|Exercices types corrigés]] (20, dont toutes les annales) : énoncé visible, correction repliée.
6. 🚨 [[topo-mes-erreurs|Mes erreurs à ne plus faire]] : à relire juste avant l'épreuve.

## 🧭 Pour retrouver une notion
- 🗂️ **[[topo-index-definitions|Index des définitions, théorèmes et méthodes]]** : le point d'entrée (avec la carte des notions).
- 🧩 [[topo-exemples-et-contre-exemples|Exemples et contre-exemples classiques]].
- ✅ [[topo-vrai-faux-classiques|Vrai/Faux classiques]].
- Dans Obsidian : `Ctrl/Cmd + O` puis le nom ou un alias (« adhérence », « Heine », « fermé borné », « A+B »…) ; la vue graphe montre les liens entre notions.
- Tous les fichiers de cette matière commencent par `topo-` pour ne pas se mélanger avec les notions du même nom en [[L3/Calcul Différentiel/README|Calcul Différentiel]].

Organisation du dossier :

```
L3/topologie/
├── README.md                        ← cette fiche
├── topo-index-definitions.md        ← sommaire de toutes les notions + carte
├── topo-exemples-et-contre-exemples.md
├── 01 à 03-*.md                     ← un fichier par chapitre (résumé + liens)
├── definitions/                     ← une note par définition (33)
├── theoremes/                       ← énoncés + démonstrations repliables (51)
├── methodes/                        ← recettes pour les exercices (17)
├── revision/                        ← plan, fiches d'une page, exercices corrigés, vrai/faux, mes erreurs
└── fichiers/                        ← PDF (polycopiés, cours rédigé, sujets, corrigés)
```

## 📖 Chapitres
- [ ] [[01-espaces-metriques|01 – Espaces métriques, espaces vectoriels normés]]
- [ ] [[02-topologie-espaces-metriques|02 – Topologie des espaces métriques]]
- [ ] [[03-espaces-metriques-compacts|03 – Espaces métriques compacts]]

## 🎯 Priorités pour l'examen (d'après 4 sujets)
1. Partie de $\mathbb R$ ou $\mathbb R^2$ : ouvert ? fermé ? adhérence, intérieur → [[topo-montrer-pas-ouvert-pas-ferme]], [[topo-calculer-interieur-adherence-frontiere]]
2. Distances : discrète, $\min(1,d)$, $\delta\le kd$, métriquement ⟹ mêmes fermés → [[topo-montrer-distance]], [[topo-comparer-distances]]
3. Questions de cours : boule fermée fermée, $\overline{B(a,r)}\subset\bar B(a,r)$, voisinage ⟺ boule → [[topo-boule-fermee-fermee]], [[topo-voisinages-et-boules]]
4. Adhérence et intérieur d'une intersection, réunion, complémentaire → [[topo-caracterisation-adherence]], [[topo-complementaire-interieur-adherence]]
5. $\{f=g\}$ fermé, $\{f\neq g\}$ ouvert → [[topo-montrer-ouvert-ferme]]
6. $A+B$ et compacité → [[topo-somme-a-plus-b]], [[topo-montrer-compact]]
7. Distance induite → [[topo-distance-induite-ouverts-relatifs]]

## 📚 Ressources utiles
Toutes dans [fichiers](fichiers/) :
- Cours : [polycopié chapitre 1](fichiers/topo-chap1-polycopie.pdf), [polycopié chapitre 2](fichiers/topo-chap2-polycopie.pdf), [cours rédigé complet ch. 1 à 3 (démonstrations, méthodes, exercices corrigés)](fichiers/topo-cours-redige-ch1-3.pdf), [cours ciblé interro](fichiers/topo-cours-cible-interro.pdf)
- Sujets : [écrit 1 2022-2023](fichiers/topo-ecrit1-2022-2023-sujet.pdf), [écrit 1 2025-2026](fichiers/topo-ecrit1-2025-2026-sujet.pdf), [interro 2025-2026](fichiers/topo-interro-2025-2026-sujet.pdf) ([corrigé](fichiers/topo-interro-2025-2026-corrige.pdf)), [interro 2026-2027](fichiers/topo-interro-2026-2027-sujet.jpg)
- Entraînement : [sujet bilan](fichiers/topo-sujet-bilan.pdf), sujets [n°1](fichiers/topo-entrainement-sujet-1.pdf), [n°2](fichiers/topo-entrainement-sujet-2.pdf), [n°3](fichiers/topo-entrainement-sujet-3.pdf) et leurs [corrigés](fichiers/topo-entrainement-corriges.pdf) *(à faire en 1 h 30 avant de lire le corrigé)*

## ❓ Questions à poser au prof
- Interro 2026-27, exercice 1 : la condition $x+y>0$ est toujours vraie sur $y=e^{x^2}$, donc $X$ est fermé. La question 1 sera-t-elle neutralisée ?
- L'examen porte-t-il sur tout le chapitre 3 (y compris Riesz et l'équivalence des normes) ?
