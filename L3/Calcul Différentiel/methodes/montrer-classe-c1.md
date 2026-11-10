---
aliases:
  - "Méthode : montrer qu'une application est de classe C1 (ou C2)"
  - "prouver C1"
  - "prouver C2"
  - "justifier la classe"
tags:
  - cd
  - cd/methode
  - cd/chapitre-03
---

# 🛠️ Méthode : montrer qu'une application est de classe C1 (ou C2)

*Méthode* · Chapitre : [[03-accroissements-finis|3 – Accroissements finis]] · Méthodes 2.6 et 3.3 du cours · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> - **Sur un ouvert de $\mathbb R^n$** : les dérivées partielles existent et sont continues (Cor. 3.16) ; pour $\mathcal C^2$, celles d'ordre 1 et 2 (Th. 4.12). Sommes, produits, composées de fonctions usuelles : $\mathcal C^\infty$.
> - **Composée** de $\mathcal C^1$ : $\mathcal C^1$ (Cor. 2.26).
> - **Cas général (matrices, fonctions)** : calculer $Df_x$, puis majorer $\lVert (Df_x-Df_a)(h)\rVert\le C(x)\lVert h\rVert$ avec $C(x)\to0$ quand $x\to a$ ; alors $\lvert\!\lvert\!\lvert Df_x-Df_a\rvert\!\rvert\!\rvert\le C(x)\to0$.

> [!EXAMPLE] Rédaction modèle : $f(X)=X^2$
> $Df_X(H)=XH+HX$. $(Df_X-Df_A)(H)=(X-A)H+H(X-A)$, donc $\lVert (Df_X-Df_A)(H)\rVert\le2\lVert X-A\rVert\lVert H\rVert$ et $\lvert\!\lvert\!\lvert Df_X-Df_A\rvert\!\rvert\!\rvert\le2\lVert X-A\rVert\xrightarrow[X\to A]{}0$. Donc $f$ est $\mathcal C^1$.

> [!EXAMPLE] Domaine + classe (Écrit 2022-2023, ex. 2)
> $f(x,y)=x(\ln x)^2+y^2$ sur $U=\{x>0\}$ (ouvert). $\partial_xf=(\ln x)^2+2\ln x$ et $\partial_yf=2y$ existent et sont continues sur $U$ : $f$ est $\mathcal C^1$ sur $U$ (Cor. 3.16).

## 🔗 Liens

- **Voir aussi** : [[classe-c1|Application de classe C1]], [[critere-c1|Critère C1 par les dérivées partielles]], [[critere-c2|Critère C2]], [[caracterisation-bilineaires-continues|Caractérisation des applications bilinéaires continues]]
