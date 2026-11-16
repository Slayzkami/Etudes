# 📄 The Gamma Function — Emil Artin

**Type :** livre (monographie de 39 pages)  
**Auteur :** Emil Artin, traduit de l'allemand par Michael Butler  
**Édition :** Holt, Rinehart and Winston, New York, 1964 (original : *Einführung in die Theorie der Gammafunktion*, Teubner, Leipzig, 1931)  
**Lien :** [artin-the-gamma-function.pdf](artin-the-gamma-function.pdf) (scan du livre)  
**Lu le :** *(à compléter)*  
**Fiabilité :** ⭐⭐⭐⭐⭐ (texte de référence)

## En une phrase
> Artin montre que toute la théorie de la fonction Gamma se déduit d'une seule idée, la log-convexité, avec seulement des outils d'analyse réelle de niveau licence.

## Plan du livre
| Chapitre | Contenu | Pages du livre |
|---|---|---|
| 1. Fonctions convexes | Convexité, dérivées à gauche et à droite, log-convexité ; la somme de deux fonctions log-convexes est log-convexe (th. 1.8) ; une intégrale du type $\int \varphi(t)\,t^{x-1}\,dt$ est log-convexe en $x$ (th. 1.9) | 1 |
| 2. Intégrales d'Euler et formule de Gauss | Définition de $\Gamma$ par l'intégrale ; théorème de Bohr–Mollerup (th. 2.1) ; formule produit de Gauss ; fonction Bêta ; produit de Weierstrass | 11 |
| 3. Grandes valeurs de $x$ | Formule de Stirling avec un reste explicite, formule de multiplication de Gauss | 20 |
| 4. Lien avec $\sin x$ | Formule des compléments $\Gamma(x)\Gamma(1-x)=\pi/\sin(\pi x)$, produit infini de $\sin$ ; une fonction périodique positive qui vérifie une certaine équation fonctionnelle est constante (th. 4.1) | 25 |
| 5. Intégrales définies | Calcul d'intégrales classiques grâce à $\Gamma$ et $B$ | 28 |
| 6. Équations fonctionnelles | $\Gamma$ est caractérisée par $f(x+1)=xf(x)$ et la formule de multiplication, si $f$ est $C^1$ (th. 6.1, 6.2) ; la continuité seule ne suffit pas (contre-exemple par une série de sinus), sauf si l'on impose la formule pour **tous** les $p$ (th. 6.3) | 33 |

## Points clés
- **Point de départ :** $\Gamma(x)=\int_0^{+\infty}t^{x-1}e^{-t}\,dt$ pour $x>0$. Artin part de l'intégrale pour éviter d'avoir à prouver la convergence du produit de Gauss.
- **Le théorème central (Bohr–Mollerup) :** si $f>0$ sur $]0,+\infty[$, $f(x+1)=xf(x)$, $f$ log-convexe et $f(1)=1$, alors $f=\Gamma$. Toutes les formules suivantes s'obtiennent en vérifiant que l'autre membre satisfait ces trois conditions.
- **La méthode est toujours la même :** pour prouver une identité $F=\Gamma$, on vérifie l'équation fonctionnelle, la log-convexité et la valeur en 1.
- **Hors programme du livre** (dit dans la préface) : le cas complexe, le théorème de Hölder (Γ ne vérifie aucune équation différentielle algébrique), la série de Kummer et la dérivée logarithmique.
- La fin des chapitres 5 et 6 utilise les séries de Fourier (théorème de Fejér) et peut être sautée en première lecture.

## Ce que ça apporte au projet
- Le fil conducteur du rapport est le même que celui du livre : convexité → Bohr–Mollerup → formules classiques → caractérisation fonctionnelle.
- Les passages les plus liés au cours de topologie : les passages à la limite (limite d'une suite de fonctions convexes, intégrales impropres vues comme limites d'intégrales sur des segments), la convergence uniforme du contre-exemple du chapitre 6, et la continuité ou la bornitude sur un segment (fonction continue sur $[0,1]$ donc bornée, utilisée au th. 4.1 ; c'est de la compacité).

## Citation à garder (courte)
> « the gamma function can be thought of as one of the elementary functions » (préface d'Artin)
