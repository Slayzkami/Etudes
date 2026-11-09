---
aliases:
  - "Groupe monogène, groupe cyclique"
  - "monogène"
  - "cyclique"
  - "partie génératrice"
  - "générateur"
  - "engendre"
tags:
  - gac
  - gac/definition
  - gac/chapitre-02
---

# 📘 Groupe monogène, groupe cyclique

*Définition* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · § II.4 et II.7 du cours · [[index-definitions|↩ Index]]

> [!NOTE] Définitions
> - $A$ **engendre** $G$ (partie génératrice) si $\mathrm{Gr}\langle A\rangle=G$.
> - $G$ est **monogène** s'il existe $a\in G$ tel que $G=\langle a\rangle$.
> - $G$ est **cyclique** s'il est monogène **et fini**.

> [!IMPORTANT] Structure
> Monogène infini $\simeq(\mathbb Z,+)$ ; cyclique d'ordre $n$ $\simeq(\mathbb Z/n\mathbb Z,+)$ et $G=\{1,a,\dots,a^{n-1}\}$ → [[structure-groupes-monogenes]].
> Un groupe monogène est **abélien**. Si $G=\langle a\rangle$ est cyclique d'ordre $n$, $\forall g\in G,\ g^n=1$.

> [!EXAMPLE] Exemples
> - Cycliques : $\mathbb Z/n\mathbb Z=\langle\bar1\rangle$, $\mathbb U_n=\langle e^{2i\pi/n}\rangle$, $\mathbb Z/2\mathbb Z\times\mathbb Z/3\mathbb Z$ (engendré par $(\bar1,\bar1)$).
> - Non cycliques : Klein, $\mathbb Z/2\mathbb Z\times\mathbb Z/4\mathbb Z$, $\mathfrak S_3$ (non abélien), $(\mathbb Q,+)$ non monogène.
> - Générateurs de $\mathbb Z/n\mathbb Z$ : les $\bar k$ avec $\operatorname{pgcd}(n,k)=1$.

> [!TIP] Méthode
> $G$ fini est cyclique $\iff$ il contient un élément d'ordre $\mathrm{Card}\,G$.

## 🔗 Liens

- **S'appuie sur** : [[sous-groupe-engendre|Sous-groupe engendré par une partie]], [[ordre-element|Ordre d'un élément]]
- **Utilisé par (définitions)** : [[groupe-abelien|Groupe abélien]]
- **Utilisé par (théorèmes)** : [[structure-groupes-monogenes|Structure des groupes monogènes]]
- **Méthodes** : [[vrai-faux-classiques|Vrai/Faux classiques (avec justification)]]
- **Voir aussi** : [[ordre-dans-znz|Ordre d'un élément de Z/nZ]], [[groupe-ordre-premier|Groupe d'ordre premier]]
