---
aliases:
  - "Méthode : continuité d'une application linéaire, norme d'opérateur"
tags:
  - topologie
  - topo/methode
  - topo/chapitre-02
---

# 🛠️ Méthode : continuité d'une application linéaire, norme d'opérateur

*Méthode* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Méthode 2.6 du cours · [[topo-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> - **Continue** : automatique en dimension finie ; sinon établir $\|f(u)\|\le C\|u\|$.
> - **Pas continue** : $(u_n)$ avec $\|u_n\|=1$ et $\|f(u_n)\|\to+\infty$.
> - **Calculer $|||f|||$** : **majorer** ($|||f|||\le C$) puis **atteindre** ($u_0\neq0$ avec $\|f(u_0)\|=C\|u_0\|$).

> [!EXAMPLE] Rédaction modèle (comme sur la copie)
> « $f(u)(x)=\int_0^xu(t)\,dt$ : $|f(u)(x)|\le x\|u\|_\infty\le\|u\|_\infty$, donc $|||f|||\le1$ ; pour $u_0=1$, $\|f(u_0)\|_\infty=1=\|u_0\|_\infty$, donc $|||f|||=1$. »

## 🔗 Liens

- **S'appuie sur** : [[topo-applications-lineaires-continues|Continuité d'une application linéaire]], [[topo-proprietes-norme-operateur|Propriétés de la norme d'opérateur]]
- **Méthodes voisines** : —
- **Voir aussi** : —
