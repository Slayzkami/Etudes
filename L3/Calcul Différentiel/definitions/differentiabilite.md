---
aliases:
  - "Différentiabilité en un point, différentielle"
  - "différentiable"
  - "différentielle"
  - "Df_a"
  - "Df(a)"
  - "différentiable en a"
tags:
  - cd
  - cd/definition
  - cd/chapitre-02
---

# 📘 Différentiabilité en un point, différentielle

*Définition* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Déf. 2.3 du cours · [[cd-index-definitions|↩ Index]]

Cadre : $E,F$ e.v.n., $U\subset E$ **ouvert**, $f:U\to F$, $a\in U$.

> [!NOTE] Définition
> $f$ est **différentiable en** $a$ s'il existe une application **linéaire continue** $L\in\mathcal L_c(E,F)$ et une application $\varepsilon:U\to F$ telles que
> - $\forall x\in U,\quad f(x)=f(a)+L(x-a)+\lVert x-a\rVert\,\varepsilon(x)$ ;
> - $\displaystyle\lim_{x\to a}\varepsilon(x)=0$.

> [!IMPORTANT] Formes équivalentes (Prop. 2.4) et unicité (Prop. 2.5)
> $f$ est différentiable en $a$ $\iff$ il existe $L\in\mathcal L_c(E,F)$ telle que
> $$\lim_{h\to0}\frac{\lVert f(a+h)-f(a)-L(h)\rVert_F}{\lVert h\rVert_E}=0,\quad\text{c'est-à-dire}\quad f(a+h)=f(a)+L(h)+o(h).$$
> $L$ est alors **unique** : c'est la **différentielle** de $f$ en $a$, notée $Df_a$ (ou $Df(a)$, $df_a$). On écrit $Df_a(h)$ pour l'image de $h$.

> [!TIP] En clair
> Près de $a$, $f$ ressemble à une application affine : $f(a+h)\approx f(a)+Df_a(h)$, et l'erreur est négligeable devant $\lVert h\rVert$.

> [!EXAMPLE] Exemple (Ex. 2.7)
> $f(X)=X^2$ sur $\mathcal M_n(\mathbb R)$ : $f(A+H)=A^2+\underbrace{AH+HA}_{\text{linéaire en }H}+\underbrace{H^2}_{o(H)}$, donc $Df_A(H)=AH+HA$.

> [!WARNING] Pièges
> - $Df_a$ est une **application linéaire**, pas un nombre : $Df_a(h)$ est un vecteur de $F$.
> - Il faut dire que $L$ est linéaire **et continue**.
> - L'existence des dérivées partielles ne suffit **pas** → [[montrer-non-differentiable]].
> - $Df_a(h)$ est linéaire en $h$, mais pas en $a$ en général.

## 🔗 Liens

- **S'appuie sur** : [[application-lineaire-continue|Application linéaire continue, espace Lc(E,F)]], [[petit-o|Petit o]], [[ouvert-ferme|Ouvert, fermé]]
- **Utilisé par (définitions)** : [[derivee-directionnelle|Dérivée directionnelle]], [[classe-c1|Application de classe C1]], [[differentielle-partielle|Différentielle partielle]], [[matrice-jacobienne|Matrice jacobienne]], [[point-critique|Point critique]]
- **Utilisé par (théorèmes)** : [[differentielle-et-derivees-directionnelles|Différentielle et dérivées directionnelles]], [[differentielles-de-reference|Différentielles de référence : constante, linéaire, bilinéaire]], [[differentiable-implique-continue|Différentiable implique continue]], [[linearite-differentielle|Linéarité de la différentielle]], [[regle-de-la-chaine|Règle de la chaîne (différentielle d'une composée)]], [[differentiabilite-par-composantes|Différentiabilité par composantes]], [[taf|Théorème des accroissements finis (TAF)]], [[iaf|Inégalité des accroissements finis (IAF)]]
- **Méthodes** : [[differentiabilite-par-definition|Montrer la différentiabilité par la définition]], [[montrer-non-differentiable|Montrer qu'une application n'est pas différentiable en a]], [[etudier-en-un-point-particulier|Étudier une fonction en un point particulier (souvent (0,0))]]
