---
aliases:
  - "Sous-groupe distingué"
  - "distingué"
  - "normal"
  - "invariant"
  - "H ◁ G"
  - "sous-groupe normal"
tags:
  - gac
  - gac/definition
  - gac/chapitre-02
---

# 📘 Sous-groupe distingué

*Définition* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · § II.2-bis et III.4 du cours · [[index-definitions|↩ Index]]

> [!NOTE] Définition
> Un [[sous-groupe]] $H$ de $G$ est **distingué** (normal, invariant), noté $H\lhd G$, si
> $$\forall g\in G,\ \forall h\in H,\qquad g^{-1}hg\in H.$$

> [!IMPORTANT] Formulations équivalentes
> $H\lhd G \iff \forall g\in G,\ \forall h\in H,\ ghg^{-1}\in H \iff \forall g\in G,\ g^{-1}Hg=H \iff \forall g\in G,\ gH=Hg$.
> Il suffit de montrer l'**inclusion** $g^{-1}Hg\subset H$ pour tout $g$.

> [!TIP] En clair
> La conjugaison ne fait jamais sortir de $H$. C'est la condition pour que $G/H$ soit un groupe → [[groupe-quotient]].

> [!EXAMPLE] Toujours distingués
> - tout sous-groupe d'un groupe [[groupe-abelien|abélien]] ;
> - le [[centre]] $Z(G)$ ;
> - le noyau d'un morphisme → [[noyau-et-image]] ;
> - tout sous-groupe d'indice 2 → [[indice-2-distingue]].

> [!EXAMPLE] Contre-exemples
> - $H=\{e,\tau_1\}$ dans $\mathfrak S_3$ : $\tau_2\tau_1\tau_2^{-1}=\tau_3\notin H$.
> - Les matrices triangulaires supérieures dans $GL_2(\mathbb R)$ (TD1 ex. 9).
> - Les $\{r_0,s_i\}$ dans $D_4$.

## 🔗 Liens

- **S'appuie sur** : [[sous-groupe|Sous-groupe]]
- **Utilisé par (définitions)** : [[centre|Centre d'un groupe]], [[congruence-modulo-sous-groupe|Congruence modulo un sous-groupe]], [[groupe-quotient|Groupe quotient]]
- **Utilisé par (théorèmes)** : [[noyau-et-image|Noyau distingué, image sous-groupe, injectivité]], [[relations-compatibles-groupe|Relations compatibles avec la loi d'un groupe]], [[indice-2-distingue|Un sous-groupe d'indice 2 est distingué]]
- **Voir aussi** : [[montrer-distingue|Méthode : montrer qu'un sous-groupe est (ou n'est pas) distingué]]
