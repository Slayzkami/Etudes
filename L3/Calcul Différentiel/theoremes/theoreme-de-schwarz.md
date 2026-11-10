---
aliases:
  - "Théorème de Schwarz"
  - "Schwarz"
  - "symétrie de la différentielle seconde"
  - "dérivées croisées égales"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-04
---

# ⭐ Théorème de Schwarz

*Théorème* · Chapitre : [[04-differentielles-ordre-superieur|4 – Différentielles d'ordre supérieur]] · Th. 4.6 et 4.10 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème (admis)
> Si $f:U\to F$ est deux fois différentiable en $a\in U$, alors $D^2f_a$ est **symétrique** :
> $$\forall(h,k)\in E\times E,\qquad D^2f_a(h,k)=D^2f_a(k,h).$$
> Sur $\mathbb R^n$ (Th. 4.10) : $\partial^2_{ij}f(a)=D^2f_a(e_i,e_j)$, donc
> $$\frac{\partial^2f}{\partial x_i\partial x_j}(a)=\frac{\partial^2f}{\partial x_j\partial x_i}(a).$$

> [!TIP] Usage
> - La [[matrice-hessienne]] est symétrique : on ne calcule qu'une dérivée croisée.
> - Vérification de calcul : si $\partial^2_{xy}f\ne\partial^2_{yx}f$ pour une fonction $\mathcal C^2$, il y a une erreur.

> [!WARNING] Piège (Ex. 4.7)
> L'hypothèse « deux fois différentiable en $a$ » est indispensable : $f(x,y)=xy\frac{x^2-y^2}{x^2+y^2}$, $f(0,0)=0$, a des dérivées croisées différentes en $(0,0)$ ($-1$ et $1$).

## 🔗 Liens

- **S'appuie sur** : [[differentielle-seconde|Différentielle seconde, classe C2]], [[derivees-partielles-ordre-2|Dérivées partielles d'ordre 2]]
- **Méthodes** : [[calculer-differentielle-seconde|Calculer une différentielle seconde, une hessienne]]
