---
aliases:
  - "Méthode : continuité d'une fonction de deux variables en (0,0)"
  - "continuité en (0,0)"
  - "fonction de deux variables"
tags:
  - topologie
  - topo/methode
  - topo/chapitre-02
---

# 🛠️ Méthode : continuité d'une fonction de deux variables en (0,0)

*Méthode* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Méthode 2.3 du cours · [[topo-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> - **Ailleurs qu'en $(0,0)$** : quotient de fonctions continues (polynômes) à dénominateur non nul.
> - **Continuité en $(0,0)$** : majorer $|f(x,y)-f(0,0)|$ par une quantité qui tend vers $0$ quand $r=\|(x,y)\|_2\to0$. Outils : $|x|,|y|\le r$ ; $x^2\le x^2+y^2$ ; $|xy|\le\frac{x^2+y^2}2$ ; coordonnées polaires.
> - **Non-continuité** : **une** suite (ou un chemin) $u_n\to(0,0)$ avec $f(u_n)\not\to f(0,0)$ : essayer $(\frac1n,0)$, $(0,\frac1n)$, $(\frac1n,\frac1n)$, $(\frac1n,\frac1{n^2})$…

> [!EXAMPLE] Rédaction modèle (comme sur la copie)
> « $f(x,y)=\frac{x^3+y^3}{x^2+y^2}$, $f(0,0)=0$. Sur $\mathbb R^2\setminus\{(0,0)\}$, $f$ est un quotient de polynômes à dénominateur non nul : continue. En $(0,0)$ : $|x^3+y^3|\le|x|x^2+|y|y^2\le(|x|+|y|)(x^2+y^2)$, donc $|f(x,y)|\le|x|+|y|\to0$ : $f$ est continue en $(0,0)$. »
>
> « $g(x,y)=\frac{x^2}{x^2+y^2}$, $g(0,0)=0$ : $(\frac1n,0)\to(0,0)$ mais $g(\frac1n,0)=1\not\to0=g(0,0)$ ; $g$ n'est pas continue en $(0,0)$. »

> [!WARNING] Pièges
> - Majorer $|g|$ par une **constante** ($|g|\le1$) ne prouve **pas** la discontinuité (mon erreur au bilan).
> - Applications partielles continues $\not\Rightarrow$ continue.

## 🔗 Liens

- **S'appuie sur** : [[topo-caracterisations-continuite-point|Caractérisations de la continuité en un point]], [[topo-operations-fonctions-continues|Opérations sur les fonctions continues réelles]], [[topo-continuite-composantes|Continuité dans un produit]]
- **Méthodes voisines** : —
- **Voir aussi** : —
