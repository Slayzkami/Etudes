---
aliases:
  - "Vrai/Faux classiques (avec justification)"
  - "vrai faux"
  - "contre-exemples"
  - "QCM"
tags:
  - gac
  - gac/methode
  - gac/chapitre-03
---

# 🛠️ Vrai/Faux classiques (avec justification)

*Méthode* · Chapitre : [[03-groupes-quotients|III – Groupes quotients]] · [[index-definitions|↩ Index]]

> [!ABSTRACT] Règle
> **Vrai** ⟹ une preuve courte. **Faux** ⟹ **un** contre-exemple explicite et vérifié.

| Affirmation                                                   | Réponse  | Justification                                                                                                                                                                                                                            |
| ------------------------------------------------------------- | -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tout groupe abélien est cyclique                              | **Faux** | Klein $K=(\mathbb Z/2\mathbb Z)^2$ est abélien (calcul coordonnée par coordonnée) ; mais $2x=0$ pour tout $x\in K$, donc $o(x)\le2$ et $\langle x\rangle$ a au plus 2 éléments $\neq K$ (4 éléments) : non cyclique → [[groupe-abelien]] |
| Tout groupe cyclique est abélien                              | **Vrai** | $a^ka^l=a^{k+l}=a^la^k$ → [[groupe-monogene-cyclique]]                                                                                                                                                                                   |
| $(M_2(\mathbb R),\times)$ est un groupe                       | **Faux** | $\begin{pmatrix}0&0\\0&0\end{pmatrix}$ n'est pas inversible                                                                                                                                                                              |
| $(M_2(\mathbb R),+)$ est un groupe abélien                    | **Vrai** | addition coefficient par coefficient, neutre $0$, opposé $-M$                                                                                                                                                                            |
| Dans un groupe, tout élément est simplifiable                 | **Vrai** | multiplier par $c^{-1}$ → [[regles-de-calcul]]                                                                                                                                                                                           |
| L'équation $x^2=x$ a pour seule solution le neutre            | **Vrai** | $xx=x\cdot1$, simplifier par $x$                                                                                                                                                                                                         |
| Les éléments d'ordre 2 forment un sous-groupe                 | **Faux** | ne contient pas le neutre (ordre 1) ; et dans $\mathfrak S_3$, $\tau_1\tau_2=\gamma^2$ est d'ordre 3                                                                                                                                     |
| La réunion de deux sous-groupes est un sous-groupe            | **Faux** | $2\mathbb Z\cup3\mathbb Z\not\ni5$ → [[intersection-sous-groupes]]                                                                                                                                                                       |
| Tout sous-groupe d'ordre 2 est normal                         | **Faux** | $\{e,\tau_1\}\subset\mathfrak S_3$                                                                                                                                                                                                       |
| Tout sous-groupe d'indice 2 est distingué                     | **Vrai** | [[indice-2-distingue]]                                                                                                                                                                                                                   |
| Deux groupes de même ordre sont isomorphes                    | **Faux** | $\mathbb Z/4\mathbb Z\not\simeq$ Klein → [[montrer-non-isomorphes]]                                                                                                                                                                      |
| Un morphisme conserve l'ordre des éléments                    | **Faux** | morphisme trivial $\mathbb Z/2\mathbb Z\to\{0\}$ : $o(\bar1)=2$, $o(0)=1$ (vrai si $f$ injectif)                                                                                                                                         |
| Une partie non vide stable est un sous-groupe                 | **Faux** | $\mathbb N\subset\mathbb Z$ (vrai si $G$ fini)                                                                                                                                                                                           |
| Un groupe d'ordre 6 peut avoir un élément d'ordre 4           | **Faux** | [[lagrange]] : $4\nmid6$                                                                                                                                                                                                                 |
| $\mathbb Z/2\mathbb Z\times\mathbb Z/3\mathbb Z$ est cyclique | **Vrai** | $o(\bar1,\bar1)=\operatorname{ppcm}(2,3)=6$                                                                                                                                                                                              |
| $(xy)^{-1}=x^{-1}y^{-1}$                                      | **Faux** | dans $\mathfrak S_3$ ; c'est $y^{-1}x^{-1}$                                                                                                                                                                                              |

## 🔗 Liens

- **Utilisé par (définitions)** : [[ordre-element|Ordre d'un élément]]
- **Voir aussi** : [[regles-de-calcul|Règles de calcul dans un groupe]], [[lagrange|Théorème de Lagrange]]
