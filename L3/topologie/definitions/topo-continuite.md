---
aliases:
  - "Continuité en un point"
  - "continuité"
  - "continue"
  - "fonction continue"
  - "ε-δ"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-02
---

# 📘 Continuité en un point

*Définition* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Déf. 2.31 du cours (poly : Déf. 2.8) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> $f:(E,d_E)\to(F,d_F)$ est **continue en $a$** si
> $$\forall\varepsilon>0,\ \exists\delta>0,\ \forall x\in E,\ d_E(a,x)<\delta\Rightarrow d_F(f(a),f(x))<\varepsilon,$$
> c'est-à-dire $f(B_E(a,\delta))\subset B_F(f(a),\varepsilon)$. $f$ est continue sur $A$ si elle l'est en tout point de $A$.

> [!IMPORTANT] À retenir
> - **Par les suites** : $f$ continue en $a\iff$ pour **toute** suite $x_n\to a$, $f(x_n)\to f(a)$ → [[topo-caracterisations-continuite-point]].
> - **Globalement** : $f$ continue $\iff f^{-1}(\text{ouvert})$ ouvert $\iff f^{-1}(\text{fermé})$ fermé → [[topo-continuite-globale]].
> - $\delta$ dépend de $\varepsilon$ **et de $a$**.

> [!WARNING] Pièges
> - Pour montrer que $f$ **n'est pas** continue, il faut **une** suite $x_n\to a$ avec $f(x_n)\not\to f(a)$ ; majorer $|f|$ par une constante ne prouve rien (mon erreur au bilan).
> - Applications partielles continues $\not\Rightarrow$ $f$ continue : $\frac{xy}{x^2+y^2}$.

## 🔗 Liens

- **S'appuie sur** : [[topo-distance|Distance, espace métrique]]
- **Utilisé par (définitions)** : [[topo-homeomorphisme|Homéomorphisme]], [[topo-continuite-uniforme|Uniforme continuité]]
- **Utilisé par (théorèmes)** : [[topo-caracterisations-continuite-point|Caractérisations de la continuité en un point]], [[topo-composition-continues|Composition d'applications continues]], [[topo-applications-lineaires-continues|Continuité d'une application linéaire]], [[topo-continuite-composantes|Continuité dans un produit]], [[topo-continuite-globale|Continuité globale : image réciproque]], [[topo-image-continue-compact|Image continue d'un compact ; bijection continue sur un compact]], [[topo-operations-fonctions-continues|Opérations sur les fonctions continues réelles]]
- **Méthodes** : [[topo-continuite-deux-variables|Méthode : continuité d'une fonction de deux variables en (0,0)]]
- **Voir aussi** : [[topo-continuite-uniforme|Uniforme continuité]]
