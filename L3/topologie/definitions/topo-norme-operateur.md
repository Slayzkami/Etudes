---
aliases:
  - "Norme d'une application linéaire continue"
  - "norme d'opérateur"
  - "|||f|||"
  - "norme subordonnée"
tags:
  - topologie
  - topo/definition
  - topo/chapitre-02
---

# 📘 Norme d'une application linéaire continue

*Définition* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Déf. 2.71 du cours (poly : §2.14) · [[topo-index-definitions|↩ Index]]

> [!NOTE] Définition
> Pour $f\in\mathcal L_c(E,F)$ (linéaire continue) :
> $$|||f|||=\sup_{u\neq0}\frac{\|f(u)\|_F}{\|u\|_E}=\sup_{\|u\|_E=1}\|f(u)\|_F=\sup_{\|u\|_E\le1}\|f(u)\|_F.$$

> [!IMPORTANT] À retenir
> - $\|f(u)\|\le|||f|||\,\|u\|$, et $|||f|||$ est la **meilleure** constante ; $|||g\circ f|||\le|||g|||\,|||f|||$ → [[topo-proprietes-norme-operateur]].
> - Calcul : **majorer**, puis **atteindre** avec un $u_0\neq0$.

## 🔗 Liens

- **S'appuie sur** : [[topo-norme|Norme, espace vectoriel normé]], [[topo-applications-lineaires-continues|Continuité d'une application linéaire]]
- **Utilisé par (définitions)** : —
- **Utilisé par (théorèmes)** : [[topo-proprietes-norme-operateur|Propriétés de la norme d'opérateur]]
- **Méthodes** : [[topo-application-lineaire-norme-operateur|Méthode : continuité d'une application linéaire, norme d'opérateur]]
- **Voir aussi** : —
