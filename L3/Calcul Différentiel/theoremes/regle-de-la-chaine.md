---
aliases:
  - "Règle de la chaîne (différentielle d'une composée)"
  - "Théorème 2.20"
  - "différentielle d'une composée"
  - "D(g∘f)"
  - "jacobienne d'une composée"
  - "composée de C1"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-02
---

# ⭐ Règle de la chaîne (différentielle d'une composée)

*Théorème* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Th. 2.20, Cor. 2.26, Prop. 2.37 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> Soient $E,F,G$ trois e.v.n., $U\subset E$ et $V\subset F$ deux ouverts, $f:U\to F$ et $g:V\to G$ avec $f(U)\subset V$. Si $f$ est différentiable en $a$ et $g$ est différentiable en $f(a)$, alors $g\circ f$ est différentiable en $a$ et
> $$D(g\circ f)_a=Dg_{f(a)}\circ Df_a,\qquad\text{soit}\qquad D(g\circ f)_a(h)=Dg_{f(a)}\big(Df_a(h)\big).$$

> [!IMPORTANT] Versions utiles
> - **Composée de $\mathcal C^1$** (Cor. 2.26) : la composée de deux applications $\mathcal C^1$ est $\mathcal C^1$.
> - **Jacobiennes** (Prop. 2.37) : $J_{g\circ f}(a)=J_g(f(a))\times J_f(a)$.
> - **Avec une fonction d'une variable** : si $u:U\to\mathbb R$ est différentiable et $\varphi:\mathbb R\to\mathbb R$ dérivable, $D(\varphi\circ u)_a(h)=\varphi'(u(a))\,Du_a(h)$.

> [!SUCCESS]- Démonstration
> Posons $b=f(a)$, $k=f(a+h)-f(a)=Df_a(h)+o(h)$. Alors
> $g(f(a+h))=g(b+k)=g(b)+Dg_b(k)+\lVert k\rVert\varepsilon_2(k)=g(b)+Dg_b(Df_a(h))+Dg_b(o(h))+\lVert k\rVert\varepsilon_2(k)$.
> - $Dg_b\circ Df_a$ est linéaire continue (composée).
> - $Dg_b(o(h))=o(h)$ (Lemme 2.2 (c)).
> - $\lVert k\rVert\le(\lvert\!\lvert\!\lvert Df_a\rvert\!\rvert\!\rvert+1)\lVert h\rVert$ pour $h$ petit, et $k\to0$ quand $h\to0$, donc $\lVert k\rVert\varepsilon_2(k)=o(h)$. $\blacksquare$

> [!WARNING] Pièges
> - $Dg$ se prend **au point $f(a)$**, pas en $a$.
> - L'ordre compte : $Dg_{f(a)}\circ Df_a$ (comme $g'(f(a))\times f'(a)$).
> - Pour les jacobiennes : produit dans l'ordre $J_g\times J_f$, tailles $(q\times p)(p\times n)$.

## 🔗 Liens

- **S'appuie sur** : [[differentiabilite|Différentiabilité en un point, différentielle]], [[norme-composee|Norme d'une composée]]
- **Utilisé par (théorèmes)** : [[differentielle-produit-bilineaire|Différentielle d'un « produit » B(f1, f2)]], [[expression-differentielle-seconde|Expression de la différentielle seconde]], [[differentielle-de-la-reciproque|Différentielle de la réciproque]]
- **Méthodes** : [[differentiabilite-par-theoremes|Montrer la différentiabilité par les théorèmes généraux]], [[appliquer-regle-de-la-chaine|Appliquer la règle de la chaîne en 4 étapes]]
