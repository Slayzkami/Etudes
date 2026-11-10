---
aliases:
  - "Méthode : montrer la différentiabilité par les théorèmes généraux"
  - "différentiable par opérations"
  - "briques de base"
tags:
  - cd
  - cd/methode
  - cd/chapitre-02
---

# 🛠️ Méthode : montrer la différentiabilité par les théorèmes généraux

*Méthode* · Chapitre : [[02-applications-differentiables|2 – Applications différentiables]] · Méthode 2.3 du cours · [[cd-index-definitions|↩ Index]]

> [!ABSTRACT] Recette
> **Briques de base** (différentiables partout) :
> - constantes ($D=0$) et linéaires continues ($D\varphi_a=\varphi$) ;
> - bilinéaires continues ($DB_{(a_1,a_2)}(h_1,h_2)=B(h_1,a_2)+B(a_1,h_2)$) ;
> - fonctions d'une variable dérivables ($Dg_t(s)=g'(t)s$).
>
> **Opérations** :
> - combinaisons linéaires (Th. 2.19) ;
> - composition (Th. 2.20) ;
> - composantes (Prop. 2.33) ;
> - « produit » $B(f_1,f_2)$ (Prop. 2.34).
>
> **Sur $\mathbb R^n$, le plus court** : « les dérivées partielles existent et sont continues, donc $f$ est $\mathcal C^1$ donc différentiable » (Cor. 3.16).

> [!EXAMPLE] Rédaction modèle (Écrit 2024-2025, ex. 1)
> « Les composantes $f_1(x,y)=\frac{\cos x-\sin y}2$ et $f_2(x,y)=\frac{\sin x-\cos y}2$ sont des combinaisons linéaires de composées de fonctions usuelles de classe $\mathcal C^1$ : elles sont $\mathcal C^1$ sur $\mathbb R^2$, donc différentiables. Par la Proposition 2.33, $f$ est différentiable sur $\mathbb R^2$. »

> [!WARNING] Piège
> Chaque brique doit être **nommée et justifiée**. Si une hypothèse manque en un point ($\abs\cdot$ en $0$, dénominateur nul), le théorème ne dit rien : on passe à [[etudier-en-un-point-particulier]].

## 🔗 Liens

- **Voir aussi** : [[differentielles-de-reference|Différentielles de référence : constante, linéaire, bilinéaire]], [[linearite-differentielle|Linéarité de la différentielle]], [[regle-de-la-chaine|Règle de la chaîne (différentielle d'une composée)]], [[differentiabilite-par-composantes|Différentiabilité par composantes]], [[differentielle-produit-bilineaire|Différentielle d'un « produit » B(f1, f2)]], [[critere-c1|Critère C1 par les dérivées partielles]]
