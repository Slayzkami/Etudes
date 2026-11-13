---
aliases:
  - "Vrai/Faux classiques topologie"
  - "vrai faux topo"
  - "contre-exemples topologie"
tags:
  - topologie
  - topo/revision
---

# ✅ Vrai/Faux classiques (avec justification)

Cacher la colonne de droite, répondre, puis comparer. · [[topo-plan-de-revision|↩ Plan de révision]] · [[topo-index-definitions|↩ Index]]

> [!ABSTRACT] Règle
> **Vrai** ⟹ une preuve courte. **Faux** ⟹ **un** contre-exemple explicite et vérifié. « Faux » seul = 0 point.

| Affirmation | Réponse | Justification courte |
|---|---|---|
| Une partie qui n'est pas ouverte est fermée | **Faux** | $[0,1[$ n'est ni ouvert ni fermé → [[topo-ouvert]] |
| Une intersection d'ouverts est ouverte | **Faux** | $\bigcap_n]-\frac1n,\frac1n[=\{0\}$ ; vrai si **finie** → [[topo-stabilite-ouverts]] |
| Une réunion de fermés est fermée | **Faux** | $\bigcup_n[\frac1n,1]=]0,1]$ ; vrai si **finie** → [[topo-stabilite-fermes]] |
| Une boule ouverte est un ouvert | **Vrai** | $r=\rho-d(a,x)$ et inégalité triangulaire → [[topo-boule-ouverte-ouverte]] |
| $\overline{B(a,r)}=\bar B(a,r)$ dans tout espace métrique | **Faux** | distance discrète : $\overline{B(a,1)}=\{a\}$, $\bar B(a,1)=E$ ; vrai dans un e.v.n. → [[topo-distance-discrete]] |
| $\overline{A\cap B}=\bar A\cap\bar B$ | **Faux** | $A=\mathbb Q$, $B=\mathbb R\setminus\mathbb Q$ ; seulement $\subset$ → [[topo-caracterisation-adherence]] |
| $\overline{A\cup B}=\bar A\cup\bar B$ | **Vrai** | réunion **finie** de fermés, plus petit fermé → [[topo-caracterisation-adherence]] |
| $\operatorname{Int}(A\cup B)=\operatorname{Int}A\cup\operatorname{Int}B$ | **Faux** | $A=[0,1]$, $B=[1,2]$ : $1$ est intérieur à la réunion seulement → [[topo-caracterisation-interieur]] |
| L'image directe d'un ouvert par une application continue est ouverte | **Faux** | $x^2$ envoie $]-1,1[$ sur $[0,1[$ → [[topo-continuite-globale]] |
| Si $f$ est continue, $\{f=0\}$ est fermé | **Vrai** | $f^{-1}(\{0\})$, image réciproque d'un fermé → [[topo-continuite-globale]] |
| Applications partielles continues ⟹ $f$ continue | **Faux** | $\frac{xy}{x^2+y^2}$ en $(0,0)$ → [[topo-continuite-composantes]] |
| Continue ⟹ uniformément continue | **Faux** | $x^2$ sur $\mathbb R$ ; vrai sur un **compact** (Heine) → [[topo-heine]] |
| Uniformément continue ⟹ lipschitzienne | **Faux** | $\sqrt{\cdot}$ sur $[0,+\infty[$ → [[topo-hierarchie-lipschitz-uc-continue]] |
| Bijective et continue ⟹ homéomorphisme | **Faux** | $t\mapsto(\cos t,\sin t)$ de $[0,2\pi[$ sur le cercle ; vrai si l'espace de départ est compact → [[topo-image-continue-compact]] |
| Topologiquement équivalentes ⟹ métriquement équivalentes | **Faux** | $\lvert x-y\rvert$ et $\lvert x^2-y^2\rvert$ sur $[0,+\infty[$ → [[topo-metriquement-implique-topologiquement]] |
| La distance discrète provient d'une norme | **Faux** | $N(\frac x2)$ vaudrait $1$ et $\frac12$ → [[topo-distance-et-norme]] |
| Toute application linéaire est continue | **Faux** | vrai en dimension finie ; dérivation sur $C^\infty([0,1])$ → [[topo-applications-lineaires-continues]] |
| Sur $\mathbb R^n$ toutes les normes sont équivalentes | **Vrai** | dimension finie → [[topo-equivalence-normes-dimension-finie]] |
| Fermé et borné ⟹ compact | **Faux** en général | $\mathbb N$ discret ; boule unité de $C([0,1])$ ; **vrai dans $\mathbb R^n$** → [[topo-borel-lebesgue]] |
| Compact ⟹ fermé et borné | **Vrai** | [[topo-compact-complet-borne]] |
| $[0,1[$ est compact car $1-\frac1n$ converge | **Faux** | la limite $1\notin[0,1[$ → [[topo-partie-compacte]] |
| L'image réciproque d'un compact est compacte | **Faux** | $\sin^{-1}([-1,1])=\mathbb R$ → [[topo-image-continue-compact]] |
| $\{0\}\cup\{\frac1n\}$ est compact | **Vrai** | fermé borné de $\mathbb R$ (ou suite + limite) → [[topo-exercices-types-corriges#13. Un compact de R (interro 2025-26)\|ex. 13]] |
| La somme de deux fermés de $\mathbb R$ est fermée | **Faux** | $\mathbb N+\{-n+\frac1n\}$ → [[topo-somme-a-plus-b]] |
| $d(A,B)=0\Rightarrow A\cap B\neq\emptyset$ | **Faux** | $]0,1[$ et $]1,2[$ ; même deux fermés : $\{n\}$ et $\{n+\frac1n\}$ → [[topo-distance-a-une-partie]] |
| $N(x_n)\to N(\ell)\Rightarrow x_n\to\ell$ | **Faux** | $(-1)^n$ → [[topo-convergence-evn]] |

## 🔗 Liens

- [[topo-exemples-et-contre-exemples]] · [[topo-mes-erreurs]] · [[topo-reconnaitre-exercice]]
