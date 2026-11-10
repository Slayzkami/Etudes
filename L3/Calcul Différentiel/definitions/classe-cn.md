---
aliases:
  - "Différentiabilité d'ordre n, classes Cn et C∞"
  - "C^n"
  - "C infini"
  - "n fois différentiable"
  - "D^n f_a"
tags:
  - cd
  - cd/definition
  - cd/chapitre-04
---

# 📘 Différentiabilité d'ordre n, classes Cn et C∞

*Définition* · Chapitre : [[04-differentielles-ordre-superieur|4 – Différentielles d'ordre supérieur]] · Déf. 4.29 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> Soit $n\ge2$.
> - $f$ est **$n$ fois différentiable en $a$** s'il existe un ouvert $V\subset U$ contenant $a$ sur lequel $f$ est $(n-1)$ fois différentiable, et si $D^{n-1}f$ est différentiable en $a$. On note $D^nf_a:=D(D^{n-1}f)_a$, vue comme une application $n$-linéaire continue (Déf. 4.27) : $D^nf_a(h_1,\dots,h_n)$.
> - $f$ est **de classe $\mathcal C^n$** sur $U$ si elle est $n$ fois différentiable sur $U$ et si $D^nf$ est continue. $f$ est $\mathcal C^\infty$ si elle est $\mathcal C^n$ pour tout $n$.

> [!IMPORTANT] Sur $\mathbb R^n$ (Th. 4.32, Prop. 4.33)
> $f$ est $\mathcal C^p$ $\iff$ toutes ses dérivées partielles jusqu'à l'ordre $p$ existent et sont continues. Sommes, produits, composées d'applications $\mathcal C^n$ sont $\mathcal C^n$ : les polynômes, $\exp$, $\sin$, $\cos$ sont $\mathcal C^\infty$.

> [!TIP] Notation
> $D^kf_a(h)^k$ désigne $D^kf_a(h,\dots,h)$ ($k$ fois) → [[formules-de-taylor]].

## 🔗 Liens

- **S'appuie sur** : [[differentielle-seconde|Différentielle seconde, classe C2]]
- **Utilisé par (théorèmes)** : [[formules-de-taylor|Formules de Taylor (ordre n)]]
