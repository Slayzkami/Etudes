# 🗺️ Plan du rapport : la fonction Gamma d'après Emil Artin

**Longueur visée :** 8 pages environ (consigne : 5 à 10)  
**Angle :** le théorème de Bohr–Mollerup au centre, avec un lien explicite avec le cours de topologie dans chaque partie (consigne du prof)  
**Source principale :** [E. Artin, *The Gamma Function*](artin-the-gamma-function.pdf), chapitres 1 et 2 → [fiche de lecture](artin-the-gamma-function.md)  
**Statut :** ✅ plan validé le 16 novembre 2026 · rédaction à commencer

## Pourquoi ce sujet colle avec la topologie
Artin ne fait presque que des **passages à la limite** : une inégalité vraie pour tout $n$ reste vraie à la limite, une fonction est déterminée par une limite, une fonction continue sur un segment est bornée. Ce sont exactement les outils du cours :
- **ch. 1** (suites, unicité de la limite) → le cœur de la preuve de Bohr–Mollerup ;
- **ch. 2** (fermés, caractérisation séquentielle, continuité) → stabilité de la convexité par passage à la limite ;
- **ch. 3** (compacité, bornes atteintes, Heine) → continuité de Γ, contre-exemple périodique.

⚠️ La continuité d'une intégrale à paramètre (convergence dominée) vient plutôt du cours d'[Intégration 1](../../../L3/Int%C3%A9gration%201/). On la cite, mais l'argument « topologique » qu'on met en avant est la **compacité des segments** $[a,b]\subset\,]0,+\infty[$.

## Le plan

### 1. Introduction (½ page)
- Comment prolonger $n!$ aux réels ? L'équation $f(x+1)=xf(x)$ a une infinité de solutions.
- Quelle condition rend la solution unique ? On annonce la réponse : la log-convexité (Bohr–Mollerup, 1922, reprise par Artin en 1931).
- On annonce le plan et le fil topologique.

### 2. Fonctions convexes et log-convexes (1,5 page)
- Définitions ; inégalité des pentes.
- Une fonction convexe sur un intervalle ouvert est continue. 🔗 [continuité](../../../L3/topologie/definitions/topo-continuite.md)
- Une limite simple de fonctions convexes est convexe ; une somme de deux log-convexes est log-convexe (th. 1.8 d'Artin). 🔗 passage à la limite dans une inégalité large : [caractérisation séquentielle des fermés](../../../L3/topologie/theoremes/topo-caracterisation-sequentielle-fermes.md), [exemples de fermés](../../../L3/topologie/theoremes/topo-exemples-fermes.md)

### 3. La fonction Γ (1,5 page)
- Convergence de l'intégrale d'Euler ; $\Gamma(x+1)=x\Gamma(x)$ ; $\Gamma(n+1)=n!$.
- Continuité de Γ : domination sur chaque segment $[a,b]\subset\,]0,+\infty[$. 🔗 [partie compacte](../../../L3/topologie/definitions/topo-partie-compacte.md), [bornes atteintes](../../../L3/topologie/theoremes/topo-bornes-atteintes.md)
- Γ est log-convexe (inégalité de Hölder, ou argument d'Artin par les sommes de Riemann et le passage à la limite).

### 4. Le théorème de Bohr–Mollerup (2 pages, le cœur du rapport)
- Énoncé ; démonstration complète : encadrement par l'inégalité des pentes, puis passage à la limite. 🔗 [suite convergente](../../../L3/topologie/definitions/topo-suite-convergente.md), [unicité de la limite](../../../L3/topologie/theoremes/topo-unicite-limite.md) : c'est elle qui donne l'unicité de Γ !
- Corollaire : la formule de Gauss $\Gamma(x)=\lim \dfrac{n^x\,n!}{x(x+1)\cdots(x+n)}$.
- Les hypothèses sont nécessaires : $f(x)=\Gamma(x)\bigl(1+\varepsilon\sin(2\pi x)\bigr)$ vérifie $f(x+1)=xf(x)$ et $f(1)=1$, mais n'est pas log-convexe. 🔗 fonction continue et périodique donc bornée : [bornes atteintes](../../../L3/topologie/theoremes/topo-bornes-atteintes.md) sur le compact $[0,1]$

### 5. Applications (1,5 page)
La même méthode à chaque fois : vérifier les trois hypothèses de Bohr–Mollerup.
- Fonction Bêta : $B(x,y)=\dfrac{\Gamma(x)\Gamma(y)}{\Gamma(x+y)}$.
- $\Gamma(\tfrac12)=\sqrt\pi$.
- Formule de duplication de Legendre : $\Gamma(\tfrac x2)\Gamma(\tfrac{x+1}2)=2^{1-x}\sqrt\pi\,\Gamma(x)$.

### 6. Conclusion et ouverture (½ page)
- Bilan : une seule idée (la log-convexité) donne unicité et formules.
- Ouverture (chapitre 6 d'Artin) : on peut remplacer la log-convexité par une équation fonctionnelle de plus si $f$ est $C^1$, mais pas avec la seule continuité. Le contre-exemple est une série de sinus **uniformément convergente**. 🔗 [continuité uniforme](../../../L3/topologie/definitions/topo-continuite-uniforme.md), [Heine](../../../L3/topologie/theoremes/topo-heine.md)

### Laissé de côté (pour tenir dans 10 pages)
Formule de Stirling, formule des compléments, formule de multiplication générale (chapitres 3 à 5 d'Artin).

## Questions encore ouvertes
- [ ] Une partie « rappels de topologie » séparée, ou des liens au fil du texte ? (pour l'instant : au fil du texte)
- [ ] Démonstrations complètes partout, ou seulement pour Bohr–Mollerup ?
- [ ] Date de rendu ?
