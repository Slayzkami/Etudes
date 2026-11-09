---
aliases:
  - "Mes erreurs à ne plus faire"
  - "pièges personnels"
  - "erreurs GAC"
tags:
  - gac
  - gac/revision
---

# 🚨 Mes erreurs à ne plus faire

Les erreurs que j'ai réellement faites en m'entraînant, avec la bonne version. À relire **juste avant le partiel**. · [[plan-de-revision|↩ Plan de révision]] · [[index-definitions|↩ Index]]

> [!WARNING] 1. Confondre $\operatorname{pgcd}$ et ordre dans $\mathbb Z/n\mathbb Z$
> ❌ « $o(\overline{12})=\operatorname{pgcd}(18,12)=6$ »
> ✅ $o(\bar k)=\dfrac{n}{\operatorname{pgcd}(n,k)}$ : $\operatorname{pgcd}(18,12)=6$, donc $o(\overline{12})=18/6=3$.
> **Contrôle** : l'ordre doit diviser $n$, et $o(\bar k)\cdot\bar k$ doit donner $\bar0$ ($3\cdot\overline{12}=\overline{36}=\bar0$ ✔).
> → [[ordre-dans-znz]], [[calculer-ordre]]

> [!WARNING] 2. Calculer les multiples avec l'ordre au lieu de l'élément
> ❌ « $2\cdot\overline{12}=2\times3=6$ »
> ✅ $2\cdot\overline{12}=\overline{12}+\overline{12}=\overline{24}=\bar6$. On multiplie **l'élément** $12$, puis on réduit modulo $18$.
> → [[calculer-dans-znz]]

> [!WARNING] 3. Ne pas réduire, ou s'arrêter trop tôt
> ❌ « $3\cdot\overline{12}=36$… 18 ? » ; ❌ « $\langle\bar6\rangle=\{\bar0,\bar6\}$ dans $\mathbb Z/18\mathbb Z$ »
> ✅ $\overline{36}=\bar0$ car $36=2\times18$. Pour $\langle\bar k\rangle$, on continue **jusqu'à retomber sur $\bar0$** :
> $\bar6,\ \overline{12},\ \overline{18}=\bar0$, donc $\langle\bar6\rangle=\{\bar0,\bar6,\overline{12}\}$.
> **Contrôle** : $\mathrm{Card}\,\langle\bar k\rangle=o(\bar k)$. Ici $o(\bar6)=18/6=3$ : il faut 3 éléments.
> → [[sous-groupe-engendre]], [[ordre-element]]

> [!WARNING] 4. Enchaîner des égalités fausses
> ❌ « $o(\overline{15})=18/\operatorname{pgcd}(18,15)=3=6$ »
> ✅ Une phrase par étape : « $\operatorname{pgcd}(18,15)=3$, donc $o(\overline{15})=18/3=6$. »
> Le signe $=$ veut dire « même objet » : $3=6$ est faux, et un correcteur enlève des points.

> [!WARNING] 5. Oublier les barres et le groupe
> ❌ « $8+4=12=0$ dans un groupe »
> ✅ « Dans $\mathbb Z/12\mathbb Z$ : $\bar8+\bar4=\overline{12}=\bar0$, donc l'opposé de $\bar8$ est $\bar4$. »

> [!WARNING] 6. Croire qu'« abélien » et « cyclique » veulent dire la même chose
> - **Abélien** : l'ordre des facteurs ne compte pas ($xy=yx$).
> - **Cyclique** : **un seul** élément fabrique tout le groupe ($G=\langle a\rangle$).
> - Cyclique ⟹ abélien, mais pas l'inverse : Klein $\mathbb Z/2\mathbb Z\times\mathbb Z/2\mathbb Z$ est abélien, et aucun élément ne l'engendre (tous vérifient $2x=0$).
> → [[groupe-abelien]], [[groupe-monogene-cyclique]]

> [!WARNING] 7. Répondre à un Vrai/Faux sans justification
> « Faux » seul = 0 point. **Faux ⟹ un contre-exemple précis et vérifié. Vrai ⟹ une preuve courte.**
> → [[vrai-faux-classiques]]

> [!TIP] Mes 5 réflexes de contrôle
> 1. Un ordre d'élément **divise** l'ordre du groupe ([[lagrange]]).
> 2. $\langle x\rangle$ a exactement $o(x)$ éléments et contient toujours le neutre.
> 3. Une application définie sur un quotient : **d'abord** vérifier qu'elle est bien définie ([[morphisme-sur-quotient]]).
> 4. Un sous-groupe contient toujours le neutre : si le neutre manque, ce n'est pas un sous-groupe.
> 5. Je relis chaque ligne : est-ce que chaque « $=$ » est vrai ?

## 🔗 Liens

- [[calculer-dans-znz]] · [[calculer-ordre]] · [[vrai-faux-classiques]] · [[exercices-types-corriges]]
