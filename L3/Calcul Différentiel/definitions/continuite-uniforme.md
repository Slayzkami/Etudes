---
aliases:
  - "Continuité uniforme"
  - "uniformément continue"
  - "continuité uniforme"
tags:
  - cd
  - cd/definition
  - cd/chapitre-01
---

# 📘 Continuité uniforme

*Définition* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Déf. 1.31 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> $f:E\to F$ est **uniformément continue** si
> $$\forall\varepsilon>0,\ \exists\delta>0,\ \forall(x,y)\in E^2,\quad \lVert x-y\rVert_E<\delta\ \Longrightarrow\ \lVert f(x)-f(y)\rVert_F<\varepsilon.$$

> [!TIP] La différence avec la continuité
> $\delta$ ne dépend que de $\varepsilon$, **pas du point**.

> [!IMPORTANT] Chaîne d'implications (Prop. 1.32, 1.34)
> [[application-lipschitzienne|Lipschitzienne]] $\Rightarrow$ uniformément continue $\Rightarrow$ continue. Les réciproques sont fausses.

> [!EXAMPLE] Contre-exemple
> $x\mapsto x^2$ est continue sur $\mathbb R$ mais pas uniformément continue : $x_n=n$, $y_n=n+\frac1n$ donnent $\lvert x_n-y_n\rvert\to0$ et $\lvert x_n^2-y_n^2\rvert=2+\frac1{n^2}\ge2$.

## 🔗 Liens

- **S'appuie sur** : [[continuite|Continuité en un point]]
