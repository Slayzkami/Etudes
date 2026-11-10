---
aliases:
  - "Différentiabilité par composantes"
  - "Proposition 2.33"
  - "Corollaire 2.35"
  - "composantes différentiables"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-02
---

# ⭐ Différentiabilité par composantes

*Théorème* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Prop. 2.33, Cor. 2.35 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Proposition
> Soit $f=(f_1,\dots,f_p):U\to F_1\times\dots\times F_p$. $f$ est différentiable en $a$ si et seulement si chaque composante $f_i$ est différentiable en $a$. Dans ce cas, pour tout $h\in E$ :
> $$Df_a(h)=\big(D(f_1)_a(h),\dots,D(f_p)_a(h)\big).$$
> Cas $\mathbb R^n\to\mathbb R^p$ (Cor. 2.35) : $Df_a(h)=J_f(a)\,h$.

> [!SUCCESS]- Démonstration
> ($\Rightarrow$) $f_i=\pi_i\circ f$ avec $\pi_i$ linéaire continue : [[regle-de-la-chaine]], $D(f_i)_a=\pi_i\circ Df_a$.
> ($\Leftarrow$) Posons $L(h)=(D(f_1)_a(h),\dots,D(f_p)_a(h))$, linéaire continue (composantes linéaires continues). Le reste $f(a+h)-f(a)-L(h)$ a pour composantes des $o(h)$, donc est un $o(h)$ (Lemme 2.2 (d)). $\blacksquare$

> [!TIP] Phrase type
> « Les composantes $f_1,\dots,f_p$ sont différentiables sur $\mathbb R^n$ (polynômes, composées de fonctions usuelles), donc $f$ est différentiable sur $\mathbb R^n$ (Proposition 2.33) et $Df_a(h)=J_f(a)h$ (Corollaire 2.35). »

## 🔗 Liens

- **S'appuie sur** : [[differentiabilite|Différentiabilité en un point, différentielle]], [[norme-produit|Norme produit]], [[matrice-jacobienne|Matrice jacobienne]]
- **Utilisé par (théorèmes)** : [[differentielle-produit-bilineaire|Différentielle d'un « produit » B(f1, f2)]]
- **Méthodes** : [[differentiabilite-par-theoremes|Montrer la différentiabilité par les théorèmes généraux]], [[calculer-jacobienne|Calculer une jacobienne et une différentielle sur R^n]]
