---
aliases:
  - "Méthode : montrer qu'une partie est ouverte ou fermée"
  - "prouver ouvert"
  - "prouver fermé"
tags:
  - cd
  - cd/methode
  - cd/chapitre-01
---

# 🛠️ Méthode : montrer qu'une partie est ouverte ou fermée

*Méthode* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Méthode 1.1 du cours · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> - **Avec une fonction continue** $g:E\to\mathbb R$ (le plus rapide) : $\{g<c\}$ est ouvert ; $\{g\le c\}$ et $\{g=c\}$ sont fermés.
> - **Ouvert par la définition** : pour $x\in A$, exhiber $r>0$ avec $B(x,r)\subset A$.
> - **Fermé par les suites** (Th. 1.24) : $x_n\in A$, $x_n\to\ell$ ; montrer $\ell\in A$.
> - **Opérations** : réunion quelconque / intersection finie d'ouverts ; intersection quelconque / réunion finie de fermés.
> - **Pas fermé** : une suite de $A$ qui converge hors de $A$.

> [!EXAMPLE] Rédaction modèle
> $U=\{(x,y)\in\mathbb R^2\mid x>0\}$. L'application $g:(x,y)\mapsto x$ est continue (linéaire en dimension finie) et $U=\{g>0\}$ : $U$ est ouvert. (Domaine de $x(\ln x)^2+y^2$, Écrit 2022-2023.)

## 🔗 Liens

- **Voir aussi** : [[ouvert-ferme|Ouvert, fermé]], [[stabilite-ouverts-fermes|Stabilité des ouverts et des fermés]], [[caracterisation-sequentielle-fermes|Caractérisation séquentielle des fermés]]
