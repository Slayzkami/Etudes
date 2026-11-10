---
aliases:
  - "Continuité et composantes"
  - "continuité composante par composante"
  - "applications partielles continues"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-01
---

# ⭐ Continuité et composantes

*Théorème* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Th. 1.40 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> Soit $f=(f_1,\dots,f_p):E\to F=F_1\times\dots\times F_p$ (norme produit). $f$ est continue (resp. uniformément continue) si et seulement si toutes ses composantes $f_i=\pi_i\circ f$ le sont.

> [!SUCCESS]- Démonstration
> ($\Rightarrow$) $f_i=\pi_i\circ f$ et $\pi_i$ est $1$-lipschitzienne (Prop. 1.39), donc continue ; une composée de continues est continue.
> ($\Leftarrow$) $\lVert f(x)-f(a)\rVert_F=\max_i\lVert f_i(x)-f_i(a)\rVert$ ; chaque terme tend vers $0$ quand $x\to a$, et il y en a un nombre fini. $\blacksquare$

> [!WARNING] Piège (Prop. 1.41, Ex. 1.42)
> Pour une fonction **de plusieurs variables** : continue $\Rightarrow$ applications partielles continues, mais la réciproque est **fausse** ($\frac{xy}{x^2+y^2}$ en $(0,0)$). Ne pas confondre *composantes* (à l'arrivée) et *applications partielles* (au départ).

## 🔗 Liens

- **S'appuie sur** : [[continuite|Continuité en un point]], [[norme-produit|Norme produit]]
- **Méthodes** : [[montrer-continue|Montrer qu'une application est (ou n'est pas) continue]]
