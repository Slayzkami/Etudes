---
aliases:
  - "Dérivées partielles d'ordre 2"
  - "dérivées secondes"
  - "∂²f/∂x_i∂x_j"
  - "∂²_ij f"
tags:
  - cd
  - cd/definition
  - cd/chapitre-04
---

# 📘 Dérivées partielles d'ordre 2

*Définition* · Chapitre : [[04-differentielles-ordre-superieur|4 – Différentielles d'ordre supérieur]] · Déf. 4.8 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> On note $\partial^2_{ij}f(a)$, ou $\dfrac{\partial^2f}{\partial x_i\partial x_j}(a)$, la dérivée partielle par rapport à $x_i$, en $a$, de la fonction $x\mapsto\partial_jf(x)$ :
> $$\partial^2_{ij}f(a)=\partial_i(\partial_jf)(a)$$
> (on dérive d'abord par rapport à $x_j$, puis par rapport à $x_i$).

> [!IMPORTANT] Symétrie
> Si $f$ est deux fois différentiable en $a$ : $\partial^2_{ij}f(a)=\partial^2_{ji}f(a)=D^2f_a(e_i,e_j)$ (Th. 4.10) → [[theoreme-de-schwarz]].

> [!WARNING] Piège
> Sans la différentiabilité seconde, la symétrie peut tomber (Ex. 4.7).

## 🔗 Liens

- **S'appuie sur** : [[derivee-partielle|Dérivée partielle]]
- **Utilisé par (définitions)** : [[matrice-hessienne|Matrice hessienne]]
- **Utilisé par (théorèmes)** : [[theoreme-de-schwarz|Théorème de Schwarz]], [[critere-c2|Critère C2]]
