---
aliases:
  - "Exemples de groupes"
  - "catalogue de groupes"
tags:
  - gac
  - gac/exemples
---

# 🧩 Exemples de groupes

Les groupes qui reviennent partout (cours, TD, sujets). Pour chacun : ordre, abélien ?, cyclique ?, sous-groupes utiles. · [[index-definitions|↩ Index]]

| Groupe | Ordre | Abélien | Cyclique | À retenir |
|---|---|---|---|---|
| $(\mathbb Z,+)$ | infini | oui | monogène ($\langle1\rangle$) | sous-groupes $a\mathbb Z$ → [[sous-groupes-de-z]] |
| $(\mathbb Q,+)$, $(\mathbb R,+)$, $(\mathbb C,+)$ | infini | oui | non | $\mathbb Z\le\mathbb Q\le\mathbb R\le\mathbb C$ |
| $(\mathbb Q^*,\times)$, $(\mathbb R^*,\times)$, $(\mathbb C^*,\times)$, $(\mathbb R_+^*,\times)$ | infini | oui | non | $(\mathbb R,+)\simeq(\mathbb R_+^*,\times)$ par $\exp$ |
| $(\mathbb U,\times)$ | infini | oui | non | $\mathbb U\simeq\mathbb R/\mathbb Z$ → [[identifier-quotient]] |
| $(\mathbb U_n,\times)$ | $n$ | oui | oui | $\mathbb U_n=\langle e^{2i\pi/n}\rangle\simeq\mathbb Z/n\mathbb Z$ |
| $(\mathbb Z/n\mathbb Z,+)$ | $n$ | oui | oui | $o(\bar k)=n/\operatorname{pgcd}(n,k)$ → [[ordre-dans-znz]], [[lister-sous-groupes-znz]] |
| Klein $\mathbb Z/2\mathbb Z\times\mathbb Z/2\mathbb Z$ | 4 | oui | **non** | $x+x=0$ ; $\not\simeq\mathbb Z/4\mathbb Z$ → [[groupe-produit]] |
| $\mathbb Z/2\mathbb Z\times\mathbb Z/4\mathbb Z$ | 8 | oui | **non** | ordres 1, 2, 4 seulement (TD1 ex. 11) |
| $\mathbb Z/2\mathbb Z\times\mathbb Z/3\mathbb Z$ | 6 | oui | **oui** | $\simeq\mathbb Z/6\mathbb Z$ → [[lemme-chinois]] |
| $\mathfrak S_3\simeq D_3$ | 6 | **non** | non | $Z=\{e\}$ ; 6 sous-groupes ; $\{e,\gamma,\gamma^2\}\lhd$, $\{e,\tau_i\}$ non → [[groupe-des-permutations]] |
| $D_4$ (isométries du carré) | 8 | **non** | non | $Z(D_4)=\{r_0,r_2\}$ ; 10 sous-groupes (TD1 ex. 16) |
| $GL_n(\mathbb R)$ | infini | non ($n\ge2$) | non | $SL_n(\mathbb R)=\mathrm{Ker}\det\lhd$ ; triangulaires sup. non distingué |
| $(M_2(\mathbb R),+)$ | infini | oui | non | mais $(M_2(\mathbb R),\times)$ **n'est pas** un groupe |
| $\mathcal S(E)$ | $n!$ si $\mathrm{Card}\,E=n$ | non si $\mathrm{Card}\,E\ge3$ | — | [[groupe-des-permutations]] |
| $(\mathbb R\setminus\{-1\},\ a+b+ab)$ | infini | oui | non | $\simeq(\mathbb R^*,\times)$ via $a\mapsto1+a$ → [[montrer-groupe]] |

> [!WARNING] Contre-exemples de « groupes »
> $(\mathbb N,+)$, $(\mathbb Z,\times)$, $(\mathbb R,\times)$, $(M_2(\mathbb R),\times)$ ne sont **pas** des groupes.

## 🔗 Liens
- [[groupe]], [[groupe-abelien]], [[groupe-monogene-cyclique]], [[sous-groupe-distingue]], [[vrai-faux-classiques]]
