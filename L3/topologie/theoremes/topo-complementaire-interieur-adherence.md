---
aliases:
  - "Intérieur et adhérence échangés par complémentaire"
  - "complémentaire de l'adhérence"
  - "int(X−Y) = X − adh(Y)"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-02
---

# ⭐ Intérieur et adhérence échangés par complémentaire

*Théorème* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Prop. 2.25 du cours (ajout) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> $$(\bar A)^c=\operatorname{Int}(A^c)\qquad\text{et}\qquad(\operatorname{Int}A)^c=\overline{A^c}.$$

> [!SUCCESS]- Démonstration
> $x\notin\bar A\iff\exists r>0,\ B(x,r)\cap A=\emptyset\iff\exists r>0,\ B(x,r)\subset A^c\iff x\in\operatorname{Int}(A^c)$. La seconde égalité : appliquer la première à $A^c$ et repasser au complémentaire.

> [!TIP] Réflexes
> **Interro 2026-27, ex. 2** : $\operatorname{int}(X\setminus Y)=X\setminus\bar Y$, puis $\overline{X\setminus Y}=X\setminus\operatorname{int}Y$. Rédaction « par les définitions » (plus grand ouvert / plus petit fermé) dans [[topo-exercices-types-corriges#12. Interro 2026-27 – exercices|ex. 12]].

## 🔗 Liens

- **S'appuie sur** : [[topo-interieur|Intérieur]], [[topo-adherence|Adhérence]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-proprietes-frontiere|Propriétés de la frontière]]
- **Méthodes** : —
- **Voir aussi** : —
