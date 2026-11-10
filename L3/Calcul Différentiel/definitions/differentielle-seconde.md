---
aliases:
  - "Différentielle seconde, classe C2"
  - "D²f_a"
  - "deux fois différentiable"
  - "C2"
  - "classe C^2"
  - "différentielle d'ordre 2"
tags:
  - cd
  - cd/definition
  - cd/chapitre-04
---

# 📘 Différentielle seconde, classe C2

*Définition* · Chapitre : [[04-differentielles-ordre-superieur|4 – Différentielles d'ordre supérieur]] · Déf. 4.1 et 4.4 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> $f:U\to F$ est **deux fois différentiable en** $a$ si $f$ est différentiable sur un voisinage de $a$ et si $Df$ est différentiable en $a$. On note
> $$D^2f_a:=D(Df)_a\in\mathcal L(E,\mathcal L(E,F))$$
> la **différentielle seconde** de $f$ en $a$. Si $f$ est deux fois différentiable sur $U$ et si $D^2f$ est continue sur $U$, $f$ est **de classe $\mathcal C^2$** sur $U$.

> [!IMPORTANT] Notation $D^2f_a(h,k)$ (Prop. 4.3, Déf. 4.4)
> On identifie $D^2f_a$ à une application **bilinéaire continue** de $E\times E$ dans $F$ en posant
> $$D^2f_a(h,k):=\big(D^2f_a(h)\big)(k).$$
> Elle est **symétrique** ([[theoreme-de-schwarz]]).

> [!EXAMPLE] Exemples (Ex. 4.2)
> - $f$ linéaire continue : $Df_x=f$ ne dépend pas de $x$, donc $D^2f=0$.
> - $f(X)=X^2$ sur $\mathcal M_n(\mathbb R)$ : $Df_X(H)=XH+HX$, donc $D^2f_A(H,K)=KH+HK$.

> [!TIP] En pratique sur $\mathbb R^n$
> $D^2f_a(h,k)={}^t\!h\,H_f(a)\,k$ → [[matrice-hessienne]], [[calculer-differentielle-seconde]].

## 🔗 Liens

- **S'appuie sur** : [[classe-c1|Application de classe C1]], [[application-bilineaire|Application bilinéaire (continue)]]
- **Utilisé par (définitions)** : [[matrice-hessienne|Matrice hessienne]], [[classe-cn|Différentiabilité d'ordre n, classes Cn et C∞]]
- **Utilisé par (théorèmes)** : [[theoreme-de-schwarz|Théorème de Schwarz]], [[expression-differentielle-seconde|Expression de la différentielle seconde]], [[critere-c2|Critère C2]], [[taylor-young-ordre-2|Formule de Taylor-Young à l'ordre 2]]
- **Méthodes** : [[calculer-differentielle-seconde|Calculer une différentielle seconde, une hessienne]]
