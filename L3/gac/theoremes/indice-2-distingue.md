---
aliases:
  - "Un sous-groupe d'indice 2 est distingué"
  - "indice 2"
tags:
  - gac
  - gac/theoreme
  - gac/chapitre-03
---

# ⭐ Un sous-groupe d'indice 2 est distingué

*Théorème* · Chapitre : [[03-groupes-quotients|III – Groupes quotients]] · § III.4 du cours · [[index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Si $H$ n'a que deux classes à gauche ($[G:H]=2$), alors $H\lhd G$.

> [!SUCCESS]- Démonstration
> Soient $x\in G$, $h\in H$. Si $x\in H$ : $x^{-1}hx\in H$. Sinon $x^{-1}\notin H$, donc $x^{-1}H\neq H$ et (deux classes, partition) $x^{-1}H=G\setminus H$. Si $x^{-1}hx\notin H$, alors $x^{-1}hx=x^{-1}h'$ avec $h'\in H$, d'où $x=h^{-1}h'\in H$ : absurde.
> (Autre version : pour $x\notin H$, $xH=G\setminus H=Hx$.)

> [!EXAMPLE] Exemples
> $\{e,\gamma,\gamma^2\}\lhd\mathfrak S_3$ ; $\mathfrak A_n\lhd\mathfrak S_n$ ; les sous-groupes d'ordre 4 de $D_4$.

> [!WARNING] Vrai/Faux
> « Tout sous-groupe d'**ordre** 2 est normal » : **FAUX** ($\{e,\tau_1\}\subset\mathfrak S_3$). « Tout sous-groupe d'**indice** 2 est distingué » : **VRAI**.

## 🔗 Liens

- **S'appuie sur** : [[indice|Indice d'un sous-groupe]], [[sous-groupe-distingue|Sous-groupe distingué]]
- **Méthodes** : [[vrai-faux-classiques|Vrai/Faux classiques (avec justification)]]
