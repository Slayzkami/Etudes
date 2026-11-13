---
aliases:
  - "Méthode : montrer qu'une application est une norme"
  - "prouver norme"
tags:
  - topologie
  - topo/methode
  - topo/chapitre-01
---

# 🛠️ Méthode : montrer qu'une application est une norme

*Méthode* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Méthode 1.2 du cours · [[topo-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> 1. **(N2) d'abord** : élimine vite les mauvais candidats.
> 2. **(N1)** : sur un espace de fonctions, c'est là que sert la continuité.
> 3. **(N3)** : se ramener à une norme connue. Si $N(v)=\|Av\|$ avec $A$ inversible (ou injective) : (N2), (N3) par linéarité, (N1) par injectivité.

> [!EXAMPLE] Rédaction modèle (comme sur la copie)
> *$N(x,y)=\max(|x+y|,|x-2y|)$ (TD 1.10).* « Posons $A=\begin{pmatrix}1&1\\1&-2\end{pmatrix}$ ; alors $N(v)=\|Av\|_\infty$ et $\det A=-3\neq0$.
> (N1) $N(v)=0\iff Av=0\iff v=0$ car $A$ est inversible. (N2) $N(\lambda v)=\|\lambda Av\|_\infty=|\lambda|N(v)$. (N3) $N(v+w)=\|Av+Aw\|_\infty\le N(v)+N(w)$. »

## 🔗 Liens

- **S'appuie sur** : [[topo-norme|Norme, espace vectoriel normé]]
- **Méthodes voisines** : [[topo-determiner-boule|Méthode : déterminer et dessiner une boule]]
- **Voir aussi** : [[topo-determiner-boule|Méthode : déterminer et dessiner une boule]]
