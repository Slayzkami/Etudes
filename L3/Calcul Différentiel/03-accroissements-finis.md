---
aliases:
  - "3 – Accroissements finis"
  - "Chapitre TAF IAF"
  - "CD chapitre 3"
tags:
  - cd
  - cd/chapitre
---

# Chapitre 03 – Accroissements finis

**Matière :** [[L3/Calcul Différentiel/README|Calcul Différentiel]]  
**Source :** cours rédigé, chapitre 3 (pages 58 à 72)  
**Index :** [[cd-index-definitions]]

## 🎯 L'essentiel en 3 lignes
- **IAF** : si $[a,b]\subset U$ et $\lvert\!\lvert\!\lvert Df_x\rvert\!\rvert\!\rvert\le M$ sur le segment, alors $\lVert f(b)-f(a)\rVert\le M\lVert b-a\rVert$ ([[iaf]]). Sur un ouvert **convexe**, $f$ est $M$-lipschitzienne ([[iaf-sur-un-convexe]]).
- **Critère $\mathcal C^1$** : sur $\mathbb R^n$, $\mathcal C^1$ ⟺ dérivées partielles **continues** ([[critere-c1]]).
- $Df=0$ sur un ouvert **connexe** ⟹ $f$ constante ([[differentielle-nulle]]).

## 📝 Notes

### 3.1 – TAF
- [[taf]] : égalité, seulement pour les fonctions **à valeurs réelles**. [[segment-et-convexe]].

### 3.2 – IAF
- [[iaf]] (Th. 3.8, 3.9, 3.11) ; [[iaf-sur-un-convexe]] (Cor. 3.13). Méthode : [[utiliser-iaf]].

### 3.3 – Classe $\mathcal C^1$
- [[classe-c1]], [[critere-c1]] (Th. 3.15, Cor. 3.16). Méthode : [[montrer-classe-c1]].
- Point sans formule : [[etudier-en-un-point-particulier]].

### 3.4 – Différentielle nulle
- [[partie-connexe]], [[convexe-implique-connexe]], [[differentielle-nulle]]. Méthode : [[montrer-constante]].

## 🔑 Définitions / formules à retenir
| Terme | Formule |
|---|---|
| [[segment-et-convexe]] | $[a,b]=\{a+t(b-a),\ t\in[0,1]\}$ ; convexe : $[a,b]\subset C$ |
| [[taf]] | $f(b)-f(a)=Df_c(b-a)$, $c\in\,]a,b[$ ($f$ à valeurs dans $\mathbb R$) |
| [[iaf]] | $\lVert f(b)-f(a)\rVert\le M\lVert b-a\rVert$ si $\lvert\!\lvert\!\lvert Df_x\rvert\!\rvert\!\rvert\le M$ sur $[a,b]\subset U$ |
| [[iaf-sur-un-convexe]] | $\lvert\!\lvert\!\lvert Df_x\rvert\!\rvert\!\rvert\le M$ sur $C$ convexe ⟹ $M$-lipschitzienne |
| [[critere-c1]] | $\mathcal C^1$ ⟺ dérivées partielles continues |
| [[differentielle-nulle]] | $Df=0$ sur $U$ connexe ⟹ $f$ constante |

## ❓ Ce que je n'ai pas compris
- 

## 🧠 Questions de révision
1. Énoncer l'inégalité des accroissements finis (Écrits 2022-2023 et 2025-2026).
2. $f:[a,b]\to\mathbb R^2$ continue, dérivable sur $]a,b[$ : existe-t-il $c$ avec $f(b)-f(a)=(b-a)f'(c)$ ? (Écrit 2022-2023)
3. Que dire de $f$ différentiable sur un ouvert $\Omega$ avec $Df(x)=0$ partout ? (Écrit 2022-2023)
4. Montrer que toute boule est convexe.
5. Montrer que $f(x,y)=(\cos(x+2y),\sin(2x+y))$ est $3$-lipschitzienne pour $\lVert \cdot\rVert_1$.
6. Donner un ouvert connexe non convexe ; un ouvert non connexe.

## 🔗 Pour aller plus loin
- Corrigés rédigés : [[cd-exercices-types-corriges]] (ex. 10) · [[cd-vrai-faux-classiques]]
- Précédent : [[02-applications-differentiables]] · Suivant : [[04-differentielles-ordre-superieur]]
- Source : [cours rédigé](fichiers/cd-cours-redige-ch1-5.pdf)
