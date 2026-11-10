---
aliases:
  - "Petit o"
  - "o(h)"
  - "négligeable"
  - "petit o de h"
tags:
  - cd
  - cd/definition
  - cd/chapitre-02
---

# 📘 Petit o

*Définition* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Déf. 2.1 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> Soit $W\subset E$ un voisinage de $0_E$ et $\delta:W\to F$. On écrit $\delta(h)=o(h)$ au voisinage de $0$ si
> $$\lim_{h\to0_E}\frac{\lVert \delta(h)\rVert_F}{\lVert h\rVert_E}=0.$$
> De façon équivalente : $\delta(h)=\lVert h\rVert\,\varepsilon(h)$ avec $\varepsilon(h)\to0$ quand $h\to0$.

> [!IMPORTANT] Règles de calcul (Lemme 2.2)
> - $o(h)+o(h)=o(h)$ ; $\lambda\,o(h)=o(h)$.
> - Si $\lVert \delta(h)\rVert\le C\lVert h\rVert^2$ pour $h$ petit, alors $\delta(h)=o(h)$.
> - Si $L$ est linéaire continue, $L(o(h))=o(h)$.
> - Dans un produit : $o(h)$ $\iff$ chaque composante est un $o(h)$.

> [!WARNING] Pièges
> - C'est un **petit** $o$ : le polycopié imprime parfois $O(h)$, il faut lire $o(h)$.
> - Un terme **linéaire** en $h$ (comme $2\langle a,h\rangle$ ou $AH+HA$) n'est jamais un $o(h)$ (sauf s'il est nul).

## 🔗 Liens

- **S'appuie sur** : [[norme|Norme, espace vectoriel normé]], [[voisinage|Voisinage]]
- **Utilisé par (définitions)** : [[differentiabilite|Différentiabilité en un point, différentielle]]
- **Utilisé par (théorèmes)** : [[taylor-young-ordre-2|Formule de Taylor-Young à l'ordre 2]]
- **Méthodes** : [[differentiabilite-par-definition|Montrer la différentiabilité par la définition]]
