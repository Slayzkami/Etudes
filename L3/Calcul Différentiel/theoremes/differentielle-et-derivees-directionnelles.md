---
aliases:
  - "Différentielle et dérivées directionnelles"
  - "Proposition 2.9"
  - "Df_a(v) = lim (f(a+tv)-f(a))/t"
  - "différentiable implique dérivable dans toute direction"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-02
---

# ⭐ Différentielle et dérivées directionnelles

*Théorème* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Prop. 2.9 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Proposition
> Si $f$ est différentiable en $a$, alors $f$ est dérivable en $a$ dans **toutes** les directions $v\in E$, et
> $$Df_a(v)=\lim_{t\to0}\frac{f(a+tv)-f(a)}{t}=\frac{\mathrm d}{\mathrm dt}f(a+tv)\Big|_{t=0}.$$

> [!SUCCESS]- Démonstration (question de cours, Écrit 2024-2025)
> Si $v=0$ : les deux membres valent $0$. Soit $v\ne0$. Comme $U$ est ouvert, $a+tv\in U$ pour $\abs t$ assez petit. Par définition, avec $h=tv$ :
> $$f(a+tv)=f(a)+Df_a(tv)+\lVert tv\rVert\,\varepsilon(a+tv)=f(a)+t\,Df_a(v)+\abs t\,\lVert v\rVert\,\varepsilon(a+tv),$$
> par linéarité de $Df_a$. Pour $t\ne0$ :
> $$\Big\|\frac{f(a+tv)-f(a)}{t}-Df_a(v)\Big\|=\lVert v\rVert\,\lVert \varepsilon(a+tv)\rVert\xrightarrow[t\to0]{}0,$$
> car $a+tv\to a$ et $\varepsilon(x)\to0$ quand $x\to a$. $\blacksquare$

> [!TIP] Trois usages
> 1. **Calculer** une dérivée directionnelle : $Df_a(v)=J_f(a)\,v$.
> 2. **Trouver le candidat** $L$ quand on veut prouver la différentiabilité.
> 3. **Réfuter** la différentiabilité (contraposée) : une dérivée directionnelle qui n'existe pas, ou $v\mapsto f'_v(0)$ non linéaire → [[montrer-non-differentiable]].

> [!WARNING] Piège
> La réciproque est fausse (Rem. 2.10).

## 🔗 Liens

- **S'appuie sur** : [[differentiabilite|Différentiabilité en un point, différentielle]], [[derivee-directionnelle|Dérivée directionnelle]]
- **Utilisé par (théorèmes)** : [[condition-necessaire-extremum|Condition nécessaire d'extremum (ordre 1)]]
- **Méthodes** : [[differentiabilite-par-definition|Montrer la différentiabilité par la définition]], [[calculer-derivee-directionnelle|Calculer une dérivée directionnelle]], [[montrer-non-differentiable|Montrer qu'une application n'est pas différentiable en a]]
