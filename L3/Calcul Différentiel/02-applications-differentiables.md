---
aliases:
  - "2 – Applications différentiables"
  - "Chapitre différentiabilité"
  - "CD chapitre 2"
tags:
  - cd
  - cd/chapitre
---

# Chapitre 02 – Applications différentiables

**Matière :** [[L3/Calcul Différentiel/README|Calcul Différentiel]]  
**Source :** polycopié *Chapitre 2 – Notion de différentiabilité* ; cours rédigé, chapitre 2 (pages 24 à 57)  
**Index :** [[cd-index-definitions]]

## 🎯 L'essentiel en 3 lignes
- $f$ est [[differentiabilite|différentiable]] en $a$ si $f(a+h)=f(a)+L(h)+o(h)$ avec $L$ **linéaire continue** ; alors $L=Df_a$ est unique.
- $Df_a(v)=\lim_{t\to0}\frac{f(a+tv)-f(a)}t$ ([[differentielle-et-derivees-directionnelles|Prop. 2.9]]) ; sur $\mathbb R^n$, $Df_a(h)=J_f(a)\,h$ ([[matrice-jacobienne]]).
- On calcule avec trois briques (constante, linéaire, bilinéaire : [[differentielles-de-reference]]) et la [[regle-de-la-chaine]] : $D(g\circ f)_a=Dg_{f(a)}\circ Df_a$.

## 📝 Notes

### 2.1 – Définitions
- [[petit-o]] et ses règles de calcul.
- [[differentiabilite]] : définition, formes équivalentes, unicité, notation $Df_a(h)$.
- [[derivee-directionnelle]] et [[differentielle-et-derivees-directionnelles]] ; la réciproque est fausse.
- [[classe-c1]].

### 2.2 – Exemples fondamentaux
- [[differentielles-de-reference]] : constante ($0$), linéaire continue ($\varphi$), bilinéaire continue ($B(h_1,a_2)+B(a_1,h_2)$).

### 2.3 – Propriétés
- [[differentiable-implique-continue]] ; [[linearite-differentielle]] ; [[regle-de-la-chaine]].
- Méthodes : [[differentiabilite-par-definition]], [[differentiabilite-par-theoremes]], [[appliquer-regle-de-la-chaine]], [[montrer-non-differentiable]].

### 2.4 – Espaces produits
- Au départ : [[differentielle-partielle]], [[derivee-partielle]], [[differentielle-et-differentielles-partielles]].
- À l'arrivée : [[differentiabilite-par-composantes]], [[differentielle-produit-bilineaire]].
- [[matrice-jacobienne]], [[gradient]]. Méthodes : [[calculer-jacobienne]], [[calculer-derivee-directionnelle]].
- Cas particuliers : [[etudier-en-un-point-particulier]], [[differentielle-sur-les-matrices]].

## 🔑 Définitions / formules à retenir
| Terme | Formule |
|---|---|
| [[differentiabilite]] | $f(a+h)=f(a)+Df_a(h)+o(h)$, $Df_a\in\mathcal L_c(E,F)$ |
| [[differentielle-et-derivees-directionnelles]] | $Df_a(v)=\lim_{t\to0}\frac{f(a+tv)-f(a)}t$ |
| [[differentielles-de-reference]] | $D\varphi_a=\varphi$ ; $DB_{(a_1,a_2)}(h_1,h_2)=B(h_1,a_2)+B(a_1,h_2)$ |
| [[regle-de-la-chaine]] | $D(g\circ f)_a=Dg_{f(a)}\circ Df_a$ ; $J_{g\circ f}(a)=J_g(f(a))J_f(a)$ |
| [[differentielle-et-differentielles-partielles]] | $Df_a(h)=\sum_jh_j\frac{\partial f}{\partial x_j}(a)$ |
| [[differentiabilite-par-composantes]] | $Df_a(h)=(D(f_1)_a(h),\dots,D(f_p)_a(h))$ |
| [[matrice-jacobienne]] | $J_f(a)=\big(\frac{\partial f_i}{\partial x_j}(a)\big)$, ligne = composante, colonne = variable |
| [[differentielle-produit-bilineaire]] | $D(fg)_a(h)=Df_a(h)g(a)+f(a)Dg_a(h)$ |
| $X\mapsto X^2$ | $Df_A(H)=AH+HA$ |

## ❓ Ce que je n'ai pas compris
- 

## 🧠 Questions de révision
1. Quand dit-on que $f$ est différentiable en $a$ ? (Écrits 2022-2023 et 2024-2025)
2. Montrer : différentiable en $a$ ⟹ continue en $a$. (Écrit 2022-2023)
3. Définir « dérivable en $a$ dans la direction $v$ » ; montrer que si $f$ est différentiable en $a$, la dérivée dans la direction $v$ vaut $Df_a(v)$. (Écrit 2024-2025)
4. Énoncer la règle de différentiation des fonctions composées. (Écrit 2022-2023)
5. Différentielle d'une application linéaire continue ? bilinéaire continue ? Le démontrer.
6. Développer $(A+H)^3$ sans commuter et en déduire la différentielle de $X\mapsto X^3$.
7. Donner une fonction qui a des dérivées partielles en $(0,0)$ mais n'y est pas continue.

## 🔗 Pour aller plus loin
- Corrigés rédigés : [[cd-exercices-types-corriges]] (ex. 4 à 9) · pièges : [[cd-mes-erreurs]]
- Précédent : [[01-espaces-vectoriels-normes]] · Suivant : [[03-accroissements-finis]]
- TD2 et TD3 → dossier [fichiers](fichiers/)
- Sources : polycopié [chapitre 2](fichiers/cd-chap2-polycopie.pdf), [cours rédigé](fichiers/cd-cours-redige-ch1-5.pdf)
