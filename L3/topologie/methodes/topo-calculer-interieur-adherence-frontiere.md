---
aliases:
  - "Méthode : calculer intérieur, adhérence, frontière"
  - "calculer l'adhérence"
  - "calculer l'intérieur"
  - "calculer la frontière"
tags:
  - topologie
  - topo/methode
  - topo/chapitre-02
---

# 🛠️ Méthode : calculer intérieur, adhérence, frontière

*Méthode* · Chapitre : [[02-topologie-espaces-metriques|2 – Topologie des espaces métriques]] · Méthode 2.2 du cours · [[topo-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> 1. **Deviner** : $\operatorname{Int}A$ = « $A$ sans son bord », $\bar A$ = « $A$ avec son bord ».
>    - Dans $\mathbb R$ : adhérence = on **ferme** les crochets ; intérieur = on **ouvre** les crochets et on enlève les points isolés.
>    - Dans $\mathbb R^2$ : adhérence = strictes → larges ; intérieur = larges → strictes ; une **égalité** (courbe) donne un intérieur vide.
> 2. **Justifier $\bar A=F$ (deux inclusions)** :
>    - $F\subset\bar A$ : chaque point ajouté est **limite d'une suite de $A$** ;
>    - $\bar A\subset F$ : **$F$ est fermé et contient $A$** (plus petit fermé).
> 3. **Justifier $\operatorname{Int}A=U$ (deux inclusions)** :
>    - $U\subset\operatorname{Int}A$ : **$U$ est ouvert et contenu dans $A$** (plus grand ouvert) ;
>    - $\operatorname{Int}A\subset U$ : chaque point de $A\setminus U$ est **limite d'une suite hors de $A$**.
> 4. $\operatorname{Fr}A=\bar A\setminus\operatorname{Int}A$.
> 5. Raccourcis : $A$ fermé $\Rightarrow\bar A=A$ ; $A$ ouvert $\Rightarrow\operatorname{Int}A=A$.

> [!EXAMPLE] Rédaction modèle (comme sur la copie)
> *$A_1=[1,2[\cup\{5\}$ dans $\mathbb R$.*
> « **Adhérence.** $y_n=2-\frac1n\in A_1$ ($1\le y_n<2$) et $y_n\to2$, donc $[1,2]\cup\{5\}=A_1\cup\{2\}\subset\bar A_1$. Inversement, $[1,2]\cup\{5\}$ est fermé (réunion **finie** de fermés) et contient $A_1$, donc $\bar A_1\subset[1,2]\cup\{5\}$. Ainsi $\bar A_1=[1,2]\cup\{5\}$.
> **Intérieur.** $]1,2[$ est ouvert et contenu dans $A_1$, donc $]1,2[\subset\operatorname{Int}A_1$. Les autres points de $A_1$ sont $1$ et $5$ : $1=\lim(1-\frac1n)$ avec $1-\frac1n\notin A_1$, et $5=\lim(5+\frac1n)$ avec $5+\frac1n\notin A_1$ ; ils ne sont pas intérieurs. Ainsi $\operatorname{Int}A_1=]1,2[$.
> **Frontière.** $\operatorname{Fr}A_1=([1,2]\cup\{5\})\setminus]1,2[=\{1,2,5\}$. »

> [!WARNING] Pièges
> - L'adhérence **contient** $A$ : ce n'est pas le complémentaire (mon erreur).
> - Ne pas oublier l'inclusion « $F$ fermé contenant $A$ » (mon erreur, interro 2025-26).
> - Pour l'intérieur, ne traiter que les points **de $A$** hors du candidat (ne pas recopier les points d'un autre exemple — mon erreur).
> - Pour $\mathbb R^2$ : la fermeture de $\{x>0\}$ est $\{x\ge0\}$, mais attention aux points ajoutés qui ne vérifient pas les autres conditions.

## 🔗 Liens

- **S'appuie sur** : [[topo-caracterisation-adherence|Caractérisations de l'adhérence]], [[topo-caracterisation-interieur|Caractérisation et propriétés de l'intérieur]], [[topo-proprietes-frontiere|Propriétés de la frontière]]
- **Méthodes voisines** : [[topo-montrer-pas-ouvert-pas-ferme|Méthode : montrer qu'une partie N'EST PAS ouverte / PAS fermée]]
- **Corrigés** : [[topo-exercices-types-corriges#5. Une partie de R – ouvert, fermé, adhérence, intérieur|ex. 5]], [[topo-exercices-types-corriges#6. Une suite qui tend vers 0 (écrit 2025-26)|ex. 6]], [[topo-exercices-types-corriges#7. La parabole (interro 2025-26)|ex. 7]]
- **Voir aussi** : [[topo-montrer-pas-ouvert-pas-ferme|Méthode : montrer qu'une partie N'EST PAS ouverte / PAS fermée]]
