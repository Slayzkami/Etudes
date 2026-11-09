---
aliases:
  - "Théorème de Lagrange"
  - "Lagrange"
  - "x^[G]=1"
  - "l'ordre divise l'ordre du groupe"
tags:
  - gac
  - gac/theoreme
  - gac/chapitre-03
---

# ⭐ Théorème de Lagrange

*Théorème* · Chapitre : [[03-groupes-quotients|III – Groupes quotients]] · § III.4 du cours · [[index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> Soit $G$ un groupe fini et $H$ un sous-groupe. Alors **$[H]$ divise $[G]$**, et $[G]=[G:H]\,[H]$ ([[indice]]).

> [!SUCCESS]- Démonstration (à savoir par cœur)
> - Les [[classes-modulo-sous-groupe|classes à gauche]] $xH$ forment une **partition** de $G$.
> - $h\mapsto xh$ est une bijection $H\to xH$ (surjective par définition, injective par simplification), donc $\mathrm{Card}(xH)=[H]$.
> - $G$ fini ⟹ nombre fini $p$ de classes, toutes de cardinal $[H]$ : $[G]=p\,[H]$.

> [!IMPORTANT] Corollaire
> $\forall x\in G$ : $o(x)\mid[G]$ et $x^{[G]}=1$.
> (Car $o(x)=\mathrm{Card}\,\langle x\rangle$ ; si $[G]=k\,o(x)$, $x^{[G]}=(x^{o(x)})^k=1$.)

> [!TIP] Réflexes
> - Un groupe d'ordre 6 n'a pas d'élément d'ordre 4.
> - Sous-groupes de $\mathfrak S_3$ : d'ordres 1, 2, 3, 6 seulement.
> - $H\subset K$ sous-groupes ⟹ $[H]\mid[K]$.
> - Fermat : $p\nmid a\Rightarrow a^{p-1}\equiv1\pmod p$ (Lagrange dans $(\mathbb Z/p\mathbb Z)^*$).

## 🔗 Liens

- **S'appuie sur** : [[classes-modulo-sous-groupe|Classes à gauche et à droite modulo un sous-groupe]], [[indice|Indice d'un sous-groupe]], [[ordre-element|Ordre d'un élément]]
- **Utilisé par (définitions)** : [[ordre-groupe|Ordre d'un groupe]]
- **Utilisé par (théorèmes)** : [[groupe-ordre-premier|Groupe d'ordre premier]]
- **Méthodes** : [[calculer-ordre|Méthode : calculer l'ordre d'un élément]], [[vrai-faux-classiques|Vrai/Faux classiques (avec justification)]]
- **Voir aussi** : [[indice-2-distingue|Un sous-groupe d'indice 2 est distingué]]
- **Méthode** : [[utiliser-lagrange|utiliser le théorème de Lagrange]]
