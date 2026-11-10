---
aliases:
  - "Théorème des accroissements finis (TAF)"
  - "TAF"
  - "égalité des accroissements finis"
  - "Rolle"
tags:
  - cd
  - cd/theoreme
  - cd/chapitre-03
---

# ⭐ Théorème des accroissements finis (TAF)

*Théorème* · Chapitre : [[03-accroissements-finis|3 – Accroissements finis]] · Th. 3.2 et 3.6 du cours · [[cd-index-definitions|↩ Index]]

> [!IMPORTANT] Théorème (une variable, Th. 3.2)
> Soient $a<b$ et $f:[a,b]\to\mathbb R$ continue sur $[a,b]$, dérivable sur $]a,b[$. Il existe $c\in\,]a,b[$ tel que $f(b)-f(a)=f'(c)(b-a)$.

> [!IMPORTANT] Théorème (à valeurs réelles, Th. 3.6)
> Soit $E$ un $\mathbb R$-e.v.n., $U\subset E$ un ouvert, $f:U\to\mathbb R$ différentiable sur $U$, et $a\ne b$ dans $U$ tels que $[a,b]\subset U$. Il existe $c\in\,]a,b[$ tel que
> $$f(b)-f(a)=Df_c(b-a).$$

> [!SUCCESS]- Démonstration (Th. 3.6)
> On pose $g(t)=f(a+t(b-a))$ pour $t\in[0,1]$. Par la règle de la chaîne, $g$ est dérivable et $g'(t)=Df_{a+t(b-a)}(b-a)$. Le TAF en une variable donne $\theta\in\,]0,1[$ avec $g(1)-g(0)=g'(\theta)$, c'est-à-dire $f(b)-f(a)=Df_c(b-a)$ avec $c=a+\theta(b-a)$. $\blacksquare$

> [!WARNING] Piège (question de cours, Écrit 2022-2023)
> L'**égalité** est fausse pour une fonction à valeurs dans $\mathbb R^2$ : $f(t)=(\cos t,\sin t)$ sur $[0,2\pi]$ vérifie $f(2\pi)-f(0)=0$ mais $f'(c)=(-\sin c,\cos c)\ne0$ pour tout $c$. À valeurs vectorielles, on n'a que l'**inégalité** → [[iaf]].

## 🔗 Liens

- **S'appuie sur** : [[differentiabilite|Différentiabilité en un point, différentielle]], [[segment-et-convexe|Segment, partie convexe]]
