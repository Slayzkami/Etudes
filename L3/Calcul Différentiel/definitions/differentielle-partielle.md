---
aliases:
  - "Différentielle partielle"
  - "différentielles partielles"
  - "∂_j f(a)"
  - "D_j f(a)"
tags:
  - cd
  - cd/definition
  - cd/chapitre-02
---

# 📘 Différentielle partielle

*Définition* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Déf. 2.27 du cours · [[cd-index-definitions|↩ Index]]

Cadre : $E=E_1\times\dots\times E_n$ (norme produit), $U\subset E$ ouvert, $f:U\to F$, $a=(a_1,\dots,a_n)\in U$.

> [!NOTE] Définition
> La $j$-ème **application partielle** en $a$ est $\varphi_j:x_j\mapsto f(a_1,\dots,a_{j-1},x_j,a_{j+1},\dots,a_n)$. Si $\varphi_j$ est différentiable en $a_j$, sa différentielle $D(\varphi_j)_{a_j}\in\mathcal L_c(E_j,F)$ est la $j$-ème **différentielle partielle** de $f$ en $a$, notée $\partial_jf(a)$ ou $D_jf(a)$.

> [!IMPORTANT] Lien avec $Df_a$ (Prop. 2.29)
> Si $f$ est différentiable en $a$, toutes les $\partial_jf(a)$ existent et
> $$Df_a(h_1,\dots,h_n)=\sum_{j=1}^n\partial_jf(a)(h_j).$$
> → [[differentielle-et-differentielles-partielles]]

> [!TIP] Quand $E_j=\mathbb R$
> $\partial_jf(a)(h_j)=h_j\,\dfrac{\partial f}{\partial x_j}(a)$ : on retrouve la [[derivee-partielle]].

## 🔗 Liens

- **S'appuie sur** : [[differentiabilite|Différentiabilité en un point, différentielle]], [[norme-produit|Norme produit]]
- **Utilisé par (théorèmes)** : [[differentielle-et-differentielles-partielles|Différentielle et différentielles partielles]], [[critere-c1|Critère C1 par les dérivées partielles]], [[fonctions-implicites|Théorème des fonctions implicites (cas général)]]
