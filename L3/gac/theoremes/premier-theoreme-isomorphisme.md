---
aliases:
  - "Premier théorème d'isomorphisme"
  - "théorème d'isomorphisme"
  - "G/Ker f ≃ Im f"
  - "factorisation"
tags:
  - gac
  - gac/theoreme
  - gac/chapitre-03
---

# ⭐ Premier théorème d'isomorphisme

*Théorème* · Chapitre : [[03-groupes-quotients|III – Groupes quotients]] · § III.6 du cours · [[index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> Pour tout morphisme $f:G_1\to G_2$ :
> $$G_1/\mathrm{Ker} f\ \simeq\ \mathrm{Im} f\qquad\text{via}\qquad \bar f:\bar x\mapsto f(x).$$
> Décomposition canonique : $f=i\circ\bar f\circ p$ → [[application-induite]].
> Si $G_1$ est fini : $[G_1]=[\mathrm{Ker} f]\cdot[\mathrm{Im} f]$.

> [!SUCCESS]- Démonstration (à savoir par cœur)
> **Lemme** : $\bar x=\bar y\iff x^{-1}y\in\mathrm{Ker} f\iff f(x^{-1}y)=1\iff f(x)^{-1}f(y)=1\iff f(x)=f(y)$.
> - bien définie : sens $\Rightarrow$ du lemme ;
> - injective : sens $\Leftarrow$ ;
> - surjective : tout élément de $\mathrm{Im} f$ est un $f(x)=\bar f(\bar x)$ ;
> - morphisme : $\bar f(\bar x\bar y)=\bar f(\overline{xy})=f(xy)=f(x)f(y)$.

> [!TIP] Utilisation
> C'est **l'outil** pour identifier un quotient → [[identifier-quotient]].

## 🔗 Liens

- **S'appuie sur** : [[image-noyau|Image, noyau, image réciproque]], [[groupe-quotient|Groupe quotient]], [[noyau-et-image|Noyau distingué, image sous-groupe, injectivité]]
- **Utilisé par (définitions)** : [[application-induite|Application induite et décomposition canonique]], [[automorphismes|Automorphismes et automorphismes intérieurs]]
- **Utilisé par (théorèmes)** : [[lemme-chinois|Lemme chinois (groupes)]], [[structure-groupes-monogenes|Structure des groupes monogènes]]
- **Méthodes** : [[morphisme-sur-quotient|Méthode : application définie sur un quotient (bien définie, morphisme)]], [[identifier-quotient|Méthode : identifier un groupe quotient G/H]]
