# 🛠️ Projet de topologie : la fonction Gamma (d'après Emil Artin)

**Matière / cadre :** [Topologie](../../L3/topologie/README.md), L3 mathématiques, semestre 5 (2026–2027), FST Limoges  
**Encadrant :** N. Igbida  
**Groupe :** seul  
**Rendu le :** *(à compléter)*  
**Statut :** 🟡 en cours  <!-- 🟢 rendu · 🔴 en pause -->

## 🎯 Objectif
Rédiger un rapport en LaTeX, rendu en PDF, mis en page comme un article de recherche (classe `amsart` : titre en petites capitales, résumé, sections numérotées, théorèmes et preuves, bibliographie).

> Sujet : la fonction Gamma, d'après *The Gamma Function* d'Emil Artin → [fiche de lecture](notes/artin-the-gamma-function.md) · [PDF du livre](notes/artin-the-gamma-function.pdf)

## 📅 Échéances
| Date | Étape | Fait ? |
|---|---|---|
| 16 novembre 2026 | Création du projet et du squelette LaTeX | ✅ |
| 16 novembre 2026 | Plan du rapport (sujet Gamma / Artin) et premier PDF | ✅ |
| *(à compléter)* | Rendu du PDF | ⬜ |

## ✅ Tâches
- [x] Créer le squelette LaTeX → [`rendus/projet-topologie.tex`](rendus/projet-topologie.tex)
- [x] Choisir le sujet : la fonction Gamma d'après Artin
- [x] Faire le plan du rapport (il suit les chapitres du livre)
- [ ] Préciser la date de rendu
- [ ] Rédiger les démonstrations (repérées par *[À rédiger : …]* dans le PDF)
- [ ] Rédiger l'introduction et la conclusion
- [ ] Relire, compiler et rendre le PDF

## 📝 Notes / avancement
### Compiler le rapport
- Sur [Overleaf](https://www.overleaf.com) : importer `rendus/projet-topologie.tex`, puis cliquer sur « Recompile ».
- En local : `pdflatex projet-topologie.tex`, à lancer deux fois pour que les numéros de références s'affichent.
- Les environnements `theoreme`, `proposition`, `lemme`, `corollaire`, `definition`, `exemple` et `remarque` sont déjà définis. Les raccourcis aussi : `\R`, `\N`, `\norm{x}`, `\abs{x}`, `\adh{A}` (adhérence), `\interieur{A}`.

Les brouillons et les idées vont dans [`notes/`](notes/).

Pour le français, le fichier utilise `\babelprovide[import, main]{french}`, qui fonctionne aussi sur les installations TeX où `[french]{babel}` n'est pas installé.

Les passages encore à écrire sont marqués avec la commande `\afaire{…}` et apparaissent en italique entre crochets dans le PDF.

## 📚 Sources
- [E. Artin, *The Gamma Function*, Holt, Rinehart and Winston, 1964](notes/artin-the-gamma-function.pdf) : le livre de référence du projet → [ma fiche de lecture](notes/artin-the-gamma-function.md)
- [Cours rédigé de topologie, ch. 1 à 3](../../L3/topologie/fichiers/topo-cours-redige-ch1-3.pdf) : le cours de référence pour les définitions et les théorèmes
- [F. Johansson, *Arbitrary-precision computation of the gamma function*](https://arxiv.org/abs/2109.08392) : l'article qui sert de modèle de mise en page

## 📦 Rendus
- [`rendus/projet-topologie.pdf`](rendus/projet-topologie.pdf) : le rapport compilé (version de travail, 3 pages)
- [`rendus/projet-topologie.tex`](rendus/projet-topologie.tex) : la source LaTeX
