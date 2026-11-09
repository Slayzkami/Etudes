---
aliases:
  - "Méthode : identifier un groupe quotient G/H"
  - "calculer un quotient"
  - "G/H ≃ ?"
tags:
  - gac
  - gac/methode
  - gac/chapitre-03
---

# 🛠️ Méthode : identifier un groupe quotient G/H

*Méthode* · Chapitre : [[03-groupes-quotients|III – Groupes quotients]] · [[index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> 1. Trouver un [[morphisme-de-groupes|morphisme]] $f:G\to K$ vers un groupe connu avec **$\mathrm{Ker} f=H$**.
> 2. Déterminer $\mathrm{Im} f$ (souvent : $f$ surjectif).
> 3. Conclure : $G/H\simeq\mathrm{Im} f$ via $\bar x\mapsto f(x)$ ([[premier-theoreme-isomorphisme]]).

> [!EXAMPLE] Exemples
> | quotient | morphisme | résultat |
> |---|---|---|
> | $\mathbb R^*/\{\pm1\}$ | $x\mapsto\lvert x\rvert$ | $\simeq\mathbb R_+^*$ |
> | $\mathbb R/\mathbb Z$ | $t\mapsto e^{2i\pi t}$ | $\simeq\mathbb U$ |
> | $\mathbb C^*/\mathbb U$ | $z\mapsto\lvert z\rvert$ | $\simeq\mathbb R_+^*$ |
> | $GL_n(\mathbb R)/SL_n(\mathbb R)$ | $\det$ | $\simeq\mathbb R^*$ |
> | $G/Z(G)$ | $a\mapsto f_a$ | $\simeq\mathcal I(G)$ |
> | $\mathbb Z/18\mathbb Z\,/\,6\mathbb Z/18\mathbb Z$ | $\bar x\mapsto x+6\mathbb Z$ | $\simeq\mathbb Z/6\mathbb Z$ |

## 🔗 Liens

- **Utilisé par (théorèmes)** : [[premier-theoreme-isomorphisme|Premier théorème d'isomorphisme]]
- **Voir aussi** : [[groupe-quotient|Groupe quotient]], [[morphisme-sur-quotient|Méthode : application définie sur un quotient (bien définie, morphisme)]]
- **Corrigé** : [[exercices-types-corriges#8. Identifier un quotient|R*/{±1} rédigé en entier]]
