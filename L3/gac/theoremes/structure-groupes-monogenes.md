---
aliases:
  - "Structure des groupes monogènes"
  - "monogène infini ≃ Z"
  - "cyclique ≃ Z/nZ"
tags:
  - gac
  - gac/theoreme
  - gac/chapitre-02
---

# ⭐ Structure des groupes monogènes

*Théorème* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · § II.7 et III.6 du cours · [[index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> - Tout [[groupe-monogene-cyclique|groupe monogène]] infini est isomorphe à $(\mathbb Z,+)$.
> - Tout groupe cyclique d'ordre $n$ est isomorphe à $(\mathbb Z/n\mathbb Z,+)$ : si $G=\langle a\rangle$, alors $o(a)=n$, $G=\{1,a,\dots,a^{n-1}\}$ et $\bar k\mapsto a^k$ est un isomorphisme.
> - Un groupe monogène est abélien.

> [!SUCCESS]- Démonstration (version quotient, III.6)
> $\varphi:\mathbb Z\to\langle x\rangle,\ n\mapsto x^n$ est un morphisme surjectif. Ordre infini : $\mathrm{Ker}\,\varphi=\{0\}$, isomorphisme. Ordre $m$ : $\mathrm{Ker}\,\varphi=m\mathbb Z$ et le [[premier-theoreme-isomorphisme]] donne $\mathbb Z/m\mathbb Z\simeq\langle x\rangle$, $\bar n\mapsto x^n$.

> [!TIP] Conséquence (TD1 ex. 12–13)
> Si $G$ cyclique d'ordre $n$ : $\forall g\in G,\ g^n=1$ (additif : $ng=0$).

## 🔗 Liens

- **S'appuie sur** : [[ordre-element|Ordre d'un élément]], [[groupe-monogene-cyclique|Groupe monogène, groupe cyclique]]
- **Utilisé par (théorèmes)** : [[groupe-ordre-premier|Groupe d'ordre premier]]
