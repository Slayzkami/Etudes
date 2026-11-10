---
aliases:
  - "Différentielles de référence : constante, linéaire, bilinéaire"
  - "différentielle d'une application linéaire"
  - "différentielle d'une application bilinéaire"
  - "Exemples 2.15 2.16 2.17"
  - "briques de base"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-02
---

# ⭐ Différentielles de référence : constante, linéaire, bilinéaire

*Théorème* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Ex. 2.15, 2.16, 2.17 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Les trois briques
> 1. **Constante** (Ex. 2.15) : $f(x)=c$ est différentiable partout et $Df_a=0$.
> 2. **Linéaire continue** (Ex. 2.16) : si $\varphi\in\mathcal L_c(E,F)$, alors $\varphi$ est différentiable partout et $D\varphi_a=\varphi$ pour tout $a$, c'est-à-dire $D\varphi_a(h)=\varphi(h)$.
> 3. **Bilinéaire continue** (Ex. 2.17) : si $B:E_1\times E_2\to F$ est bilinéaire continue, alors $B$ est différentiable partout et
> $$DB_{(a_1,a_2)}(h_1,h_2)=B(h_1,a_2)+B(a_1,h_2).$$

> [!SUCCESS]- Démonstration
> 1. $f(a+h)-f(a)=0=0(h)+0$.
> 2. $\varphi(a+h)-\varphi(a)=\varphi(h)$ par linéarité : le reste est nul, et $\varphi$ est linéaire continue par hypothèse.
> 3. Par bilinéarité, $B(a_1+h_1,a_2+h_2)=B(a_1,a_2)+\underbrace{B(h_1,a_2)+B(a_1,h_2)}_{L(h)}+B(h_1,h_2)$.
> $L$ est linéaire, et continue car $\lVert L(h)\rVert\le C(\lVert a_2\rVert+\lVert a_1\rVert)\lVert h\rVert$. Le reste vérifie $\lVert B(h_1,h_2)\rVert\le C\lVert h_1\rVert\lVert h_2\rVert\le C\lVert h\rVert^2$ (norme produit), donc c'est un $o(h)$. $\blacksquare$

> [!EXAMPLE] Exemples
> - Projections, trace, $X\mapsto(X,X)$, $X\mapsto MX$ : linéaires $\Rightarrow$ $D\varphi_A(H)=\varphi(H)$.
> - Produit matriciel $p(X,Y)=XY$ : $Dp_{(A,B)}(H,K)=HB+AK$.

> [!WARNING] Pièges (mes erreurs)
> - Écrire « $L$ est linéaire, donc différentiable » : il manque **continue** (dimension finie, ou majoration).
> - Une application bilinéaire n'est pas linéaire : $DB_{(a_1,a_2)}\ne B$.

## 🔗 Liens

- **S'appuie sur** : [[differentiabilite|Différentiabilité en un point, différentielle]], [[application-bilineaire|Application bilinéaire (continue)]], [[caracterisation-bilineaires-continues|Caractérisation des applications bilinéaires continues]]
- **Utilisé par (théorèmes)** : [[differentielle-produit-bilineaire|Différentielle d'un « produit » B(f1, f2)]]
- **Méthodes** : [[differentiabilite-par-theoremes|Montrer la différentiabilité par les théorèmes généraux]], [[appliquer-regle-de-la-chaine|Appliquer la règle de la chaîne en 4 étapes]], [[differentielle-sur-les-matrices|Calculer une différentielle sur les matrices]]
