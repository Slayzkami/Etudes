---
aliases:
  - "Méthode : montrer qu'une application est une distance"
  - "prouver distance"
  - "vérifier les axiomes de distance"
tags:
  - topologie
  - topo/methode
  - topo/chapitre-01
---

# 🛠️ Méthode : montrer qu'une application est une distance

*Méthode* · Chapitre : [[01-espaces-metriques|1 – Espaces métriques, e.v.n.]] · Méthode 1.1 du cours · [[topo-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> Pour montrer que $d$ est une distance, on vérifie **dans l'ordre** :
> 1. $d$ est à valeurs dans $\mathbb R_+$ ;
> 2. **séparation** : on suppose $d(x,y)=0$ et on montre $x=y$ (le sens $x=y\Rightarrow d=0$ est immédiat) ;
> 3. **symétrie** ;
> 4. **inégalité triangulaire** : le seul vrai travail. Astuces :
>    - $d(x,y)=\delta(\varphi(x),\varphi(y))$ avec $\delta$ distance et $\varphi$ **injective** : tout se transporte ;
>    - somme de distances, $\lambda d$ ($\lambda>0$) : distance ;
>    - **raisonner par cas** (distance discrète, $\min(1,d)$).
>
> Pour réfuter : **un** contre-exemple numérique suffit.

> [!EXAMPLE] Rédaction modèle (comme sur la copie)
> *Montrer que $\delta=\min(1,d)$ est une distance (interro 2025-26).*
> « **Séparation.** $\delta\ge0$. Si $\delta(x,y)=0$, alors $\min(1,d(x,y))=0$ ; comme $1\neq0$, $d(x,y)=0$, donc $x=y$. Réciproquement $\delta(x,x)=\min(1,0)=0$.
> **Symétrie.** $\delta(x,y)=\min(1,d(x,y))=\min(1,d(y,x))=\delta(y,x)$.
> **Inégalité triangulaire.** Soient $x,y,z\in E$.
> – Si $d(x,y)\ge1$ ou $d(y,z)\ge1$, alors $\delta(x,y)+\delta(y,z)\ge1\ge\delta(x,z)$.
> – Sinon, $\delta(x,y)+\delta(y,z)=d(x,y)+d(y,z)\ge d(x,z)\ge\min(1,d(x,z))=\delta(x,z)$.
> Donc $\delta$ est une distance sur $E$. »

> [!WARNING] Pièges
> - $\min(1,a+b)\le\min(1,a)+\min(1,b)$ **est** ce qu'il faut démontrer : l'écrire sans justification ne rapporte rien (mon erreur, interro 2025-26).
> - Oublier la positivité : $(x-y)^3$.

## 🔗 Liens

- **S'appuie sur** : [[topo-distance|Distance, espace métrique]]
- **Méthodes voisines** : —
- **Corrigés** : [[topo-exercices-types-corriges#9. Interro 2025-26 – la distance min(1, d)|ex. 9]]
- **Voir aussi** : —
