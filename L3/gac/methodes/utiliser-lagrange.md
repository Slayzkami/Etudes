---
aliases:
  - "Méthode : utiliser le théorème de Lagrange"
  - "utiliser Lagrange"
  - "ordres possibles"
  - "sous-groupes possibles"
tags:
  - gac
  - gac/methode
  - gac/chapitre-03
---

# 🛠️ Méthode : utiliser le théorème de Lagrange

*Méthode* · Chapitre : [[03-groupes-quotients|III – Groupes quotients]] · [[index-definitions|↩ Index]]

> [!ABSTRACT] Recette : dès que le groupe est **fini**, penser « divise »
> - **Ordres possibles d'un élément** : les diviseurs de $[G]$.
> - **Ordres possibles d'un sous-groupe** : les diviseurs de $[G]$.
> - **$x^{[G]}=e$** pour tout $x$.
> - **$H\cap K$** : son ordre divise $[H]$ **et** $[K]$ ; si $\operatorname{pgcd}([H],[K])=1$, alors $H\cap K=\{e\}$.
> - **Nombre de classes** : $[G:H]=[G]/[H]$ → [[classes-et-indice]].
> - **$[G]$ premier** : seuls sous-groupes $\{e\}$ et $G$, et $G$ est cyclique → [[groupe-ordre-premier]].

> [!EXAMPLE] Rédactions modèles
> - « Un groupe d'ordre 15 a-t-il un élément d'ordre 4 ? » Non : d'après Lagrange $o(x)\mid15$, et $4\nmid15$.
> - « $H,K\le G$ avec $[H]=4$, $[K]=9$. » $H\cap K$ est un sous-groupe de $H$ et de $K$, donc son ordre divise $4$ et $9$ : il vaut $1$, $H\cap K=\{e\}$.
> - « Sous-groupes de $\mathfrak S_3$ » : ordres possibles $1,2,3,6$. Ordre 2 ou 3 = premier, donc cyclique : $\{e,\tau_i\}$ (3 sous-groupes) et $\{e,\gamma,\gamma^2\}$. Total : 6 sous-groupes.

> [!WARNING] Pièges
> - Lagrange dit « si $H$ est un sous-groupe, alors $[H]\mid[G]$ ». Il **ne dit pas** qu'il existe un sous-groupe (ou un élément) pour chaque diviseur. (C'est vrai dans $\mathbb Z/n\mathbb Z$, mais par [[lister-sous-groupes-znz|un autre résultat]].)
> - Il faut un groupe **fini**.

## 🔗 Liens

- **S'appuie sur** : [[lagrange|Théorème de Lagrange]], [[ordre-groupe|Ordre d'un groupe]], [[indice|Indice]]
- **Voir aussi** : [[calculer-ordre]], [[vrai-faux-classiques]]
- **Corrigés** : [[exercices-types-corriges#2. Réunion de deux sous-groupes|ex. 2]], [[exercices-types-corriges#9. Groupe d'ordre premier|ex. 9]], [[exercices-types-corriges#14. Sous-groupes de S3|ex. 14]]
