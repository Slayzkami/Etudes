---
aliases:
  - "Méthode : appliquer la règle de la chaîne en 4 étapes"
  - "composée en 4 étapes"
  - "calculer D(g∘f)"
tags:
  - cd
  - cd/methode
  - cd/chapitre-02
---

# 🛠️ Méthode : appliquer la règle de la chaîne en 4 étapes

*Méthode* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Méthode 2.1 du cours · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> 1. **Décomposer** : écrire $F=g\circ f$ en précisant les espaces ($f:E\to F$, $g:F\to G$).
> 2. **Différentier $f$** en $a$ : $Df_a(h)=\dots$ (justifier).
> 3. **Différentier $g$** au point $b=f(a)$ : $Dg_b(k)=\dots$ (justifier).
> 4. **Composer** : $DF_a(h)=Dg_{f(a)}\big(Df_a(h)\big)$ : on remplace $k$ par $Df_a(h)$.

> [!EXAMPLE] Rédaction modèle (Écrit 2024-2025, ex. 3)
> $g(X)=\exp(-\mathrm{tr}(X\,{}^t\!X))=\varphi\circ f$ avec $f(X)=\mathrm{tr}(X\,{}^t\!X)$ et $\varphi(s)=e^{-s}$.
> - $f$ est différentiable et $Df_A(H)=2\,\mathrm{tr}(A\,{}^t\!H)$ (question précédente).
> - $\varphi$ est dérivable sur $\mathbb R$, $D\varphi_s(k)=\varphi'(s)k=-e^{-s}k$.
> - Par le Th. 2.20 : $Dg_A(H)=\varphi'(f(A))\,Df_A(H)=-2\,e^{-\mathrm{tr}(A\,{}^t\!A)}\,\mathrm{tr}(A\,{}^t\!H)$.

> [!EXAMPLE] Avec le produit matriciel (Écrit 2025-2026, ex. 3)
> $f(X)=XMX=p\circ q$, $q(X)=(X,MX)$ linéaire : $Dq_A(H)=(H,MH)$ ; $p(X,Y)=XY$ bilinéaire : $Dp_{(A,B)}(H,K)=HB+AK$.
> $Df_A(H)=Dp_{(A,MA)}(H,MH)=HMA+AMH$.

> [!WARNING] Piège
> Étape 3 : le point est $f(a)$, pas $a$.

## 🔗 Liens

- **Voir aussi** : [[regle-de-la-chaine|Règle de la chaîne (différentielle d'une composée)]], [[differentielles-de-reference|Différentielles de référence : constante, linéaire, bilinéaire]]
