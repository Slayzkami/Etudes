---
aliases:
  - "Méthode : montrer qu'un sous-groupe est (ou n'est pas) distingué"
  - "prouver distingué"
  - "normal ou pas"
tags:
  - gac
  - gac/methode
  - gac/chapitre-02
---

# 🛠️ Méthode : montrer qu'un sous-groupe est (ou n'est pas) distingué

*Méthode* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · [[index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> - **Direct** : soient $g\in G$, $h\in H$ ; montrer $g^{-1}hg\in H$ (ou $ghg^{-1}\in H$).
> - **Cas favorables** : $G$ abélien ; $H=Z(G)$ ; $H=\mathrm{Ker} f$ ; $[G:H]=2$ ; intersection de distingués.
> - **Pour réfuter** : exhiber $g$, $h$ avec $g^{-1}hg\notin H$, ou $gH\neq Hg$.

> [!EXAMPLE] Contre-exemple rédigé (TD1 ex. 9)
> $h=\begin{pmatrix}1&1\\0&1\end{pmatrix}\in K$, $g=\begin{pmatrix}0&1\\1&0\end{pmatrix}=g^{-1}$ : $g^{-1}hg=\begin{pmatrix}1&0\\1&1\end{pmatrix}\notin K$.

## 🔗 Liens

- **Voir aussi** : [[sous-groupe-distingue|Sous-groupe distingué]], [[indice-2-distingue|Un sous-groupe d'indice 2 est distingué]], [[noyau-et-image|Noyau distingué, image sous-groupe, injectivité]]
