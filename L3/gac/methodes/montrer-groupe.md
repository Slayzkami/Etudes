---
aliases:
  - "Méthode : montrer qu'un ensemble muni d'une loi est un groupe"
  - "montrer que c'est un groupe"
  - "loi exotique"
tags:
  - gac
  - gac/methode
  - gac/chapitre-01
---

# 🛠️ Méthode : montrer qu'un ensemble muni d'une loi est un groupe

*Méthode* · Chapitre : [[01-definitions-generales|I – Définitions générales]] · [[index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> 1. **Loi interne** : $x\star y\in G$ pour tous $x,y\in G$.
> 2. **Associativité** (souvent héritée, sinon calcul).
> 3. **Neutre** : le deviner, vérifier $e\in G$ et $x\star e=e\star x=x$.
> 4. **Symétrique** : pour chaque $x$, exhiber $x'\in G$ avec $x\star x'=x'\star x=e$.
>
> **Raccourcis** : montrer que c'est un [[sous-groupe]] d'un groupe connu ([[montrer-sous-groupe]]) ; ou trouver une **bijection $\varphi$ vers un groupe connu** qui transforme la loi : $\varphi(a\star b)=\varphi(a)\varphi(b)$.

> [!EXAMPLE] Loi exotique type (examen blanc)
> $G=\mathbb R\setminus\{-1\}$, $a\star b=a+b+ab$ : $1+a\star b=(1+a)(1+b)$, donc interne. $\varphi(a)=1+a$ est une bijection $G\to\mathbb R^*$ avec $\varphi(a\star b)=\varphi(a)\varphi(b)$ : on **transporte** la structure de $(\mathbb R^*,\times)$ ; neutre $\varphi^{-1}(1)=0$, symétrique $\varphi^{-1}\!\big(\tfrac1{1+a}\big)=\tfrac{-a}{1+a}$.
> Autre exemple : $]-1,1[$ avec $x\star y=\frac{x+y}{1+xy}$, isomorphe à $(\mathbb R,+)$ via $\operatorname{th}$.

## 🔗 Liens

- **Voir aussi** : [[groupe|Groupe]], [[morphisme-de-groupes|Morphisme de groupes]]
