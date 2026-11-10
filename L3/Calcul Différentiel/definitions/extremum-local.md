---
aliases:
  - "Extremum local, extremum global"
  - "minimum local"
  - "maximum local"
  - "extremum"
  - "extremum global"
  - "minimum global"
tags:
  - cd
  - cd/definition
  - cd/chapitre-04
---

# 📘 Extremum local, extremum global

*Définition* · Chapitre : [[04-differentielles-ordre-superieur|4 – Différentielles d'ordre supérieur]] · Déf. 4.17 et 4.18 du cours · [[cd-index-definitions|↩ Index]]

> [!NOTE] Définition
> Soit $U\subset E$ un ouvert et $f:U\to\mathbb R$.
> - $f$ admet en $a\in U$ un **minimum local** (resp. **maximum local**) s'il existe un ouvert $V\subset U$ contenant $a$ tel que $\forall x\in V,\ f(x)\ge f(a)$ (resp. $f(x)\le f(a)$). Si l'inégalité est stricte pour $x\ne a$ : extremum local **strict**.
> - $f$ admet en $a$ un **minimum global** (resp. maximum global) si $f(x)\ge f(a)$ (resp. $\le$) pour **tout** $x\in U$.

> [!TIP] À retenir
> Global $\Rightarrow$ local. La réciproque est fausse : pour $f(x,y)=x^3-3x+y^2$, $(1,0)$ est un minimum local mais $f(x,0)\to-\infty$ quand $x\to-\infty$.

## 🔗 Liens

- **S'appuie sur** : [[ouvert-ferme|Ouvert, fermé]]
- **Utilisé par (théorèmes)** : [[condition-necessaire-extremum|Condition nécessaire d'extremum (ordre 1)]]
- **Méthodes** : [[etudier-points-critiques|Étudier les points critiques d'une fonction de R²]], [[extremum-global|Montrer l'existence d'un extremum global]]
