---
aliases:
  - "Calcul Différentiel"
  - "CD"
  - "Calcul diff"
tags:
  - cd
---

# 🎓 Calcul Différentiel

**Prof :** M. Barkatou  
**Année / semestre :** Licence 3 de mathématiques, semestre 5 (2026–2027), FST Limoges  
**Évaluation :** Écrit 1 (1 h 30, chapitres 1 à 3 et début du 4) – **fait le 3 novembre 2026** · Écrit 2 – *date, durée et documents autorisés à compléter*

## 📅 Dates importantes
| Date | Quoi |
|---|---|
| 3 novembre 2026 | Écrit 1 (fait) |
| *à compléter* | Écrit 2 |

## 🚀 Par où commencer
1. 📅 [[cd-plan-de-revision|Plan de révision]] : le programme jour par jour, à cocher (méthode « lire, fermer, réécrire de mémoire, comparer »).
2. 📘 [[cd-fiche-definitions|Toutes les définitions sur une page]], puis ⭐ [[cd-fiche-theoremes|tous les énoncés]].
3. 🛠️ Les trois méthodes de base : [[differentiabilite-par-definition|différentiabilité par la définition]], [[calculer-jacobienne|jacobienne]], [[etudier-points-critiques|points critiques]].
4. 🧭 [[cd-reconnaitre-exercice|Reconnaître le type d'exercice]] : quelle méthode sortir face à quel énoncé.
5. ✍️ [[cd-exercices-types-corriges|Exercices types corrigés]] : énoncé visible, correction repliée.
6. 🚨 [[cd-mes-erreurs|Mes erreurs à ne plus faire]] : à relire juste avant l'épreuve.

## 🧭 Pour retrouver une notion
- 🗂️ **[[cd-index-definitions|Index des définitions, théorèmes et méthodes]]** : le point d'entrée.
- 🧩 [[exemples-et-contre-exemples|Exemples et contre-exemples classiques]].
- ✅ [[cd-vrai-faux-classiques|Vrai/Faux classiques]].
- Dans Obsidian : `Ctrl/Cmd + O` puis le nom ou un alias (« IAF », « jacobienne », « Schwarz », « rt-s² »…) ; la vue graphe montre les liens entre notions.

Organisation du dossier :

```
L3/Calcul Différentiel/
├── README.md                       ← cette fiche
├── cd-index-definitions.md         ← sommaire de toutes les notions
├── exemples-et-contre-exemples.md  ← catalogue
├── 01 à 05-*.md                    ← un fichier par chapitre (résumé + liens)
├── definitions/                    ← une note par définition
├── theoremes/                      ← énoncés + démonstrations repliables
├── methodes/                       ← recettes pour les exercices
├── revision/                       ← plan, fiches d'une page, exercices corrigés, mes erreurs
└── fichiers/                       ← PDF (polycopiés, cours rédigé, TD, sujets, corrigés)
```

> [!NOTE] Pourquoi le préfixe `cd-` ?
> Les notes `index-definitions`, `plan-de-revision`, `fiche-definitions`… existent déjà dans [GAC](../gac/). Deux notes de même nom rendraient les liens `[[plan-de-revision]]` ambigus dans Obsidian : celles de cette matière commencent donc par `cd-`.

## 📖 Chapitres
- [x] [[01-espaces-vectoriels-normes|01 – Espaces vectoriels normés et applications linéaires continues]]
- [x] [[02-applications-differentiables|02 – Applications différentiables]]
- [x] [[03-accroissements-finis|03 – Accroissements finis]]
- [ ] [[04-differentielles-ordre-superieur|04 – Différentielles d'ordre supérieur]]
- [ ] [[05-inversion-locale-fonctions-implicites|05 – Inversion locale et fonctions implicites]]

## 🎯 Ce qui tombe (d'après les Écrits 1 de 2022-2023, 2024-2025, 2025-2026)

| Rang | Type d'exercice | Présent dans | Méthode |
|---|---|---|---|
| 1 | **Questions de cours** : définitions (différentiable, dérivée directionnelle, norme d'opérateur), énoncés (règle de la chaîne, IAF, Taylor-Young), petites démonstrations | 3 sujets sur 3 | [[cd-fiche-definitions\|définitions]], [[cd-fiche-theoremes\|énoncés]] |
| 2 | **Fonction $\mathbb R^n\to\mathbb R^p$** : différentiable, jacobienne, $Df_a(h)$, dérivée dans une direction | 3 sur 3 | [[calculer-jacobienne]], [[calculer-derivee-directionnelle]] |
| 3 | **Matrices** : développer $f(A+H)$, différentielle de $X^3$, $XMX$, $\mathrm{tr}(X\,{}^t\!X)$, puis composée | 3 sur 3 | [[differentielle-sur-les-matrices]], [[appliquer-regle-de-la-chaine]] |
| 4 | **Points critiques** et nature, Taylor-Young à l'ordre 2 | 2 sur 3 | [[etudier-points-critiques]], [[ecrire-taylor-young]] |
| 5 | **Majorer $\lvert\!\lvert\!\lvert Df\rvert\!\rvert\!\rvert$, IAF, lipschitzienne** | 1 sur 3 | [[utiliser-iaf]], [[calculer-norme-operateur]] |
| 6 | **Montrer qu'une application est une norme** ; $\lvert \mathrm{tr}(X)\rvert\le C\lVert X\rVert$ | 2 sur 3 | [[montrer-norme]], [[continuite-application-lineaire]] |
| 7 | Classe $\mathcal C^1$, gradient, plan tangent | 1 sur 3 | [[montrer-classe-c1]], [[gradient]] |

Pour l'Écrit 2 (chapitres 4 et 5), je n'ai pas d'annale : les exercices du polycopié du chapitre 5 servent de référence → [[montrer-diffeomorphisme]], [[fonction-implicite]].

## 📚 Ressources utiles
Toutes dans [fichiers](fichiers/) :
- **Cours rédigé complet, chapitres 1 à 5** (démonstrations, méthodes, pièges, exercices corrigés) : [cd-cours-redige-ch1-5.pdf](fichiers/cd-cours-redige-ch1-5.pdf) – c'est sa numérotation qui est utilisée partout ici.
- Polycopiés du prof : [chapitre 1](fichiers/cd-chap1-polycopie.pdf), [chapitre 2](fichiers/cd-chap2-polycopie.pdf), [chapitre 5](fichiers/cd-chap5-polycopie.pdf)
- Feuilles de TD : [TD1](fichiers/cd-td1.pdf), [TD2](fichiers/cd-td2.pdf), [TD3](fichiers/cd-td3.pdf)
- Écrit 1, sujets : [2022-2023](fichiers/cd-ecrit1-2022-2023-sujet.pdf), [2024-2025](fichiers/cd-ecrit1-2024-2025-sujet.pdf), [2025-2026](fichiers/cd-ecrit1-2025-2026-sujet.pdf)
- Écrit 1, corrigés : [2022-2023](fichiers/cd-ecrit1-2022-2023-corrige.pdf), [2024-2025](fichiers/cd-ecrit1-2024-2025-corrige.pdf), [2025-2026 (prof)](fichiers/cd-ecrit1-2025-2026-corrige.pdf), [2025-2026 (détaillé)](fichiers/cd-ecrit1-2025-2026-corrige-detaille.pdf), [2026-2027 (détaillé)](fichiers/cd-ecrit1-2026-2027-corrige-detaille.pdf)
- Partiels blancs : [n° 5](fichiers/cd-partiel-blanc-5.pdf) ([corrigé](fichiers/cd-partiel-blanc-5-corrige.pdf)), [n° 6](fichiers/cd-partiel-blanc-6.pdf) ([corrigé](fichiers/cd-partiel-blanc-6-corrige.pdf))

## ❓ Questions à poser au prof
- Date, durée et programme exact de l'Écrit 2 ? Documents autorisés ?
- Les démonstrations du théorème d'inversion locale et des fonctions implicites sont-elles exigibles ?
- Les polycopiés des chapitres 3 et 4 (à ajouter dans `fichiers/`).
