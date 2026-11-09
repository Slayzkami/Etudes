---
aliases:
  - "Méthode : calculer l'ordre d'un élément"
  - "trouver l'ordre"
tags:
  - gac
  - gac/methode
  - gac/chapitre-02
---

# 🛠️ Méthode : calculer l'ordre d'un élément

*Méthode* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · [[index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> - **Petit cas** : calculer $x,x^2,x^3,\dots$ jusqu'à $1$ (additif : $x,2x,3x,\dots$ jusqu'à $0$).
> - **Dans $\mathbb Z/n\mathbb Z$** : $o(\bar k)=n/\operatorname{pgcd}(n,k)$ → [[ordre-dans-znz]].
> - **Dans un produit** : $o(a,b)=\operatorname{ppcm}(o(a),o(b))$ ($m(a,b)=0\iff o(a)\mid m$ et $o(b)\mid m$).
> - **Si $x^N=1$** : $o(x)\mid N$ ; et $o(x)=N\iff x^N=1$ et $x^{N/p}\neq1$ pour tout premier $p\mid N$.
> - **Groupe fini** : $o(x)\mid[G]$ ([[lagrange]]).

> [!EXAMPLE] Rédaction modèle
> Dans $\mathbb Z/12\mathbb Z$, $o(\bar9)$ : $\operatorname{pgcd}(12,9)=3$ donc $o(\bar9)=4$. Vérif : $\bar9,\overline{18}=\bar6,\overline{27}=\bar3\neq\bar0$ et $4\cdot\bar9=\overline{36}=\bar0$.

## 🔗 Liens

- **Utilisé par (définitions)** : [[groupe-produit|Groupe produit]]
- **Voir aussi** : [[ordre-element|Ordre d'un élément]], [[ordre-dans-znz|Ordre d'un élément de Z/nZ]]
