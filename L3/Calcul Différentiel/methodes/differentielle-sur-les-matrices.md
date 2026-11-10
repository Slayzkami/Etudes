---
aliases:
  - "Méthode : calculer une différentielle sur les matrices"
  - "différentielle de X², X³, tr(X³)"
  - "développer f(A+H) sans commuter"
tags:
  - cd
  - cd/methode
  - cd/chapitre-02
---

# 🛠️ Méthode : calculer une différentielle sur les matrices

*Méthode* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · [[cd-index-definitions|↩ Index]]

Cadre : $E=\mathcal M_n(\mathbb R)$ (dimension finie $n^2$), norme vérifiant $\lVert XY\rVert\le\lVert X\rVert\lVert Y\rVert$.

> [!ABSTRACT] Recette
> 1. **Développer $f(A+H)$ sans commuter** : $AH\ne HA$ en général. On garde l'ordre des facteurs.
> 2. **Trier par nombre de $H$** : 0 $H$ → $f(A)$ ; **1 $H$ → $L(H)$** ; 2 $H$ ou plus → reste $r(H)$.
> 3. **$L$ linéaire continue** : linéaire en $H$ (le dire), continue car $E$ est de dimension finie (Th. 1.44).
> 4. **Reste** : avec $\lVert XY\rVert\le\lVert X\rVert\lVert Y\rVert$, $\lVert r(H)\rVert\le C\lVert H\rVert^2$ pour $\lVert H\rVert\le1$.
> 5. **Conclure** : $Df_A(H)=L(H)$.

> [!EXAMPLE] Rédaction modèle : $f(X)=X^3$ (Écrit 2022-2023)
> $(A+H)^3=A^3+\underbrace{A^2H+AHA+HA^2}_{L(H)}+\underbrace{AH^2+HAH+H^2A+H^3}_{r(H)}$.
> $L$ est linéaire en $H$, continue (dimension finie). $\lVert r(H)\rVert\le3\lVert A\rVert\lVert H\rVert^2+\lVert H\rVert^3$, donc $\frac{\lVert r(H)\rVert}{\lVert H\rVert}\le3\lVert A\rVert\lVert H\rVert+\lVert H\rVert^2\to0$.
> Donc $Df_A(H)=A^2H+AHA+HA^2$.
> Puis $g=\mathrm{tr}\circ f$ : $\mathrm{tr}$ linéaire continue, $Dg_A(H)=\mathrm{tr}(Df_A(H))=3\,\mathrm{tr}(A^2H)$ (car $\mathrm{tr}(XY)=\mathrm{tr}(YX)$).

> [!EXAMPLE] Autres résultats à connaître
> | $f(X)$ | $Df_A(H)$ |
> |---|---|
> | $X^2$ | $AH+HA$ |
> | $XMX$ | $HMA+AMH$ |
> | ${}^t\!XX$ | ${}^t\!HA+{}^t\!AH$ |
> | $\mathrm{tr}(X\,{}^t\!X)$ | $2\,\mathrm{tr}(A\,{}^t\!H)$ |
> | $\mathrm{tr}(X)$ | $\mathrm{tr}(H)$ |

> [!WARNING] Pièges
> - Écrire $(A+H)^2=A^2+2AH+H^2$ : **faux**, c'est $A^2+AH+HA+H^2$.
> - $\mathrm{tr}$ permet de commuter **sous la trace** seulement.

## 🔗 Liens

- **Voir aussi** : [[differentiabilite-par-definition|Montrer la différentiabilité par la définition]], [[differentielles-de-reference|Différentielles de référence : constante, linéaire, bilinéaire]], [[norme-composee|Norme d'une composée]], [[lineaire-en-dimension-finie|Linéaire au départ d'une dimension finie : continue]], [[appliquer-regle-de-la-chaine|Appliquer la règle de la chaîne en 4 étapes]]
