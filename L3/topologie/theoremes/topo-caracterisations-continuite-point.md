---
aliases:
  - "Caractérisations de la continuité en un point"
  - "continuité séquentielle"
  - "continuité par les suites"
tags:
  - topologie
  - topo/theoreme
  - topo/chapitre-02
---

# ⭐ Caractérisations de la continuité en un point

*Théorème* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Th. 2.33 du cours (poly : Th. 2.6) · [[topo-index-definitions|↩ Index]]

> [!IMPORTANT] Énoncé
> Sont équivalentes :
> (i) $f$ est continue en $a$ ;
> (ii) l'image réciproque de tout voisinage de $f(a)$ est un voisinage de $a$ ;
> (iii) pour toute boule $B=B(f(a),r)$, $f^{-1}(B)$ est un voisinage de $a$ ;
> (iv) **pour toute suite $x_n\to a$, $f(x_n)\to f(a)$.**

> [!SUCCESS]- Démonstration
> (iv)⇒(i) par contraposée : si $f$ n'est pas continue en $a$, il existe $\varepsilon>0$ tel que pour tout $\delta=\frac1n$ on trouve $x_n$ avec $d(a,x_n)<\frac1n$ et $d(f(a),f(x_n))\ge\varepsilon$ : $x_n\to a$ mais $f(x_n)\not\to f(a)$.
> (iii)⇒(iv) Si $x_n\to a$ : $f^{-1}(B(f(a),\varepsilon))$ contient $B(a,\eta)$, et $x_n\in B(a,\eta)$ pour $n$ grand.

> [!TIP] Réflexes
> **Non-continuité** : exhiber **une** suite $x_n\to a$ avec $f(x_n)\not\to f(a)$. Ex. $\frac{xy}{x^2+y^2}$ en $(\frac1n,\frac1n)$ vaut $\frac12$.

## 🔗 Liens

- **S'appuie sur** : [[topo-continuite|Continuité en un point]], [[topo-voisinage|Voisinage]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-continuite-globale|Continuité globale : image réciproque]], [[topo-operations-fonctions-continues|Opérations sur les fonctions continues réelles]]
- **Méthodes** : [[topo-continuite-deux-variables|Méthode : continuité d'une fonction de deux variables en (0,0)]]
- **Voir aussi** : —
