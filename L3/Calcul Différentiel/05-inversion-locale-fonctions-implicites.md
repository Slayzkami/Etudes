---
aliases:
  - "5 – Inversion locale et fonctions implicites"
  - "Chapitre TIL TFI"
  - "CD chapitre 5"
tags:
  - cd
  - cd/chapitre
---

# Chapitre 05 – Inversion locale et fonctions implicites

**Matière :** [[L3/Calcul Différentiel/README|Calcul Différentiel]]  
**Source :** polycopié *Chapitre 5 – Inversion locale, fonctions implicites* ; cours rédigé, chapitre 5 (pages 99 à 122)  
**Index :** [[cd-index-definitions]]

> [!NOTE] Numérotation
> Le polycopié numérote deux fois « Théorème 5.1 » et « 5.2 ». Ici on suit le cours rédigé : inversion locale = Th. 5.7, inversion globale = Th. 5.12, fonctions implicites = Th. 5.15 (une variable) et 5.19 (cas général).

## 🎯 L'essentiel en 3 lignes
- Un [[diffeomorphisme]] est une bijection $\mathcal C^1$ dont la réciproque est $\mathcal C^1$ ; alors $D(f^{-1})_{f(a)}=(Df_a)^{-1}$ ([[differentielle-de-la-reciproque]]).
- **Inversion locale** : $f$ de classe $\mathcal C^1$ de $\mathbb R^n$ dans $\mathbb R^n$ et $\det J_f(a)\ne0$ ⟹ difféomorphisme local en $a$ ([[inversion-locale]]). Avec l'injectivité en plus : global ([[inversion-globale]]).
- **Fonctions implicites** : $f(a,b)=0$ et $\partial_yf(a,b)\ne0$ ⟹ près de $(a,b)$, $f(x,y)=0\iff y=\varphi(x)$, et $\varphi'=-\partial_xf/\partial_yf$ ([[fonctions-implicites-une-variable]]).

## 📝 Notes

### 5.1 – Difféomorphismes
- [[diffeomorphisme]] (global, local) ; exemple des coordonnées polaires ; contre-exemple $x^3$.
- [[differentielle-de-la-reciproque]].

### 5.2 – Inversion locale
- [[inversion-locale]] (preuve par le [[point-fixe-banach-picard|point fixe]]) ; [[inversion-globale]] et sa forme pratique (Cor. 5.13).
- Méthode : [[montrer-diffeomorphisme]].

### 5.3 – Fonctions implicites
- [[fonctions-implicites-une-variable]] (Th. 5.15) ; [[fonctions-implicites]] (Th. 5.19, Cor. 5.20).
- Méthode : [[fonction-implicite]].

## 🔑 Définitions / formules à retenir
| Terme | Formule |
|---|---|
| [[diffeomorphisme]] | bijection, $f$ de classe $\mathcal C^1$, $f^{-1}$ de classe $\mathcal C^1$ |
| [[differentielle-de-la-reciproque]] | $J_{f^{-1}}(f(a))=[J_f(a)]^{-1}$ |
| [[inversion-locale]] | $\mathcal C^1$ + $\det J_f(a)\ne0$ ⟹ difféomorphisme local en $a$ |
| [[inversion-globale]] | $\mathcal C^1$ + injective + $\det J_f\ne0$ partout ⟹ difféomorphisme de $U$ sur $f(U)$ |
| [[fonctions-implicites-une-variable]] | $f(a,b)=0$, $\partial_yf(a,b)\ne0$ ⟹ $y=\varphi(x)$, $\varphi'(a)=-\frac{\partial_xf(a,b)}{\partial_yf(a,b)}$ |
| [[fonctions-implicites]] | $J_\varphi=-[J_yf]^{-1}J_xf$ |
| inverse $2\times2$ | $\begin{pmatrix}\alpha&\beta\\ \gamma&\delta\end{pmatrix}^{-1}=\frac1{\alpha\delta-\beta\gamma}\begin{pmatrix}\delta&-\beta\\-\gamma&\alpha\end{pmatrix}$ |

## ❓ Ce que je n'ai pas compris
- 

## 🧠 Questions de révision
1. Définir : difféomorphisme, difféomorphisme local.
2. Pourquoi $x\mapsto x^3$ n'est-il pas un difféomorphisme de $\mathbb R$ sur $\mathbb R$ ?
3. Énoncer le théorème d'inversion locale. Quelles sont les trois hypothèses à vérifier ?
4. Donner une application de jacobien partout non nul qui n'est pas injective.
5. Énoncer le théorème des fonctions implicites pour $f:\mathbb R^2\to\mathbb R$. Retrouver la formule de $\varphi'$.
6. Sur le cercle $x^2+y^2=1$, en quels points ne peut-on pas écrire $y=\varphi(x)$ ?

## 🔗 Pour aller plus loin
- Corrigés rédigés : [[cd-exercices-types-corriges]] (ex. 14, 15)
- Précédent : [[04-differentielles-ordre-superieur]]
- Sources : polycopié [chapitre 5](fichiers/cd-chap5-polycopie.pdf), [cours rédigé](fichiers/cd-cours-redige-ch1-5.pdf) (les 8 exercices du polycopié y sont corrigés)
