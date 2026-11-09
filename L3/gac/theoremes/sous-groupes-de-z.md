---
aliases:
  - "Sous-groupes de (Z,+)"
  - "sous-groupes de Z"
  - "aZ"
  - "nZ"
tags:
  - gac
  - gac/theoreme
  - gac/chapitre-02
---

# ⭐ Sous-groupes de (Z,+)

*Théorème* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · § II.2 du cours · [[index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> Les sous-groupes de $(\mathbb Z,+)$ sont exactement les $a\mathbb Z=\{an\mid n\in\mathbb Z\}$, $a\in\mathbb N$, et $a$ est unique (si $H\neq\{0\}$, $a=\min(H\cap\mathbb N^*)$).
> Inclusions : $a\mathbb Z\subset b\mathbb Z\iff b\mid a$.

> [!SUCCESS]- Démonstration
> Si $H\neq\{0\}$, soit $a=\min(H\cap\mathbb N^*)$ (existe car $x\in H\Rightarrow -x\in H$).
> - $a\mathbb Z\subset H$ par stabilité.
> - Pour $x\in H$ : $x=qa+r$, $0\le r<a$ ; $r=x-qa\in H$ ; minimalité ⟹ $r=0$.
> Unicité : $a\mathbb Z=b\mathbb Z\Rightarrow a\mid b$ et $b\mid a$.

> [!TIP] Utilisé pour
> [[ordre-element]] (le noyau de $n\mapsto x^n$ est $m\mathbb Z$), $\langle a,b\rangle=\operatorname{pgcd}(a,b)\mathbb Z$, [[lister-sous-groupes-znz]], [[endomorphismes-de-z]].

## 🔗 Liens

- **S'appuie sur** : [[sous-groupe|Sous-groupe]]
- **Utilisé par (définitions)** : [[ordre-element|Ordre d'un élément]]
- **Méthodes** : [[lister-sous-groupes-znz|Méthode : lister les sous-groupes de Z/nZ (treillis)]]
- **Voir aussi** : [[sous-groupe-engendre|Sous-groupe engendré par une partie]]
