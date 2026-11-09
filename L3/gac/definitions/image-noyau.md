---
aliases:
  - "Image, noyau, image réciproque"
  - "noyau"
  - "Ker"
  - "image"
  - "Im"
  - "image réciproque"
  - "image directe"
tags:
  - gac
  - gac/definition
  - gac/chapitre-02
---

# 📘 Image, noyau, image réciproque

*Définition* · Chapitre : [[02-sous-groupes|II – Sous-groupes]] · § II.5 du cours · [[index-definitions|↩ Index]]

> [!NOTE] Définitions
> Soit $f:G\to G'$ un [[morphisme-de-groupes|morphisme]].
> - **Image** : $\mathrm{Im} f=f(G)=\{f(x)\mid x\in G\}\subset G'$.
> - **Noyau** : $\mathrm{Ker} f=\{x\in G\mid f(x)=1_{G'}\}=f^{-1}(\{1_{G'}\})\subset G$.
> - **Image réciproque** de $H'\subset G'$ : $f^{-1}(H')=\{x\in G\mid f(x)\in H'\}$.

> [!IMPORTANT] Résultats
> - L'image (directe) d'un sous-groupe est un sous-groupe ; l'image réciproque d'un sous-groupe (distingué) est un sous-groupe (distingué).
> - $\mathrm{Ker} f\lhd G$, $\mathrm{Im} f$ sous-groupe de $G'$.
> - $f$ injectif $\iff\mathrm{Ker} f=\{1_G\}$ ; $f$ surjectif $\iff\mathrm{Im} f=G'$.
>
> Preuves → [[noyau-et-image]].

> [!TIP] En clair
> $f(x)=f(y)\iff x^{-1}y\in\mathrm{Ker} f$ : le noyau mesure ce que $f$ « oublie ».

## 🔗 Liens

- **S'appuie sur** : [[morphisme-de-groupes|Morphisme de groupes]], [[sous-groupe|Sous-groupe]]
- **Utilisé par (définitions)** : [[application-induite|Application induite et décomposition canonique]]
- **Utilisé par (théorèmes)** : [[noyau-et-image|Noyau distingué, image sous-groupe, injectivité]], [[premier-theoreme-isomorphisme|Premier théorème d'isomorphisme]]
- **Voir aussi** : [[identifier-quotient|Méthode : identifier un groupe quotient G/H]]
