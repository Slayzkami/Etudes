---
aliases:
  - "Groupe"
  - "groupe"
  - "(G1)"
  - "(G2)"
  - "(G3)"
  - "élément neutre"
  - "symétrique"
  - "inverse"
  - "opposé"
tags:
  - gac
  - gac/definition
  - gac/chapitre-01
---

# 📘 Groupe

*Définition* · Chapitre : [[01-definitions-generales|I – Définitions générales]] · § I.1 (Déf. 1) du cours · [[index-definitions|↩ Index]]

> [!NOTE] Définition (Déf. 1)
> Soit $G$ un ensemble **non vide** muni d'une [[loi-composition-interne|l.c.i.]] $\star$. $(G,\star)$ est un **groupe** si :
> - **(G1)** associativité : $\forall x,y,z\in G,\ x\star(y\star z)=(x\star y)\star z$ ;
> - **(G2)** élément neutre : $\exists e\in G,\ \forall x\in G,\ x\star e=x=e\star x$ ;
> - **(G3)** symétrique : $\forall x\in G,\ \exists x'\in G,\ x\star x'=e=x'\star x$.

> [!TIP] En clair
> On peut composer, les parenthèses n'importent pas, un élément « ne fait rien », et toute opération s'annule.
> Le neutre et le symétrique sont **uniques** → [[unicite-neutre-symetrique]].

> [!NOTE] Notations
> - multiplicative : loi $xy$, neutre $1$, symétrique $x^{-1}$ (**inverse**) ;
> - additive (réservée aux groupes abéliens) : loi $x+y$, neutre $0$, symétrique $-x$ (**opposé**).

> [!EXAMPLE] Exemples et contre-exemples
> Voir [[exemples-de-groupes]]. Contre-exemples : $(\mathbb N,+)$, $(\mathbb Z,\times)$, $(\mathbb R,\times)$.

> [!WARNING] Piège
> Dans un groupe non abélien, $x\star y\neq y\star x$ en général : (G2) et (G3) exigent l'égalité **des deux côtés**.

## 🔗 Liens

- **S'appuie sur** : [[loi-composition-interne|Loi de composition interne]]
- **Utilisé par (définitions)** : [[groupe-abelien|Groupe abélien]], [[groupe-des-permutations|Groupe des permutations]], [[groupe-produit|Groupe produit]], [[morphisme-de-groupes|Morphisme de groupes]], [[puissances-multiples|Puissances et multiples]], [[sous-groupe|Sous-groupe]]
- **Utilisé par (théorèmes)** : [[regles-de-calcul|Règles de calcul dans un groupe]], [[unicite-neutre-symetrique|Unicité du neutre et du symétrique]]
- **Voir aussi** : [[montrer-groupe|Méthode : montrer qu'un ensemble muni d'une loi est un groupe]]
