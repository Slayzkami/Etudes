---
aliases:
  - "Différentielle d'un « produit » B(f1, f2)"
  - "Proposition 2.34"
  - "différentielle d'un produit"
  - "règle de Leibniz"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-02
---

# ⭐ Différentielle d'un « produit » B(f1, f2)

*Théorème* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Prop. 2.34 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Proposition
> Soient $f_1:U\to F_1$, $f_2:U\to F_2$ différentiables en $a$ et $B:F_1\times F_2\to G$ bilinéaire continue. Alors $P:x\mapsto B(f_1(x),f_2(x))$ est différentiable en $a$ et
> $$DP_a(h)=B\big(D(f_1)_a(h),f_2(a)\big)+B\big(f_1(a),D(f_2)_a(h)\big).$$

> [!SUCCESS]- Démonstration
> $P=B\circ\varphi$ avec $\varphi=(f_1,f_2)$, différentiable en $a$ par la Prop. 2.33 avec $D\varphi_a(h)=(D(f_1)_a(h),D(f_2)_a(h))$. $B$ est différentiable (Ex. 2.17). Par la règle de la chaîne :
> $DP_a(h)=DB_{(f_1(a),f_2(a))}\big(D\varphi_a(h)\big)=B(D(f_1)_a(h),f_2(a))+B(f_1(a),D(f_2)_a(h))$. $\blacksquare$

> [!EXAMPLE] Exemples
> - Produit de fonctions réelles : $D(fg)_a(h)=Df_a(h)\,g(a)+f(a)\,Dg_a(h)$.
> - $f(X)=XMX=p(X,MX)$ : $Df_A(H)=HMA+AMH$ (Écrit 2025-2026).

## 🔗 Liens

- **S'appuie sur** : [[differentielles-de-reference|Différentielles de référence : constante, linéaire, bilinéaire]], [[regle-de-la-chaine|Règle de la chaîne (différentielle d'une composée)]], [[differentiabilite-par-composantes|Différentiabilité par composantes]]
- **Méthodes** : [[differentiabilite-par-theoremes|Montrer la différentiabilité par les théorèmes généraux]]
