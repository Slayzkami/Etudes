---
aliases:
  - "Automorphismes et automorphismes intérieurs"
  - "Aut G"
  - "automorphisme intérieur"
  - "conjugaison"
  - "f_a"
  - "Int(G)"
tags:
  - gac
  - gac/definition
  - gac/chapitre-01
---

# 📘 Automorphismes et automorphismes intérieurs

*Définition* · Chapitre : [[01-definitions-generales|I – Définitions générales]] · § I.3 du cours · [[index-definitions|↩ Index]]

> [!NOTE] Définitions
> - $\mathrm{Aut}\,G$ : ensemble des automorphismes de $G$ ; c'est un groupe pour $\circ$ (sous-groupe de $\mathcal S(G)$).
> - Pour $a\in G$, l'**automorphisme intérieur** associé à $a$ est $f_a:G\to G,\ x\mapsto axa^{-1}$.
> - $\mathcal I(G)=\{f_a\mid a\in G\}$ est un [[sous-groupe]] de $\mathrm{Aut}\,G$.

> [!IMPORTANT] Calculs utiles
> $f_a\circ f_b=f_{ab}$, $f_a^{-1}=f_{a^{-1}}$. Si $G$ est abélien, $f_a=\mathrm{id}$.

> [!EXAMPLE] Exemple
> $\mathrm{Aut}(\mathbb Z/4\mathbb Z)=\{\mathrm{id},-\mathrm{id}\}\simeq\mathbb Z/2\mathbb Z$.
> $\mathcal I(G)\simeq G/Z(G)$ (avec [[premier-theoreme-isomorphisme]] et le [[centre]]).

## 🔗 Liens

- **S'appuie sur** : [[morphisme-de-groupes|Morphisme de groupes]]
- **Voir aussi** : [[sous-groupe-distingue|Sous-groupe distingué]], [[centre|Centre d'un groupe]]
