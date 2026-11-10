---
aliases:
  - "Continuité en un point"
  - "application continue"
  - "continue en a"
  - "continuité"
tags:
  - cd
  - cd/definition
  - cd/chapitre-01
---

# 📘 Continuité en un point

*Définition* · Chapitre : [[01-espaces-vectoriels-normes|1 – Espaces vectoriels normés]] · Déf. 1.28 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> $f:E\to F$ est **continue en** $a\in E$ si
> $$\forall\varepsilon>0,\ \exists\delta>0,\ \forall x\in E,\quad \lVert x-a\rVert_E<\delta\ \Longrightarrow\ \lVert f(x)-f(a)\rVert_F<\varepsilon.$$
> $f$ est continue sur $A\subset E$ si elle est continue en tout point de $A$.

> [!IMPORTANT] Caractérisation séquentielle (Th. 1.29) et composition (Th. 1.30)
> - $f$ continue en $a$ $\iff$ pour toute suite $x_n\to a$, on a $f(x_n)\to f(a)$.
> - Si $f$ est continue en $a$ et $g$ continue en $f(a)$, alors $g\circ f$ est continue en $a$.

> [!TIP] En clair
> La continuité compare toujours $f(x)$ à $f(a)$ : il faut que $\lVert f(x)-f(a)\rVert$ soit petit. Savoir que $\lVert f(x)\rVert$ est borné ne suffit **jamais**.

> [!WARNING] Pièges
> - Continuité des applications partielles $\not\Rightarrow$ continuité (Ex. 1.42) : $f(x,y)=\dfrac{xy}{x^2+y^2}$, $f(0,0)=0$ ; $f(x,0)=f(0,y)=0$ mais $f(t,t)=\frac12\not\to0$.
> - $\lVert f(u)\rVert\le C\lVert u\rVert$ ne prouve la continuité que si $f$ est **linéaire** → [[caracterisation-lineaires-continues]].

## 🔗 Liens

- **S'appuie sur** : [[norme|Norme, espace vectoriel normé]]
- **Utilisé par (définitions)** : [[continuite-uniforme|Continuité uniforme]], [[application-lineaire-continue|Application linéaire continue, espace Lc(E,F)]]
- **Utilisé par (théorèmes)** : [[continuite-et-composantes|Continuité et composantes]], [[differentiable-implique-continue|Différentiable implique continue]]
- **Méthodes** : [[montrer-continue|Montrer qu'une application est (ou n'est pas) continue]]
