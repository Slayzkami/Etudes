---
aliases:
  - "Groupe quotient"
  - "groupe quotient"
  - "G/H"
  - "projection canonique p"
tags:
  - gac
  - gac/definition
  - gac/chapitre-03
---

# 📘 Groupe quotient

*Définition* · Chapitre : [[03-groupes-quotients|III – Groupes quotients]] · § III.2 et III.5 du cours · [[index-definitions|↩ Index]]

> [!NOTE] Définition (cas général)
> Si $H\lhd G$, l'ensemble $G/H$ des classes $\bar x=xH=Hx$, muni de
> $$\bar x\,\dot\times\,\bar y=\overline{xy}\quad\text{c.-à-d.}\quad (xH)(yH)=(xy)H,$$
> est un groupe, le **groupe quotient** : neutre $\bar1=H$, inverse de $\bar x$ : $\overline{x^{-1}}$.
> La projection $p:G\to G/H,\ x\mapsto\bar x$ est un morphisme surjectif de noyau $H$. Si $G$ est fini, $[G/H]=[G:H]$.

> [!NOTE] Cas abélien (notation additive)
> $H$ sous-groupe de $(G,+)$ abélien : $\bar x\,\dot+\,\bar y=\overline{x+y}$ ; $G/H$ est un groupe abélien.

> [!TIP] En clair
> On calcule avec des représentants puis on prend la classe ; la [[relation-compatible|compatibilité]] (donc $H$ **distingué**) garantit que le résultat ne dépend pas des choix.

> [!EXAMPLE] Exemples
> $\mathbb Z/n\mathbb Z$ ; $\mathbb R/2\pi\mathbb Z$ (angles) ; $\mathbb R/\mathbb Z\simeq\mathbb U$ ; $\mathbb R^*/\{\pm1\}\simeq\mathbb R_+^*$ ; $\mathfrak S_3/\{e,\gamma,\gamma^2\}\simeq\mathbb Z/2\mathbb Z$.

> [!WARNING] Piège
> $H$ non distingué ⟹ pas de groupe $G/H$ (ex. $H=\{e,\tau_1\}\subset\mathfrak S_3$).

## 🔗 Liens

- **S'appuie sur** : [[sous-groupe-distingue|Sous-groupe distingué]], [[congruence-modulo-sous-groupe|Congruence modulo un sous-groupe]], [[loi-quotient|Loi quotient]]
- **Utilisé par (définitions)** : [[application-induite|Application induite et décomposition canonique]]
- **Utilisé par (théorèmes)** : [[premier-theoreme-isomorphisme|Premier théorème d'isomorphisme]]
- **Voir aussi** : [[identifier-quotient|Méthode : identifier un groupe quotient G/H]]
