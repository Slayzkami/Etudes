---
aliases:
  - "Dérivée partielle"
  - "dérivées partielles"
  - "∂f/∂x_j"
  - "dérivée partielle première"
tags:
  - cd
  - cd/definition
  - cd/chapitre-02
---

# 📘 Dérivée partielle

*Définition* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Déf. 2.30 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> Soit $f:U\subset\mathbb R^n\to F$ et $a\in U$. La **dérivée partielle** de $f$ en $a$ par rapport à sa $j$-ème variable est, quand la limite existe,
> $$\frac{\partial f}{\partial x_j}(a)=\lim_{t\to0}\frac{f(a+te_j)-f(a)}{t}\ \in F,$$
> où $(e_1,\dots,e_n)$ est la base canonique. C'est la dérivée de $f$ en $a$ dans la direction $e_j$ (Rem. 2.31).

> [!IMPORTANT] Si $f$ est différentiable en $a$ (Cor. 2.32)
> $$\forall h\in\mathbb R^n,\qquad Df_a(h)=h_1\frac{\partial f}{\partial x_1}(a)+\dots+h_n\frac{\partial f}{\partial x_n}(a).$$

> [!WARNING] Pièges (mes erreurs)
> - En un point où $f$ est définie « à part » (typiquement $(0,0)$), on calcule la dérivée partielle **avec la limite** $\frac{f(t,0)-f(0,0)}{t}$, **jamais** en dérivant la formule valable ailleurs → [[etudier-en-un-point-particulier]].
> - Existence des dérivées partielles $\not\Rightarrow$ différentiable, ni même continue.

## 🔗 Liens

- **S'appuie sur** : [[derivee-directionnelle|Dérivée directionnelle]]
- **Utilisé par (définitions)** : [[matrice-jacobienne|Matrice jacobienne]], [[derivees-partielles-ordre-2|Dérivées partielles d'ordre 2]]
- **Utilisé par (théorèmes)** : [[differentielle-et-differentielles-partielles|Différentielle et différentielles partielles]], [[critere-c1|Critère C1 par les dérivées partielles]], [[fonctions-implicites-une-variable|Théorème des fonctions implicites (une variable)]]
- **Méthodes** : [[etudier-en-un-point-particulier|Étudier une fonction en un point particulier (souvent (0,0))]]
