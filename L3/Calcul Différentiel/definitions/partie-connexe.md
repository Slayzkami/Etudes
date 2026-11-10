---
aliases:
  - "Partie connexe"
  - "connexe"
  - "connexité"
  - "d'un seul morceau"
tags:
  - cd
  - cd/definition
  - cd/chapitre-03
---

# 📘 Partie connexe

*Définition* · Chapitre : [[03-accroissements-finis|3 – Accroissements finis]] · Déf. 3.20 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> Un espace topologique $X$ est **connexe** si, pour tout couple $(U_1,U_2)$ d'ouverts de $X$ tels que $U_1\cap U_2=\emptyset$ et $U_1\cup U_2=X$, on a $U_1=\emptyset$ ou $U_2=\emptyset$.

> [!TIP] En clair
> $X$ est « d'un seul morceau » : on ne peut pas le couper en deux ouverts disjoints non vides. De façon équivalente (Prop. 3.21) : les seules parties à la fois ouvertes et fermées dans $X$ sont $\emptyset$ et $X$.

> [!EXAMPLE] Exemples
> - Tout convexe est connexe (Prop. 3.22) → [[convexe-implique-connexe]].
> - $\mathbb R^2\setminus\{(0,0)\}$ est connexe mais pas convexe (Ex. 3.24).
> - $\mathbb R^*=\,]-\infty,0[\ \cup\ ]0,+\infty[$ n'est **pas** connexe.

> [!WARNING] Piège
> Sur un ouvert non connexe, $Df=0$ n'entraîne pas $f$ constante : $f=1$ sur $]0,+\infty[$ et $f=-1$ sur $]-\infty,0[$ → [[differentielle-nulle]].

## 🔗 Liens

- **S'appuie sur** : [[ouvert-ferme|Ouvert, fermé]]
- **Utilisé par (théorèmes)** : [[differentielle-nulle|Différentielle nulle : f constante]], [[convexe-implique-connexe|Tout convexe est connexe]]
- **Méthodes** : [[montrer-constante|Montrer qu'une application est constante]]
