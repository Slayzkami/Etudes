---
aliases:
  - "Extrema et différentielle seconde"
  - "Théorème 4.23"
  - "condition suffisante d'extremum"
  - "hessienne définie positive"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-04
---

# ⭐ Extrema et différentielle seconde

*Théorème* · Chapitre : [[04-differentielles-ordre-superieur|4 – Différentielles d'ordre supérieur]] · Th. 4.23 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème
> Soit $U\subset\mathbb R^n$ un ouvert et $f:U\to\mathbb R$ deux fois différentiable en $a\in U$.
> 1. **Condition nécessaire.** Si $f$ admet un minimum (resp. maximum) local en $a$, alors $Df_a=0$ et $H_f(a)$ est semi-définie positive (resp. négative) : ${}^t\!h\,H_f(a)\,h\ge0$ (resp. $\le0$) pour tout $h$.
> 2. **Condition suffisante.** Si $Df_a=0$ et $H_f(a)$ est **définie positive** (resp. définie négative), c'est-à-dire ${}^t\!h\,H_f(a)\,h>0$ (resp. $<0$) pour tout $h\ne0$, alors $f$ admet en $a$ un minimum (resp. maximum) local **strict**.

> [!SUCCESS]- Démonstration de 2 (minimum)
> Taylor-Young avec $Df_a=0$ : $f(a+h)-f(a)=\frac12\,{}^t\!h\,H_f(a)\,h+\lVert h\rVert^2\varepsilon(h)$. Par le Lemme 4.22 il existe $\alpha>0$ avec ${}^t\!h\,H_f(a)\,h\ge\alpha\lVert h\rVert^2$. Donc
> $f(a+h)-f(a)\ge\lVert h\rVert^2\big(\frac\alpha2+\varepsilon(h)\big)$. Comme $\varepsilon(h)\to0$, on a $\lvert \varepsilon(h)\rvert\le\frac\alpha4$ pour $\lVert h\rVert$ assez petit, d'où $f(a+h)-f(a)\ge\frac\alpha4\lVert h\rVert^2>0$ pour $h\ne0$ petit. $\blacksquare$

> [!TIP] En dimension 2
> On utilise le [[critere-rt-s2]].

## 🔗 Liens

- **S'appuie sur** : [[condition-necessaire-extremum|Condition nécessaire d'extremum (ordre 1)]], [[matrice-hessienne|Matrice hessienne]], [[taylor-young-ordre-2|Formule de Taylor-Young à l'ordre 2]]
- **Utilisé par (théorèmes)** : [[critere-rt-s2|Critère rt − s² (dimension 2)]]
