---
aliases:
  - "Corrigé du sujet 2025"
  - "corrigé seconde session 2025"
  - "annale GAC 2025"
tags:
  - gac
  - gac/revision
---

# 📝 Corrigé – contrôle seconde session du 13 novembre 2025

[Sujet (PDF)](../fichiers/gac-sujet-2025-seconde-session.pdf) · 1 h 30 · barème indicatif sur 20 · [[plan-de-revision|↩ Plan de révision]] · [[index-definitions|↩ Index]]

> [!TIP] Mode d'emploi
> Fais d'abord le sujet **seul, chronométré**, puis déplie les corrections une par une. L'exercice 2 porte sur le groupe symétrique (partie IV) : **hors programme cette année**, corrigé pour information.

## Exercice 1 – Vrai/Faux (6 pts)

> [!SUCCESS]- 1. Les groupes abéliens sont les groupes cycliques → **Faux**
> Tout groupe cyclique est abélien ($a^ka^l=a^{k+l}=a^la^k$), mais la réciproque est fausse.
> $K=\mathbb Z/2\mathbb Z\times\mathbb Z/2\mathbb Z$ est abélien (calcul coordonnée par coordonnée), d'ordre 4, et pour tout $x\in K$, $2x=(\bar0,\bar0)$, donc $o(x)\le2$ : aucun élément n'engendre $K$. → [[groupe-abelien]]

> [!SUCCESS]- 2. $(M_2(\mathbb R),\times)$ est un groupe non abélien → **Faux**
> Ce n'est pas un groupe : le neutre ne peut être que $I_2$, et la matrice nulle n'a pas d'inverse ($0\times M=0\neq I_2$ pour toute $M$).

> [!SUCCESS]- 3. $(M_2(\mathbb R),+)$ est un groupe abélien → **Vrai**
> L'addition est interne, associative et commutative (coefficient par coefficient, comme dans $\mathbb R$), de neutre la matrice nulle, et l'opposé de $M$ est $-M$.

> [!SUCCESS]- 4. Dans un groupe, tout élément est simplifiable → **Vrai**
> Si $ax=ay$, en composant à gauche par $a^{-1}$ : $x=y$. De même à droite. → [[regles-de-calcul]]

> [!SUCCESS]- 5. L'ensemble des éléments d'ordre 2 est un sous-groupe → **Faux**
> Il ne contient pas le neutre (qui est d'ordre 1), alors que tout sous-groupe contient le neutre.

> [!SUCCESS]- 6. Seul le neutre est solution de $x^2=x$ → **Vrai**
> $x^2=x$ s'écrit $x\cdot x=x\cdot e$ ; en simplifiant par $x$ à gauche : $x=e$. Et $e^2=e$.

> [!SUCCESS]- 7. Tout sous-groupe d'ordre 2 est normal → **Faux**
> Dans $\mathfrak S_3$, $H=\{e,(1\,2)\}$ : $(1\,3)(1\,2)(1\,3)^{-1}=(2\,3)\notin H$.
> (Contre-exemple sans permutations : dans $GL_2(\mathbb R)$, $H=\{I_2,s\}$ avec $s=\begin{pmatrix}1&0\\0&-1\end{pmatrix}$ ; pour $g=\begin{pmatrix}1&1\\0&1\end{pmatrix}$, $gsg^{-1}=\begin{pmatrix}1&-2\\0&-1\end{pmatrix}\notin H$.)

> [!SUCCESS]- 8. Tout sous-groupe d'indice 2 est distingué → **Vrai**
> Il y a deux classes à gauche, $H$ et $G\setminus H$, et deux classes à droite, $H$ et $G\setminus H$. Si $g\in H$, $gH=H=Hg$ ; si $g\notin H$, $gH=G\setminus H=Hg$. Donc $gH=Hg$ pour tout $g$. → [[indice-2-distingue]]

> [!SUCCESS]- 9. Deux groupes de même ordre sont isomorphes → **Faux**
> $\mathbb Z/4\mathbb Z$ et $\mathbb Z/2\mathbb Z\times\mathbb Z/2\mathbb Z$ ont 4 éléments ; le premier a un élément d'ordre 4 ($\bar1$), le second non. Un isomorphisme conservant l'ordre des éléments, ils ne sont pas isomorphes. → [[montrer-non-isomorphes]]

> [!SUCCESS]- 10. Un morphisme conserve l'ordre des éléments → **Faux**
> Le morphisme nul $\mathbb Z/2\mathbb Z\to\mathbb Z/2\mathbb Z$ envoie $\bar1$ (d'ordre 2) sur $\bar0$ (d'ordre 1). (Vrai si le morphisme est injectif.)

## Exercice 2 – Permutations (5 pts, hors programme)

$\sigma=\begin{pmatrix}1&2&3&4&5&6&7&8\\3&4&5&2&7&8&1&6\end{pmatrix}$, $\tau=(1\,2\,3)(3\,5)(4\,6\,1)(7\,8)$ (composition de droite à gauche).

> [!SUCCESS]- Correction
> **Calcul de $\tau$** (on applique $(7\,8)$, puis $(4\,6\,1)$, puis $(3\,5)$, puis $(1\,2\,3)$) : $\tau=\begin{pmatrix}1&2&3&4&5&6&7&8\\4&3&5&6&1&2&8&7\end{pmatrix}=(1\,4\,6\,2\,3\,5)(7\,8)$.
>
> 1. $\sigma\circ\tau=\begin{pmatrix}1&2&3&4&5&6&7&8\\2&5&7&8&3&4&6&1\end{pmatrix}=(1\,2\,5\,3\,7\,6\,4\,8)$.
> 2. $\sigma=(1\,3\,5\,7)(2\,4)(6\,8)=(1\,7)(1\,5)(1\,3)(2\,4)(6\,8)$.
> 3. Inversions : $2+2+2+1+2+2+0=11$, donc $\varepsilon(\sigma)=(-1)^{11}=-1$ (cohérent avec 5 transpositions).
> 4. $o(\tau)=\operatorname{ppcm}(6,2)=6$. Comme $2025=6\times337+3$, $\tau^{2025}=\tau^3=(1\,2)(4\,3)(6\,5)(7\,8)$.

## Exercice 3 – $\mathbb Z/18\mathbb Z$ et $\mathbb Z/6\mathbb Z$ (6 pts)

$G=(\mathbb Z/18\mathbb Z,+)$, $K=(\mathbb Z/6\mathbb Z,+)$, $f(x+18\mathbb Z)=x+6\mathbb Z$.

> [!SUCCESS]- 1. $K$ est-il un sous-groupe de $G$ ?
> Non : $K$ n'est même pas une partie de $G$. Les éléments de $K$ sont des classes modulo 6 (par exemple $\bar1=1+6\mathbb Z$ contient $7$), ceux de $G$ des classes modulo 18 ; $1+6\mathbb Z\neq x+18\mathbb Z$ pour tout $x$.
> (En revanche $G$ contient un sous-groupe **isomorphe** à $K$ : $\langle\bar3\rangle$, cyclique d'ordre 6.)

> [!SUCCESS]- 2. $G$ et $K$ sont-ils isomorphes ?
> Non : un isomorphisme est une bijection, or $\mathrm{Card}\,G=18\neq6=\mathrm{Card}\,K$.

> [!SUCCESS]- 3. Ordre des éléments de $K$
> $o(\bar k)=6/\operatorname{pgcd}(6,k)$ :
>
> | $\bar k$ | $\bar0$ | $\bar1$ | $\bar2$ | $\bar3$ | $\bar4$ | $\bar5$ |
> |---|---|---|---|---|---|---|
> | ordre | 1 | 6 | 3 | 2 | 3 | 6 |

> [!SUCCESS]- 4. Treillis des sous-groupes de $G$
> Les sous-groupes de $\mathbb Z/18\mathbb Z$ sont les $\langle\bar d\rangle$, $d\mid18$, d'ordre $18/d$ : $\{\bar0\}$, $\langle\bar9\rangle$ (2), $\langle\bar6\rangle$ (3), $\langle\bar3\rangle$ (6), $\langle\bar2\rangle$ (9), $G$ (18). Inclusion : $\langle\bar a\rangle\subset\langle\bar b\rangle\iff b\mid a$.
>
> ```mermaid
> graph BT
>   Z0["{0}"] --> Z9["⟨9⟩ (2)"]
>   Z0 --> Z6["⟨6⟩ (3)"]
>   Z9 --> Z3["⟨3⟩ (6)"]
>   Z6 --> Z3
>   Z6 --> Z2["⟨2⟩ (9)"]
>   Z3 --> G["G (18)"]
>   Z2 --> G
> ```
> → [[lister-sous-groupes-znz]]

> [!SUCCESS]- 5. Réunion qui n'est pas un sous-groupe
> $H=\langle\bar9\rangle=\{\bar0,\bar9\}$ et $L=\langle\bar6\rangle=\{\bar0,\bar6,\overline{12}\}$. $\bar6,\bar9\in H\cup L$ mais $\bar6+\bar9=\overline{15}\notin H\cup L$ : $H\cup L$ n'est pas stable, ce n'est pas un sous-groupe. (Ou : $\mathrm{Card}(H\cup L)=4\nmid18$, contraire à Lagrange.)

> [!SUCCESS]- 6. $f$ bien définie, morphisme, noyau, image
> - **Bien définie** : si $x+18\mathbb Z=y+18\mathbb Z$, alors $18\mid x-y$, donc $6\mid x-y$ (car $6\mid18$), donc $x+6\mathbb Z=y+6\mathbb Z$.
> - **Morphisme** : $f\big((x+18\mathbb Z)+(y+18\mathbb Z)\big)=(x+y)+6\mathbb Z=(x+6\mathbb Z)+(y+6\mathbb Z)$.
> - **Noyau** : $f(x+18\mathbb Z)=\bar0\iff6\mid x$, donc $\mathrm{Ker}\,f=\{\bar0,\bar6,\overline{12}\}=6\mathbb Z/18\mathbb Z$.
> - **Image** : tout $k+6\mathbb Z$ vaut $f(k+18\mathbb Z)$, donc $\mathrm{Im}\,f=K$ ($f$ surjective).

> [!SUCCESS]- 7. En déduire $(\mathbb Z/18\mathbb Z)/(6\mathbb Z/18\mathbb Z)\simeq\mathbb Z/6\mathbb Z$
> D'après le premier théorème d'isomorphisme, $\bar f:G/\mathrm{Ker}\,f\to\mathrm{Im}\,f$, $\overline{x+18\mathbb Z}\mapsto x+6\mathbb Z$ est un isomorphisme. Avec 6., cela donne $(\mathbb Z/18\mathbb Z)/(6\mathbb Z/18\mathbb Z)\simeq\mathbb Z/6\mathbb Z$. → [[premier-theoreme-isomorphisme]]

## Exercice 4 – Endomorphismes de $(\mathbb Z,+)$ (3 pts)

> [!SUCCESS]- Correction
> **Analyse.** Soit $f$ un endomorphisme et $a=f(1)$. Pour $n\in\mathbb Z$, $f(n)=f(n\cdot1)=n\,f(1)=an$.
> **Synthèse.** Pour $a\in\mathbb Z$, $f_a:n\mapsto an$ vérifie $f_a(n+m)=an+am=f_a(n)+f_a(m)$.
> **Conclusion.** $\mathrm{End}(\mathbb Z,+)=\{n\mapsto an,\ a\in\mathbb Z\}$. (Bonus : automorphismes $a=\pm1$.) → [[endomorphismes-de-z]]

## 🔗 Liens

- [[exercices-types-corriges]] · [[vrai-faux-classiques]] · [[reconnaitre-exercice]] · [[mes-erreurs]]
